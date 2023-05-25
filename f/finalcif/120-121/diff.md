# Comparing `tmp/finalcif-120.tar.gz` & `tmp/finalcif-121.tar.gz`

## Comparing `finalcif-120.tar` & `finalcif-121.tar`

### file list

```diff
@@ -1,112 +1,113 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 finalcif-120/finalcif/__init__.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 finalcif-120/finalcif/app_path.py
--rw-r--r--   0        0        0    92019 2020-02-02 00:00:00.000000 finalcif-120/finalcif/appwindow.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 finalcif-120/finalcif/finalcif_start.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/__init__.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/all_cif_dicts.py
--rw-r--r--   0        0        0    18681 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/atoms.py
--rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cif_dict_foo.py
--rw-r--r--   0        0        0    38969 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cif_file_io.py
--rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cif_order.py
--rw-r--r--   0        0        0   484078 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/core_dict.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/hkl.py
--rw-r--r--   0        0        0  1041931 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/modulation_dict.py
--rw-r--r--   0        0        0   221592 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/powder_dict.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/reference.py
--rw-r--r--   0        0        0   106774 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/restraints_dict.py
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/text.py
--rw-r--r--   0        0        0    21412 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/twin_dict.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/checkcif/__init__.py
--rw-r--r--   0        0        0    10770 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/checkcif/checkcif.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cod/__init__.py
--rw-r--r--   0        0        0    18635 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cod/deposit.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cod/deposit_check.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cod/deposition_list.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cod/doi.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cod/upload.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cod/website_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/__init__.py
--rw-r--r--   0        0        0    12742 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/bruker_data.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/bruker_frame.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/ccdc_mail.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/data.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/p4p_reader.py
--rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/sadabs.py
--rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/saint.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/shelx_lst.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/displaymol/__init__.py
--rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 finalcif-120/finalcif/displaymol/molecule2D.py
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 finalcif-120/finalcif/displaymol/sdm.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 finalcif-120/finalcif/displaymol/vtk_molecule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/equip_property/__init__.py
--rw-r--r--   0        0        0    21598 2020-02-02 00:00:00.000000 finalcif-120/finalcif/equip_property/author_loop_templates.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 finalcif-120/finalcif/equip_property/equipment.py
--rw-r--r--   0        0        0    13453 2020-02-02 00:00:00.000000 finalcif-120/finalcif/equip_property/properties.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 finalcif-120/finalcif/equip_property/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/__init__.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/combobox.py
--rw-r--r--   0        0        0    11048 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/custom_classes.py
--rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/dialogs.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/equipmenttable.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/file_editor.py
--rw-r--r--   0        0        0   162120 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/finalcif_gui_ui.py
--rw-r--r--   0        0        0   187031 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/finalcif_gui_ui.ui
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/loop_creator.py
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/loop_creator_ui.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/loop_creator_ui.ui
--rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/loops.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/mainstackwidget.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/mixins.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/new_key_dialog.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/new_key_dialog_ui.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/new_key_dialog_ui.ui
--rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/plaintextedit.py
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/playground.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/propertytable.py
--rw-r--r--   0        0        0     9358 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/text_templates_ui.py
--rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/text_templates_ui.ui
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/text_value_editor.py
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/vrf_classes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/icon/__init__.py
--rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 finalcif-120/finalcif/icon/finalcif.png
--rw-r--r--   0        0        0    25352 2020-02-02 00:00:00.000000 finalcif-120/finalcif/icon/finalcif2.ico
--rw-r--r--   0        0        0    17091 2020-02-02 00:00:00.000000 finalcif-120/finalcif/icon/finalcif2.png
--rw-r--r--   0        0        0   103782 2020-02-02 00:00:00.000000 finalcif-120/finalcif/icon/multitable.ico
--rw-r--r--   0        0        0    17746 2020-02-02 00:00:00.000000 finalcif-120/finalcif/icon/multitable.png
--rw-r--r--   0        0        0   124043 2020-02-02 00:00:00.000000 finalcif-120/finalcif/icon/multitable.xcf
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/archive_report.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/mtools.py
--rw-r--r--   0        0        0    19119 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/references.py
--rw-r--r--   0        0        0    23568 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/report_text.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/symm.py
--rw-r--r--   0        0        0    37156 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/tables.py
--rw-r--r--   0        0        0    26709 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/templated_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/gui/__init__.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/gui/mainwindow.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/gui/mainwindow.ui
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/template/__init__.py
--rw-r--r--   0        0        0   151706 2020-02-02 00:00:00.000000 finalcif-120/finalcif/template/mathml2omml.xsl
--rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 finalcif-120/finalcif/template/template1.docx
--rw-r--r--   0        0        0    35411 2020-02-02 00:00:00.000000 finalcif-120/finalcif/template/template_text.docx
--rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 finalcif-120/finalcif/template/template_without_text.docx
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 finalcif-120/finalcif/template/templates.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/__init__.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/download.py
--rw-r--r--   0        0        0    43454 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/dsrmath.py
--rw-r--r--   0        0        0    32788 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/misc.py
--rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/options.py
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/platon.py
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/pupdate.py
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/settings.py
--rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/shred.py
--rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/space_groups.py
--rw-r--r--   0        0        0   137178 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/spgr_format.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/statusbar.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/sumformula.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 finalcif-120/.gitignore
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 finalcif-120/LICENSE
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 finalcif-120/README.md
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 finalcif-120/pyproject.toml
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 finalcif-120/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 finalcif-121/finalcif/__init__.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 finalcif-121/finalcif/app_path.py
+-rw-r--r--   0        0        0    92019 2020-02-02 00:00:00.000000 finalcif-121/finalcif/appwindow.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 finalcif-121/finalcif/finalcif_start.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/__init__.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/all_cif_dicts.py
+-rw-r--r--   0        0        0    18681 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/atoms.py
+-rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cif_dict_foo.py
+-rw-r--r--   0        0        0    38969 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cif_file_io.py
+-rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cif_order.py
+-rw-r--r--   0        0        0   484078 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/core_dict.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/hkl.py
+-rw-r--r--   0        0        0  1041931 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/modulation_dict.py
+-rw-r--r--   0        0        0   221592 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/powder_dict.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/reference.py
+-rw-r--r--   0        0        0   106774 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/restraints_dict.py
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/text.py
+-rw-r--r--   0        0        0    21412 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/twin_dict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/checkcif/__init__.py
+-rw-r--r--   0        0        0    10770 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/checkcif/checkcif.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cod/__init__.py
+-rw-r--r--   0        0        0    18635 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cod/deposit.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cod/deposit_check.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cod/deposition_list.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cod/doi.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cod/upload.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cod/website_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/__init__.py
+-rw-r--r--   0        0        0    12742 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/bruker_data.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/bruker_frame.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/ccdc_mail.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/data.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/p4p_reader.py
+-rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/sadabs.py
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/saint.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/shelx_lst.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/displaymol/__init__.py
+-rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 finalcif-121/finalcif/displaymol/molecule2D.py
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 finalcif-121/finalcif/displaymol/sdm.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 finalcif-121/finalcif/displaymol/vtk_molecule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/equip_property/__init__.py
+-rw-r--r--   0        0        0    21598 2020-02-02 00:00:00.000000 finalcif-121/finalcif/equip_property/author_loop_templates.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 finalcif-121/finalcif/equip_property/equipment.py
+-rw-r--r--   0        0        0    13453 2020-02-02 00:00:00.000000 finalcif-121/finalcif/equip_property/properties.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 finalcif-121/finalcif/equip_property/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/__init__.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/combobox.py
+-rw-r--r--   0        0        0    11048 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/custom_classes.py
+-rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/dialogs.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/equipmenttable.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/file_editor.py
+-rw-r--r--   0        0        0   162120 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/finalcif_gui_ui.py
+-rw-r--r--   0        0        0   187031 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/finalcif_gui_ui.ui
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/loop_creator.py
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/loop_creator_ui.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/loop_creator_ui.ui
+-rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/loops.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/mainstackwidget.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/mixins.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/new_key_dialog.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/new_key_dialog_ui.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/new_key_dialog_ui.ui
+-rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/plaintextedit.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/playground.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/propertytable.py
+-rw-r--r--   0        0        0    12927 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/spell_check_edit.py
+-rw-r--r--   0        0        0     9403 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/text_templates_ui.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/text_templates_ui.ui
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/text_value_editor.py
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/vrf_classes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/icon/__init__.py
+-rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 finalcif-121/finalcif/icon/finalcif.png
+-rw-r--r--   0        0        0    25352 2020-02-02 00:00:00.000000 finalcif-121/finalcif/icon/finalcif2.ico
+-rw-r--r--   0        0        0    17091 2020-02-02 00:00:00.000000 finalcif-121/finalcif/icon/finalcif2.png
+-rw-r--r--   0        0        0   103782 2020-02-02 00:00:00.000000 finalcif-121/finalcif/icon/multitable.ico
+-rw-r--r--   0        0        0    17746 2020-02-02 00:00:00.000000 finalcif-121/finalcif/icon/multitable.png
+-rw-r--r--   0        0        0   124043 2020-02-02 00:00:00.000000 finalcif-121/finalcif/icon/multitable.xcf
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/archive_report.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/mtools.py
+-rw-r--r--   0        0        0    19119 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/references.py
+-rw-r--r--   0        0        0    24577 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/report_text.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/symm.py
+-rw-r--r--   0        0        0    37156 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/tables.py
+-rw-r--r--   0        0        0    26709 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/templated_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/gui/__init__.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/gui/mainwindow.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/gui/mainwindow.ui
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/template/__init__.py
+-rw-r--r--   0        0        0   151706 2020-02-02 00:00:00.000000 finalcif-121/finalcif/template/mathml2omml.xsl
+-rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 finalcif-121/finalcif/template/template1.docx
+-rw-r--r--   0        0        0    35411 2020-02-02 00:00:00.000000 finalcif-121/finalcif/template/template_text.docx
+-rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 finalcif-121/finalcif/template/template_without_text.docx
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 finalcif-121/finalcif/template/templates.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/__init__.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/download.py
+-rw-r--r--   0        0        0    43454 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/dsrmath.py
+-rw-r--r--   0        0        0    32788 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/misc.py
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/options.py
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/platon.py
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/pupdate.py
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/settings.py
+-rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/shred.py
+-rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/space_groups.py
+-rw-r--r--   0        0        0   137178 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/spgr_format.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/statusbar.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/sumformula.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 finalcif-121/.gitignore
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 finalcif-121/LICENSE
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 finalcif-121/README.md
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 finalcif-121/pyproject.toml
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 finalcif-121/PKG-INFO
```

