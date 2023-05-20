# Comparing `tmp/finalcif-119.tar.gz` & `tmp/finalcif-120.tar.gz`

## Comparing `finalcif-119.tar` & `finalcif-120.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 finalcif-119/finalcif/__init__.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 finalcif-119/finalcif/app_path.py
--rw-r--r--   0        0        0    91866 2020-02-02 00:00:00.000000 finalcif-119/finalcif/appwindow.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 finalcif-119/finalcif/finalcif_start.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/__init__.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/all_cif_dicts.py
--rw-r--r--   0        0        0    18681 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/atoms.py
--rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cif_dict_foo.py
--rw-r--r--   0        0        0    38969 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cif_file_io.py
--rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cif_order.py
--rw-r--r--   0        0        0   484078 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/core_dict.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/hkl.py
--rw-r--r--   0        0        0  1041931 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/modulation_dict.py
--rw-r--r--   0        0        0   221592 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/powder_dict.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/reference.py
--rw-r--r--   0        0        0   106774 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/restraints_dict.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/text.py
--rw-r--r--   0        0        0    21412 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/twin_dict.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/checkcif/__init__.py
--rw-r--r--   0        0        0    10770 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/checkcif/checkcif.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cod/__init__.py
--rw-r--r--   0        0        0    18635 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cod/deposit.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cod/deposit_check.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cod/deposition_list.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cod/doi.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cod/upload.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cod/website_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/__init__.py
--rw-r--r--   0        0        0    12742 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/bruker_data.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/bruker_frame.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/ccdc_mail.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/data.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/p4p_reader.py
--rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/sadabs.py
--rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/saint.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/shelx_lst.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/displaymol/__init__.py
--rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 finalcif-119/finalcif/displaymol/molecule2D.py
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 finalcif-119/finalcif/displaymol/sdm.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 finalcif-119/finalcif/displaymol/vtk_molecule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/equip_property/__init__.py
--rw-r--r--   0        0        0    21598 2020-02-02 00:00:00.000000 finalcif-119/finalcif/equip_property/author_loop_templates.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 finalcif-119/finalcif/equip_property/equipment.py
--rw-r--r--   0        0        0    13453 2020-02-02 00:00:00.000000 finalcif-119/finalcif/equip_property/properties.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 finalcif-119/finalcif/equip_property/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/__init__.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/combobox.py
--rw-r--r--   0        0        0    10994 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/custom_classes.py
--rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/dialogs.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/equipmenttable.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/file_editor.py
--rw-r--r--   0        0        0   162120 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/finalcif_gui_ui.py
--rw-r--r--   0        0        0   187031 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/finalcif_gui_ui.ui
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/loop_creator.py
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/loop_creator_ui.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/loop_creator_ui.ui
--rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/loops.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/mainstackwidget.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/mixins.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/new_key_dialog.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/new_key_dialog_ui.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/new_key_dialog_ui.ui
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/plaintextedit.py
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/playground.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/propertytable.py
--rw-r--r--   0        0        0     9358 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/text_templates_ui.py
--rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/text_templates_ui.ui
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/text_value_editor.py
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/vrf_classes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/icon/__init__.py
--rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 finalcif-119/finalcif/icon/finalcif.png
--rw-r--r--   0        0        0    25352 2020-02-02 00:00:00.000000 finalcif-119/finalcif/icon/finalcif2.ico
--rw-r--r--   0        0        0    17091 2020-02-02 00:00:00.000000 finalcif-119/finalcif/icon/finalcif2.png
--rw-r--r--   0        0        0   103782 2020-02-02 00:00:00.000000 finalcif-119/finalcif/icon/multitable.ico
--rw-r--r--   0        0        0    17746 2020-02-02 00:00:00.000000 finalcif-119/finalcif/icon/multitable.png
--rw-r--r--   0        0        0   124043 2020-02-02 00:00:00.000000 finalcif-119/finalcif/icon/multitable.xcf
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/archive_report.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/mtools.py
--rw-r--r--   0        0        0    18509 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/references.py
--rw-r--r--   0        0        0    22298 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/report_text.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/symm.py
--rw-r--r--   0        0        0    37156 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/tables.py
--rw-r--r--   0        0        0    26776 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/templated_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/gui/__init__.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/gui/mainwindow.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/gui/mainwindow.ui
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/template/__init__.py
--rw-r--r--   0        0        0   151706 2020-02-02 00:00:00.000000 finalcif-119/finalcif/template/mathml2omml.xsl
--rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 finalcif-119/finalcif/template/template1.docx
--rw-r--r--   0        0        0    35411 2020-02-02 00:00:00.000000 finalcif-119/finalcif/template/template_text.docx
--rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 finalcif-119/finalcif/template/template_without_text.docx
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 finalcif-119/finalcif/template/templates.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/__init__.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/download.py
--rw-r--r--   0        0        0    43454 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/dsrmath.py
--rw-r--r--   0        0        0    32789 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/misc.py
--rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/options.py
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/platon.py
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/pupdate.py
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/settings.py
--rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/shred.py
--rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/space_groups.py
--rw-r--r--   0        0        0   137178 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/spgr_format.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/statusbar.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/sumformula.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 finalcif-119/.gitignore
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 finalcif-119/LICENSE
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 finalcif-119/README.md
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 finalcif-119/pyproject.toml
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 finalcif-119/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 finalcif-120/finalcif/__init__.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 finalcif-120/finalcif/app_path.py
+-rw-r--r--   0        0        0    92019 2020-02-02 00:00:00.000000 finalcif-120/finalcif/appwindow.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 finalcif-120/finalcif/finalcif_start.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/__init__.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/all_cif_dicts.py
+-rw-r--r--   0        0        0    18681 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/atoms.py
+-rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cif_dict_foo.py
+-rw-r--r--   0        0        0    38969 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cif_file_io.py
+-rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cif_order.py
+-rw-r--r--   0        0        0   484078 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/core_dict.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/hkl.py
+-rw-r--r--   0        0        0  1041931 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/modulation_dict.py
+-rw-r--r--   0        0        0   221592 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/powder_dict.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/reference.py
+-rw-r--r--   0        0        0   106774 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/restraints_dict.py
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/text.py
+-rw-r--r--   0        0        0    21412 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/twin_dict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/checkcif/__init__.py
+-rw-r--r--   0        0        0    10770 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/checkcif/checkcif.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cod/__init__.py
+-rw-r--r--   0        0        0    18635 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cod/deposit.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cod/deposit_check.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cod/deposition_list.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cod/doi.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cod/upload.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 finalcif-120/finalcif/cif/cod/website_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/__init__.py
+-rw-r--r--   0        0        0    12742 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/bruker_data.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/bruker_frame.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/ccdc_mail.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/data.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/p4p_reader.py
+-rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/sadabs.py
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/saint.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/shelx_lst.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 finalcif-120/finalcif/datafiles/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/displaymol/__init__.py
+-rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 finalcif-120/finalcif/displaymol/molecule2D.py
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 finalcif-120/finalcif/displaymol/sdm.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 finalcif-120/finalcif/displaymol/vtk_molecule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/equip_property/__init__.py
+-rw-r--r--   0        0        0    21598 2020-02-02 00:00:00.000000 finalcif-120/finalcif/equip_property/author_loop_templates.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 finalcif-120/finalcif/equip_property/equipment.py
+-rw-r--r--   0        0        0    13453 2020-02-02 00:00:00.000000 finalcif-120/finalcif/equip_property/properties.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 finalcif-120/finalcif/equip_property/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/__init__.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/combobox.py
+-rw-r--r--   0        0        0    11048 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/custom_classes.py
+-rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/dialogs.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/equipmenttable.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/file_editor.py
+-rw-r--r--   0        0        0   162120 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/finalcif_gui_ui.py
+-rw-r--r--   0        0        0   187031 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/finalcif_gui_ui.ui
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/loop_creator.py
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/loop_creator_ui.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/loop_creator_ui.ui
+-rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/loops.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/mainstackwidget.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/mixins.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/new_key_dialog.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/new_key_dialog_ui.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/new_key_dialog_ui.ui
+-rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/plaintextedit.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/playground.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/propertytable.py
+-rw-r--r--   0        0        0     9358 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/text_templates_ui.py
+-rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/text_templates_ui.ui
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/text_value_editor.py
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 finalcif-120/finalcif/gui/vrf_classes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/icon/__init__.py
+-rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 finalcif-120/finalcif/icon/finalcif.png
+-rw-r--r--   0        0        0    25352 2020-02-02 00:00:00.000000 finalcif-120/finalcif/icon/finalcif2.ico
+-rw-r--r--   0        0        0    17091 2020-02-02 00:00:00.000000 finalcif-120/finalcif/icon/finalcif2.png
+-rw-r--r--   0        0        0   103782 2020-02-02 00:00:00.000000 finalcif-120/finalcif/icon/multitable.ico
+-rw-r--r--   0        0        0    17746 2020-02-02 00:00:00.000000 finalcif-120/finalcif/icon/multitable.png
+-rw-r--r--   0        0        0   124043 2020-02-02 00:00:00.000000 finalcif-120/finalcif/icon/multitable.xcf
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/archive_report.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/mtools.py
+-rw-r--r--   0        0        0    19119 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/references.py
+-rw-r--r--   0        0        0    23568 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/report_text.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/symm.py
+-rw-r--r--   0        0        0    37156 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/tables.py
+-rw-r--r--   0        0        0    26709 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/templated_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/gui/__init__.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/gui/mainwindow.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 finalcif-120/finalcif/report/gui/mainwindow.ui
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/template/__init__.py
+-rw-r--r--   0        0        0   151706 2020-02-02 00:00:00.000000 finalcif-120/finalcif/template/mathml2omml.xsl
+-rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 finalcif-120/finalcif/template/template1.docx
+-rw-r--r--   0        0        0    35411 2020-02-02 00:00:00.000000 finalcif-120/finalcif/template/template_text.docx
+-rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 finalcif-120/finalcif/template/template_without_text.docx
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 finalcif-120/finalcif/template/templates.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/__init__.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/download.py
+-rw-r--r--   0        0        0    43454 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/dsrmath.py
+-rw-r--r--   0        0        0    32788 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/misc.py
+-rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/options.py
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/platon.py
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/pupdate.py
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/settings.py
+-rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/shred.py
+-rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/space_groups.py
+-rw-r--r--   0        0        0   137178 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/spgr_format.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/statusbar.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 finalcif-120/finalcif/tools/sumformula.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 finalcif-120/.gitignore
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 finalcif-120/LICENSE
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 finalcif-120/README.md
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 finalcif-120/pyproject.toml
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 finalcif-120/PKG-INFO
```

### Comparing `finalcif-119/finalcif/app_path.py` & `finalcif-120/finalcif/app_path.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/appwindow.py` & `finalcif-120/finalcif/appwindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -498,18 +498,21 @@
 
     def apply_text_template(self) -> None:
         """
         Use text from self.textedit.ui.plainTextEdit and fill it into current cell. Then go back to
         main table. And scroll to changed row.
         """
         text = self.textedit.ui.plainTextEdit.toPlainText()
-        TextEditItem._num = 1
-        self.ui.cif_main_table.setText(key=self.textedit.cif_key, column =Column.EDIT, txt=text)
-        self.ui.MainStackedWidget.got_to_main_page()
-        self.textedit.clear_fields()
+        if text:
+            TextEditItem._num = 1
+            self.ui.cif_main_table.setText(key=self.textedit.cif_key, column=Column.EDIT, txt=text)
+            self.ui.MainStackedWidget.got_to_main_page()
+            self.textedit.clear_fields()
+        else:
+            self.status_bar.show_message('No combined text to apply.')
 
     def toggle_hkl_option(self, iucr_is_checked: bool) -> None:
         if iucr_is_checked:
             self.ui.structfactCheckBox.setChecked(False)
 
     def toggle_iucr_option(self, hkl_is_checked: bool):
         if hkl_is_checked:
@@ -529,15 +532,15 @@
                 Path(filename).write_bytes(r.content)
                 r.close()
                 self.load_cif_file(Path(filename))
             else:
                 #self.ui.SelectCif_LineEdit.setText('')
                 self.status_bar.show_message(f'No COD entry for {input_txt} found.')
         else:
-            self.status_bar.show_message(f'Not a valid COD number. It must be seven digits.')
+            self.status_bar.show_message('Not a valid COD number. It must be seven digits.')
 
     @property
     def current_block(self) -> int:
         return self.ui.datanameComboBox.currentIndex()
 
     def open_cod_page(self) -> None:
         self.save_current_cif_file()
@@ -616,15 +619,15 @@
         changes_cif.save(self.finalcif_changes_filename)
 
     def check_for_update_version(self) -> None:
         if os.environ.get('NO_NETWORK'):
             print('Skipping version.txt download because NO_NETWORK variable is set.')
             return
         mainurl = "https://dkratzert.de/files/finalcif/version.txt"
-        self.upd = MyDownloader(mainurl)
+        self.upd = MyDownloader(mainurl, parent=self)
         version_thread = QThread()
         self.threadpool.append(version_thread)
         start_worker(self.upd, version_thread, onload=self.is_update_necessary)
 
     def is_update_necessary(self, content: bytes) -> None:
         """
         Reads the reply from the server and displays a warning in case of an old version.
@@ -686,16 +689,16 @@
         """
         Sends a get request to the platon server in order to get the current check.def file.
         """
         if os.environ.get('NO_NETWORK'):
             print('Skipping check.def download because NO_NETWORK variable is set.')
             return
         url = 'http://www.platonsoft.nl/xraysoft/unix/platon/check.def'
-        self.updc = MyDownloader(url)
-        checkdef_thread = QThread()
+        self.updc = MyDownloader(url, parent=self)
+        checkdef_thread = QThread(parent=self)
         self.threadpool.append(checkdef_thread)
         start_worker(self.updc, checkdef_thread, onload=self._save_checkdef)
 
     def _save_checkdef(self, reply: bytes) -> None:
         """
         Is called by the finished signal from the downloader.
         """
```

### Comparing `finalcif-119/finalcif/finalcif_start.py` & `finalcif-120/finalcif/finalcif_start.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,12 +53,12 @@
     # windows_style = QStyleFactory.create('Fusion')
     # app.setStyle(windows_style)
     w = AppWindow()
     app.setWindowIcon(QIcon(os.path.join(application_path, r'icon/finalcif2.png')))
     w.setWindowTitle('FinalCif v{}'.format(VERSION))
     # w.showMaximized()  # For full screen view
     w.setBaseSize(1200, 780)
-    sys.exit(app.exec_())
+    sys.exit(app.exec())
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `finalcif-119/finalcif/cif/all_cif_dicts.py` & `finalcif-120/finalcif/cif/all_cif_dicts.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/atoms.py` & `finalcif-120/finalcif/cif/atoms.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/cif_dict_foo.py` & `finalcif-120/finalcif/cif/cif_dict_foo.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/cif_file_io.py` & `finalcif-120/finalcif/cif/cif_file_io.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/cif_order.py` & `finalcif-120/finalcif/cif/cif_order.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/core_dict.py` & `finalcif-120/finalcif/cif/core_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/hkl.py` & `finalcif-120/finalcif/cif/hkl.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/modulation_dict.py` & `finalcif-120/finalcif/cif/modulation_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/powder_dict.py` & `finalcif-120/finalcif/cif/powder_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/reference.py` & `finalcif-120/finalcif/cif/reference.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/restraints_dict.py` & `finalcif-120/finalcif/cif/restraints_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/text.py` & `finalcif-120/finalcif/cif/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,21 @@
     Quotes a cif string and wraps it. The shorter strings are directly handled by cif.quote().
     """
     if len(string) < 80:
         return gemmi.cif.quote(string)
     lines = ''
     for line in string.split('\n'):
         if len(line) > wrapping:
-            line = textwrap.fill(line, width=wrapping)
+            line = textwrap.fill(line, width=wrapping, drop_whitespace=False)
         lines += f'{line}\n'
     quoted = gemmi.cif.quote(lines.rstrip('\n'))
     return quoted
 
 
-charcters = {
+characters = {
     '—'      : r'--',
     '±'      : r'+-',
     '×'      : r'\\times',
     '≠'      : r'\\neq',
     '→'      : r'\\rightarrow',
     '←'      : r'\\leftarrow',
     '∞'      : r'\\infty',
@@ -150,38 +150,41 @@
     u"\u00B0": r"\%",
     '·'      : r"{middle dot}",
     # "1̄": r'\=1',  # Does not work in QT?
 }
 
 false_characters_map = {
     # Fix for wrong characters in FinalCif prior to version 96:
+    # Removing it from 110, because there are no v96 users left.
     'ü': r'u\"',
     'Ü': r'U\"',
     'ö': r'o\"',
     'Ö': r'O\"',
     'ä': r'a\"',
     'Ä': r'A\"',
 }
 
 
 def invert_dict(input: dict) -> dict:
     return {v: k for k, v in input.items()}
 
 
-inverted_characters_map = invert_dict(charcters)
-inverted_characters_map.update(invert_dict(false_characters_map))
+inverted_characters_map = invert_dict(characters)
+
+# Removed, because it became obsolete
+# inverted_characters_map.update(invert_dict(false_characters_map))
 
 
 def utf8_to_str(txt: str) -> str:
     """
     Translates an utf-8 text to a CIF ascii string.
     """
     for char in txt:
-        if char in charcters:
-            txt = txt.replace(char, charcters[char])
+        if char in characters:
+            txt = txt.replace(char, characters[char])
     return utf8_to_html_ascii(txt)
 
 
 def delimit_string(txt: str) -> str:
     return utf8_to_str(txt)
```

### Comparing `finalcif-119/finalcif/cif/twin_dict.py` & `finalcif-120/finalcif/cif/twin_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/checkcif/checkcif.py` & `finalcif-120/finalcif/cif/checkcif/checkcif.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/cod/deposit.py` & `finalcif-120/finalcif/cif/cod/deposit.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/cod/deposit_check.py` & `finalcif-120/finalcif/cif/cod/deposit_check.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/cod/deposition_list.py` & `finalcif-120/finalcif/cif/cod/deposition_list.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/cod/doi.py` & `finalcif-120/finalcif/cif/cod/doi.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/cod/upload.py` & `finalcif-120/finalcif/cif/cod/upload.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/cif/cod/website_parser.py` & `finalcif-120/finalcif/cif/cod/website_parser.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/datafiles/bruker_data.py` & `finalcif-120/finalcif/datafiles/bruker_data.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/datafiles/bruker_frame.py` & `finalcif-120/finalcif/datafiles/bruker_frame.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/datafiles/ccdc_mail.py` & `finalcif-120/finalcif/datafiles/ccdc_mail.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/datafiles/data.py` & `finalcif-120/finalcif/datafiles/data.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/datafiles/p4p_reader.py` & `finalcif-120/finalcif/datafiles/p4p_reader.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/datafiles/sadabs.py` & `finalcif-120/finalcif/datafiles/sadabs.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/datafiles/saint.py` & `finalcif-120/finalcif/datafiles/saint.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/datafiles/shelx_lst.py` & `finalcif-120/finalcif/datafiles/shelx_lst.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/datafiles/utils.py` & `finalcif-120/finalcif/datafiles/utils.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/displaymol/molecule2D.py` & `finalcif-120/finalcif/displaymol/molecule2D.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/displaymol/sdm.py` & `finalcif-120/finalcif/displaymol/sdm.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/displaymol/vtk_molecule.py` & `finalcif-120/finalcif/displaymol/vtk_molecule.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/equip_property/author_loop_templates.py` & `finalcif-120/finalcif/equip_property/author_loop_templates.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/equip_property/equipment.py` & `finalcif-120/finalcif/equip_property/equipment.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/equip_property/properties.py` & `finalcif-120/finalcif/equip_property/properties.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/equip_property/tools.py` & `finalcif-120/finalcif/equip_property/tools.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/combobox.py` & `finalcif-120/finalcif/gui/combobox.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,17 +25,17 @@
         self.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Expanding)
         self.setEditable(True)  # only editable as new template
         self.installEventFilter(self)
         self.actionDelete = QAction("Delete Row", self)
         self.setContextMenuPolicy(Qt.ActionsContextMenu)
         self.addAction(self.actionDelete)
         self.actionDelete.triggered.connect(self._delete_row)
-        #action_template = QAction("Text Template", self)
-        #self.addAction(action_template)
-        #action_template.triggered.connect(self._on_create_template)
+        action_template = QAction("Text Template", self)
+        self.addAction(action_template)
+        action_template.triggered.connect(lambda: self.textTemplate.emit(self.row))
 
     def __str__(self):
         return self.currentText()
 
     @property
     def row(self) -> int:
         return self.parent.vheaderitems.index(self.cif_key)
@@ -56,12 +56,12 @@
         return QObject.eventFilter(self, widget, event)
 
     def setUneditable(self):
         # noinspection PyUnresolvedReferences
         self.setFlags(self.flags() ^ Qt.ItemIsEditable)
 
     def setText(self, txt: str):
-        self.setEditText('\n'.join(wrap(txt, width=30)))
+        self.setEditText('\n'.join(wrap(txt, width=80)))
 
     def addItem(self, *__args):
-        text = '\n'.join(wrap(__args[0], width=60))
-        super().addItem(text, __args[1])
+        text = '\n'.join(wrap(__args[0], width=80))
+        super().addItem(text, __args[1])
```

### Comparing `finalcif-119/finalcif/gui/custom_classes.py` & `finalcif-120/finalcif/gui/custom_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from finalcif.gui.combobox import MyComboBox
 from finalcif.gui.dialogs import show_keyword_help
 from finalcif.gui.mixins import ItemTextMixin
 from finalcif.gui.plaintextedit import MyQPlainTextEdit
 
 white = QColor(255, 255, 255)
 light_green = QColor(217, 255, 201)
-light_blue = QColor(193, 217, 247)
+light_blue = QColor(220, 232, 247)
 blue = QColor(102, 150, 179)
 yellow = QColor(250, 247, 150)  # #faf796
 
 
 class Column(IntEnum):
     CIF = 0
     DATA = 1
@@ -33,16 +33,17 @@
 
 class MyCifTable(QTableWidget, ItemTextMixin):
     row_deleted = QtCore.pyqtSignal(str)
     textTemplate = QtCore.pyqtSignal(int)
     new_key = QtCore.pyqtSignal(str)
 
     def __init__(self, parent: QWidget = None, *args, **kwargs):
-        self.parent = parent
         super().__init__(*args, **kwargs)
+        self.parent = parent
+        self.setAttribute(QtCore.Qt.WA_DeleteOnClose)
         self.setParent(parent)
         self.installEventFilter(self)
         self.setSizeAdjustPolicy(QAbstractScrollArea.AdjustToContents)
         self.setVerticalScrollBarPolicy(Qt.ScrollBarAsNeeded)
         self.setHorizontalScrollBarPolicy(Qt.ScrollBarAsNeeded)
         # item = MyTableWidgetItem()
         # self.setItemPrototype(item)