### Comparing `finalcif-120/finalcif/app_path.py` & `finalcif-121/finalcif/app_path.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/appwindow.py` & `finalcif-121/finalcif/appwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -619,15 +619,15 @@
         changes_cif.save(self.finalcif_changes_filename)
 
     def check_for_update_version(self) -> None:
         if os.environ.get('NO_NETWORK'):
             print('Skipping version.txt download because NO_NETWORK variable is set.')
             return
         mainurl = "https://dkratzert.de/files/finalcif/version.txt"
-        self.upd = MyDownloader(mainurl, parent=self)
+        self.upd = MyDownloader(mainurl, parent=None)
         version_thread = QThread()
         self.threadpool.append(version_thread)
         start_worker(self.upd, version_thread, onload=self.is_update_necessary)
 
     def is_update_necessary(self, content: bytes) -> None:
         """
         Reads the reply from the server and displays a warning in case of an old version.
@@ -689,15 +689,15 @@
         """
         Sends a get request to the platon server in order to get the current check.def file.
         """
         if os.environ.get('NO_NETWORK'):
             print('Skipping check.def download because NO_NETWORK variable is set.')
             return
         url = 'http://www.platonsoft.nl/xraysoft/unix/platon/check.def'
-        self.updc = MyDownloader(url, parent=self)
+        self.updc = MyDownloader(url, parent=None)
         checkdef_thread = QThread(parent=self)
         self.threadpool.append(checkdef_thread)
         start_worker(self.updc, checkdef_thread, onload=self._save_checkdef)
 
     def _save_checkdef(self, reply: bytes) -> None:
         """
         Is called by the finished signal from the downloader.
```

### Comparing `finalcif-120/finalcif/finalcif_start.py` & `finalcif-121/finalcif/finalcif_start.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/all_cif_dicts.py` & `finalcif-121/finalcif/cif/all_cif_dicts.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/atoms.py` & `finalcif-121/finalcif/cif/atoms.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/cif_dict_foo.py` & `finalcif-121/finalcif/cif/cif_dict_foo.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/cif_file_io.py` & `finalcif-121/finalcif/cif/cif_file_io.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/cif_order.py` & `finalcif-121/finalcif/cif/cif_order.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/core_dict.py` & `finalcif-121/finalcif/cif/core_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/hkl.py` & `finalcif-121/finalcif/cif/hkl.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/modulation_dict.py` & `finalcif-121/finalcif/cif/modulation_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/powder_dict.py` & `finalcif-121/finalcif/cif/powder_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/reference.py` & `finalcif-121/finalcif/cif/reference.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/restraints_dict.py` & `finalcif-121/finalcif/cif/restraints_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/text.py` & `finalcif-121/finalcif/cif/text.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/twin_dict.py` & `finalcif-121/finalcif/cif/twin_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/checkcif/checkcif.py` & `finalcif-121/finalcif/cif/checkcif/checkcif.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/cod/deposit.py` & `finalcif-121/finalcif/cif/cod/deposit.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/cod/deposit_check.py` & `finalcif-121/finalcif/cif/cod/deposit_check.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/cod/deposition_list.py` & `finalcif-121/finalcif/cif/cod/deposition_list.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/cod/doi.py` & `finalcif-121/finalcif/cif/cod/doi.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/cod/upload.py` & `finalcif-121/finalcif/cif/cod/upload.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/cif/cod/website_parser.py` & `finalcif-121/finalcif/cif/cod/website_parser.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/datafiles/bruker_data.py` & `finalcif-121/finalcif/datafiles/bruker_data.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/datafiles/bruker_frame.py` & `finalcif-121/finalcif/datafiles/bruker_frame.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/datafiles/ccdc_mail.py` & `finalcif-121/finalcif/datafiles/ccdc_mail.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/datafiles/data.py` & `finalcif-121/finalcif/datafiles/data.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/datafiles/p4p_reader.py` & `finalcif-121/finalcif/datafiles/p4p_reader.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/datafiles/sadabs.py` & `finalcif-121/finalcif/datafiles/sadabs.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/datafiles/saint.py` & `finalcif-121/finalcif/datafiles/saint.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/datafiles/shelx_lst.py` & `finalcif-121/finalcif/datafiles/shelx_lst.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/datafiles/utils.py` & `finalcif-121/finalcif/datafiles/utils.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/displaymol/molecule2D.py` & `finalcif-121/finalcif/displaymol/molecule2D.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/displaymol/sdm.py` & `finalcif-121/finalcif/displaymol/sdm.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/displaymol/vtk_molecule.py` & `finalcif-121/finalcif/displaymol/vtk_molecule.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/equip_property/author_loop_templates.py` & `finalcif-121/finalcif/equip_property/author_loop_templates.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/equip_property/equipment.py` & `finalcif-121/finalcif/equip_property/equipment.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/equip_property/properties.py` & `finalcif-121/finalcif/equip_property/properties.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/equip_property/tools.py` & `finalcif-121/finalcif/equip_property/tools.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/combobox.py` & `finalcif-121/finalcif/gui/combobox.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/custom_classes.py` & `finalcif-121/finalcif/gui/custom_classes.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/dialogs.py` & `finalcif-121/finalcif/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/equipmenttable.py` & `finalcif-121/finalcif/gui/equipmenttable.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/file_editor.py` & `finalcif-121/finalcif/gui/file_editor.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/finalcif_gui_ui.py` & `finalcif-121/finalcif/gui/finalcif_gui_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/finalcif_gui_ui.ui` & `finalcif-121/finalcif/gui/finalcif_gui_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/loop_creator.py` & `finalcif-121/finalcif/gui/loop_creator.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/loop_creator_ui.py` & `finalcif-121/finalcif/gui/loop_creator_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/loop_creator_ui.ui` & `finalcif-121/finalcif/gui/loop_creator_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/loops.py` & `finalcif-121/finalcif/gui/loops.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/mainstackwidget.py` & `finalcif-121/finalcif/gui/mainstackwidget.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/mixins.py` & `finalcif-121/finalcif/gui/mixins.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/new_key_dialog.py` & `finalcif-121/finalcif/gui/new_key_dialog.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/new_key_dialog_ui.py` & `finalcif-121/finalcif/gui/new_key_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/new_key_dialog_ui.ui` & `finalcif-121/finalcif/gui/new_key_dialog_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/plaintextedit.py` & `finalcif-121/finalcif/gui/plaintextedit.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         menu.addSeparator()
         action_template = menu.addAction("Text Template")
         new_key = menu.addAction('Add new CIF keys')
         action_copy_vhead.triggered.connect(self.copy_vhead_item)
         action_template.triggered.connect(self._on_create_template)
         deleterow.triggered.connect(self._delete_row)
         new_key.triggered.connect(self._add_cif_keys)