```

### Comparing `finalcif-119/finalcif/gui/dialogs.py` & `finalcif-120/finalcif/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/equipmenttable.py` & `finalcif-120/finalcif/gui/equipmenttable.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/file_editor.py` & `finalcif-120/finalcif/gui/file_editor.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/finalcif_gui_ui.py` & `finalcif-120/finalcif/gui/finalcif_gui_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/finalcif_gui_ui.ui` & `finalcif-120/finalcif/gui/finalcif_gui_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/loop_creator.py` & `finalcif-120/finalcif/gui/loop_creator.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/loop_creator_ui.py` & `finalcif-120/finalcif/gui/loop_creator_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/loop_creator_ui.ui` & `finalcif-120/finalcif/gui/loop_creator_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/loops.py` & `finalcif-120/finalcif/gui/loops.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/mainstackwidget.py` & `finalcif-120/finalcif/gui/mainstackwidget.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/mixins.py` & `finalcif-120/finalcif/gui/mixins.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/new_key_dialog.py` & `finalcif-120/finalcif/gui/new_key_dialog.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/new_key_dialog_ui.py` & `finalcif-120/finalcif/gui/new_key_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/new_key_dialog_ui.ui` & `finalcif-120/finalcif/gui/new_key_dialog_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/plaintextedit.py` & `finalcif-120/finalcif/gui/plaintextedit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from contextlib import suppress
 from functools import cache
 
 from PyQt5.QtCore import pyqtSignal, Qt, QObject, QEvent, QSize
-from PyQt5.QtGui import QTextOption, QFontMetrics, QContextMenuEvent, QFont
+from PyQt5.QtGui import QTextOption, QFontMetrics, QContextMenuEvent, QFont, QColor
 from PyQt5.QtWidgets import QPlainTextEdit, QFrame, QApplication, QAbstractScrollArea
 
 from finalcif.gui.new_key_dialog import NewKey
 
 with suppress(ImportError):
     from finalcif.gui.custom_classes import MyCifTable
 
@@ -17,16 +17,14 @@
     """
     templateRequested = pyqtSignal(int)
     new_key = pyqtSignal(str)
 
     def __init__(self, parent=None, *args, **kwargs):
         """
         Plaintext edit field for most of the table cells.
-        :param parent:
-        :param minheight: minimum height of the widget.
         """
         super().__init__(parent, *args, **kwargs)
         self.setParent(parent)
         self.cif_key = ''
         font = QFont()
         font.setPointSize(self.document().defaultFont().pointSize() + 1)
         self.setFont(font)
@@ -80,20 +78,20 @@
             clipboard = QApplication.clipboard()
             clipboard.setText(self.cif_key)
 
     @property
     def row(self) -> int:
         return self.parent.vheaderitems.index(self.cif_key)
 
-    def setBackground(self, color):
+    def setBackground(self, color: QColor) -> None:
         """
         Set background color of the text field.
         """
         self.setStyleSheet("background-color: {};".format(str(color.name())))
-        # No idea why tis does not work
+        # No idea why this does not work
         # pal = self.palette()
         # pal.setColor(QPalette.Base, color)
         # self.setPalette(pal)
 
     def setUneditable(self):
         self.setReadOnly(True)
```

### Comparing `finalcif-119/finalcif/gui/playground.py` & `finalcif-120/finalcif/gui/playground.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/propertytable.py` & `finalcif-120/finalcif/gui/propertytable.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/text_templates_ui.py` & `finalcif-120/finalcif/gui/text_templates_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/text_templates_ui.ui` & `finalcif-120/finalcif/gui/text_templates_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/text_value_editor.py` & `finalcif-120/finalcif/gui/text_value_editor.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/gui/vrf_classes.py` & `finalcif-120/finalcif/gui/vrf_classes.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/icon/finalcif.png` & `finalcif-120/finalcif/icon/finalcif.png`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/icon/finalcif2.ico` & `finalcif-120/finalcif/icon/finalcif2.ico`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/icon/finalcif2.png` & `finalcif-120/finalcif/icon/finalcif2.png`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/icon/multitable.ico` & `finalcif-120/finalcif/icon/multitable.ico`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/icon/multitable.png` & `finalcif-120/finalcif/icon/multitable.png`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/icon/multitable.xcf` & `finalcif-120/finalcif/icon/multitable.xcf`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/report/archive_report.py` & `finalcif-120/finalcif/report/archive_report.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/report/mtools.py` & `finalcif-120/finalcif/report/mtools.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/report/references.py` & `finalcif-120/finalcif/report/references.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,17 @@
             template = 'references'
         for num, ref in enumerate(self._references, 1):
             paragraph_reflist = document.add_paragraph('', template)
             paragraph_reflist.add_run(f'[{str(num)}] \t')
             ref.add_reference(paragraph_reflist)
             # paragraph_reflist.add_run('\n')
 
+    def __repr__(self):
+        return '\n'.join([f'[{num}] {x}' for num, x in enumerate(self._references)])
+
 
 class ReferenceFormatter():
     def __init__(self):
         self.authors = ''
         self.journal = ''
         self.year = ''
         self.volume = ''
@@ -305,14 +308,30 @@
         # self.year = '2012'
         # if '6.28' in self.year:
         #    self.year = '2001'
         self.volume = version
         self.pages = 'Bruker AXS Inc., Madison, Wisconsin, USA'
 
 
+class XRedReference(ReferenceFormatter):
+    def __init__(self, name: str, version: str):
+        """
+        >>> XRedReference('X-RED', 'version')
+        Stoe & Cie, X-RED, version, Stoe & Cie, Darmstadt, Germany.
+        """
+        super().__init__()
+        self.authors = 'Stoe & Cie'
+        self.journal = name
+        # self.year = '2012'
+        # if '6.28' in self.year:
+        #    self.year = '2001'
+        self.volume = version
+        self.pages = 'Stoe & Cie, Darmstadt, Germany'
+
+
 class XDSReference(ReferenceFormatter):
     def __init__(self):
         """
         >>> XDSReference()
         W. Kabsch, Acta Cryst. 2010, D66, 125-132.
         """
         super().__init__()
```

### Comparing `finalcif-119/finalcif/report/report_text.py` & `finalcif-120/finalcif/report/report_text.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from finalcif.app_path import application_path
 from finalcif.cif.cif_file_io import CifContainer
 from finalcif.cif.text import retranslate_delimiter, string_to_utf8
 from finalcif.report.references import DummyReference, SAINTReference, SORTAVReference, ReferenceList, CCDCReference, \
     SHELXLReference, SHELXTReference, SHELXSReference, FinalCifReference, ShelXleReference, Olex2Reference, \
     SHELXDReference, SadabsTwinabsReference, CrysalisProReference, Nosphera2Reference, XDSReference, DSRReference2015, \
-    DSRReference2018
+    DSRReference2018, XRedReference
 from finalcif.tools.misc import protected_space, angstrom, zero_width_space, remove_line_endings, flatten
 
 
 def math_to_word(eq: str) -> str:
     """Transform a sympy equation to be printed in word document."""
     tree = etree.fromstring(eq)
     xslt = etree.parse(os.path.join(application_path, 'template/mathml2omml.xsl'))
@@ -27,113 +27,110 @@
     new_dom = transform(tree)
     return new_dom.getroot()
 
 
 def clean_string(string: str) -> str:
     """
     Removes control characters from a string.
-    >>> clean_string('This is a sentence\\r with newline.')
+    >>> clean_string('This is a sentence\\nwith newline.')
     'This is a sentence with newline'
     >>> clean_string('')
     ''