-        choosed_action = menu.exec(event.globalPos())
+        menu.exec(event.globalPos())
 
     def _add_cif_keys(self):
         new_key = NewKey(self)
         new_key.show()
         new_key.new_key_added.connect(lambda x: self.new_key.emit(x))
 
     def _on_create_template(self):
```

### Comparing `finalcif-120/finalcif/gui/playground.py` & `finalcif-121/finalcif/gui/playground.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/propertytable.py` & `finalcif-121/finalcif/gui/propertytable.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/gui/text_templates_ui.py` & `finalcif-121/finalcif/gui/text_templates_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         sizePolicy.setHeightForWidth(self.combinedTestGroupBox.sizePolicy().hasHeightForWidth())
         self.combinedTestGroupBox.setSizePolicy(sizePolicy)
         self.combinedTestGroupBox.setObjectName("combinedTestGroupBox")
         self.verticalLayout_4 = QtWidgets.QVBoxLayout(self.combinedTestGroupBox)
         self.verticalLayout_4.setContentsMargins(12, 6, 12, 6)
         self.verticalLayout_4.setSpacing(6)
         self.verticalLayout_4.setObjectName("verticalLayout_4")
-        self.plainTextEdit = QtWidgets.QPlainTextEdit(self.combinedTestGroupBox)
+        self.plainTextEdit = SpellTextEdit(self.combinedTestGroupBox)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.plainTextEdit.sizePolicy().hasHeightForWidth())
         self.plainTextEdit.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
         font.setPointSize(10)
@@ -136,14 +136,15 @@
         self.plainTextEdit.setPlaceholderText(_translate("TextTemplatesWidget", "The text of the selected templates is added here in the order of selection."))
         self.applyTextPushButton.setText(_translate("TextTemplatesWidget", "Apply Text"))
         self.cancelTextPushButton.setText(_translate("TextTemplatesWidget", "Cancel"))
         self.savePushButton.setText(_translate("TextTemplatesWidget", "Save as Template"))
         self.importPushButton.setText(_translate("TextTemplatesWidget", "Import Template"))
         self.exportTextPushButton.setText(_translate("TextTemplatesWidget", "Export to CIF"))
         self.deletePushButton.setText(_translate("TextTemplatesWidget", "Delete Template"))
+from finalcif.gui.spell_check_edit import SpellTextEdit
 
 
 if __name__ == "__main__":
     import sys
     app = QtWidgets.QApplication(sys.argv)
     TextTemplatesWidget = QtWidgets.QWidget()
     ui = Ui_TextTemplatesWidget()
```

### Comparing `finalcif-120/finalcif/gui/text_templates_ui.ui` & `finalcif-121/finalcif/gui/text_templates_ui.ui`

 * *Files 3% similar despite different names*

#### Comparing `finalcif-120/finalcif/gui/text_templates_ui.ui` & `finalcif-121/finalcif/gui/text_templates_ui.ui`

```diff
@@ -163,15 +163,15 @@
                 <property name="rightMargin">
                   <number>12</number>
                 </property>
                 <property name="bottomMargin">
                   <number>6</number>
                 </property>
                 <item>
-                  <widget class="QPlainTextEdit" name="plainTextEdit">
+                  <widget class="SpellTextEdit" name="plainTextEdit">
                     <property name="sizePolicy">
                       <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
                         <horstretch>0</horstretch>
                         <verstretch>0</verstretch>
                       </sizepolicy>
                     </property>
                     <property name="font">
@@ -268,10 +268,17 @@
               </property>
             </widget>
           </item>
         </layout>
       </item>
     </layout>
   </widget>
+  <customwidgets>
+    <customwidget>
+      <class>SpellTextEdit</class>
+      <extends>QPlainTextEdit</extends>
+      <header>finalcif.gui.spell_check_edit.h</header>
+    </customwidget>
+  </customwidgets>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `finalcif-120/finalcif/gui/text_value_editor.py` & `finalcif-121/finalcif/gui/text_value_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Tuple, List, Union
 
 from PyQt5.QtCore import QSize, Qt, pyqtSignal
 from PyQt5.QtWidgets import QWidget, QHBoxLayout, QCheckBox, QApplication, QPlainTextEdit, \
     QListWidgetItem, QVBoxLayout, QLabel
 
 from finalcif.gui import text_templates_ui
+from finalcif.gui.spell_check_edit import SpellTextEdit
 
 
 # print('Compiling textedit ui ...')
 # application_path = Path(os.path.abspath(__file__)).parent.parent
 # uic.compileUiDir(os.path.join(application_path, 'gui'))
 
 
@@ -24,15 +25,15 @@
         super().__init__(parent)
         layout = QHBoxLayout(self)
         self.vlayout = QVBoxLayout()
         self.vlayout.setAlignment(Qt.AlignVCenter)
         self.checkbox = QCheckBox()
         self.number_label = QLabel()
         self.vlayout.addWidget(self.number_label)
-        self.textfield = QPlainTextEdit(self)
+        self.textfield = SpellTextEdit(self)
         font = self.textfield.font()
         font.setPixelSize(12)
         self.textfield.setFont(font)
         self.vlayout.addWidget(self.checkbox)
         layout.addLayout(self.vlayout)
         layout.addWidget(self.textfield)
         layout.setContentsMargins(12, 8, 30, 8)
```

### Comparing `finalcif-120/finalcif/gui/vrf_classes.py` & `finalcif-121/finalcif/gui/vrf_classes.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/icon/finalcif.png` & `finalcif-121/finalcif/icon/finalcif.png`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/icon/finalcif2.ico` & `finalcif-121/finalcif/icon/finalcif2.ico`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/icon/finalcif2.png` & `finalcif-121/finalcif/icon/finalcif2.png`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/icon/multitable.ico` & `finalcif-121/finalcif/icon/multitable.ico`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/icon/multitable.png` & `finalcif-121/finalcif/icon/multitable.png`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/icon/multitable.xcf` & `finalcif-121/finalcif/icon/multitable.xcf`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/report/archive_report.py` & `finalcif-121/finalcif/report/archive_report.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/report/mtools.py` & `finalcif-121/finalcif/report/mtools.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/report/references.py` & `finalcif-121/finalcif/report/references.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/report/report_text.py` & `finalcif-121/finalcif/report/report_text.py`

 * *Files 4% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             saintversion = integration.split()[1]
         integration_prog = 'SAINT'
         data_reduct_ref = SAINTReference('SAINT', saintversion)
         return data_reduct_ref, integration_prog
 
     def add_x_red_reference(self, integration):
         xredversion = 'unknown version'