-    >>> clean_string('  This is  a sentence\\r with. newline.  ')
+    >>> clean_string('  This is  a sentence\\nwith. newline.  ')
     'This is  a sentence with. newline'
     """
-    return string \
-        .replace('\n', '') \
-        .replace('\r', '') \
-        .replace('\t', '') \
-        .replace('\f', '') \
-        .replace('\0', '') \
+    repl = string.replace('\t', ' ') \
+        .replace('\f', ' ') \
+        .replace('\0', ' ') \
         .strip(' ') \
         .strip('.')
+    return remove_line_endings(repl)
 
 
 def gstr(string: str) -> str:
     """
     Turn a string into a gemmi string and remove control characters.
     """
-    return clean_string(gemmi.cif.as_string(string).strip("'"))
+    return clean_string(gemmi.cif.as_string(string))
 
 
 class FormatMixin():
 
     def bold(self, run: Run):
         r = run.bold = True
         return r
 
 
-class ReportText():
-    def __init__(self):
-        pass
+class Crystallization(FormatMixin):
+    def __init__(self, cif: CifContainer, paragraph: Paragraph):
+        crystalization_method = gstr(cif['_exptl_crystal_recrystallization_method'])
+        if not crystalization_method:
+            crystalization_method = "[No _exptl_crystal_recrystallization_method like 'The compound was " \
+                                    "crystallized from methanol by evaporation at 25 °C.' was given]"
+        delimiter = retranslate_delimiter(f"{crystalization_method}. ")
+        paragraph.add_run(delimiter)
 
 
-class Crystallization(FormatMixin):
+class CrystalSelection(FormatMixin):
     def __init__(self, cif: CifContainer, paragraph: Paragraph):
-        self.cif = cif
-        self.crytsalization_method = gstr(self.cif['_exptl_crystal_recrystallization_method'])
-        if not self.crytsalization_method:
-            self.crytsalization_method = '[No crystallization method was given]'
-        sentence = "The sample was crystallized {}. "
-        self.text = sentence.format(remove_line_endings(retranslate_delimiter(self.crytsalization_method)))
-        paragraph.add_run(retranslate_delimiter(self.text))
+        shape = gstr(cif['_exptl_crystal_description'])
+        crystal_mount = gstr(cif['_diffrn_measurement_specimen_support'])
+        colour = gstr(cif['_exptl_crystal_colour']).strip()
+        if colour:
+            colour = f" {colour}{',' if shape else ''}"
+        # adhesive = gstr(cif['_diffrn_measurement_specimen_adhesive'])
+        # if not adhesive:
+        #    adhesive = '[No _diffrn_measurement_specimen_adhesive given]'
+        shaped = f" {shape}-shaped " if shape else ' '
+        if crystal_mount:
+            txt_crystal = (f"A{colour}{shaped}crystal of {cif.block.name} was mounted on a "
+                           f"{crystal_mount} with perfluoroether oil. ")
+            paragraph.add_run(retranslate_delimiter(txt_crystal))
+        else:
+            txt_crystal = (f"A{colour}{shaped}crystal of {cif.block.name} "
+                           f"was mounted on the goniometer. ")
+            paragraph.add_run(retranslate_delimiter(txt_crystal))
 
 
-class CrstalSelection(FormatMixin):
+class DataCollection(FormatMixin):
     def __init__(self, cif: CifContainer, paragraph: Paragraph):
-        self.cif = cif
-        temperature = gstr(self.cif['_diffrn_ambient_temperature'])
+        temperature = gstr(cif['_diffrn_ambient_temperature'])
         if not temperature:
             temperature = '[No _diffrn_ambient_temperature given]'
-        shape = gstr(self.cif['_exptl_crystal_description'])
-        if not shape:
-            shape = '[No _exptl_crystal_description given]'
-        colour = gstr(self.cif['_exptl_crystal_colour'])
-        crystal_mount = gstr(self.cif['_diffrn_measurement_specimen_support'])
-        # adhesive = gstr(self.cif['_diffrn_measurement_specimen_adhesive'])
-        # if not adhesive:
-        #    adhesive = '[No _diffrn_measurement_specimen_adhesive given]'
-        if not crystal_mount:
-            crystal_mount = '[No _diffrn_measurement_specimen_support given]'
         method = 'shock-cooled '
         try:
             if float(temperature.split('(')[0]) > 200:
                 method = ''
         except ValueError:
             method = ''
-        txt_crystal = (
-            f"A {colour}{', ' if colour else ''}{shape} shaped crystal of {self.cif.block.name} was mounted on a "
-            f"{crystal_mount} with perfluoroether oil. ")
-        txt_data = (f"Data were collected from a {method}single crystal at {temperature}{protected_space}K ")
-        paragraph.add_run(retranslate_delimiter(txt_crystal))
-        Crystallization(cif, paragraph)
+        txt_data = (f"Data were collected from a {method}single crystal at "
+                    f"{temperature}{protected_space}K")
         paragraph.add_run(retranslate_delimiter(txt_data))
 
 
 class MachineType():
     def __init__(self, cif: CifContainer, paragraph: Paragraph):
-        self.cif = cif
-        self.difftype = gstr(self.cif['_diffrn_measurement_device_type']) \
+        self.difftype = gstr(cif['_diffrn_measurement_device_type']) \
                         or '[No _diffrn_measurement_device_type given]'
-        self.device = gstr(self.cif['_diffrn_measurement_device']) \
+        self.device = gstr(cif['_diffrn_measurement_device']) \
                       or '[No _diffrn_measurement_device given]'
-        self.source = gstr(self.cif['_diffrn_source']).strip('\n\r') \
+        self.source = gstr(cif['_diffrn_source']).strip('\n\r') \
                       or '[No _diffrn_source given]'
-        self.monochrom = gstr(self.cif['_diffrn_radiation_monochromator']) \
+        self.monochrom = gstr(cif['_diffrn_radiation_monochromator']) \
                          or '[No _diffrn_radiation_monochromator given]'
         if not self.monochrom:
             self.monochrom = '?'
-        self.cooling = self._get_cooling_device(self.cif)
-        self.rad_type = gstr(self.cif['_diffrn_radiation_type']) \
+        self.cooling = self._get_cooling_device(cif)
+        self.rad_type = gstr(cif['_diffrn_radiation_type']) \
                         or '[No _diffrn_radiation_type given]'
         radtype = format_radiation(self.rad_type)
-        self.wavelen = gstr(self.cif['_diffrn_radiation_wavelength']) \
+        self.wavelen = gstr(cif['_diffrn_radiation_wavelength']) \
                        or '[No _diffrn_radiation_wavelength given]'
         self.detector_type = ''
-        detector_type = gstr(self.cif['_diffrn_detector_type']) \
+        detector_type = gstr(cif['_diffrn_detector_type']) \
                         or '[No _diffrn_detector_type given]'
         if detector_type:
             self.detector_type = " and a {} detector".format(detector_type)
         sentence1 = "on {0} {1} {2} with {3} {4} using a {5} as monochromator{6}. " \
                     "The diffractometer was equipped with {7} {8}low temperature device and used "
         sentence2 = " radiation (λ = {}" + protected_space + "{}). ".format(angstrom)
         txt = sentence1.format(get_inf_article(self.difftype), self.difftype, self.device,
@@ -161,31 +158,32 @@
             return olx + ' '
         elif iucr:
             return iucr + ' '
         else:
             return ''
 
 
-class DataReduct():
+class DataReduction():
     def __init__(self, cif: CifContainer, paragraph: Paragraph, ref: ReferenceList):
-        self.cif = cif
-        integration = gstr(self.cif['_computing_data_reduction']) or '??'
-        abstype = gstr(self.cif['_exptl_absorpt_correction_type']) or '??'
-        abs_details = gstr(self.cif['_exptl_absorpt_process_details']) or '??'
+        integration = gstr(cif['_computing_data_reduction']) or '??'
+        abstype = gstr(cif['_exptl_absorpt_correction_type']) or '??'
+        abs_details = gstr(cif['_exptl_absorpt_process_details']) or '??'
         data_reduct_ref = DummyReference()
         absorpt_ref = DummyReference()
         integration_prog = '[unknown integration program]'
         scale_prog = '[unknown program]'
         if 'SAINT' in integration:
             data_reduct_ref, integration_prog = self.add_saint_reference(integration)
         if 'XDS' in integration:
             data_reduct_ref = XDSReference()
             integration_prog = 'XDS'
         if 'CrysAlisPro'.lower() in integration.lower():
             data_reduct_ref, absorpt_ref, integration_prog = self.add_crysalispro_reference(integration)
+        if 'STOE X-RED'.lower() in integration.lower():
+            data_reduct_ref, integration_prog = self.add_x_red_reference(integration)
         absdetails = cif['_exptl_absorpt_process_details'].replace('-', ' ')
         if 'SADABS' in absdetails.upper() or 'TWINABS' in absdetails.upper():
             # if len(absdetails.split()) > 1:
             #    version = absdetails.split()[1]
             # else:
             #    version = 'unknown version'
             if 'SADABS' in absdetails:
@@ -208,14 +206,22 @@
         saintversion = 'unknown version'
         if len(integration.split()) > 1:
             saintversion = integration.split()[1]
         integration_prog = 'SAINT'
         data_reduct_ref = SAINTReference('SAINT', saintversion)
         return data_reduct_ref, integration_prog
 
+    def add_x_red_reference(self, integration):
+        xredversion = 'unknown version'
+        #if len(integration.split()) > 1:
+        #    xredversion = integration.split()[1]
+        integration_prog = 'STOE X-RED'
+        data_reduct_ref = XRedReference('X-RED', xredversion)
+        return data_reduct_ref, integration_prog
+
     def add_crysalispro_reference(self, integration: str) -> Tuple[CrysalisProReference, CrysalisProReference, str]:
         """
         CrysAlisPro, Agilent Technologies,Version 1.171.37.31h (release 21-03-2014 CrysAlis171 .NET)
             (compiled Mar 21 2014,18:13:45)
         CrysAlisPro 1.171.42.58a (Rigaku OD, 2022)
         """
         year = 'unknown version'
@@ -235,48 +241,57 @@
         data_reduct_ref = CrysalisProReference(version=version, year=year, pages=pages)
         absorpt_ref = CrysalisProReference(version=version, year=year, pages=pages)
         return data_reduct_ref, absorpt_ref, integration_prog
 
 
 class SolveRefine():
     def __init__(self, cif: CifContainer, paragraph: Paragraph, ref: ReferenceList):
-        self.cif = cif
+        manual_method = False
         refineref = DummyReference()
         solveref = DummyReference()
-        solution_prog = gstr(self.cif['_computing_structure_solution']) or '??'
-        solution_method = gstr(self.cif['_atom_sites_solution_primary']) or '??'
+        solution_prog = gstr(cif['_computing_structure_solution']) or '[No _computing_structure_solution given]'
+        solution_method = gstr(cif['_atom_sites_solution_primary']).strip(
+            '\n\r') or '[No _atom_sites_solution_primary given]'
+        if 'isomor' in solution_method:
+            manual_method = True
         if solution_prog.upper().startswith(('SHELXT', 'XT')):
             solveref = SHELXTReference()
         if 'SHELXS' in solution_prog.upper():
             solveref = SHELXSReference()
         if 'SHELXD' in solution_prog.upper():
             solveref = SHELXDReference()
-        refined = gstr(self.cif['_computing_structure_refinement']) or '??'
+        refined = gstr(cif['_computing_structure_refinement']).split(' ')[
+                      0] or '[No _computing_structure_refinement given]'
         if refined.upper().startswith(('SHELXL', 'XL')):
             refineref = SHELXLReference()
         if 'OLEX' in refined.upper():
             refineref = Olex2Reference()
-        if 'NOSPHERA2' in solution_prog.upper() or 'NOSPHERA2' in self.cif['_refine_special_details'].upper() \
-                or 'NOSPHERA2' in self.cif['_olex2_refine_details'].upper():
+        if 'NOSPHERA2' in solution_prog.upper() or 'NOSPHERA2' in cif['_refine_special_details'].upper() \
+            or 'NOSPHERA2' in cif['_olex2_refine_details'].upper():
             refineref = [Olex2Reference(), Nosphera2Reference()]
-        refine_coef = gstr(self.cif['_refine_ls_structure_factor_coef'])
-        newline = '\n\r'
-        txt = (f"The structure was solved by {solution_method.strip(newline)} methods using "
-               f"{solution_prog.split()[0]} and refined by full-matrix least-squares methods against ")
+        refine_coef = gstr(cif['_refine_ls_structure_factor_coef'])
+        if manual_method:
+            methods = f"{solution_prog} "
+        else:
+            methods = f"{solution_method} methods using {solution_prog.split(' ')[0]} "
+        txt = (f"The structure was solved by {methods}and refined by full-matrix least-squares methods against ")
         paragraph.add_run(retranslate_delimiter(txt))
         paragraph.add_run('F').font.italic = True
         if refine_coef.lower() == 'fsqd':
             paragraph.add_run('2').font.superscript = True
-        paragraph.add_run(f' by {refined.split()[0]}')
-        shelxle = None
-        if 'shelxle' in refined.lower() or 'shelxle' in self.cif['_computing_molecular_graphics'].lower():
+        paragraph.add_run(f' by {refined}')
+        gui_reference = None
+        if 'shelxle' in refined.lower() or 'shelxle' in cif['_computing_molecular_graphics'].lower():
             paragraph.add_run(' using ShelXle')
-            shelxle = ShelXleReference()
+            gui_reference = ShelXleReference()
+        if 'olex' in refined.lower() or 'olex' in cif['_computing_molecular_graphics'].lower():
+            paragraph.add_run(' using Olex2')
+            gui_reference = Olex2Reference()
         paragraph.add_run('.')
-        ref.append(flatten([solveref, refineref, shelxle]))
+        ref.append(flatten([solveref, refineref, gui_reference]))
 
 
 class Atoms():
     def __init__(self, cif: CifContainer, paragraph: Paragraph):
         """
         Text for non-hydrogen atoms.
         """
@@ -309,24 +324,24 @@
     @staticmethod
     def atom_is_isotropic(site, without_h: bool):
         if without_h:
             return not site.aniso.nonzero() and not site.element.is_hydrogen
         else:
             return not site.aniso.nonzero()
 
+
 class Hydrogens():
     def __init__(self, cif: CifContainer, paragraph: Paragraph):
         """
         The hydrogen atoms were refined isotropically on calculated positions using
         a riding model with their Uiso values constrained to 1.5 times the Ueq of
         their pivot atoms for terminal sp3 carbon atoms and 1.2 times for all other
         carbon atoms.
         """
-        self.cif = cif
-        hatoms: List[SHXAtom] = [x for x in self.cif.shx.atoms.all_atoms if x.is_hydrogen]
+        hatoms: List[SHXAtom] = [x for x in cif.shx.atoms.all_atoms if x.is_hydrogen]
         n_hatoms = len(hatoms)
         n_anisotropic_h = len([x for x in hatoms if sum([abs(y) for y in x.uvals[1:]]) > 0.0001])
         n_constr_h = len([x for x in hatoms if x.uvals[0] < -1.0])
         riding_atoms = [x for x in hatoms if x.afix]
         pivot_atoms = self.get_hydrogen_pivot_atoms(riding_atoms)
         n_riding = len(riding_atoms)
         n_non_riding = len(hatoms) - n_riding
@@ -406,57 +421,65 @@
 
     def u_iso(self, paragraph):
         paragraph.add_run('U').font.italic = True
         paragraph.add_run('iso').font.subscript = True
 
 
 class Disorder():
-    def __init__(self, cif: CifContainer, paragraph: Paragraph):
-        self.cif = cif
+    def __init__(self, cif: CifContainer, paragraph: Paragraph, reflist: ReferenceList):
+        """
+        TODO: Search for SIMU, DELU, SADI, DFIX, etc in cif.shx.restraints in order to
+              make the sentence1 more specific.
+        """
+
         self.dsr_sentence = ''
         sentence1 = "Disordered moieties were refined using bond lengths " \
                     "restraints and displacement parameter restraints. "
-        if self.cif.dsr_used:
-            self.dsr_sentence = "Some parts of the disorder model were introduced by the " \
-                                "program DSR."
         paragraph.add_run(sentence1)
-        if self.dsr_sentence:
-            paragraph.add_run(self.dsr_sentence)
+        if cif.dsr_used:
+            dsr_sentence = "Some parts of the disorder model were introduced by the " \
+                           "program DSR."
+            paragraph.add_run(dsr_sentence)
+            reflist.append([DSRReference2015(), DSRReference2018()])
+            SpaceChar(paragraph).regular()
 
 
 class SpaceChar(object):
     def __init__(self, paragraph: Paragraph):
         self.p = paragraph
 
-    def regular(self):
+    def regular(self) -> None:
         self.p.add_run(' ')
 
-    def porotected(self):
+    def protected(self):
         self.p.add_run(protected_space)
 
 
 class CCDC():
     def __init__(self, cif: CifContainer, paragraph: Paragraph, ref: ReferenceList):
-        self.cif = cif
-        ccdc_num = gstr(self.cif['_database_code_depnum_ccdc_archive']) or '??????'
-        sentence1 = "Crystallographic data for the structures reported in this " \
-                    "paper have been deposited with the Cambridge Crystallographic Data Centre."
-        sentence2 = "CCDC {} contain the supplementary crystallographic data for this paper. " \
+        ccdc_num = gstr(cif['_database_code_depnum_ccdc_archive']) or '??????'
+        splitted_number = ccdc_num.split(' ')
+        if len(splitted_number) > 1 and splitted_number[1].isdigit():
+            ccdc_num = splitted_number[1]
+        sentence1 = "Crystallographic data for the structures reported here " \
+                    "have been deposited with the Cambridge Crystallographic Data Centre."
+        sentence2 = f"CCDC {ccdc_num} contain the supplementary crystallographic data for this paper. " \
                     "These data can be obtained free of charge from The Cambridge Crystallographic Data Centre " \
-                    "via www.ccdc.cam.ac.uk/{}structures.".format(ccdc_num, zero_width_space)
+                    f"via www.ccdc.cam.ac.uk/{zero_width_space}structures."
         paragraph.add_run(sentence1)
         ref.append(CCDCReference())
         SpaceChar(paragraph).regular()
         paragraph.add_run(sentence2)
 
 
 class FinalCifreport():
-    def __init__(self, paragraph: Paragraph):
+    def __init__(self, paragraph: Paragraph, reflist: ReferenceList):
         sentence = "This report and the CIF file were generated using FinalCif."
         paragraph.add_run(sentence)
+        reflist.append(FinalCifReference())
 
 
 class RefinementDetails():
     def __init__(self, cif: CifContainer, document: Document):
         ph = document.add_paragraph(style='Heading 2')
         ph.add_run(text=fr"Refinement details for {cif.block.name}")
         p = document.add_paragraph()
@@ -487,28 +510,27 @@
 
 def make_report_text(cif, document: Document) -> ReferenceList:
     paragr = document.add_paragraph()
     paragr.style = document.styles['fliesstext']
     ref = ReferenceList(paragr)
     # -- The main text:
     paragr.add_run('The following text is only a suggestion: ').font.bold = True
-    CrstalSelection(cif, paragr)
+    Crystallization(cif, paragr)
+    CrystalSelection(cif, paragr)
+    DataCollection(cif, paragr)
+    SpaceChar(paragr).regular()
     MachineType(cif, paragr)
-    DataReduct(cif, paragr, ref)
+    DataReduction(cif, paragr, ref)
     SpaceChar(paragr).regular()
     SolveRefine(cif, paragr, ref)
     SpaceChar(paragr).regular()
     if cif.hydrogen_atoms_present:
         a = Atoms(cif, paragr)
         if a.n_isotropic_with_h != 0 and (a.n_isotropic_with_h > a.n_isotropic):
             Hydrogens(cif, paragr)
             SpaceChar(paragr).regular()
     if cif.disorder_present:
-        d = Disorder(cif, paragr)
-        if d.dsr_sentence:
-            ref.append([DSRReference2015(), DSRReference2018()])
-            SpaceChar(paragr).regular()
+        Disorder(cif, paragr, ref)
     CCDC(cif, paragr, ref)
     SpaceChar(paragr).regular()
-    FinalCifreport(paragr)
-    ref.append(FinalCifReference())
+    FinalCifreport(paragr, ref)
     return ref
```

### Comparing `finalcif-119/finalcif/report/symm.py` & `finalcif-120/finalcif/report/symm.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/report/tables.py` & `finalcif-120/finalcif/report/tables.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/report/templated_report.py` & `finalcif-120/finalcif/report/templated_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,18 +325,18 @@
         limit_h_max = cif['_diffrn_reflns_limit_h_max']
         limit_k_min = cif['_diffrn_reflns_limit_k_min']
         limit_k_max = cif['_diffrn_reflns_limit_k_max']
         limit_l_min = cif['_diffrn_reflns_limit_l_min']
         limit_l_max = cif['_diffrn_reflns_limit_l_max']
         return f'{minus_sign if limit_h_min != "0" else ""}{limit_h_min.replace("-", "")} ' \
                f'{less_or_equal} h {less_or_equal} {limit_h_max}\n' \
-               + f'{minus_sign if limit_k_min != "0" else ""}{limit_k_min.replace("-", "")} ' \
-                 f'{less_or_equal} k {less_or_equal} {limit_k_max}\n' \
-               + f'{minus_sign if limit_l_min != "0" else ""}{limit_l_min.replace("-", "")} ' \
-                 f'{less_or_equal} l {less_or_equal} {limit_l_max}'
+            + f'{minus_sign if limit_k_min != "0" else ""}{limit_k_min.replace("-", "")} ' \
+              f'{less_or_equal} k {less_or_equal} {limit_k_max}\n' \
+            + f'{minus_sign if limit_l_min != "0" else ""}{limit_l_min.replace("-", "")} ' \
+              f'{less_or_equal} l {less_or_equal} {limit_l_max}'
 
     @staticmethod
     def get_radiation(cif: CifContainer) -> RichText:
         rad_element, radtype, radline = format_radiation(cif['_diffrn_radiation_type'])
         radiation = RichText(rad_element)
         radiation.add(radtype, italic=True)
         radiation.add(radline, italic=True, subscript=True)
@@ -447,15 +447,15 @@
     def refinement_prog(self, cif: CifContainer) -> str:
         refined = gstr(cif['_computing_structure_refinement']) or '??'
         if 'SHELXL' in refined.upper() or 'XL' in refined.upper():
             self.literature['refinement'] = SHELXLReference()
         if 'OLEX' in refined.upper():
             self.literature['refinement'] = Olex2Reference()
         if ('NOSPHERA2' in refined.upper() or 'NOSPHERA2' in cif['_refine_special_details'].upper() or
-                'NOSPHERAT2' in cif['_olex2_refine_details'].upper()):
+            'NOSPHERAT2' in cif['_olex2_refine_details'].upper()):
             self.literature['refinement'] = Nosphera2Reference()
         return refined.split()[0]
 
     def get_atomic_coordinates(self, cif: CifContainer):
         for at in cif.atoms(without_h=False):
             yield {'label': at.label,
                    'type' : at.type,
@@ -477,16 +477,15 @@
                       U22=u22.replace('-', minus_sign),
                       U33=u33.replace('-', minus_sign),
                       U12=u12.replace('-', minus_sign),
                       U13=u13.replace('-', minus_sign),
                       U23=u23.replace('-', minus_sign))
 
     def get_crystallization_method(self, cif):
-        return remove_line_endings(retranslate_delimiter(
-            cif['_exptl_crystal_recrystallization_method'])) or '[No crystallization method given!]'
+        return gstr(cif['_exptl_crystal_recrystallization_method']) or '[No crystallization method given!]'
 
     def make_picture(self, options: Options, picfile: Path, tpl_doc: DocxTemplate):
         if options.report_text and picfile and picfile.exists():
             return InlineImage(tpl_doc, str(picfile.resolve()), width=Cm(options.picture_width))
         return None
 
     def make_templated_report(self, options: Options, cif: CifContainer, output_filename: str, picfile: Path,
```

### Comparing `finalcif-119/finalcif/report/gui/mainwindow.py` & `finalcif-120/finalcif/report/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/report/gui/mainwindow.ui` & `finalcif-120/finalcif/report/gui/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/template/mathml2omml.xsl` & `finalcif-120/finalcif/template/mathml2omml.xsl`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/template/template1.docx` & `finalcif-120/finalcif/template/template1.docx`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/template/template_text.docx` & `finalcif-120/finalcif/template/template_text.docx`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/template/template_without_text.docx` & `finalcif-120/finalcif/template/template_without_text.docx`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/template/templates.py` & `finalcif-120/finalcif/template/templates.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/tools/download.py` & `finalcif-120/finalcif/tools/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 # noinspection PyUnresolvedReferences
 class MyDownloader(QObject):
     progress = pyqtSignal(str)
     failed = pyqtSignal(int)
     finished = pyqtSignal()
     loaded = pyqtSignal(bytes)
 
-    def __init__(self, url):
-        super().__init__()
+    def __init__(self, url, parent=None):
+        super().__init__(parent)
         self.url = url
 
     def failed_to_load(self, txt: str) -> None:
         print('Failed to load {}', self.url)
 
     @pyqtSlot()
     def download(self) -> None:
```

### Comparing `finalcif-119/finalcif/tools/dsrmath.py` & `finalcif-120/finalcif/tools/dsrmath.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/tools/misc.py` & `finalcif-120/finalcif/tools/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -888,15 +888,15 @@
 
 
 def unify_line_endings(text: str):
     return '\n'.join(text.splitlines())
 
 
 def remove_line_endings(text: str):
-    return ' '.join(text.splitlines())
+    return ''.join(text.splitlines())
 
 
 def open_file(report_filename: Path):
     if report_filename.exists():
         if os.name == 'nt':
             os.startfile(report_filename)
         if sys.platform == 'darwin':
```

### Comparing `finalcif-119/finalcif/tools/options.py` & `finalcif-120/finalcif/tools/options.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/tools/platon.py` & `finalcif-120/finalcif/tools/platon.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/tools/pupdate.py` & `finalcif-120/finalcif/tools/pupdate.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/tools/settings.py` & `finalcif-120/finalcif/tools/settings.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/tools/shred.py` & `finalcif-120/finalcif/tools/shred.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/tools/space_groups.py` & `finalcif-120/finalcif/tools/space_groups.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/tools/spgr_format.py` & `finalcif-120/finalcif/tools/spgr_format.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/tools/statusbar.py` & `finalcif-120/finalcif/tools/statusbar.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/finalcif/tools/sumformula.py` & `finalcif-120/finalcif/tools/sumformula.py`

 * *Files identical despite different names*

### Comparing `finalcif-119/.gitignore` & `finalcif-120/.gitignore`

 * *Files identical despite different names*

### Comparing `finalcif-119/README.md` & `finalcif-120/README.md`

 * *Files identical despite different names*

### Comparing `finalcif-119/pyproject.toml` & `finalcif-120/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "finalcif"
-version = "119"
+version = "120"
 authors = [
     { name = "Daniel Kratzert", email = "dkratzert@gmx.de" },
 ]
 description = "CIF file editor"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -34,15 +34,15 @@
     'PyQt5-sip~=12.11',
     'PyQtWebEngine~=5.15',
     'python-docx~=0.8',
     'pywin32-ctypes~=0.2',
     'QtAwesome',
     'QtPy',
     'requests',
-    'urllib3',
+    'urllib3~=1.26',
     'docxtpl',
     'shelxfile',
     'crossrefapi',
     'numpy',
 ]
 
 [project.urls]
```

### Comparing `finalcif-119/PKG-INFO` & `finalcif-120/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalcif
-Version: 119
+Version: 120
 Summary: CIF file editor
 Project-URL: Homepage, https://dkratzert.de/finalcif.html
 Project-URL: Bug Tracker, https://github.com/dkratzert/FinalCif/issues
 Author-email: Daniel Kratzert <dkratzert@gmx.de>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -29,15 +29,15 @@
 Requires-Dist: pyqtwebengine~=5.15
 Requires-Dist: python-docx~=0.8
 Requires-Dist: pywin32-ctypes~=0.2
 Requires-Dist: qtawesome
 Requires-Dist: qtpy
 Requires-Dist: requests
 Requires-Dist: shelxfile
-Requires-Dist: urllib3
+Requires-Dist: urllib3~=1.26
 Requires-Dist: wheel
 Description-Content-Type: text/markdown
 
 ![Lates Release](https://img.shields.io/github/v/tag/dkratzert/FinalCif?label=Release)
 [![Unit Tests](https://github.com/dkratzert/FinalCif/actions/workflows/python-app_windows.yml/badge.svg?branch=master)](https://github.com/dkratzert/FinalCif/actions/workflows/python-app_windows.yml)
 ![Contributions](https://img.shields.io/badge/contributions-welcome-blue)
 [![PyPI package](https://repology.org/badge/version-for-repo/pypi/python:finalcif.svg)](https://repology.org/project/python:finalcif/versions)
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: finalcif Version: 119 Summary: CIF file editor
+Metadata-Version: 2.1 Name: finalcif Version: 120 Summary: CIF file editor
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
 Requires-Dist: pefile Requires-Dist: pybind11 Requires-Dist: pyqt5-sip~=12.11
 Requires-Dist: pyqt5~=5.15 Requires-Dist: pyqtwebengine~=5.15 Requires-Dist:
 python-docx~=0.8 Requires-Dist: pywin32-ctypes~=0.2 Requires-Dist: qtawesome
 Requires-Dist: qtpy Requires-Dist: requests Requires-Dist: shelxfile Requires-
-Dist: urllib3 Requires-Dist: wheel Description-Content-Type: text/markdown !
-[Lates Release](https://img.shields.io/github/v/tag/dkratzert/
+Dist: urllib3~=1.26 Requires-Dist: wheel Description-Content-Type: text/
+markdown ![Lates Release](https://img.shields.io/github/v/tag/dkratzert/
 FinalCif?label=Release) [![Unit Tests](https://github.com/dkratzert/FinalCif/
 actions/workflows/python-app_windows.yml/badge.svg?branch=master)](https://
 github.com/dkratzert/FinalCif/actions/workflows/python-app_windows.yml) !
 [Contributions](https://img.shields.io/badge/contributions-welcome-blue) [!
 [PyPI package](https://repology.org/badge/version-for-repo/pypi/python:
 finalcif.svg)](https://repology.org/project/python:finalcif/versions)
 [Packaging_status] # FinalCif FinalCif helps you to get a complete [CIF](https:
```