-        #if len(integration.split()) > 1:
+        # if len(integration.split()) > 1:
         #    xredversion = integration.split()[1]
         integration_prog = 'STOE X-RED'
         data_reduct_ref = XRedReference('X-RED', xredversion)
         return data_reduct_ref, integration_prog
 
     def add_crysalispro_reference(self, integration: str) -> Tuple[CrysalisProReference, CrysalisProReference, str]:
         """
@@ -439,15 +439,37 @@
             dsr_sentence = "Some parts of the disorder model were introduced by the " \
                            "program DSR."
             paragraph.add_run(dsr_sentence)
             reflist.append([DSRReference2015(), DSRReference2018()])
             SpaceChar(paragraph).regular()
 
 
-class SpaceChar(object):
+class Twinning():
+    def __init__(self, cif: CifContainer, paragraph: Paragraph, reflist: ReferenceList):
+        """ _twin_formation_mechanism         gt
+            _twin_dimensionality              triperiodic
+            _twin_morphology                  polysynthetic
+            _twin_special_details             'The data was integrated as a 2-component twin.'
+            _twin_individual_id               2
+            _twin_individual_twin_matrix_11   -0.00018
+            _twin_individual_twin_matrix_12   -0.00091
+            _twin_individual_twin_matrix_13   -0.9998
+            _twin_individual_twin_matrix_21   0.99999
+            _twin_individual_twin_matrix_22   -0.26475
+            _twin_individual_twin_matrix_23   -0.36925
+            _twin_individual_twin_matrix_31   0.00018
+            _twin_individual_twin_matrix_32   -1.00019
+            _twin_individual_twin_matrix_33   0.00187
+        """
+        twining = cif['_twin_individual_id']
+        if twining:
+            sentence = f''
+
+
+class SpaceChar():
     def __init__(self, paragraph: Paragraph):
         self.p = paragraph
 
     def regular(self) -> None:
         self.p.add_run(' ')
 
     def protected(self):
```

### Comparing `finalcif-120/finalcif/report/symm.py` & `finalcif-121/finalcif/report/symm.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/report/tables.py` & `finalcif-121/finalcif/report/tables.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/report/templated_report.py` & `finalcif-121/finalcif/report/templated_report.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/report/gui/mainwindow.py` & `finalcif-121/finalcif/report/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/report/gui/mainwindow.ui` & `finalcif-121/finalcif/report/gui/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/template/mathml2omml.xsl` & `finalcif-121/finalcif/template/mathml2omml.xsl`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/template/template1.docx` & `finalcif-121/finalcif/template/template1.docx`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/template/template_text.docx` & `finalcif-121/finalcif/template/template_text.docx`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/template/template_without_text.docx` & `finalcif-121/finalcif/template/template_without_text.docx`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/template/templates.py` & `finalcif-121/finalcif/template/templates.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/tools/download.py` & `finalcif-121/finalcif/tools/download.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/tools/dsrmath.py` & `finalcif-121/finalcif/tools/dsrmath.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/tools/misc.py` & `finalcif-121/finalcif/tools/misc.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/tools/options.py` & `finalcif-121/finalcif/tools/options.py`

 * *Files 20% similar despite different names*

```diff
@@ -54,60 +54,47 @@
             'track_changes'          : self.ui.trackChangesCifCheckBox.isChecked(),
         }
         # print('saving:', self._options)
         self.settings.save_options(self._options)
 
     @property
     def values(self):
-        # print('loading:', self._options, self.settings.load_options())
         return self.settings.load_options()
 
     def __getitem__(self, item):
         return self.settings.load_options()[item]
 
+    def _get_setting(self, setting: str, default: object):
+        with suppress(KeyError):
+            return self.settings.load_options()[setting]
+        return default
+
     @property
     def report_text(self) -> bool:
-        try:
-            return self.settings.load_options()['report_text']
-        except KeyError:
-            return True
+        return self._get_setting('report_text', True)
 
     @property
     def report_adp(self) -> bool:
-        with suppress(KeyError):
-            return self.settings.load_options()['report_adp']
-        return True
+        return self._get_setting('report_adp', True)
 
     @property
     def without_h(self) -> bool:
-        try:
-            return self.settings.load_options()['without_h']
-        except KeyError:
-            return False
+        return self._get_setting('without_h', False)
 
     @property
     def track_changes(self) -> bool:
-        try:
-            return self.settings.load_options()['track_changes']
-        except KeyError:
-            return False
+        return self._get_setting('track_changes', False)
 
     @property
     def current_template(self) -> int:
-        try:
-            return self.settings.load_options()['current_report_template']
-        except KeyError:
-            return 0
+        return self._get_setting('current_report_template', 0)
 
     @property
     def picture_width(self) -> float:
-        try:
-            width = self.settings.load_options()['picture_width']
-        except KeyError:
-            return 7.5
+        width = self._get_setting('picture_width', 7.5)
         if width < 0.001:
             # preventing invisible picture
             return 7.5
         else:
             return width
 
     @property
```

### Comparing `finalcif-120/finalcif/tools/platon.py` & `finalcif-121/finalcif/tools/platon.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/tools/pupdate.py` & `finalcif-121/finalcif/tools/pupdate.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/tools/settings.py` & `finalcif-121/finalcif/tools/settings.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/tools/shred.py` & `finalcif-121/finalcif/tools/shred.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/tools/space_groups.py` & `finalcif-121/finalcif/tools/space_groups.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/tools/spgr_format.py` & `finalcif-121/finalcif/tools/spgr_format.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/tools/statusbar.py` & `finalcif-121/finalcif/tools/statusbar.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/finalcif/tools/sumformula.py` & `finalcif-121/finalcif/tools/sumformula.py`

 * *Files identical despite different names*

### Comparing `finalcif-120/.gitignore` & `finalcif-121/.gitignore`

 * *Files identical despite different names*

### Comparing `finalcif-120/README.md` & `finalcif-121/README.md`

 * *Files identical despite different names*

### Comparing `finalcif-120/pyproject.toml` & `finalcif-121/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "finalcif"
-version = "120"
+version = "121"
 authors = [
     { name = "Daniel Kratzert", email = "dkratzert@gmx.de" },
 ]
 description = "CIF file editor"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -39,14 +39,15 @@
     'QtPy',
     'requests',
     'urllib3~=1.26',
     'docxtpl',
     'shelxfile',
     'crossrefapi',
     'numpy',
+    'pyenchant',
 ]
 
 [project.urls]
 "Homepage" = "https://dkratzert.de/finalcif.html"
 "Bug Tracker" = "https://github.com/dkratzert/FinalCif/issues"
 
 [tool.hatch.build.targets.sdist]
```

### Comparing `finalcif-120/PKG-INFO` & `finalcif-121/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalcif
-Version: 120
+Version: 121
 Summary: CIF file editor
 Project-URL: Homepage, https://dkratzert.de/finalcif.html
 Project-URL: Bug Tracker, https://github.com/dkratzert/FinalCif/issues
 Author-email: Daniel Kratzert <dkratzert@gmx.de>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +20,15 @@
 Requires-Dist: future
 Requires-Dist: gemmi
 Requires-Dist: html2text
 Requires-Dist: lxml
 Requires-Dist: numpy
 Requires-Dist: pefile
 Requires-Dist: pybind11
+Requires-Dist: pyenchant
 Requires-Dist: pyqt5-sip~=12.11
 Requires-Dist: pyqt5~=5.15
 Requires-Dist: pyqtwebengine~=5.15
 Requires-Dist: python-docx~=0.8
 Requires-Dist: pywin32-ctypes~=0.2
 Requires-Dist: qtawesome
 Requires-Dist: qtpy
```

#### html2text {}

```diff
@@ -1,42 +1,43 @@
-Metadata-Version: 2.1 Name: finalcif Version: 120 Summary: CIF file editor
+Metadata-Version: 2.1 Name: finalcif Version: 121 Summary: CIF file editor
 Project-URL: Homepage, https://dkratzert.de/finalcif.html Project-URL: Bug
 Tracker, https://github.com/dkratzert/FinalCif/issues Author-email: Daniel
 Kratzert
 gmx.de> License-File: LICENSE Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Chemistry Requires-Python: >=3.9
 Requires-Dist: altgraph Requires-Dist: certifi Requires-Dist: chardet Requires-
 Dist: crossrefapi Requires-Dist: docxtpl Requires-Dist: future Requires-Dist:
 gemmi Requires-Dist: html2text Requires-Dist: lxml Requires-Dist: numpy
-Requires-Dist: pefile Requires-Dist: pybind11 Requires-Dist: pyqt5-sip~=12.11
-Requires-Dist: pyqt5~=5.15 Requires-Dist: pyqtwebengine~=5.15 Requires-Dist:
-python-docx~=0.8 Requires-Dist: pywin32-ctypes~=0.2 Requires-Dist: qtawesome
-Requires-Dist: qtpy Requires-Dist: requests Requires-Dist: shelxfile Requires-
-Dist: urllib3~=1.26 Requires-Dist: wheel Description-Content-Type: text/
-markdown ![Lates Release](https://img.shields.io/github/v/tag/dkratzert/
-FinalCif?label=Release) [![Unit Tests](https://github.com/dkratzert/FinalCif/
-actions/workflows/python-app_windows.yml/badge.svg?branch=master)](https://
-github.com/dkratzert/FinalCif/actions/workflows/python-app_windows.yml) !
-[Contributions](https://img.shields.io/badge/contributions-welcome-blue) [!
-[PyPI package](https://repology.org/badge/version-for-repo/pypi/python:
-finalcif.svg)](https://repology.org/project/python:finalcif/versions)
-[Packaging_status] # FinalCif FinalCif helps you to get a complete [CIF](https:
-//www.iucr.org/resources/cif) file from a single-xrystal X-ray diffraction
-experiment. See here [https://dkratzert.de/finalcif.html](https://dkratzert.de/
-finalcif.html) for details. For tables from multiple CIF files, you may want to
-use the program [multitable](https://github.com/dkratzert/multitable). **Report
-templates** You only need them if you want to make report tables that differ
-from the default ones. - [A template with everything in](https://github.com/
-dkratzert/FinalCif/raw/master/finalcif/template/template_text.docx) - [A
-template without the report text](https://github.com/dkratzert/FinalCif/raw/
-master/finalcif/template/template_without_text.docx) **Some screenshots**
-(click to enlarge) ![FinalCif main Window](https://github.com/dkratzert/
-FinalCif/raw/master/screenshots/finalcif_main.png) ![FinalCif details](https://
-github.com/dkratzert/FinalCif/raw/master/screenshots/finalcif_details.png) !
-[FinalCif report](https://github.com/dkratzert/FinalCif/raw/master/screenshots/
+Requires-Dist: pefile Requires-Dist: pybind11 Requires-Dist: pyenchant
+Requires-Dist: pyqt5-sip~=12.11 Requires-Dist: pyqt5~=5.15 Requires-Dist:
+pyqtwebengine~=5.15 Requires-Dist: python-docx~=0.8 Requires-Dist: pywin32-
+ctypes~=0.2 Requires-Dist: qtawesome Requires-Dist: qtpy Requires-Dist:
+requests Requires-Dist: shelxfile Requires-Dist: urllib3~=1.26 Requires-Dist:
+wheel Description-Content-Type: text/markdown ![Lates Release](https://
+img.shields.io/github/v/tag/dkratzert/FinalCif?label=Release) [![Unit Tests]
+(https://github.com/dkratzert/FinalCif/actions/workflows/python-
+app_windows.yml/badge.svg?branch=master)](https://github.com/dkratzert/
+FinalCif/actions/workflows/python-app_windows.yml) ![Contributions](https://
+img.shields.io/badge/contributions-welcome-blue) [![PyPI package](https://
+repology.org/badge/version-for-repo/pypi/python:finalcif.svg)](https://
+repology.org/project/python:finalcif/versions) [Packaging_status] # FinalCif
+FinalCif helps you to get a complete [CIF](https://www.iucr.org/resources/cif)
+file from a single-xrystal X-ray diffraction experiment. See here [https://
+dkratzert.de/finalcif.html](https://dkratzert.de/finalcif.html) for details.
+For tables from multiple CIF files, you may want to use the program
+[multitable](https://github.com/dkratzert/multitable). **Report templates** You
+only need them if you want to make report tables that differ from the default
+ones. - [A template with everything in](https://github.com/dkratzert/FinalCif/
+raw/master/finalcif/template/template_text.docx) - [A template without the
+report text](https://github.com/dkratzert/FinalCif/raw/master/finalcif/
+template/template_without_text.docx) **Some screenshots** (click to enlarge) !
+[FinalCif main Window](https://github.com/dkratzert/FinalCif/raw/master/
+screenshots/finalcif_main.png) ![FinalCif details](https://github.com/
+dkratzert/FinalCif/raw/master/screenshots/finalcif_details.png) ![FinalCif
+report](https://github.com/dkratzert/FinalCif/raw/master/screenshots/
 finalcif_report.png) ![FinalCif CheckCIF](https://github.com/dkratzert/
 FinalCif/raw/master/screenshots/finalcif_checkcif.png) ![FinalCif responses]
 (https://github.com/dkratzert/FinalCif/raw/master/screenshots/
 finalcif_responses.png) ![FinalCif responses](https://github.com/dkratzert/
 FinalCif/raw/master/screenshots/finalcif_loops.png)
```

