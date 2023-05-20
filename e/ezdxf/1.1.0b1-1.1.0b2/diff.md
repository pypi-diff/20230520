# Comparing `tmp/ezdxf-1.1.0b1.zip` & `tmp/ezdxf-1.1.0b2.zip`

## zipinfo {}

```diff
@@ -1,831 +1,840 @@
-Zip file size: 2070630 bytes, number of entries: 829
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/integration_tests/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/
--rw-rw-rw-  2.0 fat     1092 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/LICENSE
--rw-rw-rw-  2.0 fat      302 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/MANIFEST.in
--rw-rw-rw-  2.0 fat   101339 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/NEWS.md
--rw-rw-rw-  2.0 fat    69206 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/PKG-INFO
--rw-rw-rw-  2.0 fat     6142 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/README.md
--rw-rw-rw-  2.0 fat       55 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/requirements.txt
--rw-rw-rw-  2.0 fat       74 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/setup.cfg
--rw-rw-rw-  2.0 fat     5402 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/integration_tests/data/
--rw-rw-rw-  2.0 fat      567 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/check_disable_c_ext_by_config_file.py
--rw-rw-rw-  2.0 fat      541 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/check_disable_c_ext_by_env_var.py
--rw-rw-rw-  2.0 fat      410 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/conftest.py
--rw-rw-rw-  2.0 fat     1054 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_acad_table.py
--rw-rw-rw-  2.0 fat     4686 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_all_dimline_styles.py
--rw-rw-rw-  2.0 fat     4133 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_all_ellipse_transformations.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_anonymous_blocks.py
--rw-rw-rw-  2.0 fat      871 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_audit_critical_dxf_files.py
--rw-rw-rw-  2.0 fat     1603 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_audit_layouts.py
--rw-rw-rw-  2.0 fat     1726 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_complex_line_type_2.py
--rw-rw-rw-  2.0 fat     1003 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_create_basic_graphics.py
--rw-rw-rw-  2.0 fat     1921 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_document_guid.py
--rw-rw-rw-  2.0 fat     1832 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_document_page_setup.py
--rw-rw-rw-  2.0 fat      998 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_dxf_info_scanning.py
--rw-rw-rw-  2.0 fat     1558 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_entities_iterator.py
--rw-rw-rw-  2.0 fat      934 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_fix_dulicate_handles.py
--rw-rw-rw-  2.0 fat     1901 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_geo.py
--rw-rw-rw-  2.0 fat     1250 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_groups.py
--rw-rw-rw-  2.0 fat      630 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_ignore_junk_beyond_EOF.py
--rw-rw-rw-  2.0 fat     1155 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_launcher.py
--rw-rw-rw-  2.0 fat      631 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_leica_disto_r12.py
--rw-rw-rw-  2.0 fat      737 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_load_dxf_unicode_notation.py
--rw-rw-rw-  2.0 fat     2931 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_mapbox_earcut.py
--rw-rw-rw-  2.0 fat     2230 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_mtext_columns.py
--rw-rw-rw-  2.0 fat     2392 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_mtext_explode_addon.py
--rw-rw-rw-  2.0 fat     1846 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_mtext_text_frame.py
--rw-rw-rw-  2.0 fat     1053 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_new_table_entries.py
--rw-rw-rw-  2.0 fat      887 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_none_ascii_read_write.py
--rw-rw-rw-  2.0 fat     3435 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_odafc.py
--rw-rw-rw-  2.0 fat     1737 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_open_binary_DXF_files.py
--rw-rw-rw-  2.0 fat      751 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_open_coord_order_issue.py
--rw-rw-rw-  2.0 fat     3842 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_open_exotic_dxf_files.py
--rw-rw-rw-  2.0 fat      879 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_open_R13_R14.py
--rw-rw-rw-  2.0 fat     3152 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_polyline_entity.py
--rw-rw-rw-  2.0 fat     1749 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_preserve_binary_data_in_xrecords.py
--rw-rw-rw-  2.0 fat     6944 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_r12export.py
--rw-rw-rw-  2.0 fat     6256 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_r12strict.py
--rw-rw-rw-  2.0 fat     3410 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_r12writer.py
--rw-rw-rw-  2.0 fat      567 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_read_file_without_handles.py
--rw-rw-rw-  2.0 fat     1121 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_read_write_modern_entites.py
--rw-rw-rw-  2.0 fat     5375 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_recover.py
--rw-rw-rw-  2.0 fat     1959 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_redraw_order.py
--rw-rw-rw-  2.0 fat     1819 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_rotated_block_attributes.py
--rw-rw-rw-  2.0 fat      774 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_surface_entities.py
--rw-rw-rw-  2.0 fat      928 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_write_fixed_meta_data.py
--rw-rw-rw-  2.0 fat     1806 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_write_without_handles.py
--rw-rw-rw-  2.0 fat     3638 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_xref_detach.py
--rw-rw-rw-  2.0 fat     3060 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/AC1003_LINE_Example.dxf
--rw-rw-rw-  2.0 fat   179505 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/acad_table_with_blk_ref.dxf
--rw-rw-rw-  2.0 fat     7956 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/ASCII_R12.dxf
--rw-rw-rw-  2.0 fat     3761 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r12.dxf
--rw-rw-rw-  2.0 fat    20914 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r13.dxf
--rw-rw-rw-  2.0 fat    21137 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r14.dxf
--rw-rw-rw-  2.0 fat    11564 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r2000.dxf
--rw-rw-rw-  2.0 fat     6424 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/cc_dxflib.dxf
--rw-rw-rw-  2.0 fat   173753 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/custom_blocks.dxf
--rw-rw-rw-  2.0 fat    32203 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/duplicate_handles.dxf
--rw-rw-rw-  2.0 fat    18554 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/dxf_unicode.dxf
--rw-rw-rw-  2.0 fat     1592 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/empty_handles.dxf
--rw-rw-rw-  2.0 fat    97103 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/groups.dxf
--rw-rw-rw-  2.0 fat     9146 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/Leica_Disto_S910.dxf
--rw-rw-rw-  2.0 fat    17986 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/MODEL.dxf
--rw-rw-rw-  2.0 fat    25799 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/mtext_columns_R2007.dxf
--rw-rw-rw-  2.0 fat    23927 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/mtext_columns_R2018.dxf
--rw-rw-rw-  2.0 fat    98230 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/mtext_framed_columns.dxf
--rw-rw-rw-  2.0 fat   106574 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/mtext_text_frame.dxf
--rw-rw-rw-  2.0 fat    12001 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/no_layouts.dxf
--rw-rw-rw-  2.0 fat    28788 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/POLI-ALL210_12.DXF
--rw-rw-rw-  2.0 fat      144 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/R12_with_trash_beyond_EOF.dxf
--rw-rw-rw-  2.0 fat   212407 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/recover01.dxf
--rw-rw-rw-  2.0 fat   115423 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/recover02.dxf
--rw-rw-rw-  2.0 fat    21178 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/small_r13.dxf
--rw-rw-rw-  2.0 fat    10326 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/small_r14.dxf
--rw-rw-rw-  2.0 fat    11286 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/XRECORD_0.bin
--rw-rw-rw-  2.0 fat    11662 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/XRECORD_1.bin
--rw-rw-rw-  2.0 fat    15337 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/XRECORD_2.bin
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/acc/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/acis/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/addons/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/entities/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/fonts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/lldxf/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/math/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/path/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/pp/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/render/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/resources/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/sections/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/tools/
--rw-rw-rw-  2.0 fat     4710 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/appsettings.py
--rw-rw-rw-  2.0 fat    19818 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/audit.py
--rw-rw-rw-  2.0 fat     5324 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/bbox.py
--rw-rw-rw-  2.0 fat     7888 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/blkrefs.py
--rw-rw-rw-  2.0 fat    13157 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/colors.py
--rw-rw-rw-  2.0 fat    31861 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/commands.py
--rw-rw-rw-  2.0 fat     1549 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/comments.py
--rw-rw-rw-  2.0 fat    22100 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/disassemble.py
--rw-rw-rw-  2.0 fat    52708 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/document.py
--rw-rw-rw-  2.0 fat      832 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/dwginfo.py
--rw-rw-rw-  2.0 fat    16248 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entitydb.py
--rw-rw-rw-  2.0 fat     7495 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/enums.py
--rw-rw-rw-  2.0 fat    13948 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/explode.py
--rw-rw-rw-  2.0 fat     1653 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/eztypes.py
--rw-rw-rw-  2.0 fat    10333 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/filemanagement.py
--rw-rw-rw-  2.0 fat    12157 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/gfxattribs.py
--rw-rw-rw-  2.0 fat   107500 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/graphicsfactory.py
--rw-rw-rw-  2.0 fat     3416 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/groupby.py
--rw-rw-rw-  2.0 fat     3244 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/npshapes.py
--rw-rw-rw-  2.0 fat     2567 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/protocols.py
--rw-rw-rw-  2.0 fat    32672 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/proxygraphic.py
--rw-rw-rw-  2.0 fat       95 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/py.typed
--rw-rw-rw-  2.0 fat    22499 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/query.py
--rw-rw-rw-  2.0 fat     2780 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/queryparser.py
--rw-rw-rw-  2.0 fat     9580 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/r12strict.py
--rw-rw-rw-  2.0 fat    30769 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/recover.py
--rw-rw-rw-  2.0 fat     3515 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/reorder.py
--rw-rw-rw-  2.0 fat    10364 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/transform.py
--rw-rw-rw-  2.0 fat     5648 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/units.py
--rw-rw-rw-  2.0 fat     8280 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/upright.py
--rw-rw-rw-  2.0 fat     9875 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/urecord.py
--rw-rw-rw-  2.0 fat     1024 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/version.py
--rw-rw-rw-  2.0 fat    63359 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/xref.py
--rw-rw-rw-  2.0 fat     2853 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/zoom.py
--rw-rw-rw-  2.0 fat    10979 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/_options.py
--rw-rw-rw-  2.0 fat     2566 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/__init__.py
--rw-rw-rw-  2.0 fat     2786 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/__main__.py
--rw-rw-rw-  2.0 fat     6072 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/bezier3p.pyx
--rw-rw-rw-  2.0 fat     9983 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/bezier4p.pyx
--rw-rw-rw-  2.0 fat    12964 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/bspline.pyx
--rw-rw-rw-  2.0 fat       90 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/construct.pxd
--rw-rw-rw-  2.0 fat     6584 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/construct.pyx
--rw-rw-rw-  2.0 fat     3113 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/linetypes.pyx
--rw-rw-rw-  2.0 fat    23989 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/mapbox_earcut.pyx
--rw-rw-rw-  2.0 fat      386 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/matrix44.pxd
--rw-rw-rw-  2.0 fat    23742 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/matrix44.pyx
--rw-rw-rw-  2.0 fat     2014 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/vector.pxd
--rw-rw-rw-  2.0 fat    23705 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/vector.pyx
--rw-rw-rw-  2.0 fat     1784 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.cpp
--rw-rw-rw-  2.0 fat      599 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.hpp
--rw-rw-rw-  2.0 fat      424 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.pxd
--rw-rw-rw-  2.0 fat      960 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_quad_bezier.cpp
--rw-rw-rw-  2.0 fat      464 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_quad_bezier.hpp
--rw-rw-rw-  2.0 fat      407 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_quad_bezier.pxd
--rw-rw-rw-  2.0 fat     2135 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_vec3.hpp
--rw-rw-rw-  2.0 fat      572 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_vec3.pxd
--rw-rw-rw-  2.0 fat     1265 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/__init__.py
--rw-rw-rw-  2.0 fat     6393 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/abstract.py
--rw-rw-rw-  2.0 fat      884 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/api.py
--rw-rw-rw-  2.0 fat     5484 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/const.py
--rw-rw-rw-  2.0 fat     6726 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/dbg.py
--rw-rw-rw-  2.0 fat     2980 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/dxf.py
--rw-rw-rw-  2.0 fat    28991 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/entities.py
--rw-rw-rw-  2.0 fat     4088 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/hdr.py
--rw-rw-rw-  2.0 fat    12823 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/mesh.py
--rw-rw-rw-  2.0 fat    18690 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/sab.py
--rw-rw-rw-  2.0 fat    13184 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/sat.py
--rw-rw-rw-  2.0 fat      115 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/addons/browser/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/
--rw-rw-rw-  2.0 fat    26415 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/acadctb.py
--rw-rw-rw-  2.0 fat    22229 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/binpacking.py
--rw-rw-rw-  2.0 fat    27692 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dimlines.py
--rw-rw-rw-  2.0 fat    31371 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dxf2code.py
--rw-rw-rw-  2.0 fat    22037 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/genetic_algorithm.py
--rw-rw-rw-  2.0 fat    36445 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/geo.py
--rw-rw-rw-  2.0 fat     2674 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/gerber_D6673.py
--rw-rw-rw-  2.0 fat    25472 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/importer.py
--rw-rw-rw-  2.0 fat    17355 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/iterdxf.py
--rw-rw-rw-  2.0 fat     8940 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/menger_sponge.py
--rw-rw-rw-  2.0 fat    24787 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/meshex.py
--rw-rw-rw-  2.0 fat      492 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/mixins.py
--rw-rw-rw-  2.0 fat     6203 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/mtextsurrogate.py
--rw-rw-rw-  2.0 fat    13528 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/mtxpl.py
--rw-rw-rw-  2.0 fat    16400 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/odafc.py
--rw-rw-rw-  2.0 fat     9456 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/openscad.py
--rw-rw-rw-  2.0 fat    15878 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/pycsg.py
--rw-rw-rw-  2.0 fat    22496 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/r12export.py
--rw-rw-rw-  2.0 fat    27198 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/r12writer.py
--rw-rw-rw-  2.0 fat     7615 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/sierpinski_pyramid.py
--rw-rw-rw-  2.0 fat    33167 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/tablepainter.py
--rw-rw-rw-  2.0 fat    12789 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/text2path.py
--rw-rw-rw-  2.0 fat     2312 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/xqt.py
--rw-rw-rw-  2.0 fat      453 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/__init__.py
--rw-rw-rw-  2.0 fat    10023 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/browser.py
--rw-rw-rw-  2.0 fat     1907 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/data.py
--rw-rw-rw-  2.0 fat       64 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/__init__.py
--rw-rw-rw-  2.0 fat      820 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/bookmarks.py
--rw-rw-rw-  2.0 fat    29367 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/browser.py
--rw-rw-rw-  2.0 fat    14891 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/data.py
--rw-rw-rw-  2.0 fat    10993 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/find_dialog.py
--rw-rw-rw-  2.0 fat     1281 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/loader.py
--rw-rw-rw-  2.0 fat    20974 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/model.py
--rw-rw-rw-  2.0 fat     2214 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/tags.py
--rw-rw-rw-  2.0 fat     1382 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/views.py
--rw-rw-rw-  2.0 fat      133 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/__init__.py
--rw-rw-rw-  2.0 fat     7301 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/backend.py
--rw-rw-rw-  2.0 fat     3611 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/clipper.py
--rw-rw-rw-  2.0 fat     6737 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/config.py
--rw-rw-rw-  2.0 fat     1716 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/debug_backend.py
--rw-rw-rw-  2.0 fat      514 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/debug_utils.py
--rw-rw-rw-  2.0 fat    42098 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/frontend.py
--rw-rw-rw-  2.0 fat     1823 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/gfxproxy.py
--rw-rw-rw-  2.0 fat    12669 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/matplotlib.py
--rw-rw-rw-  2.0 fat     9878 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/mtext_complex.py
--rw-rw-rw-  2.0 fat    39188 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/properties.py
--rw-rw-rw-  2.0 fat    10656 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/pyqt.py
--rw-rw-rw-  2.0 fat    16738 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/qtviewer.py
--rw-rw-rw-  2.0 fat     5914 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/recorder.py
--rw-rw-rw-  2.0 fat    13023 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/text.py
--rw-rw-rw-  2.0 fat      963 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/text_renderer.py
--rw-rw-rw-  2.0 fat      344 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/type_hints.py
--rw-rw-rw-  2.0 fat     1899 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/unified_text_renderer.py
--rw-rw-rw-  2.0 fat      171 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/__init__.py
--rw-rw-rw-  2.0 fat     3112 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/classes_section.py
--rw-rw-rw-  2.0 fat      763 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/const.py
--rw-rw-rw-  2.0 fat     6091 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/crc.py
--rw-rw-rw-  2.0 fat     3160 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/fileheader.py
--rw-rw-rw-  2.0 fat    14851 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/header_section.py
--rw-rw-rw-  2.0 fat     2976 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/loader.py
--rw-rw-rw-  2.0 fat      141 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/__init__.py
--rw-rw-rw-  2.0 fat     9531 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/api.py
--rw-rw-rw-  2.0 fat     6655 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/backend.py
--rw-rw-rw-  2.0 fat      513 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/compiler.py
--rw-rw-rw-  2.0 fat      571 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/deps.py
--rw-rw-rw-  2.0 fat     4720 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/dxf_backend.py
--rw-rw-rw-  2.0 fat    16087 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/interpreter.py
--rw-rw-rw-  2.0 fat     4836 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/page.py
--rw-rw-rw-  2.0 fat     3527 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/pdf_backend.py
--rw-rw-rw-  2.0 fat    11957 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/plotter.py
--rw-rw-rw-  2.0 fat     1411 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/polygon_buffer.py
--rw-rw-rw-  2.0 fat     5953 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/properties.py
--rw-rw-rw-  2.0 fat     3731 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/svg_backend.py
--rw-rw-rw-  2.0 fat     6258 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/tokenizer.py
--rw-rw-rw-  2.0 fat      164 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/__init__.py
--rw-rw-rw-  2.0 fat     4757 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/acad_proxy_entity.py
--rw-rw-rw-  2.0 fat    18315 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/acad_table.py
--rw-rw-rw-  2.0 fat    25923 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/acis.py
--rw-rw-rw-  2.0 fat     4890 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/appdata.py
--rw-rw-rw-  2.0 fat     1954 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/appid.py
--rw-rw-rw-  2.0 fat     4942 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/arc.py
--rw-rw-rw-  2.0 fat    26138 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/attrib.py
--rw-rw-rw-  2.0 fat     7867 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/block.py
--rw-rw-rw-  2.0 fat    10536 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/blockrecord.py
--rw-rw-rw-  2.0 fat    50143 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/boundary_paths.py
--rw-rw-rw-  2.0 fat     7961 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/circle.py
--rw-rw-rw-  2.0 fat    23664 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dictionary.py
--rw-rw-rw-  2.0 fat    48743 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dimension.py
--rw-rw-rw-  2.0 fat    35012 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dimstyle.py
--rw-rw-rw-  2.0 fat    23829 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dimstyleoverride.py
--rw-rw-rw-  2.0 fat     4399 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dxfclass.py
--rw-rw-rw-  2.0 fat    42404 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dxfentity.py
--rw-rw-rw-  2.0 fat    26923 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dxfgfx.py
--rw-rw-rw-  2.0 fat    15279 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dxfgroups.py
--rw-rw-rw-  2.0 fat    23699 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dxfns.py
--rw-rw-rw-  2.0 fat    13746 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dxfobj.py
--rw-rw-rw-  2.0 fat    11186 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/ellipse.py
--rw-rw-rw-  2.0 fat     4170 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/factory.py
--rw-rw-rw-  2.0 fat    23785 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/geodata.py
--rw-rw-rw-  2.0 fat     4020 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/gradient.py
--rw-rw-rw-  2.0 fat    12263 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/hatch.py
--rw-rw-rw-  2.0 fat     3944 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/helix.py
--rw-rw-rw-  2.0 fat     4747 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/idbuffer.py
--rw-rw-rw-  2.0 fat    26057 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/image.py
--rw-rw-rw-  2.0 fat    27932 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/insert.py
--rw-rw-rw-  2.0 fat    27834 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/layer.py
--rw-rw-rw-  2.0 fat    14252 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/layout.py
--rw-rw-rw-  2.0 fat    12978 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/leader.py
--rw-rw-rw-  2.0 fat     4718 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/light.py
--rw-rw-rw-  2.0 fat     3718 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/line.py
--rw-rw-rw-  2.0 fat     9677 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/ltype.py
--rw-rw-rw-  2.0 fat    18878 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/lwpolyline.py
--rw-rw-rw-  2.0 fat    19653 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/material.py
--rw-rw-rw-  2.0 fat    18435 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/mesh.py
--rw-rw-rw-  2.0 fat    57367 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/mleader.py
--rw-rw-rw-  2.0 fat    37144 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/mline.py
--rw-rw-rw-  2.0 fat     8385 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/mpolygon.py
--rw-rw-rw-  2.0 fat    48153 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/mtext.py
--rw-rw-rw-  2.0 fat     4351 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/mtext_columns.py
--rw-rw-rw-  2.0 fat     6284 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/objectcollection.py
--rw-rw-rw-  2.0 fat     2111 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/oleframe.py
--rw-rw-rw-  2.0 fat     4332 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/pattern.py
--rw-rw-rw-  2.0 fat     5238 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/point.py
--rw-rw-rw-  2.0 fat    16416 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/polygon.py
--rw-rw-rw-  2.0 fat    40087 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/polyline.py
--rw-rw-rw-  2.0 fat     4822 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/shape.py
--rw-rw-rw-  2.0 fat    10443 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/solid.py
--rw-rw-rw-  2.0 fat    24085 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/spline.py
--rw-rw-rw-  2.0 fat     8246 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/subentity.py
--rw-rw-rw-  2.0 fat     5196 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/sun.py
--rw-rw-rw-  2.0 fat     2449 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/table.py
--rw-rw-rw-  2.0 fat    17602 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/text.py
--rw-rw-rw-  2.0 fat     9035 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/textstyle.py
--rw-rw-rw-  2.0 fat     3597 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/tolerance.py
--rw-rw-rw-  2.0 fat     2703 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/ucs.py
--rw-rw-rw-  2.0 fat    14366 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/underlay.py
--rw-rw-rw-  2.0 fat     6040 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/view.py
--rw-rw-rw-  2.0 fat    27893 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/viewport.py
--rw-rw-rw-  2.0 fat     7867 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/visualstyle.py
--rw-rw-rw-  2.0 fat     9970 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/vport.py
--rw-rw-rw-  2.0 fat    17024 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/xdata.py
--rw-rw-rw-  2.0 fat     8495 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/xdict.py
--rw-rw-rw-  2.0 fat     3062 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/xline.py
--rw-rw-rw-  2.0 fat     3127 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/__init__.py
--rw-rw-rw-  2.0 fat    22867 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/fonts.py
--rw-rw-rw-  2.0 fat     2242 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/font_face.py
--rw-rw-rw-  2.0 fat    15227 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/font_manager.py
--rw-rw-rw-  2.0 fat     1702 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/font_measurements.py
--rw-rw-rw-  2.0 fat      825 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/glyphs.py
--rw-rw-rw-  2.0 fat    10794 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/lff.py
--rw-rw-rw-  2.0 fat    35217 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/shapefile.py
--rw-rw-rw-  2.0 fat     7086 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/ttfonts.py
--rw-rw-rw-  2.0 fat       64 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/__init__.py
--rw-rw-rw-  2.0 fat    16696 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/layouts/base.py
--rw-rw-rw-  2.0 fat     4343 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/layouts/blocklayout.py
--rw-rw-rw-  2.0 fat    29014 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/layouts/layout.py
--rw-rw-rw-  2.0 fat    15314 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/layouts/layouts.py
--rw-rw-rw-  2.0 fat      232 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/layouts/__init__.py
--rw-rw-rw-  2.0 fat     8327 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/attributes.py
--rw-rw-rw-  2.0 fat    16500 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/const.py
--rw-rw-rw-  2.0 fat     1614 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/encoding.py
--rw-rw-rw-  2.0 fat    17013 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/extendedtags.py
--rw-rw-rw-  2.0 fat     5363 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/fileindex.py
--rw-rw-rw-  2.0 fat      727 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/hdrvars.py
--rw-rw-rw-  2.0 fat     5469 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/loader.py
--rw-rw-rw-  2.0 fat     7447 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/packedtags.py
--rw-rw-rw-  2.0 fat     6355 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/repair.py
--rw-rw-rw-  2.0 fat    13058 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/tagger.py
--rw-rw-rw-  2.0 fat    14336 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/tags.py
--rw-rw-rw-  2.0 fat     8952 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/tagwriter.py
--rw-rw-rw-  2.0 fat    12064 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/types.py
--rw-rw-rw-  2.0 fat    17069 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/validator.py
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/__init__.py
--rw-rw-rw-  2.0 fat    19193 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/arc.py
--rw-rw-rw-  2.0 fat    16270 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/bbox.py
--rw-rw-rw-  2.0 fat     9318 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/bezier.py
--rw-rw-rw-  2.0 fat     2452 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/bezier_interpolation.py
--rw-rw-rw-  2.0 fat     8730 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/box.py
--rw-rw-rw-  2.0 fat    52916 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/bspline.py
--rw-rw-rw-  2.0 fat     5608 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/bulge.py
--rw-rw-rw-  2.0 fat     9002 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/circle.py
--rw-rw-rw-  2.0 fat    24003 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/clipping.py
--rw-rw-rw-  2.0 fat     4319 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/clustering.py
--rw-rw-rw-  2.0 fat    12236 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/construct2d.py
--rw-rw-rw-  2.0 fat    26265 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/construct3d.py
--rw-rw-rw-  2.0 fat     1283 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/cspline.py
--rw-rw-rw-  2.0 fat     9114 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/curvetools.py
--rw-rw-rw-  2.0 fat    22048 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/ellipse.py
--rw-rw-rw-  2.0 fat     4406 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/eulerspiral.py
--rw-rw-rw-  2.0 fat    38883 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/linalg.py
--rw-rw-rw-  2.0 fat    10231 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/line.py
--rw-rw-rw-  2.0 fat     3053 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/offset2d.py
--rw-rw-rw-  2.0 fat     8256 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/parametrize.py
--rw-rw-rw-  2.0 fat    15602 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/perlin.py
--rw-rw-rw-  2.0 fat    15921 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/polyline.py
--rw-rw-rw-  2.0 fat    11867 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/rtree.py
--rw-rw-rw-  2.0 fat     3910 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/shape.py
--rw-rw-rw-  2.0 fat     2568 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/surfaces.py
--rw-rw-rw-  2.0 fat    12155 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/transformtools.py
--rw-rw-rw-  2.0 fat     3631 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/triangulation.py
--rw-rw-rw-  2.0 fat    16971 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/ucs.py
--rw-rw-rw-  2.0 fat     7213 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_bezier3p.py
--rw-rw-rw-  2.0 fat    12967 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_bezier4p.py
--rw-rw-rw-  2.0 fat     9440 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_bspline.py
--rw-rw-rw-  2.0 fat     7272 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_construct.py
--rw-rw-rw-  2.0 fat     2261 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_ctypes.py
--rw-rw-rw-  2.0 fat    24954 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    27606 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_matrix44.py
--rw-rw-rw-  2.0 fat    25912 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_vector.py
--rw-rw-rw-  2.0 fat     2003 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/__init__.py
--rw-rw-rw-  2.0 fat     1306 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/path/commands.py
--rw-rw-rw-  2.0 fat    39194 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/path/converter.py
--rw-rw-rw-  2.0 fat     6748 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/path/nesting.py
--rw-rw-rw-  2.0 fat    20453 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/path/path.py
--rw-rw-rw-  2.0 fat    10140 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/path/shapes.py
--rw-rw-rw-  2.0 fat    34692 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/path/tools.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/path/__init__.py
--rw-rw-rw-  2.0 fat     2987 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.css
--rw-rw-rw-  2.0 fat     1148 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.html
--rw-rw-rw-  2.0 fat    11304 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.js
--rw-rw-rw-  2.0 fat    17144 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.py
--rw-rw-rw-  2.0 fat     3770 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/pprint.py
--rw-rw-rw-  2.0 fat      812 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.css
--rw-rw-rw-  2.0 fat      316 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.html
--rw-rw-rw-  2.0 fat     2545 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.py
--rw-rw-rw-  2.0 fat     6896 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/reflinks.py
--rw-rw-rw-  2.0 fat      123 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/__init__.py
--rw-rw-rw-  2.0 fat    10039 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/abstract_mtext_renderer.py
--rw-rw-rw-  2.0 fat    20495 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/arrows.py
--rw-rw-rw-  2.0 fat    17749 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/curves.py
--rw-rw-rw-  2.0 fat     4041 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/dimension.py
--rw-rw-rw-  2.0 fat    52028 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/dim_base.py
--rw-rw-rw-  2.0 fat    35702 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/dim_curved.py
--rw-rw-rw-  2.0 fat     6894 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/dim_diameter.py
--rw-rw-rw-  2.0 fat    24751 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/dim_linear.py
--rw-rw-rw-  2.0 fat     8084 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/dim_ordinate.py
--rw-rw-rw-  2.0 fat    20295 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/dim_radius.py
--rw-rw-rw-  2.0 fat    47170 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/forms.py
--rw-rw-rw-  2.0 fat    24213 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/hatching.py
--rw-rw-rw-  2.0 fat     4728 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/leader.py
--rw-rw-rw-  2.0 fat      664 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/linetypes.py
--rw-rw-rw-  2.0 fat    64121 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/mesh.py
--rw-rw-rw-  2.0 fat    60923 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/mleader.py
--rw-rw-rw-  2.0 fat     8437 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/mline.py
--rw-rw-rw-  2.0 fat     2964 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/point.py
--rw-rw-rw-  2.0 fat     8736 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/polyline.py
--rw-rw-rw-  2.0 fat     7886 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/r12spline.py
--rw-rw-rw-  2.0 fat    22541 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/trace.py
--rw-rw-rw-  2.0 fat     2881 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/_linetypes.py
--rw-rw-rw-  2.0 fat      778 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/__init__.py
--rw-rw-rw-  2.0 fat     1050 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/16x16.png
--rw-rw-rw-  2.0 fat     1420 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/24x24.png
--rw-rw-rw-  2.0 fat    10638 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/256x256.png
--rw-rw-rw-  2.0 fat     1758 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/32x32.png
--rw-rw-rw-  2.0 fat     2335 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/48x48.png
--rw-rw-rw-  2.0 fat     3050 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/64x64.png
--rw-rw-rw-  2.0 fat     2090 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-copy-64px.png
--rw-rw-rw-  2.0 fat     3109 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-find-64px.png
--rw-rw-rw-  2.0 fat     2388 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-bookmark-64px.png
--rw-rw-rw-  2.0 fat     2519 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-handle-64px.png
--rw-rw-rw-  2.0 fat     2409 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-line-64px.png
--rw-rw-rw-  2.0 fat     2231 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-left-arrow-64px.png
--rw-rw-rw-  2.0 fat     2322 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-next-entity-64px.png
--rw-rw-rw-  2.0 fat     2320 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-prev-entity-64px.png
--rw-rw-rw-  2.0 fat     2244 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-right-arrow-64px.png
--rw-rw-rw-  2.0 fat     2553 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-show-in-tree-64px.png
--rw-rw-rw-  2.0 fat     2373 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-store-bookmark-64px.png
--rw-rw-rw-  2.0 fat    10650 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/acdsdata.py
--rw-rw-rw-  2.0 fat    16508 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/blocks.py
--rw-rw-rw-  2.0 fat    11639 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/classes.py
--rw-rw-rw-  2.0 fat     4137 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/entities.py
--rw-rw-rw-  2.0 fat    11953 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/header.py
--rw-rw-rw-  2.0 fat    60696 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/headervars.py
--rw-rw-rw-  2.0 fat    27009 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/objects.py
--rw-rw-rw-  2.0 fat    26581 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/table.py
--rw-rw-rw-  2.0 fat     5270 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/tables.py
--rw-rw-rw-  2.0 fat       67 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/__init__.py
--rw-rw-rw-  2.0 fat    19711 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/analyze.py
--rw-rw-rw-  2.0 fat    20434 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/binarydata.py
--rw-rw-rw-  2.0 fat     2931 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/codepage.py
--rw-rw-rw-  2.0 fat     7645 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/complex_ltype.py
--rw-rw-rw-  2.0 fat     1782 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/crypt.py
--rw-rw-rw-  2.0 fat     1511 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/debug.py
--rw-rw-rw-  2.0 fat     2341 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/difftags.py
--rw-rw-rw-  2.0 fat     1235 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/handle.py
--rw-rw-rw-  2.0 fat      780 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/indexing.py
--rw-rw-rw-  2.0 fat     2145 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/juliandate.py
--rw-rw-rw-  2.0 fat     6166 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/pattern.py
--rw-rw-rw-  2.0 fat     1256 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/rawloader.py
--rw-rw-rw-  2.0 fat   129174 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/standards.py
--rw-rw-rw-  2.0 fat     6049 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/strip.py
--rw-rw-rw-  2.0 fat     1466 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/test.py
--rw-rw-rw-  2.0 fat    65518 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/text.py
--rw-rw-rw-  2.0 fat    54234 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/text_layout.py
--rw-rw-rw-  2.0 fat     6893 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/text_size.py
--rw-rw-rw-  2.0 fat     3077 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/zipmanager.py
--rw-rw-rw-  2.0 fat   142734 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/_iso_pattern.py
--rw-rw-rw-  2.0 fat     3564 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       47 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/entry_points.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat    69206 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      302 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/requires.txt
--rw-rw-rw-  2.0 fat    31430 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/top_level.txt
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_01_dxf_entities/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_05_tools/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_06_math/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_07_render/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_08_addons/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_09_cython_acceleration/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_10_issues/
--rw-rw-rw-  2.0 fat      410 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/conftest.py
--rw-rw-rw-  2.0 fat     2336 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
--rw-rw-rw-  2.0 fat      780 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
--rw-rw-rw-  2.0 fat     2599 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
--rw-rw-rw-  2.0 fat     1124 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
--rw-rw-rw-  2.0 fat     5456 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
--rw-rw-rw-  2.0 fat      582 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
--rw-rw-rw-  2.0 fat      473 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_011_codepage.py
--rw-rw-rw-  2.0 fat    11593 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py
--rw-rw-rw-  2.0 fat     1191 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
--rw-rw-rw-  2.0 fat     1033 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
--rw-rw-rw-  2.0 fat     4792 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
--rw-rw-rw-  2.0 fat      989 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py
--rw-rw-rw-  2.0 fat     1383 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_018_handle.py
--rw-rw-rw-  2.0 fat     5518 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
--rw-rw-rw-  2.0 fat     8168 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
--rw-rw-rw-  2.0 fat     3787 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
--rw-rw-rw-  2.0 fat      401 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
--rw-rw-rw-  2.0 fat      539 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
--rw-rw-rw-  2.0 fat     2092 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
--rw-rw-rw-  2.0 fat    10917 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_040_tags.py
--rw-rw-rw-  2.0 fat     3073 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
--rw-rw-rw-  2.0 fat     6419 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
--rw-rw-rw-  2.0 fat     1632 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
--rw-rw-rw-  2.0 fat    11265 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
--rw-rw-rw-  2.0 fat     3363 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
--rw-rw-rw-  2.0 fat     1974 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
--rw-rw-rw-  2.0 fat     2321 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
--rw-rw-rw-  2.0 fat      568 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
--rw-rw-rw-  2.0 fat     8682 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
--rw-rw-rw-  2.0 fat     1051 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
--rw-rw-rw-  2.0 fat     1500 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
--rw-rw-rw-  2.0 fat    11689 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py
--rw-rw-rw-  2.0 fat     2893 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_102_appdata.py
--rw-rw-rw-  2.0 fat     2312 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_103_reactors.py
--rw-rw-rw-  2.0 fat     4001 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_104_extension_dict.py
--rw-rw-rw-  2.0 fat    20860 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_105_xdata.py
--rw-rw-rw-  2.0 fat    14169 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_110_dxfentity.py
--rw-rw-rw-  2.0 fat     2433 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
--rw-rw-rw-  2.0 fat     6781 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py
--rw-rw-rw-  2.0 fat      695 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_112b_dxfobj.py
--rw-rw-rw-  2.0 fat     2431 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_113_dxfclass.py
--rw-rw-rw-  2.0 fat     4044 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_114_factory.py
--rw-rw-rw-  2.0 fat     2256 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
--rw-rw-rw-  2.0 fat    15794 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_116_dictionary.py
--rw-rw-rw-  2.0 fat     4999 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_118_appid_table_entry.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
--rw-rw-rw-  2.0 fat     3003 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_120_style_table_entry.py
--rw-rw-rw-  2.0 fat     2943 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
--rw-rw-rw-  2.0 fat      379 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_122_vport_table_entry.py
--rw-rw-rw-  2.0 fat     1113 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_123_view_table_entry.py
--rw-rw-rw-  2.0 fat     8757 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
--rw-rw-rw-  2.0 fat     1698 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_125_image_def.py
--rw-rw-rw-  2.0 fat     1312 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py
--rw-rw-rw-  2.0 fat     1430 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_127_raster_variables.py
--rw-rw-rw-  2.0 fat     1540 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_128_pdf_definition.py
--rw-rw-rw-  2.0 fat     2778 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_129_xrecord.py
--rw-rw-rw-  2.0 fat     2423 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_130_id_buffer.py
--rw-rw-rw-  2.0 fat     2470 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_131_field_list.py
--rw-rw-rw-  2.0 fat     2435 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_132_layer_filter.py
--rw-rw-rw-  2.0 fat     2153 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_133_sun.py
--rw-rw-rw-  2.0 fat      852 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_134_material.py
--rw-rw-rw-  2.0 fat    11497 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_135_geo_data.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_136_vba_project.py
--rw-rw-rw-  2.0 fat     3099 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_137_sortentstable.py
--rw-rw-rw-  2.0 fat      704 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
--rw-rw-rw-  2.0 fat     7570 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_139_user_record.py
--rw-rw-rw-  2.0 fat      714 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_140_block_record.py
--rw-rw-rw-  2.0 fat     9153 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py
--rw-rw-rw-  2.0 fat     2231 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/conftest.py
--rw-rw-rw-  2.0 fat     6532 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_200_line.py
--rw-rw-rw-  2.0 fat     4273 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_201_point.py
--rw-rw-rw-  2.0 fat     6827 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_202_circle.py
--rw-rw-rw-  2.0 fat     8949 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_203_arc.py
--rw-rw-rw-  2.0 fat     2852 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_204_shape.py
--rw-rw-rw-  2.0 fat     8242 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_205_solid.py
--rw-rw-rw-  2.0 fat     8476 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_206_text.py
--rw-rw-rw-  2.0 fat     4947 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_207_attdef.py
--rw-rw-rw-  2.0 fat     6312 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_208_attrib.py
--rw-rw-rw-  2.0 fat     2671 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_209_vertex.py
--rw-rw-rw-  2.0 fat     5930 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_1.py
--rw-rw-rw-  2.0 fat    13489 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_2.py
--rw-rw-rw-  2.0 fat     6650 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py
--rw-rw-rw-  2.0 fat     1780 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
--rw-rw-rw-  2.0 fat     7847 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_211_viewport.py
--rw-rw-rw-  2.0 fat    12629 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_212_insert.py
--rw-rw-rw-  2.0 fat     6024 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_213_minsert.py
--rw-rw-rw-  2.0 fat     3284 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_214_block.py
--rw-rw-rw-  2.0 fat     6882 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_215_dimension.py
--rw-rw-rw-  2.0 fat     4907 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
--rw-rw-rw-  2.0 fat    13186 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
--rw-rw-rw-  2.0 fat     6471 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
--rw-rw-rw-  2.0 fat     5535 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
--rw-rw-rw-  2.0 fat     3056 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
--rw-rw-rw-  2.0 fat     7181 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
--rw-rw-rw-  2.0 fat     2066 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
--rw-rw-rw-  2.0 fat     3615 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
--rw-rw-rw-  2.0 fat     6919 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_221_ellipse.py
--rw-rw-rw-  2.0 fat     2223 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_222_xline.py
--rw-rw-rw-  2.0 fat     1493 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_223_ray.py
--rw-rw-rw-  2.0 fat     2176 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_224_group.py
--rw-rw-rw-  2.0 fat    10917 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_225_mtext.py
--rw-rw-rw-  2.0 fat    12020 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_226_spline.py
--rw-rw-rw-  2.0 fat     5529 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
--rw-rw-rw-  2.0 fat    10893 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
--rw-rw-rw-  2.0 fat    15116 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_228_mesh.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
--rw-rw-rw-  2.0 fat    21421 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
--rw-rw-rw-  2.0 fat     6587 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
--rw-rw-rw-  2.0 fat     3140 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
--rw-rw-rw-  2.0 fat    12486 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
--rw-rw-rw-  2.0 fat     2274 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_231_underlay.py
--rw-rw-rw-  2.0 fat     5243 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_231_underlay_2.py
--rw-rw-rw-  2.0 fat     2294 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_acis.py
--rw-rw-rw-  2.0 fat     6799 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_acis_2.py
--rw-rw-rw-  2.0 fat     1854 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_surface.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_233_helix.py
--rw-rw-rw-  2.0 fat     2040 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_234_light.py
--rw-rw-rw-  2.0 fat     3806 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_235_leader.py
--rw-rw-rw-  2.0 fat    20392 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_236_multileader.py
--rw-rw-rw-  2.0 fat    10992 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_237_mline.py
--rw-rw-rw-  2.0 fat     2356 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_238_tolerance.py
--rw-rw-rw-  2.0 fat    27392 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
--rw-rw-rw-  2.0 fat     4347 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py
--rw-rw-rw-  2.0 fat     1069 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_241_hyperlink.py
--rw-rw-rw-  2.0 fat    11313 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_242_random_transform.py
--rw-rw-rw-  2.0 fat     3725 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_243_replace_entity.py
--rw-rw-rw-  2.0 fat     1445 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
--rw-rw-rw-  2.0 fat     4456 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_245_wipeout.py
--rw-rw-rw-  2.0 fat     6175 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_246_spline_audit.py
--rw-rw-rw-  2.0 fat     8165 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
--rw-rw-rw-  2.0 fat     6003 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_248_mpolygon.py
--rw-rw-rw-  2.0 fat    13682 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
--rw-rw-rw-  2.0 fat     5713 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py
--rw-rw-rw-  2.0 fat     8331 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
--rw-rw-rw-  2.0 fat     7331 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_251_upright.py
--rw-rw-rw-  2.0 fat     4795 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
--rw-rw-rw-  2.0 fat     2082 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_253_ole2frame.py
--rw-rw-rw-  2.0 fat      821 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_254_get_font_name.py
--rw-rw-rw-  2.0 fat     5149 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_300_layout.py
--rw-rw-rw-  2.0 fat     4274 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
--rw-rw-rw-  2.0 fat     5582 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_302_block_references.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py
--rw-rw-rw-  2.0 fat      913 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py
--rw-rw-rw-  2.0 fat     3279 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
--rw-rw-rw-  2.0 fat     2609 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
--rw-rw-rw-  2.0 fat     2343 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_307_groupby.py
--rw-rw-rw-  2.0 fat    17748 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_308_query.py
--rw-rw-rw-  2.0 fat     6382 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_309_query_parser.py
--rw-rw-rw-  2.0 fat     5031 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
--rw-rw-rw-  2.0 fat     5782 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py
--rw-rw-rw-  2.0 fat      647 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_313_redraw_order.py
--rw-rw-rw-  2.0 fat     6128 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py
--rw-rw-rw-  2.0 fat     2750 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py
--rw-rw-rw-  2.0 fat     5208 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
--rw-rw-rw-  2.0 fat     6795 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py
--rw-rw-rw-  2.0 fat     4981 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
--rw-rw-rw-  2.0 fat     2450 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_405_classes.py
--rw-rw-rw-  2.0 fat     9094 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
--rw-rw-rw-  2.0 fat      848 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
--rw-rw-rw-  2.0 fat     3375 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
--rw-rw-rw-  2.0 fat     1433 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
--rw-rw-rw-  2.0 fat     5736 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_410_table.py
--rw-rw-rw-  2.0 fat     6607 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
--rw-rw-rw-  2.0 fat     2246 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
--rw-rw-rw-  2.0 fat    18072 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
--rw-rw-rw-  2.0 fat     4638 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
--rw-rw-rw-  2.0 fat    12327 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
--rw-rw-rw-  2.0 fat     6509 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
--rw-rw-rw-  2.0 fat     5656 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py
--rw-rw-rw-  2.0 fat     5434 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
--rw-rw-rw-  2.0 fat      733 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
--rw-rw-rw-  2.0 fat     1240 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
--rw-rw-rw-  2.0 fat     5007 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
--rw-rw-rw-  2.0 fat      769 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
--rw-rw-rw-  2.0 fat     7289 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_424_audit.py
--rw-rw-rw-  2.0 fat     3737 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
--rw-rw-rw-  2.0 fat     2981 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
--rw-rw-rw-  2.0 fat     2416 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
--rw-rw-rw-  2.0 fat     2533 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
--rw-rw-rw-  2.0 fat   112800 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/conftest.py
--rw-rw-rw-  2.0 fat     5510 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_500_units.py
--rw-rw-rw-  2.0 fat     1052 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_501_truecolor.py
--rw-rw-rw-  2.0 fat     1021 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_502_raw_color.py
--rw-rw-rw-  2.0 fat     1695 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_503_indexing.py
--rw-rw-rw-  2.0 fat     1442 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_504_suppress_zeros.py
--rw-rw-rw-  2.0 fat      216 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_506_version.py
--rw-rw-rw-  2.0 fat      579 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_507_dxf_pretty_printer.py
--rw-rw-rw-  2.0 fat      657 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_508_read_zip.py
--rw-rw-rw-  2.0 fat     1445 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_509_comments.py
--rw-rw-rw-  2.0 fat     1185 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_510_byte_stream.py
--rw-rw-rw-  2.0 fat     4239 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_511_bit_stream.py
--rw-rw-rw-  2.0 fat     5595 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_512_pattern.py
--rw-rw-rw-  2.0 fat     2372 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_513_reorder_entities.py
--rw-rw-rw-  2.0 fat    17710 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_514_text.py
--rw-rw-rw-  2.0 fat     9269 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_515a_fonts_truetype.py
--rw-rw-rw-  2.0 fat     4729 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_515b_fonts_shapefiles.py
--rw-rw-rw-  2.0 fat     2225 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_515c_fonts_lff.py
--rw-rw-rw-  2.0 fat     4002 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_516_zoom.py
--rw-rw-rw-  2.0 fat    34209 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_517_text_layout.py
--rw-rw-rw-  2.0 fat      474 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_518_header_guid.py
--rw-rw-rw-  2.0 fat     3716 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_519_mtext_editor.py
--rw-rw-rw-  2.0 fat     3205 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_520_mtext_context.py
--rw-rw-rw-  2.0 fat    24496 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_521_mtext_parser.py
--rw-rw-rw-  2.0 fat     3863 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_522_text_scanner.py
--rw-rw-rw-  2.0 fat     5207 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_523_text_size.py
--rw-rw-rw-  2.0 fat     5063 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_524_block_reference_manager.py
--rw-rw-rw-  2.0 fat      773 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_525_transparency.py
--rw-rw-rw-  2.0 fat     2133 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_526_explode.py
--rw-rw-rw-  2.0 fat    13521 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_527_gfxattribs.py
--rw-rw-rw-  2.0 fat     2748 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_528_difftags.py
--rw-rw-rw-  2.0 fat     6700 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_529_acis_sat.py
--rw-rw-rw-  2.0 fat     2062 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_530_acis_sab.py
--rw-rw-rw-  2.0 fat    12366 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_531_acis_entities.py
--rw-rw-rw-  2.0 fat     7533 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_532_acis_mesh.py
--rw-rw-rw-  2.0 fat    43206 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_533_shapefiles.py
--rw-rw-rw-  2.0 fat     1034 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_534_dwg_info.py
--rw-rw-rw-  2.0 fat    47915 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_535_xref_basic.py
--rw-rw-rw-  2.0 fat    27614 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_536_xref_conflict.py
--rw-rw-rw-  2.0 fat     6887 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_537_transform.py
--rw-rw-rw-  2.0 fat     2246 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
--rw-rw-rw-  2.0 fat     3159 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_539_npshapes.py
--rw-rw-rw-  2.0 fat     2605 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_540_lff_parser.py
--rw-rw-rw-  2.0 fat     4026 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/conftest.py
--rw-rw-rw-  2.0 fat     7460 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_600_base.py
--rw-rw-rw-  2.0 fat     2098 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_601_bulge.py
--rw-rw-rw-  2.0 fat    14651 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_602_vec3.py
--rw-rw-rw-  2.0 fat     8956 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_603_vec2.py
--rw-rw-rw-  2.0 fat     2801 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_604_banded_matrix.py
--rw-rw-rw-  2.0 fat     9738 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_604_linalg.py
--rw-rw-rw-  2.0 fat    13943 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_605_matrix44.py
--rw-rw-rw-  2.0 fat     5888 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_606_convexhull.py
--rw-rw-rw-  2.0 fat     1010 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_607_perlin_noise.py
--rw-rw-rw-  2.0 fat     3833 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_608_intersection_line_line_2d.py
--rw-rw-rw-  2.0 fat     1676 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_609_point_on_line.py
--rw-rw-rw-  2.0 fat     3171 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_610_ocs.py
--rw-rw-rw-  2.0 fat     7529 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_611_ucs.py
--rw-rw-rw-  2.0 fat     1831 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_612_ucs_pass_trough.py
--rw-rw-rw-  2.0 fat     2586 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_613_point_in_poygon.py
--rw-rw-rw-  2.0 fat    10913 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_614_construct_3d.py
--rw-rw-rw-  2.0 fat      602 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_615_rytz_axis.py
--rw-rw-rw-  2.0 fat     5215 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_616_plane.py
--rw-rw-rw-  2.0 fat      772 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_617_clockwise_orientation.py
--rw-rw-rw-  2.0 fat     6384 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_618_clipping.py
--rw-rw-rw-  2.0 fat    10108 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_619_greiner_hormann.py
--rw-rw-rw-  2.0 fat     2669 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_620_knot.py
--rw-rw-rw-  2.0 fat    18821 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_621_bspline.py
--rw-rw-rw-  2.0 fat     7652 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_622_bsplineu.py
--rw-rw-rw-  2.0 fat    11327 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_623_rbspline.py
--rw-rw-rw-  2.0 fat    10809 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_624_global_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1247 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_626_local_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1967 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_627_bspline_basis.py
--rw-rw-rw-  2.0 fat    10545 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_629_bezier.py
--rw-rw-rw-  2.0 fat    10714 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_630a_bezier4p_base.py
--rw-rw-rw-  2.0 fat    10204 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_630b_bezier4p_functions.py
--rw-rw-rw-  2.0 fat     1683 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_631_euler_spiral.py
--rw-rw-rw-  2.0 fat     4021 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_632_bezier3p.py
--rw-rw-rw-  2.0 fat    19463 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_640_bbox.py
--rw-rw-rw-  2.0 fat     5393 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_641_construction_ray.py
--rw-rw-rw-  2.0 fat     3673 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_642_construction_line.py
--rw-rw-rw-  2.0 fat     9459 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_643_construction_box.py
--rw-rw-rw-  2.0 fat    10941 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_644_construction_circle.py
--rw-rw-rw-  2.0 fat    10988 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_645_construction_arc.py
--rw-rw-rw-  2.0 fat     3422 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_646_offset_vertices_2d.py
--rw-rw-rw-  2.0 fat     7672 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_647_transform_tools.py
--rw-rw-rw-  2.0 fat     8993 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_648_construction_ellipse.py
--rw-rw-rw-  2.0 fat     4243 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_650_elliptic_arc_span.py
--rw-rw-rw-  2.0 fat     9011 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_651_construction_polyline.py
--rw-rw-rw-  2.0 fat     3168 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_652_approx_param_t.py
--rw-rw-rw-  2.0 fat     5806 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_653_polyline_intersection.py
--rw-rw-rw-  2.0 fat     5193 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_654_rtree.py
--rw-rw-rw-  2.0 fat      788 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_655_dbscan.py
--rw-rw-rw-  2.0 fat      834 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_656_k_means.py
--rw-rw-rw-  2.0 fat     4654 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_657_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    11628 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_658_bevel_tools.py
--rw-rw-rw-  2.0 fat     1875 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py
--rw-rw-rw-  2.0 fat     1428 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
--rw-rw-rw-  2.0 fat     1741 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
--rw-rw-rw-  2.0 fat     3307 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_662_is_convex_polygon_2d.py
--rw-rw-rw-  2.0 fat     1466 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_701_arrows.py
--rw-rw-rw-  2.0 fat    17245 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_702_render_forms.py
--rw-rw-rw-  2.0 fat    34220 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_703_mesh_builder.py
--rw-rw-rw-  2.0 fat     3852 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_704_render_linear_dimension.py
--rw-rw-rw-  2.0 fat     1345 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_705_shape.py
--rw-rw-rw-  2.0 fat      483 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_706_random_path.py
--rw-rw-rw-  2.0 fat     5603 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_707_trace.py
--rw-rw-rw-  2.0 fat    33834 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_708a_path.py
--rw-rw-rw-  2.0 fat    27351 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_708b_path_tools.py
--rw-rw-rw-  2.0 fat     3633 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_708c_matplotlib_path_tools.py
--rw-rw-rw-  2.0 fat     3099 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_708d_qpainter_path_tools.py
--rw-rw-rw-  2.0 fat     4589 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_708e_path_shapes.py
--rw-rw-rw-  2.0 fat     4118 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_708f_path_nesting.py
--rw-rw-rw-  2.0 fat     1308 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_709_linetype_renderer.py
--rw-rw-rw-  2.0 fat     2815 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_711_points.py
--rw-rw-rw-  2.0 fat     6594 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_712_render_curved_dimension.py
--rw-rw-rw-  2.0 fat     1472 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_713_mleader_builder.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_714_mleader_render_engine.py
--rw-rw-rw-  2.0 fat    11778 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_715_hatching.py
--rw-rw-rw-  2.0 fat     2626 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
--rw-rw-rw-  2.0 fat     4771 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_800_mtext_surrogate.py
--rw-rw-rw-  2.0 fat     1352 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_801_r12spline.py
--rw-rw-rw-  2.0 fat     7881 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_802_table_painter.py
--rw-rw-rw-  2.0 fat    12386 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_803_entities_to_code.py
--rw-rw-rw-  2.0 fat     6844 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_804_importer.py
--rw-rw-rw-  2.0 fat     2362 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_805_pycsg.py
--rw-rw-rw-  2.0 fat    15467 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_806_acadctb.py
--rw-rw-rw-  2.0 fat     4860 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_807_dwg_loader_basics.py
--rw-rw-rw-  2.0 fat    10862 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_810_drawing_properties.py
--rw-rw-rw-  2.0 fat    11353 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_811a_drawing_frontend.py
--rw-rw-rw-  2.0 fat     2619 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_811b_drawing_recorder.py
--rw-rw-rw-  2.0 fat     4157 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py
--rw-rw-rw-  2.0 fat    12547 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_813_geo_interface.py
--rw-rw-rw-  2.0 fat    14853 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_814_text2path.py
--rw-rw-rw-  2.0 fat    16239 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_815_dxf_browser.py
--rw-rw-rw-  2.0 fat    11275 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_816_bin_packing.py
--rw-rw-rw-  2.0 fat    12554 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_817_genetic_algorithm.py
--rw-rw-rw-  2.0 fat     9008 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_818_meshex.py
--rw-rw-rw-  2.0 fat     1003 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_819_menger_sponge.py
--rw-rw-rw-  2.0 fat     4433 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_820_openscad.py
--rw-rw-rw-  2.0 fat    15527 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_821_hpgl2.py
--rw-rw-rw-  2.0 fat     1322 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
--rw-rw-rw-  2.0 fat      976 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_822_clipper.py
--rw-rw-rw-  2.0 fat     2527 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py
--rw-rw-rw-  2.0 fat     2199 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py
--rw-rw-rw-  2.0 fat     2142 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
--rw-rw-rw-  2.0 fat     3158 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
--rw-rw-rw-  2.0 fat     1452 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
--rw-rw-rw-  2.0 fat     4755 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py
--rw-rw-rw-  2.0 fat     2656 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_10_issues/test_issue_414_bbox_calculation.py
--rw-rw-rw-  2.0 fat     1213 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
--rw-rw-rw-  2.0 fat     2268 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_10_issues/test_issue_574_flattening_error.py
--rw-rw-rw-  2.0 fat     1754 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
--rw-rw-rw-  2.0 fat      682 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_10_issues/test_issue_749_text_layout.py
-829 files, 8541096 bytes uncompressed, 1921652 bytes compressed:  77.5%
+Zip file size: 2098898 bytes, number of entries: 838
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-May-20 08:27 ezdxf-1.1.0b2/LICENSE
+-rw-rw-rw-  2.0 fat      302 b- defN 23-May-20 08:27 ezdxf-1.1.0b2/MANIFEST.in
+-rw-rw-rw-  2.0 fat   101467 b- defN 23-May-20 08:27 ezdxf-1.1.0b2/NEWS.md
+-rw-rw-rw-  2.0 fat    69334 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/PKG-INFO
+-rw-rw-rw-  2.0 fat     6142 b- defN 23-May-20 08:27 ezdxf-1.1.0b2/README.md
+-rw-rw-rw-  2.0 fat       55 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/requirements.txt
+-rw-rw-rw-  2.0 fat       74 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/setup.cfg
+-rw-rw-rw-  2.0 fat     5402 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/
+-rw-rw-rw-  2.0 fat      567 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/check_disable_c_ext_by_config_file.py
+-rw-rw-rw-  2.0 fat      541 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/check_disable_c_ext_by_env_var.py
+-rw-rw-rw-  2.0 fat      410 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/conftest.py
+-rw-rw-rw-  2.0 fat     1054 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_acad_table.py
+-rw-rw-rw-  2.0 fat     4686 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_all_dimline_styles.py
+-rw-rw-rw-  2.0 fat     4133 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_all_ellipse_transformations.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_anonymous_blocks.py
+-rw-rw-rw-  2.0 fat      871 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_audit_critical_dxf_files.py
+-rw-rw-rw-  2.0 fat     1603 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_audit_layouts.py
+-rw-rw-rw-  2.0 fat     1726 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_complex_line_type_2.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_create_basic_graphics.py
+-rw-rw-rw-  2.0 fat     1921 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_document_guid.py
+-rw-rw-rw-  2.0 fat     1832 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_document_page_setup.py
+-rw-rw-rw-  2.0 fat      998 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_dxf_info_scanning.py
+-rw-rw-rw-  2.0 fat     1558 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_entities_iterator.py
+-rw-rw-rw-  2.0 fat      934 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_fix_dulicate_handles.py
+-rw-rw-rw-  2.0 fat     1901 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_geo.py
+-rw-rw-rw-  2.0 fat     1250 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_groups.py
+-rw-rw-rw-  2.0 fat      901 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_hpgl2_addon.py
+-rw-rw-rw-  2.0 fat      630 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_ignore_junk_beyond_EOF.py
+-rw-rw-rw-  2.0 fat     1155 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_launcher.py
+-rw-rw-rw-  2.0 fat      631 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_leica_disto_r12.py
+-rw-rw-rw-  2.0 fat      737 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_load_dxf_unicode_notation.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat     2230 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_mtext_columns.py
+-rw-rw-rw-  2.0 fat     2392 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_mtext_explode_addon.py
+-rw-rw-rw-  2.0 fat     1846 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_mtext_text_frame.py
+-rw-rw-rw-  2.0 fat     1053 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_new_table_entries.py
+-rw-rw-rw-  2.0 fat      887 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_none_ascii_read_write.py
+-rw-rw-rw-  2.0 fat     3435 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_odafc.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_open_binary_DXF_files.py
+-rw-rw-rw-  2.0 fat      751 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_open_coord_order_issue.py
+-rw-rw-rw-  2.0 fat     3842 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_open_exotic_dxf_files.py
+-rw-rw-rw-  2.0 fat      879 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_open_R13_R14.py
+-rw-rw-rw-  2.0 fat     3152 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_polyline_entity.py
+-rw-rw-rw-  2.0 fat     1749 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_preserve_binary_data_in_xrecords.py
+-rw-rw-rw-  2.0 fat     6944 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_r12export.py
+-rw-rw-rw-  2.0 fat     6256 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_r12strict.py
+-rw-rw-rw-  2.0 fat     3410 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_r12writer.py
+-rw-rw-rw-  2.0 fat      567 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_read_file_without_handles.py
+-rw-rw-rw-  2.0 fat     1121 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_read_write_modern_entites.py
+-rw-rw-rw-  2.0 fat     5375 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_recover.py
+-rw-rw-rw-  2.0 fat     1959 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_redraw_order.py
+-rw-rw-rw-  2.0 fat     1819 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_rotated_block_attributes.py
+-rw-rw-rw-  2.0 fat      774 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_surface_entities.py
+-rw-rw-rw-  2.0 fat      928 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_write_fixed_meta_data.py
+-rw-rw-rw-  2.0 fat     1806 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_write_without_handles.py
+-rw-rw-rw-  2.0 fat     3638 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_xref_detach.py
+-rw-rw-rw-  2.0 fat     3060 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/AC1003_LINE_Example.dxf
+-rw-rw-rw-  2.0 fat   179505 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/acad_table_with_blk_ref.dxf
+-rw-rw-rw-  2.0 fat     7956 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/ASCII_R12.dxf
+-rw-rw-rw-  2.0 fat     3761 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r12.dxf
+-rw-rw-rw-  2.0 fat    20914 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r13.dxf
+-rw-rw-rw-  2.0 fat    21137 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r14.dxf
+-rw-rw-rw-  2.0 fat    11564 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r2000.dxf
+-rw-rw-rw-  2.0 fat     6424 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/cc_dxflib.dxf
+-rw-rw-rw-  2.0 fat   173753 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/custom_blocks.dxf
+-rw-rw-rw-  2.0 fat    32203 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/duplicate_handles.dxf
+-rw-rw-rw-  2.0 fat    18554 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/dxf_unicode.dxf
+-rw-rw-rw-  2.0 fat     1592 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/empty_handles.dxf
+-rw-rw-rw-  2.0 fat    97103 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/groups.dxf
+-rw-rw-rw-  2.0 fat     9146 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/Leica_Disto_S910.dxf
+-rw-rw-rw-  2.0 fat    17986 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/MODEL.dxf
+-rw-rw-rw-  2.0 fat    25799 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/mtext_columns_R2007.dxf
+-rw-rw-rw-  2.0 fat    23927 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/mtext_columns_R2018.dxf
+-rw-rw-rw-  2.0 fat    98230 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/mtext_framed_columns.dxf
+-rw-rw-rw-  2.0 fat   106574 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/mtext_text_frame.dxf
+-rw-rw-rw-  2.0 fat    12001 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/no_layouts.dxf
+-rw-rw-rw-  2.0 fat    16295 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/PLOTFILE.plt
+-rw-rw-rw-  2.0 fat    28788 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/POLI-ALL210_12.DXF
+-rw-rw-rw-  2.0 fat      144 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+-rw-rw-rw-  2.0 fat   212407 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/recover01.dxf
+-rw-rw-rw-  2.0 fat   115423 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/recover02.dxf
+-rw-rw-rw-  2.0 fat    21178 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/small_r13.dxf
+-rw-rw-rw-  2.0 fat    10326 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/small_r14.dxf
+-rw-rw-rw-  2.0 fat    11286 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/XRECORD_0.bin
+-rw-rw-rw-  2.0 fat    11662 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/XRECORD_1.bin
+-rw-rw-rw-  2.0 fat    15337 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/XRECORD_2.bin
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/
+-rw-rw-rw-  2.0 fat     4710 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/appsettings.py
+-rw-rw-rw-  2.0 fat    19818 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/audit.py
+-rw-rw-rw-  2.0 fat     5324 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/bbox.py
+-rw-rw-rw-  2.0 fat     7888 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/blkrefs.py
+-rw-rw-rw-  2.0 fat    13157 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/colors.py
+-rw-rw-rw-  2.0 fat    32340 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/commands.py
+-rw-rw-rw-  2.0 fat     1549 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/comments.py
+-rw-rw-rw-  2.0 fat    22100 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/disassemble.py
+-rw-rw-rw-  2.0 fat    52708 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/document.py
+-rw-rw-rw-  2.0 fat      832 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/dwginfo.py
+-rw-rw-rw-  2.0 fat    16248 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entitydb.py
+-rw-rw-rw-  2.0 fat     7495 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/enums.py
+-rw-rw-rw-  2.0 fat    13948 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/explode.py
+-rw-rw-rw-  2.0 fat     1653 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/eztypes.py
+-rw-rw-rw-  2.0 fat    10333 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/filemanagement.py
+-rw-rw-rw-  2.0 fat    12157 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/gfxattribs.py
+-rw-rw-rw-  2.0 fat   107500 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/graphicsfactory.py
+-rw-rw-rw-  2.0 fat     3416 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/groupby.py
+-rw-rw-rw-  2.0 fat     3241 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/npshapes.py
+-rw-rw-rw-  2.0 fat     2567 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/protocols.py
+-rw-rw-rw-  2.0 fat    33129 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/proxygraphic.py
+-rw-rw-rw-  2.0 fat       95 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/py.typed
+-rw-rw-rw-  2.0 fat    22499 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/query.py
+-rw-rw-rw-  2.0 fat     2780 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/queryparser.py
+-rw-rw-rw-  2.0 fat     9580 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/r12strict.py
+-rw-rw-rw-  2.0 fat    30769 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/recover.py
+-rw-rw-rw-  2.0 fat     3515 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/reorder.py
+-rw-rw-rw-  2.0 fat    10364 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/transform.py
+-rw-rw-rw-  2.0 fat     5750 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/units.py
+-rw-rw-rw-  2.0 fat     8280 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/upright.py
+-rw-rw-rw-  2.0 fat     9875 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/urecord.py
+-rw-rw-rw-  2.0 fat     1024 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/version.py
+-rw-rw-rw-  2.0 fat    63359 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/xref.py
+-rw-rw-rw-  2.0 fat     2853 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/zoom.py
+-rw-rw-rw-  2.0 fat    10986 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/_options.py
+-rw-rw-rw-  2.0 fat     2566 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/__init__.py
+-rw-rw-rw-  2.0 fat     3259 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/__main__.py
+-rw-rw-rw-  2.0 fat     6072 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/bezier3p.pyx
+-rw-rw-rw-  2.0 fat     9983 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/bezier4p.pyx
+-rw-rw-rw-  2.0 fat    12964 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/bspline.pyx
+-rw-rw-rw-  2.0 fat       90 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/construct.pxd
+-rw-rw-rw-  2.0 fat     6584 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/construct.pyx
+-rw-rw-rw-  2.0 fat     3113 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/linetypes.pyx
+-rw-rw-rw-  2.0 fat    23989 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/mapbox_earcut.pyx
+-rw-rw-rw-  2.0 fat      386 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/matrix44.pxd
+-rw-rw-rw-  2.0 fat    23742 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/matrix44.pyx
+-rw-rw-rw-  2.0 fat     2014 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/vector.pxd
+-rw-rw-rw-  2.0 fat    23705 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/vector.pyx
+-rw-rw-rw-  2.0 fat     1784 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.cpp
+-rw-rw-rw-  2.0 fat      599 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.hpp
+-rw-rw-rw-  2.0 fat      424 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.pxd
+-rw-rw-rw-  2.0 fat      960 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_quad_bezier.cpp
+-rw-rw-rw-  2.0 fat      464 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_quad_bezier.hpp
+-rw-rw-rw-  2.0 fat      407 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_quad_bezier.pxd
+-rw-rw-rw-  2.0 fat     2135 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_vec3.hpp
+-rw-rw-rw-  2.0 fat      572 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_vec3.pxd
+-rw-rw-rw-  2.0 fat     1265 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/__init__.py
+-rw-rw-rw-  2.0 fat     6393 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/abstract.py
+-rw-rw-rw-  2.0 fat      884 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/api.py
+-rw-rw-rw-  2.0 fat     5484 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/const.py
+-rw-rw-rw-  2.0 fat     6726 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/dbg.py
+-rw-rw-rw-  2.0 fat     2980 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/dxf.py
+-rw-rw-rw-  2.0 fat    28991 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/entities.py
+-rw-rw-rw-  2.0 fat     4088 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/hdr.py
+-rw-rw-rw-  2.0 fat    12823 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/mesh.py
+-rw-rw-rw-  2.0 fat    18690 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/sab.py
+-rw-rw-rw-  2.0 fat    13184 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/sat.py
+-rw-rw-rw-  2.0 fat      115 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/__init__.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/
+-rw-rw-rw-  2.0 fat    26415 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/acadctb.py
+-rw-rw-rw-  2.0 fat    22229 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/binpacking.py
+-rw-rw-rw-  2.0 fat    27692 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dimlines.py
+-rw-rw-rw-  2.0 fat    31371 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dxf2code.py
+-rw-rw-rw-  2.0 fat    22037 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/genetic_algorithm.py
+-rw-rw-rw-  2.0 fat    36445 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/geo.py
+-rw-rw-rw-  2.0 fat     2674 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/gerber_D6673.py
+-rw-rw-rw-  2.0 fat    25472 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/importer.py
+-rw-rw-rw-  2.0 fat    17355 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/iterdxf.py
+-rw-rw-rw-  2.0 fat     8940 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/menger_sponge.py
+-rw-rw-rw-  2.0 fat    24787 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/meshex.py
+-rw-rw-rw-  2.0 fat      492 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/mixins.py
+-rw-rw-rw-  2.0 fat     6203 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/mtextsurrogate.py
+-rw-rw-rw-  2.0 fat    13528 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/mtxpl.py
+-rw-rw-rw-  2.0 fat    16400 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/odafc.py
+-rw-rw-rw-  2.0 fat     9456 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/openscad.py
+-rw-rw-rw-  2.0 fat    15878 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/pycsg.py
+-rw-rw-rw-  2.0 fat    22496 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/r12export.py
+-rw-rw-rw-  2.0 fat    27198 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/r12writer.py
+-rw-rw-rw-  2.0 fat     7615 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/sierpinski_pyramid.py
+-rw-rw-rw-  2.0 fat    33167 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/tablepainter.py
+-rw-rw-rw-  2.0 fat    12789 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/text2path.py
+-rw-rw-rw-  2.0 fat     3623 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/xplayer.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/xqt.py
+-rw-rw-rw-  2.0 fat      453 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/__init__.py
+-rw-rw-rw-  2.0 fat    10023 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/browser.py
+-rw-rw-rw-  2.0 fat     1907 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/data.py
+-rw-rw-rw-  2.0 fat       64 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/__init__.py
+-rw-rw-rw-  2.0 fat      820 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/bookmarks.py
+-rw-rw-rw-  2.0 fat    29367 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/browser.py
+-rw-rw-rw-  2.0 fat    14891 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/data.py
+-rw-rw-rw-  2.0 fat    10993 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/find_dialog.py
+-rw-rw-rw-  2.0 fat     1281 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/loader.py
+-rw-rw-rw-  2.0 fat    20974 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/model.py
+-rw-rw-rw-  2.0 fat     2214 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/tags.py
+-rw-rw-rw-  2.0 fat     1382 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/views.py
+-rw-rw-rw-  2.0 fat      133 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/__init__.py
+-rw-rw-rw-  2.0 fat     7319 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/backend.py
+-rw-rw-rw-  2.0 fat     3960 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/clipper.py
+-rw-rw-rw-  2.0 fat     8991 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/config.py
+-rw-rw-rw-  2.0 fat     1707 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/debug_backend.py
+-rw-rw-rw-  2.0 fat      514 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/debug_utils.py
+-rw-rw-rw-  2.0 fat    44702 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/frontend.py
+-rw-rw-rw-  2.0 fat     1823 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/gfxproxy.py
+-rw-rw-rw-  2.0 fat    14228 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/layout.py
+-rw-rw-rw-  2.0 fat    12660 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/matplotlib.py
+-rw-rw-rw-  2.0 fat     9878 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/mtext_complex.py
+-rw-rw-rw-  2.0 fat    39035 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/properties.py
+-rw-rw-rw-  2.0 fat    11034 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/pyqt.py
+-rw-rw-rw-  2.0 fat    22624 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/qtviewer.py
+-rw-rw-rw-  2.0 fat     8944 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/recorder.py
+-rw-rw-rw-  2.0 fat    14774 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/svg.py
+-rw-rw-rw-  2.0 fat    13023 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/text.py
+-rw-rw-rw-  2.0 fat      963 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/text_renderer.py
+-rw-rw-rw-  2.0 fat      344 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/type_hints.py
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/unified_text_renderer.py
+-rw-rw-rw-  2.0 fat      171 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/__init__.py
+-rw-rw-rw-  2.0 fat     3112 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/classes_section.py
+-rw-rw-rw-  2.0 fat      763 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/const.py
+-rw-rw-rw-  2.0 fat     6091 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/crc.py
+-rw-rw-rw-  2.0 fat     3160 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/fileheader.py
+-rw-rw-rw-  2.0 fat    14851 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/header_section.py
+-rw-rw-rw-  2.0 fat     2976 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/loader.py
+-rw-rw-rw-  2.0 fat      141 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/__init__.py
+-rw-rw-rw-  2.0 fat     9537 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/api.py
+-rw-rw-rw-  2.0 fat     8208 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/backend.py
+-rw-rw-rw-  2.0 fat      513 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/compiler.py
+-rw-rw-rw-  2.0 fat      571 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/deps.py
+-rw-rw-rw-  2.0 fat     4720 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/dxf_backend.py
+-rw-rw-rw-  2.0 fat    16087 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/interpreter.py
+-rw-rw-rw-  2.0 fat     4836 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/page.py
+-rw-rw-rw-  2.0 fat     3527 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/pdf_backend.py
+-rw-rw-rw-  2.0 fat    11957 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/plotter.py
+-rw-rw-rw-  2.0 fat     1411 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/polygon_buffer.py
+-rw-rw-rw-  2.0 fat     5953 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/properties.py
+-rw-rw-rw-  2.0 fat     3731 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/svg_backend.py
+-rw-rw-rw-  2.0 fat     6258 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/tokenizer.py
+-rw-rw-rw-  2.0 fat    14190 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/viewer.py
+-rw-rw-rw-  2.0 fat      164 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/__init__.py
+-rw-rw-rw-  2.0 fat     4757 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat    18315 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/acad_table.py
+-rw-rw-rw-  2.0 fat    25923 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/acis.py
+-rw-rw-rw-  2.0 fat     4890 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/appdata.py
+-rw-rw-rw-  2.0 fat     1954 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/appid.py
+-rw-rw-rw-  2.0 fat     4942 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/arc.py
+-rw-rw-rw-  2.0 fat    26138 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/attrib.py
+-rw-rw-rw-  2.0 fat     7867 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/block.py
+-rw-rw-rw-  2.0 fat    10536 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/blockrecord.py
+-rw-rw-rw-  2.0 fat    50143 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/boundary_paths.py
+-rw-rw-rw-  2.0 fat     7961 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/circle.py
+-rw-rw-rw-  2.0 fat    23664 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dictionary.py
+-rw-rw-rw-  2.0 fat    48743 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dimension.py
+-rw-rw-rw-  2.0 fat    35012 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dimstyle.py
+-rw-rw-rw-  2.0 fat    23829 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dimstyleoverride.py
+-rw-rw-rw-  2.0 fat     4399 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dxfclass.py
+-rw-rw-rw-  2.0 fat    42404 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dxfentity.py
+-rw-rw-rw-  2.0 fat    26923 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dxfgfx.py
+-rw-rw-rw-  2.0 fat    15279 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dxfgroups.py
+-rw-rw-rw-  2.0 fat    23699 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dxfns.py
+-rw-rw-rw-  2.0 fat    13746 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dxfobj.py
+-rw-rw-rw-  2.0 fat    11186 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/ellipse.py
+-rw-rw-rw-  2.0 fat     4170 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/factory.py
+-rw-rw-rw-  2.0 fat    23785 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/geodata.py
+-rw-rw-rw-  2.0 fat     4020 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/gradient.py
+-rw-rw-rw-  2.0 fat    12263 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/hatch.py
+-rw-rw-rw-  2.0 fat     3944 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/helix.py
+-rw-rw-rw-  2.0 fat     4747 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/idbuffer.py
+-rw-rw-rw-  2.0 fat    26057 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/image.py
+-rw-rw-rw-  2.0 fat    27932 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/insert.py
+-rw-rw-rw-  2.0 fat    27834 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/layer.py
+-rw-rw-rw-  2.0 fat    14252 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/layout.py
+-rw-rw-rw-  2.0 fat    12978 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/leader.py
+-rw-rw-rw-  2.0 fat     4718 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/light.py
+-rw-rw-rw-  2.0 fat     3718 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/line.py
+-rw-rw-rw-  2.0 fat     9677 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/ltype.py
+-rw-rw-rw-  2.0 fat    18878 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/lwpolyline.py
+-rw-rw-rw-  2.0 fat    19653 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/material.py
+-rw-rw-rw-  2.0 fat    18435 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/mesh.py
+-rw-rw-rw-  2.0 fat    57367 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/mleader.py
+-rw-rw-rw-  2.0 fat    37144 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/mline.py
+-rw-rw-rw-  2.0 fat     8385 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/mpolygon.py
+-rw-rw-rw-  2.0 fat    48153 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/mtext.py
+-rw-rw-rw-  2.0 fat     4351 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/mtext_columns.py
+-rw-rw-rw-  2.0 fat     6284 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/objectcollection.py
+-rw-rw-rw-  2.0 fat     2111 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/oleframe.py
+-rw-rw-rw-  2.0 fat     4332 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/pattern.py
+-rw-rw-rw-  2.0 fat     5238 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/point.py
+-rw-rw-rw-  2.0 fat    16416 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/polygon.py
+-rw-rw-rw-  2.0 fat    40087 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/polyline.py
+-rw-rw-rw-  2.0 fat     4822 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/shape.py
+-rw-rw-rw-  2.0 fat    10443 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/solid.py
+-rw-rw-rw-  2.0 fat    24085 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/spline.py
+-rw-rw-rw-  2.0 fat     8246 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/subentity.py
+-rw-rw-rw-  2.0 fat     5196 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/sun.py
+-rw-rw-rw-  2.0 fat     2449 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/table.py
+-rw-rw-rw-  2.0 fat    17602 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/text.py
+-rw-rw-rw-  2.0 fat     9035 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/textstyle.py
+-rw-rw-rw-  2.0 fat     3597 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/tolerance.py
+-rw-rw-rw-  2.0 fat     2703 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/ucs.py
+-rw-rw-rw-  2.0 fat    14366 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/underlay.py
+-rw-rw-rw-  2.0 fat     6040 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/view.py
+-rw-rw-rw-  2.0 fat    28177 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/viewport.py
+-rw-rw-rw-  2.0 fat     7867 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/visualstyle.py
+-rw-rw-rw-  2.0 fat     9970 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/vport.py
+-rw-rw-rw-  2.0 fat    17024 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/xdata.py
+-rw-rw-rw-  2.0 fat     8495 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/xdict.py
+-rw-rw-rw-  2.0 fat     3062 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/xline.py
+-rw-rw-rw-  2.0 fat     3127 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/__init__.py
+-rw-rw-rw-  2.0 fat    23474 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/fonts.py
+-rw-rw-rw-  2.0 fat     2242 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/font_face.py
+-rw-rw-rw-  2.0 fat    17004 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/font_manager.py
+-rw-rw-rw-  2.0 fat     1702 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/font_measurements.py
+-rw-rw-rw-  2.0 fat      825 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/glyphs.py
+-rw-rw-rw-  2.0 fat    10794 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/lff.py
+-rw-rw-rw-  2.0 fat    35217 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/shapefile.py
+-rw-rw-rw-  2.0 fat     7219 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/ttfonts.py
+-rw-rw-rw-  2.0 fat       64 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/__init__.py
+-rw-rw-rw-  2.0 fat    16696 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/layouts/base.py
+-rw-rw-rw-  2.0 fat     4343 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/layouts/blocklayout.py
+-rw-rw-rw-  2.0 fat    29369 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/layouts/layout.py
+-rw-rw-rw-  2.0 fat    15314 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/layouts/layouts.py
+-rw-rw-rw-  2.0 fat      232 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/layouts/__init__.py
+-rw-rw-rw-  2.0 fat     8327 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/attributes.py
+-rw-rw-rw-  2.0 fat    16500 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/const.py
+-rw-rw-rw-  2.0 fat     1614 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/encoding.py
+-rw-rw-rw-  2.0 fat    17013 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/extendedtags.py
+-rw-rw-rw-  2.0 fat     5363 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/fileindex.py
+-rw-rw-rw-  2.0 fat      727 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/hdrvars.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/loader.py
+-rw-rw-rw-  2.0 fat     7447 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/packedtags.py
+-rw-rw-rw-  2.0 fat     6355 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/repair.py
+-rw-rw-rw-  2.0 fat    13058 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/tagger.py
+-rw-rw-rw-  2.0 fat    14336 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/tags.py
+-rw-rw-rw-  2.0 fat     8952 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/tagwriter.py
+-rw-rw-rw-  2.0 fat    12064 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/types.py
+-rw-rw-rw-  2.0 fat    17069 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/validator.py
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/__init__.py
+-rw-rw-rw-  2.0 fat    19193 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/arc.py
+-rw-rw-rw-  2.0 fat    16270 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/bbox.py
+-rw-rw-rw-  2.0 fat     9318 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/bezier.py
+-rw-rw-rw-  2.0 fat     2452 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/bezier_interpolation.py
+-rw-rw-rw-  2.0 fat     8730 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/box.py
+-rw-rw-rw-  2.0 fat    52916 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/bspline.py
+-rw-rw-rw-  2.0 fat     5608 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/bulge.py
+-rw-rw-rw-  2.0 fat     9002 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/circle.py
+-rw-rw-rw-  2.0 fat    24003 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/clipping.py
+-rw-rw-rw-  2.0 fat     4319 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/clustering.py
+-rw-rw-rw-  2.0 fat    12236 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/construct2d.py
+-rw-rw-rw-  2.0 fat    26265 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/construct3d.py
+-rw-rw-rw-  2.0 fat     1283 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/cspline.py
+-rw-rw-rw-  2.0 fat     9114 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/curvetools.py
+-rw-rw-rw-  2.0 fat    22048 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/ellipse.py
+-rw-rw-rw-  2.0 fat     4406 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/eulerspiral.py
+-rw-rw-rw-  2.0 fat    38883 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/linalg.py
+-rw-rw-rw-  2.0 fat    10231 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/line.py
+-rw-rw-rw-  2.0 fat     3053 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/offset2d.py
+-rw-rw-rw-  2.0 fat     8256 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/parametrize.py
+-rw-rw-rw-  2.0 fat    15602 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/perlin.py
+-rw-rw-rw-  2.0 fat    15921 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/polyline.py
+-rw-rw-rw-  2.0 fat    11867 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/rtree.py
+-rw-rw-rw-  2.0 fat     3910 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/shape.py
+-rw-rw-rw-  2.0 fat     2568 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/surfaces.py
+-rw-rw-rw-  2.0 fat    12155 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/transformtools.py
+-rw-rw-rw-  2.0 fat     3631 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/triangulation.py
+-rw-rw-rw-  2.0 fat    16971 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/ucs.py
+-rw-rw-rw-  2.0 fat     7213 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_bezier3p.py
+-rw-rw-rw-  2.0 fat    12967 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_bezier4p.py
+-rw-rw-rw-  2.0 fat     9440 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_bspline.py
+-rw-rw-rw-  2.0 fat     7272 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_construct.py
+-rw-rw-rw-  2.0 fat     2261 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_ctypes.py
+-rw-rw-rw-  2.0 fat    24954 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    27606 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_matrix44.py
+-rw-rw-rw-  2.0 fat    25912 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_vector.py
+-rw-rw-rw-  2.0 fat     2003 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/__init__.py
+-rw-rw-rw-  2.0 fat     1306 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/commands.py
+-rw-rw-rw-  2.0 fat    39194 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/converter.py
+-rw-rw-rw-  2.0 fat     6748 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/nesting.py
+-rw-rw-rw-  2.0 fat    20453 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/path.py
+-rw-rw-rw-  2.0 fat    10140 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/shapes.py
+-rw-rw-rw-  2.0 fat    34692 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/tools.py
+-rw-rw-rw-  2.0 fat      385 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/__init__.py
+-rw-rw-rw-  2.0 fat     2987 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.css
+-rw-rw-rw-  2.0 fat     1148 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.html
+-rw-rw-rw-  2.0 fat    11304 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.js
+-rw-rw-rw-  2.0 fat    17144 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.py
+-rw-rw-rw-  2.0 fat     3770 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/pprint.py
+-rw-rw-rw-  2.0 fat      812 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.css
+-rw-rw-rw-  2.0 fat      316 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.html
+-rw-rw-rw-  2.0 fat     2545 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.py
+-rw-rw-rw-  2.0 fat     6896 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/reflinks.py
+-rw-rw-rw-  2.0 fat      123 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/__init__.py
+-rw-rw-rw-  2.0 fat    10039 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/abstract_mtext_renderer.py
+-rw-rw-rw-  2.0 fat    20495 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/arrows.py
+-rw-rw-rw-  2.0 fat    17749 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/curves.py
+-rw-rw-rw-  2.0 fat     4041 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/dimension.py
+-rw-rw-rw-  2.0 fat    52028 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/dim_base.py
+-rw-rw-rw-  2.0 fat    35702 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/dim_curved.py
+-rw-rw-rw-  2.0 fat     6894 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/dim_diameter.py
+-rw-rw-rw-  2.0 fat    24751 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/dim_linear.py
+-rw-rw-rw-  2.0 fat     8084 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/dim_ordinate.py
+-rw-rw-rw-  2.0 fat    20295 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/dim_radius.py
+-rw-rw-rw-  2.0 fat    47170 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/forms.py
+-rw-rw-rw-  2.0 fat    24213 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/hatching.py
+-rw-rw-rw-  2.0 fat     4728 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/leader.py
+-rw-rw-rw-  2.0 fat      664 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/linetypes.py
+-rw-rw-rw-  2.0 fat    64121 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/mesh.py
+-rw-rw-rw-  2.0 fat    60923 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/mleader.py
+-rw-rw-rw-  2.0 fat     8437 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/mline.py
+-rw-rw-rw-  2.0 fat     2964 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/point.py
+-rw-rw-rw-  2.0 fat     8736 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/polyline.py
+-rw-rw-rw-  2.0 fat     7886 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/r12spline.py
+-rw-rw-rw-  2.0 fat    22541 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/trace.py
+-rw-rw-rw-  2.0 fat     2881 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/_linetypes.py
+-rw-rw-rw-  2.0 fat      778 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/__init__.py
+-rw-rw-rw-  2.0 fat     1050 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/16x16.png
+-rw-rw-rw-  2.0 fat     1420 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/24x24.png
+-rw-rw-rw-  2.0 fat    10638 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/256x256.png
+-rw-rw-rw-  2.0 fat     1758 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/32x32.png
+-rw-rw-rw-  2.0 fat     2335 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/48x48.png
+-rw-rw-rw-  2.0 fat     3050 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/64x64.png
+-rw-rw-rw-  2.0 fat     2090 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-copy-64px.png
+-rw-rw-rw-  2.0 fat     3109 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-find-64px.png
+-rw-rw-rw-  2.0 fat     2388 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-bookmark-64px.png
+-rw-rw-rw-  2.0 fat     2519 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-handle-64px.png
+-rw-rw-rw-  2.0 fat     2409 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-line-64px.png
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-left-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2322 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-next-entity-64px.png
+-rw-rw-rw-  2.0 fat     2320 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-prev-entity-64px.png
+-rw-rw-rw-  2.0 fat     2244 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-right-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2553 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-show-in-tree-64px.png
+-rw-rw-rw-  2.0 fat     2373 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-store-bookmark-64px.png
+-rw-rw-rw-  2.0 fat    10650 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/acdsdata.py
+-rw-rw-rw-  2.0 fat    16508 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/blocks.py
+-rw-rw-rw-  2.0 fat    11639 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/classes.py
+-rw-rw-rw-  2.0 fat     4137 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/entities.py
+-rw-rw-rw-  2.0 fat    11953 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/header.py
+-rw-rw-rw-  2.0 fat    60696 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/headervars.py
+-rw-rw-rw-  2.0 fat    27009 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/objects.py
+-rw-rw-rw-  2.0 fat    26581 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/table.py
+-rw-rw-rw-  2.0 fat     5270 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/tables.py
+-rw-rw-rw-  2.0 fat       67 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/__init__.py
+-rw-rw-rw-  2.0 fat    19711 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/analyze.py
+-rw-rw-rw-  2.0 fat    20434 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/binarydata.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/codepage.py
+-rw-rw-rw-  2.0 fat     7645 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/complex_ltype.py
+-rw-rw-rw-  2.0 fat     1782 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/crypt.py
+-rw-rw-rw-  2.0 fat     1511 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/debug.py
+-rw-rw-rw-  2.0 fat     2341 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/difftags.py
+-rw-rw-rw-  2.0 fat     1235 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/handle.py
+-rw-rw-rw-  2.0 fat      780 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/indexing.py
+-rw-rw-rw-  2.0 fat     2145 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/juliandate.py
+-rw-rw-rw-  2.0 fat     6166 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/pattern.py
+-rw-rw-rw-  2.0 fat     1256 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/rawloader.py
+-rw-rw-rw-  2.0 fat   129174 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/standards.py
+-rw-rw-rw-  2.0 fat     6049 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/strip.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/test.py
+-rw-rw-rw-  2.0 fat    65518 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/text.py
+-rw-rw-rw-  2.0 fat    54234 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/text_layout.py
+-rw-rw-rw-  2.0 fat     6893 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/text_size.py
+-rw-rw-rw-  2.0 fat     3077 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/zipmanager.py
+-rw-rw-rw-  2.0 fat   142734 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/_iso_pattern.py
+-rw-rw-rw-  2.0 fat     3564 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat       47 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/not-zip-safe
+-rw-rw-rw-  2.0 fat    69334 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      302 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat    31795 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/top_level.txt
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_09_cython_acceleration/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_10_issues/
+-rw-rw-rw-  2.0 fat      410 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/conftest.py
+-rw-rw-rw-  2.0 fat     2336 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+-rw-rw-rw-  2.0 fat      780 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+-rw-rw-rw-  2.0 fat     2599 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+-rw-rw-rw-  2.0 fat     1124 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+-rw-rw-rw-  2.0 fat     5456 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+-rw-rw-rw-  2.0 fat      582 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+-rw-rw-rw-  2.0 fat      473 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+-rw-rw-rw-  2.0 fat    11593 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+-rw-rw-rw-  2.0 fat     1191 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+-rw-rw-rw-  2.0 fat     1033 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+-rw-rw-rw-  2.0 fat     4792 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+-rw-rw-rw-  2.0 fat      989 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+-rw-rw-rw-  2.0 fat     1383 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_018_handle.py
+-rw-rw-rw-  2.0 fat     5518 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+-rw-rw-rw-  2.0 fat     8168 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+-rw-rw-rw-  2.0 fat     3787 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+-rw-rw-rw-  2.0 fat      401 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+-rw-rw-rw-  2.0 fat      539 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+-rw-rw-rw-  2.0 fat     2092 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_040_tags.py
+-rw-rw-rw-  2.0 fat     3073 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+-rw-rw-rw-  2.0 fat     6419 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+-rw-rw-rw-  2.0 fat     1632 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+-rw-rw-rw-  2.0 fat    11265 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+-rw-rw-rw-  2.0 fat     3363 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+-rw-rw-rw-  2.0 fat     1974 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+-rw-rw-rw-  2.0 fat     2321 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+-rw-rw-rw-  2.0 fat      568 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+-rw-rw-rw-  2.0 fat     8682 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+-rw-rw-rw-  2.0 fat     1051 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
+-rw-rw-rw-  2.0 fat     1500 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+-rw-rw-rw-  2.0 fat    11689 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+-rw-rw-rw-  2.0 fat     2893 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_102_appdata.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_103_reactors.py
+-rw-rw-rw-  2.0 fat     4001 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_104_extension_dict.py
+-rw-rw-rw-  2.0 fat    20860 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_105_xdata.py
+-rw-rw-rw-  2.0 fat    14169 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_110_dxfentity.py
+-rw-rw-rw-  2.0 fat     2433 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+-rw-rw-rw-  2.0 fat     6781 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+-rw-rw-rw-  2.0 fat      695 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_112b_dxfobj.py
+-rw-rw-rw-  2.0 fat     2431 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_113_dxfclass.py
+-rw-rw-rw-  2.0 fat     4044 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_114_factory.py
+-rw-rw-rw-  2.0 fat     2256 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+-rw-rw-rw-  2.0 fat    15794 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_116_dictionary.py
+-rw-rw-rw-  2.0 fat     4999 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+-rw-rw-rw-  2.0 fat      385 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+-rw-rw-rw-  2.0 fat     3003 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_120_style_table_entry.py
+-rw-rw-rw-  2.0 fat     2943 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+-rw-rw-rw-  2.0 fat      379 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+-rw-rw-rw-  2.0 fat     1113 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_123_view_table_entry.py
+-rw-rw-rw-  2.0 fat     8757 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_125_image_def.py
+-rw-rw-rw-  2.0 fat     1312 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+-rw-rw-rw-  2.0 fat     1430 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_127_raster_variables.py
+-rw-rw-rw-  2.0 fat     1540 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_128_pdf_definition.py
+-rw-rw-rw-  2.0 fat     2778 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_129_xrecord.py
+-rw-rw-rw-  2.0 fat     2423 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_130_id_buffer.py
+-rw-rw-rw-  2.0 fat     2470 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_131_field_list.py
+-rw-rw-rw-  2.0 fat     2435 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_132_layer_filter.py
+-rw-rw-rw-  2.0 fat     2153 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_133_sun.py
+-rw-rw-rw-  2.0 fat      852 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_134_material.py
+-rw-rw-rw-  2.0 fat    11497 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_135_geo_data.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_136_vba_project.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_137_sortentstable.py
+-rw-rw-rw-  2.0 fat      704 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+-rw-rw-rw-  2.0 fat     7570 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_139_user_record.py
+-rw-rw-rw-  2.0 fat      714 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_140_block_record.py
+-rw-rw-rw-  2.0 fat     9153 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/conftest.py
+-rw-rw-rw-  2.0 fat     6532 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_200_line.py
+-rw-rw-rw-  2.0 fat     4273 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_201_point.py
+-rw-rw-rw-  2.0 fat     6827 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_202_circle.py
+-rw-rw-rw-  2.0 fat     8949 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_203_arc.py
+-rw-rw-rw-  2.0 fat     2852 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_204_shape.py
+-rw-rw-rw-  2.0 fat     8242 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_205_solid.py
+-rw-rw-rw-  2.0 fat     8476 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_206_text.py
+-rw-rw-rw-  2.0 fat     4947 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_207_attdef.py
+-rw-rw-rw-  2.0 fat     6312 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_208_attrib.py
+-rw-rw-rw-  2.0 fat     2671 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_209_vertex.py
+-rw-rw-rw-  2.0 fat     5930 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_1.py
+-rw-rw-rw-  2.0 fat    13489 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_2.py
+-rw-rw-rw-  2.0 fat     6650 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+-rw-rw-rw-  2.0 fat     1780 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+-rw-rw-rw-  2.0 fat     7847 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_211_viewport.py
+-rw-rw-rw-  2.0 fat    12629 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_212_insert.py
+-rw-rw-rw-  2.0 fat     6024 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_213_minsert.py
+-rw-rw-rw-  2.0 fat     3284 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_214_block.py
+-rw-rw-rw-  2.0 fat     6882 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_215_dimension.py
+-rw-rw-rw-  2.0 fat     4907 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+-rw-rw-rw-  2.0 fat    13186 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+-rw-rw-rw-  2.0 fat     6471 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+-rw-rw-rw-  2.0 fat     5535 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+-rw-rw-rw-  2.0 fat     3056 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+-rw-rw-rw-  2.0 fat     7181 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+-rw-rw-rw-  2.0 fat     2066 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+-rw-rw-rw-  2.0 fat     3615 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+-rw-rw-rw-  2.0 fat     6919 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_221_ellipse.py
+-rw-rw-rw-  2.0 fat     2223 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_222_xline.py
+-rw-rw-rw-  2.0 fat     1493 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_223_ray.py
+-rw-rw-rw-  2.0 fat     2176 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_224_group.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_225_mtext.py
+-rw-rw-rw-  2.0 fat    12020 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_226_spline.py
+-rw-rw-rw-  2.0 fat     5529 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+-rw-rw-rw-  2.0 fat    10893 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+-rw-rw-rw-  2.0 fat    15116 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_228_mesh.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+-rw-rw-rw-  2.0 fat    21421 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+-rw-rw-rw-  2.0 fat     6587 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+-rw-rw-rw-  2.0 fat     3140 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+-rw-rw-rw-  2.0 fat    12486 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+-rw-rw-rw-  2.0 fat     2274 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_231_underlay.py
+-rw-rw-rw-  2.0 fat     5243 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_231_underlay_2.py
+-rw-rw-rw-  2.0 fat     2294 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_acis.py
+-rw-rw-rw-  2.0 fat     6799 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_acis_2.py
+-rw-rw-rw-  2.0 fat     1854 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_surface.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_233_helix.py
+-rw-rw-rw-  2.0 fat     2040 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_234_light.py
+-rw-rw-rw-  2.0 fat     3806 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_235_leader.py
+-rw-rw-rw-  2.0 fat    20392 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_236_multileader.py
+-rw-rw-rw-  2.0 fat    10992 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_237_mline.py
+-rw-rw-rw-  2.0 fat     2356 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_238_tolerance.py
+-rw-rw-rw-  2.0 fat    27392 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+-rw-rw-rw-  2.0 fat     4347 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_241_hyperlink.py
+-rw-rw-rw-  2.0 fat    11313 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_242_random_transform.py
+-rw-rw-rw-  2.0 fat     3725 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_243_replace_entity.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+-rw-rw-rw-  2.0 fat     4456 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_245_wipeout.py
+-rw-rw-rw-  2.0 fat     6175 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_246_spline_audit.py
+-rw-rw-rw-  2.0 fat     8165 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+-rw-rw-rw-  2.0 fat     6003 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_248_mpolygon.py
+-rw-rw-rw-  2.0 fat    13682 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+-rw-rw-rw-  2.0 fat     5713 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+-rw-rw-rw-  2.0 fat     8331 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+-rw-rw-rw-  2.0 fat     7331 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_251_upright.py
+-rw-rw-rw-  2.0 fat     4795 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat     2082 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_253_ole2frame.py
+-rw-rw-rw-  2.0 fat      821 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_254_get_font_name.py
+-rw-rw-rw-  2.0 fat     5149 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_300_layout.py
+-rw-rw-rw-  2.0 fat     4274 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+-rw-rw-rw-  2.0 fat     5582 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_302_block_references.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+-rw-rw-rw-  2.0 fat      913 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+-rw-rw-rw-  2.0 fat     3279 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+-rw-rw-rw-  2.0 fat     2609 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+-rw-rw-rw-  2.0 fat     2343 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_307_groupby.py
+-rw-rw-rw-  2.0 fat    17748 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_308_query.py
+-rw-rw-rw-  2.0 fat     6382 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_309_query_parser.py
+-rw-rw-rw-  2.0 fat     5031 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+-rw-rw-rw-  2.0 fat     5782 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+-rw-rw-rw-  2.0 fat      647 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_313_redraw_order.py
+-rw-rw-rw-  2.0 fat     6128 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+-rw-rw-rw-  2.0 fat     2750 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+-rw-rw-rw-  2.0 fat     5208 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+-rw-rw-rw-  2.0 fat     6795 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+-rw-rw-rw-  2.0 fat     4981 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+-rw-rw-rw-  2.0 fat     2450 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_405_classes.py
+-rw-rw-rw-  2.0 fat     9094 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+-rw-rw-rw-  2.0 fat      848 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+-rw-rw-rw-  2.0 fat     3375 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+-rw-rw-rw-  2.0 fat     1433 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+-rw-rw-rw-  2.0 fat     5736 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_410_table.py
+-rw-rw-rw-  2.0 fat     6607 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+-rw-rw-rw-  2.0 fat    18072 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+-rw-rw-rw-  2.0 fat     4638 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+-rw-rw-rw-  2.0 fat    12327 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+-rw-rw-rw-  2.0 fat     6509 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+-rw-rw-rw-  2.0 fat     5656 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+-rw-rw-rw-  2.0 fat     5434 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+-rw-rw-rw-  2.0 fat      733 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+-rw-rw-rw-  2.0 fat     1240 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+-rw-rw-rw-  2.0 fat     5007 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+-rw-rw-rw-  2.0 fat      769 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+-rw-rw-rw-  2.0 fat     7289 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_424_audit.py
+-rw-rw-rw-  2.0 fat     3737 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+-rw-rw-rw-  2.0 fat     2981 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+-rw-rw-rw-  2.0 fat     2416 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+-rw-rw-rw-  2.0 fat     2533 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+-rw-rw-rw-  2.0 fat   112800 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/conftest.py
+-rw-rw-rw-  2.0 fat     5510 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_500_units.py
+-rw-rw-rw-  2.0 fat     1052 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_501_truecolor.py
+-rw-rw-rw-  2.0 fat     1021 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_502_raw_color.py
+-rw-rw-rw-  2.0 fat     1695 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_503_indexing.py
+-rw-rw-rw-  2.0 fat     1442 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_504_suppress_zeros.py
+-rw-rw-rw-  2.0 fat      216 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_506_version.py
+-rw-rw-rw-  2.0 fat      579 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_507_dxf_pretty_printer.py
+-rw-rw-rw-  2.0 fat      657 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_508_read_zip.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_509_comments.py
+-rw-rw-rw-  2.0 fat     1185 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_510_byte_stream.py
+-rw-rw-rw-  2.0 fat     4239 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_511_bit_stream.py
+-rw-rw-rw-  2.0 fat     5595 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_512_pattern.py
+-rw-rw-rw-  2.0 fat     2372 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_513_reorder_entities.py
+-rw-rw-rw-  2.0 fat    17710 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_514_text.py
+-rw-rw-rw-  2.0 fat     9269 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_515a_fonts_truetype.py
+-rw-rw-rw-  2.0 fat     4729 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_515b_fonts_shapefiles.py
+-rw-rw-rw-  2.0 fat     2225 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_515c_fonts_lff.py
+-rw-rw-rw-  2.0 fat     4002 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_516_zoom.py
+-rw-rw-rw-  2.0 fat    34209 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_517_text_layout.py
+-rw-rw-rw-  2.0 fat      474 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_518_header_guid.py
+-rw-rw-rw-  2.0 fat     3716 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_519_mtext_editor.py
+-rw-rw-rw-  2.0 fat     3205 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_520_mtext_context.py
+-rw-rw-rw-  2.0 fat    24496 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_521_mtext_parser.py
+-rw-rw-rw-  2.0 fat     3863 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_522_text_scanner.py
+-rw-rw-rw-  2.0 fat     5207 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_523_text_size.py
+-rw-rw-rw-  2.0 fat     5063 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_524_block_reference_manager.py
+-rw-rw-rw-  2.0 fat      773 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_525_transparency.py
+-rw-rw-rw-  2.0 fat     2133 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_526_explode.py
+-rw-rw-rw-  2.0 fat    13521 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_527_gfxattribs.py
+-rw-rw-rw-  2.0 fat     2748 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_528_difftags.py
+-rw-rw-rw-  2.0 fat     6700 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_529_acis_sat.py
+-rw-rw-rw-  2.0 fat     2062 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_530_acis_sab.py
+-rw-rw-rw-  2.0 fat    12366 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_531_acis_entities.py
+-rw-rw-rw-  2.0 fat     7533 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_532_acis_mesh.py
+-rw-rw-rw-  2.0 fat    43206 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_533_shapefiles.py
+-rw-rw-rw-  2.0 fat     1034 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_534_dwg_info.py
+-rw-rw-rw-  2.0 fat    47915 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_535_xref_basic.py
+-rw-rw-rw-  2.0 fat    27614 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_536_xref_conflict.py
+-rw-rw-rw-  2.0 fat     6887 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_537_transform.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+-rw-rw-rw-  2.0 fat     3159 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_539_npshapes.py
+-rw-rw-rw-  2.0 fat     2605 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_540_lff_parser.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/conftest.py
+-rw-rw-rw-  2.0 fat     7460 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_600_base.py
+-rw-rw-rw-  2.0 fat     2098 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_601_bulge.py
+-rw-rw-rw-  2.0 fat    14651 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_602_vec3.py
+-rw-rw-rw-  2.0 fat     8956 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_603_vec2.py
+-rw-rw-rw-  2.0 fat     2801 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_604_banded_matrix.py
+-rw-rw-rw-  2.0 fat     9738 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_604_linalg.py
+-rw-rw-rw-  2.0 fat    13943 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_605_matrix44.py
+-rw-rw-rw-  2.0 fat     5888 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_606_convexhull.py
+-rw-rw-rw-  2.0 fat     1010 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_607_perlin_noise.py
+-rw-rw-rw-  2.0 fat     3833 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_608_intersection_line_line_2d.py
+-rw-rw-rw-  2.0 fat     1676 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_609_point_on_line.py
+-rw-rw-rw-  2.0 fat     3171 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_610_ocs.py
+-rw-rw-rw-  2.0 fat     7529 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_611_ucs.py
+-rw-rw-rw-  2.0 fat     1831 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_612_ucs_pass_trough.py
+-rw-rw-rw-  2.0 fat     2586 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_613_point_in_poygon.py
+-rw-rw-rw-  2.0 fat    10913 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_614_construct_3d.py
+-rw-rw-rw-  2.0 fat      602 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_615_rytz_axis.py
+-rw-rw-rw-  2.0 fat     5215 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_616_plane.py
+-rw-rw-rw-  2.0 fat      772 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_617_clockwise_orientation.py
+-rw-rw-rw-  2.0 fat     6384 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_618_clipping.py
+-rw-rw-rw-  2.0 fat    10108 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_619_greiner_hormann.py
+-rw-rw-rw-  2.0 fat     2669 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_620_knot.py
+-rw-rw-rw-  2.0 fat    18821 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_621_bspline.py
+-rw-rw-rw-  2.0 fat     7652 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_622_bsplineu.py
+-rw-rw-rw-  2.0 fat    11327 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_623_rbspline.py
+-rw-rw-rw-  2.0 fat    10809 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_624_global_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1247 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_626_local_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1967 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_627_bspline_basis.py
+-rw-rw-rw-  2.0 fat    10545 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_629_bezier.py
+-rw-rw-rw-  2.0 fat    10714 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_630a_bezier4p_base.py
+-rw-rw-rw-  2.0 fat    10204 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_630b_bezier4p_functions.py
+-rw-rw-rw-  2.0 fat     1683 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_631_euler_spiral.py
+-rw-rw-rw-  2.0 fat     4021 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_632_bezier3p.py
+-rw-rw-rw-  2.0 fat    19463 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_640_bbox.py
+-rw-rw-rw-  2.0 fat     5393 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_641_construction_ray.py
+-rw-rw-rw-  2.0 fat     3673 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_642_construction_line.py
+-rw-rw-rw-  2.0 fat     9459 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_643_construction_box.py
+-rw-rw-rw-  2.0 fat    10941 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_644_construction_circle.py
+-rw-rw-rw-  2.0 fat    10988 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_645_construction_arc.py
+-rw-rw-rw-  2.0 fat     3422 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_646_offset_vertices_2d.py
+-rw-rw-rw-  2.0 fat     7672 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_647_transform_tools.py
+-rw-rw-rw-  2.0 fat     8993 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_648_construction_ellipse.py
+-rw-rw-rw-  2.0 fat     4243 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_650_elliptic_arc_span.py
+-rw-rw-rw-  2.0 fat     9011 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_651_construction_polyline.py
+-rw-rw-rw-  2.0 fat     3168 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_652_approx_param_t.py
+-rw-rw-rw-  2.0 fat     5806 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_653_polyline_intersection.py
+-rw-rw-rw-  2.0 fat     5193 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_654_rtree.py
+-rw-rw-rw-  2.0 fat      788 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_655_dbscan.py
+-rw-rw-rw-  2.0 fat      834 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_656_k_means.py
+-rw-rw-rw-  2.0 fat     4654 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_657_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    11628 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_658_bevel_tools.py
+-rw-rw-rw-  2.0 fat     1875 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1428 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1741 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+-rw-rw-rw-  2.0 fat     3307 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_662_is_convex_polygon_2d.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_701_arrows.py
+-rw-rw-rw-  2.0 fat    17245 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_702_render_forms.py
+-rw-rw-rw-  2.0 fat    34220 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_703_mesh_builder.py
+-rw-rw-rw-  2.0 fat     3852 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_704_render_linear_dimension.py
+-rw-rw-rw-  2.0 fat     1345 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_705_shape.py
+-rw-rw-rw-  2.0 fat      483 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_706_random_path.py
+-rw-rw-rw-  2.0 fat     5603 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_707_trace.py
+-rw-rw-rw-  2.0 fat    33834 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_708a_path.py
+-rw-rw-rw-  2.0 fat    27351 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_708b_path_tools.py
+-rw-rw-rw-  2.0 fat     3633 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_708c_matplotlib_path_tools.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_708d_qpainter_path_tools.py
+-rw-rw-rw-  2.0 fat     4589 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_708e_path_shapes.py
+-rw-rw-rw-  2.0 fat     4118 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_708f_path_nesting.py
+-rw-rw-rw-  2.0 fat     1308 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_709_linetype_renderer.py
+-rw-rw-rw-  2.0 fat     2815 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_711_points.py
+-rw-rw-rw-  2.0 fat     6594 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_712_render_curved_dimension.py
+-rw-rw-rw-  2.0 fat     1472 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_713_mleader_builder.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_714_mleader_render_engine.py
+-rw-rw-rw-  2.0 fat    11778 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_715_hatching.py
+-rw-rw-rw-  2.0 fat     2626 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+-rw-rw-rw-  2.0 fat     4771 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_800_mtext_surrogate.py
+-rw-rw-rw-  2.0 fat     1352 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_801_r12spline.py
+-rw-rw-rw-  2.0 fat     7881 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_802_table_painter.py
+-rw-rw-rw-  2.0 fat    12386 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_803_entities_to_code.py
+-rw-rw-rw-  2.0 fat     6844 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_804_importer.py
+-rw-rw-rw-  2.0 fat     2362 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_805_pycsg.py
+-rw-rw-rw-  2.0 fat    15467 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_806_acadctb.py
+-rw-rw-rw-  2.0 fat     4860 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_807_dwg_loader_basics.py
+-rw-rw-rw-  2.0 fat    10862 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_810_drawing_properties.py
+-rw-rw-rw-  2.0 fat    11353 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_811a_drawing_frontend.py
+-rw-rw-rw-  2.0 fat     4304 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_811b_drawing_recorder.py
+-rw-rw-rw-  2.0 fat     4157 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+-rw-rw-rw-  2.0 fat    12547 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_813_geo_interface.py
+-rw-rw-rw-  2.0 fat    14853 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_814_text2path.py
+-rw-rw-rw-  2.0 fat    16239 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_815_dxf_browser.py
+-rw-rw-rw-  2.0 fat    11275 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_816_bin_packing.py
+-rw-rw-rw-  2.0 fat    12554 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_817_genetic_algorithm.py
+-rw-rw-rw-  2.0 fat     9008 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_818_meshex.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_819_menger_sponge.py
+-rw-rw-rw-  2.0 fat     4433 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_820_openscad.py
+-rw-rw-rw-  2.0 fat    15527 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_821_hpgl2.py
+-rw-rw-rw-  2.0 fat     1322 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+-rw-rw-rw-  2.0 fat      976 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_822_clipper.py
+-rw-rw-rw-  2.0 fat     5284 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_823_drawing_layout.py
+-rw-rw-rw-  2.0 fat     3030 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_824_svg_drawing_backend.py
+-rw-rw-rw-  2.0 fat     2527 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+-rw-rw-rw-  2.0 fat     2199 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+-rw-rw-rw-  2.0 fat     2142 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+-rw-rw-rw-  2.0 fat     3158 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+-rw-rw-rw-  2.0 fat     1452 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+-rw-rw-rw-  2.0 fat     4755 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+-rw-rw-rw-  2.0 fat     2656 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_10_issues/test_issue_414_bbox_calculation.py
+-rw-rw-rw-  2.0 fat     1213 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_10_issues/test_issue_574_flattening_error.py
+-rw-rw-rw-  2.0 fat     1754 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+-rw-rw-rw-  2.0 fat      682 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_10_issues/test_issue_749_text_layout.py
+-rw-rw-rw-  2.0 fat    11094 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
+838 files, 8647859 bytes uncompressed, 1948272 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -1,2488 +1,2515 @@
-Filename: ezdxf-1.1.0b1/
+Filename: ezdxf-1.1.0b2/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/
+Filename: ezdxf-1.1.0b2/integration_tests/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/
+Filename: ezdxf-1.1.0b2/src/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/
+Filename: ezdxf-1.1.0b2/tests/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/LICENSE
+Filename: ezdxf-1.1.0b2/LICENSE
 Comment: 
 
-Filename: ezdxf-1.1.0b1/MANIFEST.in
+Filename: ezdxf-1.1.0b2/MANIFEST.in
 Comment: 
 
-Filename: ezdxf-1.1.0b1/NEWS.md
+Filename: ezdxf-1.1.0b2/NEWS.md
 Comment: 
 
-Filename: ezdxf-1.1.0b1/PKG-INFO
+Filename: ezdxf-1.1.0b2/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.1.0b1/README.md
+Filename: ezdxf-1.1.0b2/README.md
 Comment: 
 
-Filename: ezdxf-1.1.0b1/requirements.txt
+Filename: ezdxf-1.1.0b2/requirements.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b1/setup.cfg
+Filename: ezdxf-1.1.0b2/setup.cfg
 Comment: 
 
-Filename: ezdxf-1.1.0b1/setup.py
+Filename: ezdxf-1.1.0b2/setup.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/
+Filename: ezdxf-1.1.0b2/integration_tests/data/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/check_disable_c_ext_by_config_file.py
+Filename: ezdxf-1.1.0b2/integration_tests/check_disable_c_ext_by_config_file.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/check_disable_c_ext_by_env_var.py
+Filename: ezdxf-1.1.0b2/integration_tests/check_disable_c_ext_by_env_var.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/conftest.py
+Filename: ezdxf-1.1.0b2/integration_tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_acad_table.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_acad_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_all_dimline_styles.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_all_dimline_styles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_all_ellipse_transformations.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_all_ellipse_transformations.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_anonymous_blocks.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_anonymous_blocks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_audit_critical_dxf_files.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_audit_critical_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_audit_layouts.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_audit_layouts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_complex_line_type_2.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_complex_line_type_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_create_basic_graphics.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_create_basic_graphics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_document_guid.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_document_guid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_document_page_setup.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_document_page_setup.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_dxf_info_scanning.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_dxf_info_scanning.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_entities_iterator.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_entities_iterator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_fix_dulicate_handles.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_fix_dulicate_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_geo.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_geo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_groups.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_groups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_ignore_junk_beyond_EOF.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_hpgl2_addon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_launcher.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_ignore_junk_beyond_EOF.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_leica_disto_r12.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_launcher.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_load_dxf_unicode_notation.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_leica_disto_r12.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_mapbox_earcut.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_load_dxf_unicode_notation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_mtext_columns.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_mtext_explode_addon.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_mtext_text_frame.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_mtext_explode_addon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_new_table_entries.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_mtext_text_frame.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_none_ascii_read_write.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_new_table_entries.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_odafc.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_none_ascii_read_write.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_open_binary_DXF_files.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_odafc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_open_coord_order_issue.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_open_binary_DXF_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_open_exotic_dxf_files.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_open_coord_order_issue.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_open_R13_R14.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_open_exotic_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_polyline_entity.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_open_R13_R14.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_preserve_binary_data_in_xrecords.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_polyline_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_r12export.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_preserve_binary_data_in_xrecords.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_r12strict.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_r12export.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_r12writer.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_r12strict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_read_file_without_handles.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_r12writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_read_write_modern_entites.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_read_file_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_recover.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_read_write_modern_entites.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_redraw_order.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_recover.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_rotated_block_attributes.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_surface_entities.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_rotated_block_attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_write_fixed_meta_data.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_surface_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_write_without_handles.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_write_fixed_meta_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/test_xref_detach.py
+Filename: ezdxf-1.1.0b2/integration_tests/test_write_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/AC1003_LINE_Example.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/test_xref_detach.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/acad_table_with_blk_ref.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/AC1003_LINE_Example.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/ASCII_R12.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/acad_table_with_blk_ref.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r12.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/ASCII_R12.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r13.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r12.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r14.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r2000.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/cc_dxflib.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r2000.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/custom_blocks.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/cc_dxflib.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/duplicate_handles.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/custom_blocks.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/dxf_unicode.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/duplicate_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/empty_handles.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/dxf_unicode.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/groups.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/empty_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/Leica_Disto_S910.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/groups.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/MODEL.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/Leica_Disto_S910.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/mtext_columns_R2007.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/MODEL.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/mtext_columns_R2018.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/mtext_columns_R2007.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/mtext_framed_columns.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/mtext_columns_R2018.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/mtext_text_frame.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/mtext_framed_columns.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/no_layouts.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/mtext_text_frame.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/POLI-ALL210_12.DXF
+Filename: ezdxf-1.1.0b2/integration_tests/data/no_layouts.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/PLOTFILE.plt
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/recover01.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/POLI-ALL210_12.DXF
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/recover02.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/R12_with_trash_beyond_EOF.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/small_r13.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/recover01.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/small_r14.dxf
+Filename: ezdxf-1.1.0b2/integration_tests/data/recover02.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/XRECORD_0.bin
+Filename: ezdxf-1.1.0b2/integration_tests/data/small_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/XRECORD_1.bin
+Filename: ezdxf-1.1.0b2/integration_tests/data/small_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b1/integration_tests/data/XRECORD_2.bin
+Filename: ezdxf-1.1.0b2/integration_tests/data/XRECORD_0.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/
+Filename: ezdxf-1.1.0b2/integration_tests/data/XRECORD_1.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/
+Filename: ezdxf-1.1.0b2/integration_tests/data/XRECORD_2.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/
+Filename: ezdxf-1.1.0b2/src/ezdxf/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acis/
+Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/
+Filename: ezdxf-1.1.0b2/src/ezdxf/acis/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/layouts/
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/
+Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/
+Filename: ezdxf-1.1.0b2/src/ezdxf/layouts/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/path/
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/pp/
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/
+Filename: ezdxf-1.1.0b2/src/ezdxf/path/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/
+Filename: ezdxf-1.1.0b2/src/ezdxf/pp/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/sections/
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/appsettings.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/sections/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/audit.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/bbox.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/appsettings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/blkrefs.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/colors.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/commands.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/blkrefs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/comments.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/colors.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/disassemble.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/document.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/comments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/dwginfo.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/disassemble.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entitydb.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/document.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/enums.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/dwginfo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/explode.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entitydb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/eztypes.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/enums.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/filemanagement.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/gfxattribs.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/eztypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/graphicsfactory.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/filemanagement.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/groupby.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/npshapes.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/graphicsfactory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/protocols.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/groupby.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/proxygraphic.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/npshapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/py.typed
+Filename: ezdxf-1.1.0b2/src/ezdxf/protocols.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/query.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/proxygraphic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/queryparser.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/py.typed
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/r12strict.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/query.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/recover.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/queryparser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/reorder.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/r12strict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/transform.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/recover.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/units.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/reorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/upright.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/urecord.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/units.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/version.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/upright.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/xref.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/urecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/zoom.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/version.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/_options.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/xref.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/zoom.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/__main__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/_options.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/bezier3p.pyx
+Filename: ezdxf-1.1.0b2/src/ezdxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/bezier4p.pyx
+Filename: ezdxf-1.1.0b2/src/ezdxf/__main__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/bspline.pyx
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/bezier3p.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/construct.pxd
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/bezier4p.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/construct.pyx
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/bspline.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/linetypes.pyx
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/construct.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/mapbox_earcut.pyx
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/construct.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/matrix44.pxd
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/linetypes.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/matrix44.pyx
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/mapbox_earcut.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/vector.pxd
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/matrix44.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/vector.pyx
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/matrix44.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.cpp
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/vector.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.hpp
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/vector.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.pxd
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.cpp
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_quad_bezier.cpp
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_quad_bezier.hpp
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_quad_bezier.pxd
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_quad_bezier.cpp
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_vec3.hpp
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_quad_bezier.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_vec3.pxd
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_quad_bezier.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acc/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_vec3.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acis/abstract.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_vec3.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acis/api.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/acc/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acis/const.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/acis/abstract.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acis/dbg.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/acis/api.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acis/dxf.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/acis/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acis/entities.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/acis/dbg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acis/hdr.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/acis/dxf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acis/mesh.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/acis/entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acis/sab.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/acis/hdr.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acis/sat.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/acis/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/acis/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/acis/sab.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/
+Filename: ezdxf-1.1.0b2/src/ezdxf/acis/sat.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/
+Filename: ezdxf-1.1.0b2/src/ezdxf/acis/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/acadctb.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/binpacking.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dimlines.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/acadctb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dxf2code.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/binpacking.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/genetic_algorithm.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dimlines.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/geo.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dxf2code.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/gerber_D6673.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/importer.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/geo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/iterdxf.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/gerber_D6673.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/menger_sponge.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/importer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/meshex.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/iterdxf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/mixins.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/mtextsurrogate.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/meshex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/mtxpl.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/mixins.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/odafc.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/mtextsurrogate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/openscad.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/mtxpl.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/pycsg.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/odafc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/r12export.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/openscad.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/r12writer.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/pycsg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/sierpinski_pyramid.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/r12export.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/tablepainter.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/r12writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/text2path.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/sierpinski_pyramid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/xqt.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/tablepainter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/text2path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/browser.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/xplayer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/data.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/xqt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/bookmarks.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/browser.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/data.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/find_dialog.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/bookmarks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/loader.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/model.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/tags.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/find_dialog.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/views.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/model.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/backend.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/clipper.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/views.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/config.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/debug_backend.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/debug_utils.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/clipper.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/frontend.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/config.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/gfxproxy.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/debug_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/matplotlib.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/debug_utils.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/mtext_complex.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/frontend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/properties.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/gfxproxy.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/pyqt.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/qtviewer.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/matplotlib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/recorder.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/mtext_complex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/text.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/text_renderer.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/pyqt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/type_hints.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/qtviewer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/unified_text_renderer.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/recorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/svg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/classes_section.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/const.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/crc.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/type_hints.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/fileheader.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/unified_text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/header_section.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/loader.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/classes_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/api.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/crc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/backend.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/fileheader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/compiler.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/header_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/deps.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/dxf_backend.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/interpreter.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/api.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/page.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/pdf_backend.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/compiler.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/plotter.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/deps.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/polygon_buffer.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/dxf_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/properties.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/interpreter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/svg_backend.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/page.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/tokenizer.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/pdf_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/plotter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/acad_proxy_entity.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/polygon_buffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/acad_table.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/acis.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/svg_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/appdata.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/tokenizer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/appid.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/viewer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/arc.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/attrib.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/block.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/acad_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/blockrecord.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/acis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/boundary_paths.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/appdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/circle.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/appid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dictionary.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dimension.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/attrib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dimstyle.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/block.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dimstyleoverride.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/blockrecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dxfclass.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dxfentity.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dxfgfx.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dictionary.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dxfgroups.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dxfns.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dimstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dxfobj.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dimstyleoverride.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/ellipse.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/factory.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/geodata.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/gradient.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/hatch.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dxfns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/helix.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/idbuffer.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/image.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/factory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/insert.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/geodata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/layer.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/gradient.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/layout.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/hatch.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/leader.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/helix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/light.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/idbuffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/line.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/image.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/ltype.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/insert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/lwpolyline.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/layer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/material.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/mesh.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/mleader.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/light.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/mline.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/mpolygon.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/ltype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/mtext.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/lwpolyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/mtext_columns.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/material.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/objectcollection.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/oleframe.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/mleader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/pattern.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/point.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/polygon.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/mtext.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/polyline.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/shape.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/objectcollection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/solid.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/oleframe.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/spline.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/subentity.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/sun.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/polygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/table.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/text.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/textstyle.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/solid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/tolerance.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/ucs.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/subentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/underlay.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/sun.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/view.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/viewport.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/visualstyle.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/textstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/vport.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/tolerance.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/xdata.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/xdict.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/underlay.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/xline.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/view.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/entities/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/viewport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/fonts.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/visualstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/font_face.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/vport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/font_manager.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/xdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/font_measurements.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/xdict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/glyphs.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/xline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/lff.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/entities/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/shapefile.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/fonts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/ttfonts.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/font_face.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/font_manager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/layouts/base.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/font_measurements.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/layouts/blocklayout.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/glyphs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/layouts/layout.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/lff.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/layouts/layouts.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/shapefile.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/layouts/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/ttfonts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/attributes.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/const.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/layouts/base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/encoding.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/layouts/blocklayout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/extendedtags.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/layouts/layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/fileindex.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/layouts/layouts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/hdrvars.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/layouts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/loader.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/packedtags.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/repair.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/encoding.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/tagger.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/extendedtags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/tags.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/fileindex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/tagwriter.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/hdrvars.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/types.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/validator.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/packedtags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/repair.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/arc.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/tagger.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/bbox.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/bezier.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/tagwriter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/bezier_interpolation.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/types.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/box.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/validator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/bspline.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/bulge.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/circle.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/clipping.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/bezier.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/clustering.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/bezier_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/construct2d.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/box.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/construct3d.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/cspline.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/bulge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/curvetools.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/ellipse.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/clipping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/eulerspiral.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/clustering.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/linalg.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/construct2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/line.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/construct3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/offset2d.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/cspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/parametrize.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/curvetools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/perlin.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/polyline.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/eulerspiral.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/rtree.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/linalg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/shape.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/surfaces.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/offset2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/transformtools.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/parametrize.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/triangulation.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/perlin.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/ucs.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/_bezier3p.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/rtree.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/_bezier4p.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/_bspline.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/surfaces.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/_construct.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/transformtools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/_ctypes.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/triangulation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/_mapbox_earcut.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/_matrix44.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/_vector.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/math/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/_bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/path/commands.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/_construct.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/path/converter.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/_ctypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/path/nesting.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/path/path.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/path/shapes.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/_vector.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/path/tools.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/math/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/path/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/path/commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.css
+Filename: ezdxf-1.1.0b2/src/ezdxf/path/converter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.html
+Filename: ezdxf-1.1.0b2/src/ezdxf/path/nesting.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.js
+Filename: ezdxf-1.1.0b2/src/ezdxf/path/path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/path/shapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/pp/pprint.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/path/tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.css
+Filename: ezdxf-1.1.0b2/src/ezdxf/path/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.html
+Filename: ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.css
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.html
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/pp/reflinks.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.js
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/pp/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/abstract_mtext_renderer.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/pp/pprint.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/arrows.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.css
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/curves.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.html
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/dimension.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/dim_base.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/pp/reflinks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/dim_curved.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/pp/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/dim_diameter.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/abstract_mtext_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/dim_linear.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/arrows.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/dim_ordinate.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/curves.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/dim_radius.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/forms.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/dim_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/hatching.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/dim_curved.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/leader.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/dim_diameter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/linetypes.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/dim_linear.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/mesh.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/dim_ordinate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/mleader.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/dim_radius.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/mline.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/forms.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/point.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/hatching.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/polyline.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/r12spline.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/linetypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/trace.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/_linetypes.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/mleader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/render/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/16x16.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/24x24.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/256x256.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/r12spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/32x32.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/trace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/48x48.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/_linetypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/64x64.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/render/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-copy-64px.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/16x16.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-find-64px.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/24x24.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-bookmark-64px.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/256x256.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-handle-64px.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/32x32.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-line-64px.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/48x48.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-left-arrow-64px.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/64x64.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-next-entity-64px.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-copy-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-prev-entity-64px.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-find-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-right-arrow-64px.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-show-in-tree-64px.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-handle-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-store-bookmark-64px.png
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-line-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/sections/acdsdata.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-left-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/sections/blocks.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-next-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/sections/classes.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-prev-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/sections/entities.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-right-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/sections/header.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-show-in-tree-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/sections/headervars.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-store-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/sections/objects.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/sections/acdsdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/sections/table.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/sections/blocks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/sections/tables.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/sections/classes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/sections/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/sections/entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/analyze.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/sections/header.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/binarydata.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/sections/headervars.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/codepage.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/sections/objects.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/complex_ltype.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/sections/table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/crypt.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/sections/tables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/debug.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/sections/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/difftags.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/analyze.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/handle.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/binarydata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/indexing.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/codepage.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/juliandate.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/complex_ltype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/pattern.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/crypt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/rawloader.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/debug.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/standards.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/difftags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/strip.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/handle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/test.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/indexing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/text.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/juliandate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/text_layout.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/text_size.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/rawloader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/zipmanager.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/standards.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/_iso_pattern.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/strip.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf/tools/__init__.py
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/test.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/dependency_links.txt
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/entry_points.txt
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/text_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/not-zip-safe
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/text_size.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/PKG-INFO
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/zipmanager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/requires.txt
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/_iso_pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/SOURCES.txt
+Filename: ezdxf-1.1.0b2/src/ezdxf/tools/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/top_level.txt
+Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/
+Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/entry_points.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/
+Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/not-zip-safe
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/
+Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/
+Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/requires.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/
+Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/
+Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/top_level.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_09_cython_acceleration/
+Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_10_issues/
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/conftest.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+Filename: ezdxf-1.1.0b2/tests/test_09_cython_acceleration/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+Filename: ezdxf-1.1.0b2/tests/test_10_issues/
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+Filename: ezdxf-1.1.0b2/tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_018_handle.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_011_codepage.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_012_crypt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_016_encoding.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_018_handle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_040_tags.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_040_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_102_appdata.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_103_reactors.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_104_extension_dict.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_105_xdata.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_110_dxfentity.py
+Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_101_dxfnamespace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_102_appdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_112b_dxfobj.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_103_reactors.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_113_dxfclass.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_104_extension_dict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_114_factory.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_105_xdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_110_dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_116_dictionary.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_112a_dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_112b_dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_113_dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_120_style_table_entry.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_114_factory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_116_dictionary.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_123_view_table_entry.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_117_layer_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_118_appid_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_125_image_def.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_120_style_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_127_raster_variables.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_128_pdf_definition.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_122_vport_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_129_xrecord.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_123_view_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_130_id_buffer.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_131_field_list.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_125_image_def.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_132_layer_filter.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_126_image_def_reactor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_133_sun.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_127_raster_variables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_134_material.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_128_pdf_definition.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_135_geo_data.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_129_xrecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_136_vba_project.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_130_id_buffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_137_sortentstable.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_131_field_list.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_132_layer_filter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_139_user_record.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_133_sun.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_140_block_record.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_134_material.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_135_geo_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/conftest.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_136_vba_project.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_200_line.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_137_sortentstable.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_201_point.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_202_circle.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_139_user_record.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_203_arc.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_140_block_record.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_204_shape.py
+Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_141_layer_vp_override.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_205_solid.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_206_text.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_200_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_207_attdef.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_201_point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_208_attrib.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_202_circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_209_vertex.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_203_arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_1.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_204_shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_2.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_205_solid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_206_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_207_attdef.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_211_viewport.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_208_attrib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_212_insert.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_209_vertex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_213_minsert.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_1.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_214_block.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_215_dimension.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_211_viewport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_212_insert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_213_minsert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_214_block.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_215_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_221_ellipse.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_222_xline.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_223_ray.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_224_group.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_225_mtext.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_226_spline.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_221_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_222_xline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_228_mesh.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_223_ray.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_224_group.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_225_mtext.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_226_spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_231_underlay.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_228_mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_231_underlay_2.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_acis.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_acis_2.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_surface.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_233_helix.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_234_light.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_231_underlay.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_235_leader.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_231_underlay_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_236_multileader.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_acis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_237_mline.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_acis_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_238_tolerance.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_surface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_233_helix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_234_light.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_241_hyperlink.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_235_leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_242_random_transform.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_236_multileader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_243_replace_entity.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_237_mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_238_tolerance.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_245_wipeout.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_246_spline_audit.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_240_arc_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_241_hyperlink.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_248_mpolygon.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_242_random_transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_243_replace_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_245_wipeout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_251_upright.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_246_spline_audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_253_ole2frame.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_248_mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_254_get_font_name.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_300_layout.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_249_boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_302_block_references.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_251_upright.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_253_ole2frame.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_254_get_font_name.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_300_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_307_groupby.py
+Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_308_query.py
+Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_302_block_references.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_309_query_parser.py
+Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_303_auto_block_references.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_304_new_entity_space.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_313_redraw_order.py
+Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_307_groupby.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_308_query.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_309_query_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_312_virtual_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_405_classes.py
+Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_313_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_401_headersection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_402_classessection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_404a_tables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_410_table.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_405_classes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_410_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_424_audit.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_417_bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/conftest.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_500_units.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_424_audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_501_truecolor.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_502_raw_color.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_503_indexing.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_504_suppress_zeros.py
+Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_506_version.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_507_dxf_pretty_printer.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_500_units.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_508_read_zip.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_501_truecolor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_509_comments.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_502_raw_color.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_510_byte_stream.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_503_indexing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_511_bit_stream.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_504_suppress_zeros.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_512_pattern.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_506_version.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_513_reorder_entities.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_507_dxf_pretty_printer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_514_text.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_508_read_zip.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_515a_fonts_truetype.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_509_comments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_515b_fonts_shapefiles.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_510_byte_stream.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_515c_fonts_lff.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_511_bit_stream.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_516_zoom.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_512_pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_517_text_layout.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_513_reorder_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_518_header_guid.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_514_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_519_mtext_editor.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_515a_fonts_truetype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_520_mtext_context.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_515b_fonts_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_521_mtext_parser.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_515c_fonts_lff.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_522_text_scanner.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_516_zoom.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_523_text_size.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_517_text_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_524_block_reference_manager.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_518_header_guid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_525_transparency.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_519_mtext_editor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_526_explode.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_520_mtext_context.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_527_gfxattribs.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_521_mtext_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_528_difftags.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_522_text_scanner.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_529_acis_sat.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_523_text_size.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_530_acis_sab.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_524_block_reference_manager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_531_acis_entities.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_525_transparency.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_532_acis_mesh.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_526_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_533_shapefiles.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_527_gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_534_dwg_info.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_528_difftags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_535_xref_basic.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_529_acis_sat.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_536_xref_conflict.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_530_acis_sab.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_537_transform.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_531_acis_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_532_acis_mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_539_npshapes.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_533_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_540_lff_parser.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_534_dwg_info.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/conftest.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_535_xref_basic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_600_base.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_536_xref_conflict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_601_bulge.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_537_transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_602_vec3.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_603_vec2.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_539_npshapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_604_banded_matrix.py
+Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_540_lff_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_604_linalg.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_605_matrix44.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_600_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_606_convexhull.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_601_bulge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_607_perlin_noise.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_602_vec3.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_608_intersection_line_line_2d.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_603_vec2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_609_point_on_line.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_604_banded_matrix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_610_ocs.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_604_linalg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_611_ucs.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_605_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_612_ucs_pass_trough.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_606_convexhull.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_613_point_in_poygon.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_607_perlin_noise.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_614_construct_3d.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_608_intersection_line_line_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_615_rytz_axis.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_609_point_on_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_616_plane.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_610_ocs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_617_clockwise_orientation.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_611_ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_618_clipping.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_612_ucs_pass_trough.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_619_greiner_hormann.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_613_point_in_poygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_620_knot.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_614_construct_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_621_bspline.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_615_rytz_axis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_622_bsplineu.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_616_plane.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_623_rbspline.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_617_clockwise_orientation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_624_global_bspline_interpolation.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_618_clipping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_626_local_bspline_interpolation.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_619_greiner_hormann.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_627_bspline_basis.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_620_knot.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_629_bezier.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_621_bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_630a_bezier4p_base.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_622_bsplineu.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_630b_bezier4p_functions.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_623_rbspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_631_euler_spiral.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_624_global_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_632_bezier3p.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_626_local_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_640_bbox.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_627_bspline_basis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_641_construction_ray.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_629_bezier.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_642_construction_line.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_630a_bezier4p_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_643_construction_box.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_630b_bezier4p_functions.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_644_construction_circle.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_631_euler_spiral.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_645_construction_arc.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_632_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_646_offset_vertices_2d.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_640_bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_647_transform_tools.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_641_construction_ray.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_648_construction_ellipse.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_642_construction_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_650_elliptic_arc_span.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_643_construction_box.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_651_construction_polyline.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_644_construction_circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_652_approx_param_t.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_645_construction_arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_653_polyline_intersection.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_646_offset_vertices_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_654_rtree.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_647_transform_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_655_dbscan.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_648_construction_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_656_k_means.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_650_elliptic_arc_span.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_657_mapbox_earcut.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_651_construction_polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_658_bevel_tools.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_652_approx_param_t.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_653_polyline_intersection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_654_rtree.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_655_dbscan.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_06_math/test_662_is_convex_polygon_2d.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_656_k_means.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_701_arrows.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_657_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_702_render_forms.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_658_bevel_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_703_mesh_builder.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_659_intersection_line_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_704_render_linear_dimension.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_705_shape.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_706_random_path.py
+Filename: ezdxf-1.1.0b2/tests/test_06_math/test_662_is_convex_polygon_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_707_trace.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_701_arrows.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_708a_path.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_702_render_forms.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_708b_path_tools.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_703_mesh_builder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_708c_matplotlib_path_tools.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_704_render_linear_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_708d_qpainter_path_tools.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_705_shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_708e_path_shapes.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_706_random_path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_708f_path_nesting.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_707_trace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_709_linetype_renderer.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_708a_path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_711_points.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_708b_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_712_render_curved_dimension.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_708c_matplotlib_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_713_mleader_builder.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_708d_qpainter_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_714_mleader_render_engine.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_708e_path_shapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_715_hatching.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_708f_path_nesting.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_709_linetype_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_800_mtext_surrogate.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_711_points.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_801_r12spline.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_712_render_curved_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_802_table_painter.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_713_mleader_builder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_803_entities_to_code.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_714_mleader_render_engine.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_804_importer.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_715_hatching.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_805_pycsg.py
+Filename: ezdxf-1.1.0b2/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_806_acadctb.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_800_mtext_surrogate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_807_dwg_loader_basics.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_801_r12spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_810_drawing_properties.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_802_table_painter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_811a_drawing_frontend.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_803_entities_to_code.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_811b_drawing_recorder.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_804_importer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_805_pycsg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_813_geo_interface.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_806_acadctb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_814_text2path.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_807_dwg_loader_basics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_815_dxf_browser.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_810_drawing_properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_816_bin_packing.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_811a_drawing_frontend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_817_genetic_algorithm.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_811b_drawing_recorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_818_meshex.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_812_drawing_graphic_proxy.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_819_menger_sponge.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_813_geo_interface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_820_openscad.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_814_text2path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_821_hpgl2.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_815_dxf_browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_816_bin_packing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_822_clipper.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_817_genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_818_meshex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_819_menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_820_openscad.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_821_hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_822_clipper.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_823_drawing_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_824_svg_drawing_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_10_issues/test_issue_574_flattening_error.py
+Filename: ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_901_acc_vec2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Filename: ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_902_acc_vec3.py
 Comment: 
 
-Filename: ezdxf-1.1.0b1/tests/test_10_issues/test_issue_749_text_layout.py
+Filename: ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+Comment: 
+
+Filename: ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+Comment: 
+
+Filename: ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+Comment: 
+
+Filename: ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+Comment: 
+
+Filename: ezdxf-1.1.0b2/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Comment: 
+
+Filename: ezdxf-1.1.0b2/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Comment: 
+
+Filename: ezdxf-1.1.0b2/tests/test_10_issues/test_issue_574_flattening_error.py
+Comment: 
+
+Filename: ezdxf-1.1.0b2/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Comment: 
+
+Filename: ezdxf-1.1.0b2/tests/test_10_issues/test_issue_749_text_layout.py
+Comment: 
+
+Filename: ezdxf-1.1.0b2/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
 Comment: 
 
 Zip file comment:
```

## Comparing `ezdxf-1.1.0b1/LICENSE` & `ezdxf-1.1.0b2/LICENSE`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/NEWS.md` & `ezdxf-1.1.0b2/NEWS.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 
 News
 ====
 
-Version 1.1.0b0 - dev
+Version 1.1.0b2 - dev
 ---------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-1.html
 - WARNING: The font support changed drastically in this version, if you use the 
   `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
   v1.0.3 in your `requirements.txt` file to use the previous version!
 - NEW: `numpy` is a hard dependency, requires Python version >= 3.8
 - NEW: `fontTools` is a hard dependency
 - NEW: `ezdxf.path.Path2d()` class, `Path` class with `Vec2` vertices
 - NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
-- NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG
-- NEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF
-- NEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG
-- NEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF
+- NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF, SVG, PDF, PNG
+- NEW: `ezdxf hpgl` command to view and/or convert HPGL/2 plot files to various formats: DXF, SVG, PDF
+- NEW: native `SVG` backend for the `drawing` add-on
+- NEW: `ColorPolicy` and `BackgroundPolicy` configuration settings for the `drawing` 
+  add-on to change/override foreground- and background color by the frontend 
 - NEW: support for measuring and rendering of .shx, .shp and .lff fonts, the basic 
   stroke fonts included in CAD applications
 - NEW: added setter to `BlockLayout.base_point` property
 - CHANGED: moved font related modules into a new subpackage `ezdxf.fonts` 
   including a big refactoring
 - CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
   renamed to `width` and is also an int value (1-9) now
```

## Comparing `ezdxf-1.1.0b1/PKG-INFO` & `ezdxf-1.1.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.1.0b1
+Version: 1.1.0b2
 Summary: A Python package to create/manipulate DXF drawings.
 Home-page: https://ezdxf.mozman.at
 Author: Manfred Moitzi
 Author-email: me@mozman.at
 License: MIT License
 Download-URL: https://pypi.org/project/ezdxf/
 Keywords: DXF,CAD
@@ -211,29 +211,30 @@
 Feedback is greatly appreciated.
 
 Manfred
 
 News
 ====
 
-Version 1.1.0b0 - dev
+Version 1.1.0b2 - dev
 ---------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-1.html
 - WARNING: The font support changed drastically in this version, if you use the 
   `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
   v1.0.3 in your `requirements.txt` file to use the previous version!
 - NEW: `numpy` is a hard dependency, requires Python version >= 3.8
 - NEW: `fontTools` is a hard dependency
 - NEW: `ezdxf.path.Path2d()` class, `Path` class with `Vec2` vertices
 - NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
-- NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG
-- NEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF
-- NEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG
-- NEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF
+- NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF, SVG, PDF, PNG
+- NEW: `ezdxf hpgl` command to view and/or convert HPGL/2 plot files to various formats: DXF, SVG, PDF
+- NEW: native `SVG` backend for the `drawing` add-on
+- NEW: `ColorPolicy` and `BackgroundPolicy` configuration settings for the `drawing` 
+  add-on to change/override foreground- and background color by the frontend 
 - NEW: support for measuring and rendering of .shx, .shp and .lff fonts, the basic 
   stroke fonts included in CAD applications
 - NEW: added setter to `BlockLayout.base_point` property
 - CHANGED: moved font related modules into a new subpackage `ezdxf.fonts` 
   including a big refactoring
 - CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
   renamed to `width` and is also an int value (1-9) now
```

## Comparing `ezdxf-1.1.0b1/README.md` & `ezdxf-1.1.0b2/README.md`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/setup.py` & `ezdxf-1.1.0b2/setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/check_disable_c_ext_by_config_file.py` & `ezdxf-1.1.0b2/integration_tests/check_disable_c_ext_by_config_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/check_disable_c_ext_by_env_var.py` & `ezdxf-1.1.0b2/integration_tests/check_disable_c_ext_by_env_var.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_acad_table.py` & `ezdxf-1.1.0b2/integration_tests/test_acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_all_dimline_styles.py` & `ezdxf-1.1.0b2/integration_tests/test_all_dimline_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_all_ellipse_transformations.py` & `ezdxf-1.1.0b2/integration_tests/test_all_ellipse_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_anonymous_blocks.py` & `ezdxf-1.1.0b2/integration_tests/test_anonymous_blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_audit_critical_dxf_files.py` & `ezdxf-1.1.0b2/integration_tests/test_audit_critical_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_audit_layouts.py` & `ezdxf-1.1.0b2/integration_tests/test_audit_layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_complex_line_type_2.py` & `ezdxf-1.1.0b2/integration_tests/test_complex_line_type_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_create_basic_graphics.py` & `ezdxf-1.1.0b2/integration_tests/test_create_basic_graphics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_document_guid.py` & `ezdxf-1.1.0b2/integration_tests/test_document_guid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_document_page_setup.py` & `ezdxf-1.1.0b2/integration_tests/test_document_page_setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_dxf_info_scanning.py` & `ezdxf-1.1.0b2/integration_tests/test_dxf_info_scanning.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_entities_iterator.py` & `ezdxf-1.1.0b2/integration_tests/test_entities_iterator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_fix_dulicate_handles.py` & `ezdxf-1.1.0b2/integration_tests/test_fix_dulicate_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_geo.py` & `ezdxf-1.1.0b2/integration_tests/test_geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_groups.py` & `ezdxf-1.1.0b2/integration_tests/test_groups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_ignore_junk_beyond_EOF.py` & `ezdxf-1.1.0b2/integration_tests/test_ignore_junk_beyond_EOF.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_launcher.py` & `ezdxf-1.1.0b2/integration_tests/test_launcher.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_leica_disto_r12.py` & `ezdxf-1.1.0b2/integration_tests/test_leica_disto_r12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_load_dxf_unicode_notation.py` & `ezdxf-1.1.0b2/integration_tests/test_load_dxf_unicode_notation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_mapbox_earcut.py` & `ezdxf-1.1.0b2/integration_tests/test_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_mtext_columns.py` & `ezdxf-1.1.0b2/integration_tests/test_mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_mtext_explode_addon.py` & `ezdxf-1.1.0b2/integration_tests/test_mtext_explode_addon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_mtext_text_frame.py` & `ezdxf-1.1.0b2/integration_tests/test_mtext_text_frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_new_table_entries.py` & `ezdxf-1.1.0b2/integration_tests/test_new_table_entries.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_none_ascii_read_write.py` & `ezdxf-1.1.0b2/integration_tests/test_none_ascii_read_write.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_odafc.py` & `ezdxf-1.1.0b2/integration_tests/test_odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_open_binary_DXF_files.py` & `ezdxf-1.1.0b2/integration_tests/test_open_binary_DXF_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_open_coord_order_issue.py` & `ezdxf-1.1.0b2/integration_tests/test_open_coord_order_issue.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_open_exotic_dxf_files.py` & `ezdxf-1.1.0b2/integration_tests/test_open_exotic_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_open_R13_R14.py` & `ezdxf-1.1.0b2/integration_tests/test_open_R13_R14.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_polyline_entity.py` & `ezdxf-1.1.0b2/integration_tests/test_polyline_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_preserve_binary_data_in_xrecords.py` & `ezdxf-1.1.0b2/integration_tests/test_preserve_binary_data_in_xrecords.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_r12export.py` & `ezdxf-1.1.0b2/integration_tests/test_r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_r12strict.py` & `ezdxf-1.1.0b2/integration_tests/test_r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_r12writer.py` & `ezdxf-1.1.0b2/integration_tests/test_r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_read_file_without_handles.py` & `ezdxf-1.1.0b2/integration_tests/test_read_file_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_read_write_modern_entites.py` & `ezdxf-1.1.0b2/integration_tests/test_read_write_modern_entites.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_recover.py` & `ezdxf-1.1.0b2/integration_tests/test_recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_redraw_order.py` & `ezdxf-1.1.0b2/integration_tests/test_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_rotated_block_attributes.py` & `ezdxf-1.1.0b2/integration_tests/test_rotated_block_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_surface_entities.py` & `ezdxf-1.1.0b2/integration_tests/test_surface_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_write_fixed_meta_data.py` & `ezdxf-1.1.0b2/integration_tests/test_write_fixed_meta_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_write_without_handles.py` & `ezdxf-1.1.0b2/integration_tests/test_write_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/test_xref_detach.py` & `ezdxf-1.1.0b2/integration_tests/test_xref_detach.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/AC1003_LINE_Example.dxf` & `ezdxf-1.1.0b2/integration_tests/data/AC1003_LINE_Example.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/acad_table_with_blk_ref.dxf` & `ezdxf-1.1.0b2/integration_tests/data/acad_table_with_blk_ref.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/ASCII_R12.dxf` & `ezdxf-1.1.0b2/integration_tests/data/ASCII_R12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r12.dxf` & `ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r13.dxf` & `ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r14.dxf` & `ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r2000.dxf` & `ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r2000.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/cc_dxflib.dxf` & `ezdxf-1.1.0b2/integration_tests/data/cc_dxflib.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/custom_blocks.dxf` & `ezdxf-1.1.0b2/integration_tests/data/custom_blocks.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/duplicate_handles.dxf` & `ezdxf-1.1.0b2/integration_tests/data/duplicate_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/dxf_unicode.dxf` & `ezdxf-1.1.0b2/integration_tests/data/dxf_unicode.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/empty_handles.dxf` & `ezdxf-1.1.0b2/integration_tests/data/empty_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/groups.dxf` & `ezdxf-1.1.0b2/integration_tests/data/groups.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/Leica_Disto_S910.dxf` & `ezdxf-1.1.0b2/integration_tests/data/Leica_Disto_S910.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/MODEL.dxf` & `ezdxf-1.1.0b2/integration_tests/data/MODEL.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/mtext_columns_R2007.dxf` & `ezdxf-1.1.0b2/integration_tests/data/mtext_columns_R2007.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/mtext_columns_R2018.dxf` & `ezdxf-1.1.0b2/integration_tests/data/mtext_columns_R2018.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/mtext_framed_columns.dxf` & `ezdxf-1.1.0b2/integration_tests/data/mtext_framed_columns.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/mtext_text_frame.dxf` & `ezdxf-1.1.0b2/integration_tests/data/mtext_text_frame.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/no_layouts.dxf` & `ezdxf-1.1.0b2/integration_tests/data/no_layouts.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/POLI-ALL210_12.DXF` & `ezdxf-1.1.0b2/integration_tests/data/POLI-ALL210_12.DXF`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/recover01.dxf` & `ezdxf-1.1.0b2/integration_tests/data/recover01.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/recover02.dxf` & `ezdxf-1.1.0b2/integration_tests/data/recover02.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/small_r13.dxf` & `ezdxf-1.1.0b2/integration_tests/data/small_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/small_r14.dxf` & `ezdxf-1.1.0b2/integration_tests/data/small_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/XRECORD_0.bin` & `ezdxf-1.1.0b2/integration_tests/data/XRECORD_0.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/XRECORD_1.bin` & `ezdxf-1.1.0b2/integration_tests/data/XRECORD_1.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/integration_tests/data/XRECORD_2.bin` & `ezdxf-1.1.0b2/integration_tests/data/XRECORD_2.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/appsettings.py` & `ezdxf-1.1.0b2/src/ezdxf/appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/audit.py` & `ezdxf-1.1.0b2/src/ezdxf/audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/bbox.py` & `ezdxf-1.1.0b2/src/ezdxf/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/blkrefs.py` & `ezdxf-1.1.0b2/src/ezdxf/blkrefs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/colors.py` & `ezdxf-1.1.0b2/src/ezdxf/colors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/commands.py` & `ezdxf-1.1.0b2/src/ezdxf/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-#  Copyright (c) 2021-2022, Manfred Moitzi
+#  Copyright (c) 2021-2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
+
+import pathlib
 from typing import Callable, Optional, TYPE_CHECKING, Type
 import abc
 import sys
 import os
 import glob
 import signal
 import time
@@ -12,15 +14,14 @@
 from pathlib import Path
 
 import ezdxf
 from ezdxf import recover
 from ezdxf.lldxf import const
 from ezdxf.lldxf.validator import is_dxf_file, is_binary_dxf_file
 from ezdxf.dwginfo import dwg_file_info
-from ezdxf import units
 
 if TYPE_CHECKING:
     from ezdxf.entities import DXFGraphic
     from ezdxf.addons.drawing.properties import Properties
 
 __all__ = ["get", "add_parsers"]
 
@@ -367,20 +368,20 @@
         ctx = RenderContext(doc)
         out = MatplotlibBackend(ax)
 
         if args.all_layers_visible:
             for layer_properties in ctx.layers.values():
                 layer_properties.is_visible = True
 
-        config = Configuration.defaults()
+        config = Configuration()
         if args.all_entities_visible:
 
             class AllVisibleFrontend(Frontend):
                 def override_properties(
-                    self, entity: "DXFGraphic", properties: "Properties"
+                    self, entity: DXFGraphic, properties: Properties
                 ) -> None:
                     properties.is_visible = True
 
             frontend = AllVisibleFrontend(ctx, out, config=config)
         else:
             frontend = Frontend(ctx, out, config=config)
         t0 = time.perf_counter()
@@ -440,26 +441,25 @@
     def run(args):
         # Import on demand for a quicker startup:
         try:
             from ezdxf.addons.xqt import QtWidgets
         except ImportError as e:
             print(str(e))
             sys.exit(1)
-        from ezdxf.addons.drawing.qtviewer import CadViewer
+        from ezdxf.addons.drawing.qtviewer import CADViewer
         from ezdxf.addons.drawing.config import Configuration
 
-        config = Configuration.defaults()
-        config = config.with_changes(
+        config = Configuration(
             lineweight_scaling=args.lwscale,
         )
 
         signal.signal(signal.SIGINT, signal.SIG_DFL)  # handle Ctrl+C properly
         app = QtWidgets.QApplication(sys.argv)
         set_app_icon(app)
-        viewer = CadViewer(config=config)
+        viewer = CADViewer.from_config(config)
         filename = args.file
         if filename:
             doc, auditor = load_document(filename)
             viewer.set_document(
                 doc,
                 auditor,
                 layout=args.layout,
@@ -845,182 +845,193 @@
         "stream; use this flag when no HPGL/2 data was found and you are sure the "
         "file is a HPGL/2 plot file",
     )
     return parser
 
 
 @register
-class Plt2Dxf(Command):
-    """Launcher sub-command: plt2dxf"""
+class HPGL(Command):
+    """Launcher sub-command: hpgl"""
 
-    NAME = "plt2dxf"
+    NAME = "hpgl"
 
     @staticmethod
     def add_parser(subparsers):
-        parser = make_plt2fmt_parser(subparsers, Plt2Dxf.NAME, "DXF")
-        parser.epilog = (
-            "Note that plot files are intended to be plotted on white paper."
+        parser = subparsers.add_parser(
+            HPGL.NAME, help=f"view and/or convert HPGL/2 plot files to various formats"
+        )
+        parser.add_argument(
+            "file",
+            metavar="FILE",
+            nargs="?",
+            default="",
+            help=f"view and/or convert HPGL/2 plot files, wildcards (*, ?) supported in command line mode",
+        )
+        parser.add_argument(
+            "-e",
+            "--export",
+            metavar="FORMAT",
+            required=False,
+            help=f"convert HPGL/2 plot file to SVG, PDF or DXF from the command line (no gui)",
+        )
+        parser.add_argument(
+            "-r",
+            "--rotate",
+            type=int,
+            choices=(0, 90, 180, 270),
+            default=0,
+            required=False,
+            help="rotate page about 90, 180 or 270 degrees (no gui)",
+        )
+        parser.add_argument(
+            "-x",
+            "--scale_x",
+            type=float,
+            metavar="SX",
+            default=1.0,
+            required=False,
+            help="scale page in x-axis direction, use negative values to mirror page, (no gui)",
+        )
+        parser.add_argument(
+            "-y",
+            "--scale_y",
+            type=float,
+            metavar="SY",
+            default=1.0,
+            required=False,
+            help="scale page in y-axis direction, use negative values to mirror page (no gui)",
+        )
+        parser.add_argument(
+            "-m",
+            "--merge_control",
+            type=int,
+            required=False,
+            default=2,
+            choices=(0, 1, 2),
+            help="provides control over the order of filled polygons, 0=off (print order), "
+            "1=luminance (order by luminance), 2=auto (default)",
+        )
+        parser.add_argument(
+            "-f",
+            "--force",
+            action="store_true",
+            required=False,
+            help="inserts the mandatory 'enter HPGL/2 mode' escape sequence into the data "
+            "stream; use this flag when no HPGL/2 data was found and you are sure the "
+            "file is a HPGL/2 plot file",
         )
         parser.add_argument(
             "--aci",
             action="store_true",
             required=False,
-            help="use pen numbers as ACI colors",
+            help="use pen numbers as ACI colors (DXF only)",
         )
         parser.add_argument(
             "--map_black_to_white",
             action="store_true",
             required=False,
-            help="map black RGB plot colors (and only real black (0, 0, 0)) to white RGB, "
-            "does not affect ACI colors",
+            help="map black RGB plot colors to white RGB, does not affect ACI colors (DXF only)",
+        )
+        parser.epilog = (
+            "Note that plot files are intended to be plotted on white paper."
         )
 
     @staticmethod
     def run(args):
-        from ezdxf.addons.hpgl2 import api as hpgl2
-        from ezdxf.addons.hpgl2.dxf_backend import ColorMode
-
-        def _convert(filepath: Path) -> None:
-            msg = f"converting HPGL/2 plot file to DXF: {filename}"
-            print(msg)
-            try:
-                data = filepath.read_bytes()
-            except IOError as e:
-                print(str(e), file=sys.stderr)
-                return
-            if args.force:
-                data = b"%1B" + data
-
-            color_mode = ColorMode.ACI if args.aci else ColorMode.RGB
-            doc = hpgl2.to_dxf(
-                data,
-                rotation=args.rotate,
-                sx=args.scale_x,
-                sy=args.scale_y,
-                color_mode=color_mode,
-                map_black_rgb_to_white_rgb=args.map_black_to_white,
-                merge_control=args.merge_control,
-            )
-            dxf_filepath = filepath.with_suffix(".dxf")
-            try:
-                doc.saveas(dxf_filepath)
-            except IOError as e:
-                print(str(e), file=sys.stderr)
-
-        for pattern in args.files:
-            names = list(glob.glob(pattern))
-            if len(names) == 0:
-                msg = f"File(s) '{pattern}' not found."
-                print(msg, file=sys.stderr)
-                logger.error(msg)
-                continue
-            for filename in names:
-                _convert(Path(filename))
-
-
-@register
-class Plt2Svg(Command):
-    """Launcher sub-command: plt2svg"""
-
-    NAME = "plt2svg"
-
-    @staticmethod
-    def add_parser(subparsers):
-        make_plt2fmt_parser(subparsers, Plt2Svg.NAME, "SVG")
-
-    @staticmethod
-    def run(args):
-        from ezdxf.addons.hpgl2 import api as hpgl2
-
-        def _convert(filepath: Path) -> None:
-            msg = f"converting HPGL/2 plot file to SVG: {filename}"
-            print(msg)
-            logger.info(msg)
-            try:
-                data = filepath.read_bytes()
-            except IOError as e:
-                print(str(e), file=sys.stderr)
-                return
-
-            if args.force:
-                data = b"%1B" + data
-
-            svg_string = hpgl2.to_svg(
-                data,
-                rotation=args.rotate,
-                sx=args.scale_x,
-                sy=args.scale_y,
-                merge_control=args.merge_control,
-            )
-            svg_filepath = filepath.with_suffix(".svg")
-            try:
-                svg_filepath.write_text(svg_string)
-            except IOError as e:
-                print(str(e), file=sys.stderr)
-
-        for pattern in args.files:
-            names = list(glob.glob(pattern))
-            if len(names) == 0:
-                msg = f"File(s) '{pattern}' not found."
-                print(msg)
-                logger.error(msg)
-                continue
-            for filename in names:
-                _convert(Path(filename))
-
-
-@register
-class Plt2Pdf(Command):
-    """Launcher sub-command: plt2pdf"""
-
-    NAME = "plt2pdf"
-
-    @staticmethod
-    def add_parser(subparsers):
-        make_plt2fmt_parser(subparsers, Plt2Pdf.NAME, "PDF")
+        if args.export:
+            for filename in glob.glob(args.file):
+                export_hpgl2(Path(filename), args)
+        else:
+            filename = ""
+            if args.file:
+                names = list(glob.glob(args.file))
+                if len(names):
+                    filename = names[0]
+            launch_hpgl2_viewer(filename, args.force)
 
-    @staticmethod
-    def run(args):
-        from ezdxf.addons.hpgl2 import api as hpgl2
 
-        def _convert(filepath: Path) -> None:
-            msg = f"converting HPGL/2 plot file to PDF: {filename}"
-            print(msg)
-            logger.info(msg)
-            try:
-                data = filepath.read_bytes()
-            except IOError as e:
-                print(str(e), file=sys.stderr)
-                return
+def export_hpgl2(filepath: Path, args) -> None:
+    from ezdxf.addons.hpgl2 import api as hpgl2
+    from ezdxf.addons.hpgl2.dxf_backend import ColorMode
 
-            if args.force:
-                data = b"%1B" + data
+    fmt = args.export.upper()
+    start_msg = f"converting HPGL/2 plot file '{filepath.name}' to {fmt}"
+    try:
+        data = filepath.read_bytes()
+    except IOError as e:
+        print(str(e), file=sys.stderr)
+        return
+    if args.force:
+        data = b"%1B" + data
+    export_path = filepath.with_suffix(f".{fmt.lower()}")
+    if fmt == "DXF":
+        print(start_msg)
+        color_mode = ColorMode.ACI if args.aci else ColorMode.RGB
+        doc = hpgl2.to_dxf(
+            data,
+            rotation=args.rotate,
+            sx=args.scale_x,
+            sy=args.scale_y,
+            color_mode=color_mode,
+            map_black_rgb_to_white_rgb=args.map_black_to_white,
+            merge_control=args.merge_control,
+        )
+        try:
+            doc.saveas(export_path)
+        except IOError as e:
+            print(str(e), file=sys.stderr)
+
+    elif fmt == "SVG":
+        print(start_msg)
+        svg_string = hpgl2.to_svg(
+            data,
+            rotation=args.rotate,
+            sx=args.scale_x,
+            sy=args.scale_y,
+            merge_control=args.merge_control,
+        )
+        try:
+            export_path.write_text(svg_string)
+        except IOError as e:
+            print(str(e), file=sys.stderr)
+    elif fmt == "PDF":
+        print(start_msg)
+        pdf_bytes = hpgl2.to_pdf(
+            data,
+            rotation=args.rotate,
+            sx=args.scale_x,
+            sy=args.scale_y,
+            merge_control=args.merge_control,
+        )
+        try:
+            export_path.write_bytes(pdf_bytes)
+        except IOError as e:
+            print(str(e), file=sys.stderr)
+    else:
+        print(f"invalid export format: {fmt}")
+        exit(1)
+    print(f"file '{export_path.name}' successfully written")
 
-            pdf_bytes = hpgl2.to_pdf(
-                data,
-                rotation=args.rotate,
-                sx=args.scale_x,
-                sy=args.scale_y,
-                merge_control=args.merge_control,
-            )
-            pdf_filepath = filepath.with_suffix(".pdf")
-            try:
-                pdf_filepath.write_bytes(pdf_bytes)
-            except IOError as e:
-                print(str(e), file=sys.stderr)
 
-        for pattern in args.files:
-            names = list(glob.glob(pattern))
-            if len(names) == 0:
-                msg = f"File(s) '{pattern}' not found."
-                print(msg)
-                logger.error(msg)
-                continue
-            for filename in names:
-                _convert(Path(filename))
+def launch_hpgl2_viewer(filename: str, force: bool) -> None:
+    try:
+        from ezdxf.addons.xqt import QtWidgets
+    except ImportError as e:
+        print(str(e))
+        exit(1)
+    from ezdxf.addons.hpgl2.viewer import HPGL2Viewer
+
+    signal.signal(signal.SIGINT, signal.SIG_DFL)  # handle Ctrl+C properly
+    app = QtWidgets.QApplication(sys.argv)
+    set_app_icon(app)
+    viewer = HPGL2Viewer()
+    viewer.show()
+    if filename and os.path.exists(filename):
+        viewer.load_plot_file(filename, force=force)
+    sys.exit(app.exec())
 
 
 def set_app_icon(app):
     from ezdxf.addons.xqt import QtGui, QtCore
 
     app_icon = QtGui.QIcon()
     p = resources_path()
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/comments.py` & `ezdxf-1.1.0b2/src/ezdxf/comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/disassemble.py` & `ezdxf-1.1.0b2/src/ezdxf/disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/document.py` & `ezdxf-1.1.0b2/src/ezdxf/document.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/dwginfo.py` & `ezdxf-1.1.0b2/src/ezdxf/dwginfo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entitydb.py` & `ezdxf-1.1.0b2/src/ezdxf/entitydb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/enums.py` & `ezdxf-1.1.0b2/src/ezdxf/enums.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/explode.py` & `ezdxf-1.1.0b2/src/ezdxf/explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/eztypes.py` & `ezdxf-1.1.0b2/src/ezdxf/eztypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/filemanagement.py` & `ezdxf-1.1.0b2/src/ezdxf/filemanagement.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/gfxattribs.py` & `ezdxf-1.1.0b2/src/ezdxf/gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/graphicsfactory.py` & `ezdxf-1.1.0b2/src/ezdxf/graphicsfactory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/groupby.py` & `ezdxf-1.1.0b2/src/ezdxf/groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/npshapes.py` & `ezdxf-1.1.0b2/src/ezdxf/npshapes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     pass
 
 
 class EmptyShapeError(NumpyShapesException):
     pass
 
 
-class _NumpyShape2d(abc.ABC):
+class NumpyShape2d(abc.ABC):
     """This is an optimization to store many 2D paths and polylines in a compact way
     without sacrificing basic functions like transformation and bounding box calculation.
     """
 
     _vertices: np.ndarray
 
     def extents(self) -> tuple[Vec2, Vec2]:
@@ -42,25 +42,25 @@
         m.transform_array_inplace(v, 2)
 
     def vertices(self) -> list[Vec2]:
         """Returns the shape vertices as list of :class:`Vec2`."""
         return Vec2.list(self._vertices)
 
 
-class NumpyPoints2d(_NumpyShape2d):
+class NumpyPoints2d(NumpyShape2d):
     """Represents an array of 2D points stored as a ndarray."""
 
     def __init__(self, points: Iterable[UVec]) -> None:
         self._vertices = np.array(Vec2.list(points), dtype=np.float64)
 
     def __len__(self) -> int:
         return len(self._vertices)
 
 
-class NumpyPath2d(_NumpyShape2d):
+class NumpyPath2d(NumpyShape2d):
     """Represents a 2D path, the path control vertices and commands are stored as ndarray."""
 
     def __init__(self, path: AbstractPath) -> None:
         vertices = Vec2.list(path.control_vertices())
         if len(vertices) == 0:
             try:  # control_vertices() does not return start point of empty paths
                 vertices = [path.start]
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/protocols.py` & `ezdxf-1.1.0b2/src/ezdxf/protocols.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/proxygraphic.py` & `ezdxf-1.1.0b2/src/ezdxf/proxygraphic.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,17 +393,26 @@
 
     def attribute_thickness(self, data: bytes):
         self.thickness = struct.unpack("<d", data)[0]
 
     def circle(self, data: bytes):
         bs = ByteStream(data)
         attribs = self._build_dxf_attribs()
-        attribs["center"] = Vec3(bs.read_vertex())
+        center = Vec3(bs.read_vertex())
         attribs["radius"] = bs.read_float()
-        attribs["extrusion"] = bs.read_vertex()
+        normal = Vec3(bs.read_vertex())
+        attribs["extrusion"] = normal
+        if not normal.isclose(Z_AXIS):
+            # TODO: (issue 873) circle has a normal vector but center is in WCS
+            #  It's not clear if all coordinates in proxy graphics are WCS coordinates
+            #  even for OCS entities - the ODA DWG documentation contains no information
+            #  about that.
+            ocs = OCS(normal)
+            center = ocs.from_wcs(center)
+        attribs["center"] = center
         return self._factory("CIRCLE", dxfattribs=attribs)
 
     def circle_3p(self, data: bytes):
         bs = ByteStream(data)
         attribs = self._build_dxf_attribs()
         p1 = Vec3(bs.read_vertex())
         p2 = Vec3(bs.read_vertex())
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/query.py` & `ezdxf-1.1.0b2/src/ezdxf/query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/queryparser.py` & `ezdxf-1.1.0b2/src/ezdxf/queryparser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/r12strict.py` & `ezdxf-1.1.0b2/src/ezdxf/r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/recover.py` & `ezdxf-1.1.0b2/src/ezdxf/recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/reorder.py` & `ezdxf-1.1.0b2/src/ezdxf/reorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/transform.py` & `ezdxf-1.1.0b2/src/ezdxf/transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/units.py` & `ezdxf-1.1.0b2/src/ezdxf/units.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# Copyright (c) 2019-2021 Manfred Moitzi
+# Copyright (c) 2019-2023 Manfred Moitzi
 # License: MIT License
 from typing import Optional
 from ezdxf.enums import InsertUnits
 
 # Documentation: https://ezdxf.mozman.at/docs/concepts/units.html#insunits
 
 MSP_METRIC_UNITS_FACTORS = {
+    # length in units / factor = length in meters
+    # length in meters * factor = length in units
     "km": 0.001,
     "m": 1.0,
     "dm": 10.0,
     "cm": 100.0,
     "mm": 1000.0,
     "µm": 1000000.0,
     "yd": 1.093613298,
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/upright.py` & `ezdxf-1.1.0b2/src/ezdxf/upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/urecord.py` & `ezdxf-1.1.0b2/src/ezdxf/urecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/version.py` & `ezdxf-1.1.0b2/src/ezdxf/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # examples:
 #   major pre-release alpha 2: VERSION = "0.9.0a2"; version = (0, 9, 0, 'a2')
 #   major release candidate 0: VERSION = "0.9.0rc0"; version = (0, 9, 0, 'rc0')
 #   major release: VERSION = "0.9.0"; version = (0, 9, 0, 'release')
 #   1. bug fix release beta0: VERSION = "0.9.1b0"; version = (0, 9, 1, 'b0')
 #   2. bug fix release: VERSION = "0.9.2"; version = (0, 9, 2, 'release')
 
-version = (1, 1, 0, "b1")
-__version__ = "1.1.0b1"
+version = (1, 1, 0, "b2")
+__version__ = "1.1.0b2"
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/xref.py` & `ezdxf-1.1.0b2/src/ezdxf/xref.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/zoom.py` & `ezdxf-1.1.0b2/src/ezdxf/zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/_options.py` & `ezdxf-1.1.0b2/src/ezdxf/_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Copyright (c) 2011-2022, Manfred Moitzi
+# Copyright (c) 2011-2023, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
-from typing import TextIO, Union, Sequence
+from typing import TextIO, Sequence
 import os
 import sys
 from pathlib import Path
 from configparser import ConfigParser
 
 # Recommended uses of the global object "options":
 # import ezdxf
@@ -226,16 +226,16 @@
         self.set(
             CORE,
             "DEFAULT_DIMENSION_TEXT_STYLE",
             style,
         )
 
     @property
-    def support_dirs(self) -> Sequence[str]:
-        return self.get(CORE, "SUPPORT_DIRS", "").split(DIR_SEPARATOR)
+    def support_dirs(self) -> list[str]:
+        return [d for d in self.get(CORE, "SUPPORT_DIRS", "").split(DIR_SEPARATOR) if d]
 
     @support_dirs.setter
     def support_dirs(self, support_dirs: Sequence[str]) -> None:
         self.set(CORE, "SUPPORT_DIRS", DIR_SEPARATOR.join(support_dirs))
 
     @property
     def test_files(self) -> str:
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/__init__.py` & `ezdxf-1.1.0b2/src/ezdxf/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/__main__.py` & `ezdxf-1.1.0b2/src/ezdxf/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,20 @@
     parser.add_argument(
         "-V",
         "--version",
         action="store_true",
         help="show version and exit",
     )
     parser.add_argument(
+        "-f",
+        "--fonts",
+        action="store_true",
+        help="rebuild system font cache and print all fonts found",
+    )
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         help="give more output",
     )
     parser.add_argument(
         "--config",
@@ -37,14 +43,21 @@
     )
 
 
 def print_version(verbose=False):
     print_config(verbose=verbose, stream=sys.stdout)
 
 
+def print_available_fonts(verbose=False):
+    from ezdxf.fonts import fonts
+    print("Rebuilding system font cache.")
+    fonts.build_system_font_cache()
+    fonts.font_manager.print_available_fonts(verbose)
+
+
 def setup_log(args):
     import logging
     from datetime import datetime
     from io import StringIO
 
     level = "DEBUG" if args.verbose else "INFO"
     if args.log.lower() == "stderr":
@@ -86,14 +99,17 @@
         else:
             print(f'config file "{config}" not found')
     if args.log:
         setup_log(args)
     if args.version:
         print_version(verbose=args.verbose)
         help_ = False
+    if args.fonts:
+        print_available_fonts(args.verbose)
+        help_ = False
 
     run = commands.get(args.command)
     if run:
         # For the case automatic font loading is disabled:
         fonts.load()
         run(args)
     elif help_:
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/bezier3p.pyx` & `ezdxf-1.1.0b2/src/ezdxf/acc/bezier3p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/bezier4p.pyx` & `ezdxf-1.1.0b2/src/ezdxf/acc/bezier4p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/bspline.pyx` & `ezdxf-1.1.0b2/src/ezdxf/acc/bspline.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/construct.pyx` & `ezdxf-1.1.0b2/src/ezdxf/acc/construct.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/linetypes.pyx` & `ezdxf-1.1.0b2/src/ezdxf/acc/linetypes.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/mapbox_earcut.pyx` & `ezdxf-1.1.0b2/src/ezdxf/acc/mapbox_earcut.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/matrix44.pyx` & `ezdxf-1.1.0b2/src/ezdxf/acc/matrix44.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/vector.pxd` & `ezdxf-1.1.0b2/src/ezdxf/acc/vector.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/vector.pyx` & `ezdxf-1.1.0b2/src/ezdxf/acc/vector.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.cpp` & `ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.cpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.hpp` & `ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.hpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_quad_bezier.cpp` & `ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_quad_bezier.cpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_vec3.hpp` & `ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_vec3.hpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_vec3.pxd` & `ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_vec3.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acc/__init__.py` & `ezdxf-1.1.0b2/src/ezdxf/acc/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acis/abstract.py` & `ezdxf-1.1.0b2/src/ezdxf/acis/abstract.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acis/api.py` & `ezdxf-1.1.0b2/src/ezdxf/acis/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acis/const.py` & `ezdxf-1.1.0b2/src/ezdxf/acis/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acis/dbg.py` & `ezdxf-1.1.0b2/src/ezdxf/acis/dbg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acis/dxf.py` & `ezdxf-1.1.0b2/src/ezdxf/acis/dxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acis/entities.py` & `ezdxf-1.1.0b2/src/ezdxf/acis/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acis/hdr.py` & `ezdxf-1.1.0b2/src/ezdxf/acis/hdr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acis/mesh.py` & `ezdxf-1.1.0b2/src/ezdxf/acis/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acis/sab.py` & `ezdxf-1.1.0b2/src/ezdxf/acis/sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/acis/sat.py` & `ezdxf-1.1.0b2/src/ezdxf/acis/sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/acadctb.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/binpacking.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/binpacking.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/dimlines.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/dimlines.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/dxf2code.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/dxf2code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/genetic_algorithm.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/geo.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/gerber_D6673.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/gerber_D6673.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/importer.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/iterdxf.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/iterdxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/menger_sponge.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/meshex.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/mtextsurrogate.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/mtextsurrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/mtxpl.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/mtxpl.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/odafc.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/openscad.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/pycsg.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/r12export.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/r12writer.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/sierpinski_pyramid.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/sierpinski_pyramid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/tablepainter.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/tablepainter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/text2path.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/xqt.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/xqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/browser.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/data.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/browser/bookmarks.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/browser/bookmarks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/browser/browser.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/browser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/browser/data.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/browser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/browser/find_dialog.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/browser/find_dialog.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/browser/loader.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/browser/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/browser/model.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/browser/model.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/browser/tags.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/browser/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/browser/views.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/browser/views.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/backend.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     def finalize(self) -> None:
         raise NotImplementedError
 
 
 class Backend(BackendInterface, metaclass=ABCMeta):
     def __init__(self) -> None:
         self.entity_stack: list[tuple[DXFGraphic, Properties]] = []
-        self.config: Configuration
+        self.config: Configuration = Configuration()
 
     def configure(self, config: Configuration) -> None:
         self.config = config
 
     def enter_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         # gets the full DXF properties information
         self.entity_stack.append((entity, properties))
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/clipper.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/clipper.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,21 +49,26 @@
         if self.view is not None:
             return self.view.clip_line(start, end)
         return start, end
 
     def clip_filled_paths(
         self, paths: Iterable[Path | Path2d], max_sagitta: float
     ) -> Iterator[Path | Path2d]:
+        m = self.m
         for path in paths:
+            if m is not None:
+                path = path.transform(m)
+            # path in paperspace units!
             box = BoundingBox2d(path.control_vertices())
             view = self.view
             assert view is not None
             if view.is_inside(box.extmin) and view.is_inside(box.extmax):
+                # no clipping needed
                 yield path
-            else:
+            else:  # clipping is required, but only clipping of polygons is supported
                 yield from_vertices(
                     view.clip_polygon(
                         Vec2.list(path.flattening(max_sagitta, segments=16))
                     ),
                     close=True,
                 )
 
@@ -73,24 +78,27 @@
         view = self.view
         assert view is not None
         m = self.m
 
         for path in paths:
             if m is not None:
                 path = path.transform(m)
+            # path in paperspace units!
             box = BoundingBox2d(path.control_vertices())
             if view.is_inside(box.extmin) and view.is_inside(box.extmax):
                 yield path
             for sub_path in single_paths([path]):  # type: ignore
                 polyline = Vec2.list(sub_path.flattening(max_sagitta, segments=16))
                 for part in view.clip_polyline(polyline):
                     yield from_vertices(part, close=False)
 
     def clip_polygon(self, points: Iterable[AnyVec]) -> Sequence[Vec2]:
         if self.m is not None:
             points = self.m.fast_2d_transform(points)
+            # points in paperspace units!
+        points = list(points)
         view = self.view
         if view is not None:
             box = BoundingBox2d(points)
             if not view.is_inside(box.extmin) or not view.is_inside(box.extmax):
                 return view.clip_polygon(points)
-        return list(points)
+        return points
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/config.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-# Copyright (c) 2021-2022, Matthew Broadway
+# Copyright (c) 2021-2023, Matthew Broadway
 # License: MIT License
 from __future__ import annotations
 from typing import Optional
+import warnings
 import dataclasses
 from dataclasses import dataclass
 from enum import Enum, auto
 
 from ezdxf import disassemble
 from ezdxf.enums import Measurement
+from .type_hints import Color
 
 
 class LinePolicy(Enum):
     """
     Attributes:
         SOLID: draw all lines as solid regardless of the linetype style
-        APPROXIMATE: use the closest approximation available to the
-            backend for rendering styled lines
-        ACCURATE: analyse and render styled lines as accurately as
-            possible. This approach is slower and is not well suited
-            to interactive applications.
+        ACCURATE: render styled lines as accurately as possible
+
     """
 
     SOLID = auto()
     APPROXIMATE = auto()  # ignored since v0.18.1 => ACCURATE
     ACCURATE = auto()
 
 
@@ -32,15 +31,15 @@
     .. note::
 
         To get proxy graphics support proxy graphics have to be loaded:
         Set the global option :attr:`ezdxf.options.load_proxy_graphics` to
         ``True``, which is the default value.
 
         This can not prevent drawing proxy graphic inside of blocks,
-        because this is outside of the domain of the drawing add-on!
+        because this is beyond the domain of the drawing add-on!
 
     Attributes:
         IGNORE: do not display proxy graphics (skip_entity will be called instead)
         SHOW: if the entity cannot be rendered directly (eg if not implemented)
             but a proxy is present: display the proxy
         PREFER: display proxy graphics even for entities where direct rendering
             is available
@@ -63,14 +62,78 @@
 
     IGNORE = auto()
     SHOW_OUTLINE = auto()
     SHOW_SOLID = auto()
     SHOW_APPROXIMATE_PATTERN = auto()  # ignored since v0.18.1
 
 
+class LineweightPolicy(Enum):
+    """This enum is used to define how to determine the lineweight.
+
+    Attributes:
+        ABSOLUTE: in mm as resolved by the :class:`Frontend` class
+        RELATIVE: lineweight is relative to page size
+        RELATIVE_FIXED: fixed lineweight relative to page size for all strokes
+
+    """
+
+    ABSOLUTE = auto()
+    # set fixed lineweight for all strokes in absolute mode:
+    # set Configuration.min_lineweight to the desired lineweight in 1/300 inch!
+    # set Configuration.lineweight_scaling to 0
+
+    # The RELATIVE policy is a backend feature and is not supported by all backends!
+    RELATIVE = auto()
+    RELATIVE_FIXED = auto()
+
+
+class ColorPolicy(Enum):
+    """This enum is used to define how to determine the line/fill color.
+
+    Attributes:
+        COLOR: as resolved by the :class:`Frontend` class
+        COLOR_SWAP_BW: as resolved by the :class:`Frontend` class but swaps black and white
+        COLOR_NEGATIVE: invert colors
+        MONOCHROME_BLACK_BG: all colors to gray scale for black background
+        MONOCHROME_WHITE_BG:  all colors to gray scale for white background
+        BLACK: all colors to black
+        WHITE: all colors to white
+        CUSTOM: all colors to custom color by :attr:`Configuration.custom_fg_color`
+
+    """
+
+    COLOR = auto()
+    COLOR_SWAP_BW = auto()
+    COLOR_NEGATIVE = auto()
+    MONOCHROME_BLACK_BG = auto()
+    MONOCHROME_WHITE_BG = auto()
+    BLACK = auto()
+    WHITE = auto()
+    CUSTOM = auto()
+
+
+class BackgroundPolicy(Enum):
+    """This enum is used to define the background color.
+
+    Attributes:
+        DEFAULT: as resolved by the :class:`Frontend` class
+        WHITE: white background
+        BLACK: black background
+        OFF: fully transparent background
+        CUSTOM: custom background color by :attr:`Configuration.custom_bg_color`
+
+    """
+
+    DEFAULT = auto()
+    WHITE = auto()
+    BLACK = auto()
+    OFF = auto()
+    CUSTOM = auto()
+
+
 @dataclass(frozen=True)
 class Configuration:
     """Configuration options for the :mod:`drawing` add-on.
 
     Attributes:
         pdsize: the size to draw POINT entities (in drawing units)
             set to None to use the $PDSIZE value from the dxf document header
@@ -117,49 +180,51 @@
             into drawing units. Sets Path() approximation accuracy
         circle_approximation_count: Approximate a full circle by `n` segments, arcs
             have proportional less segments. Only used for approximation of arcs
             in banded polylines.
         hatching_timeout: hatching timeout for a single entity, very dense
             hatching patterns can cause a very long execution time, the default
             timeout for a single entity is 30 seconds.
+        color_policy:
+        custom_fg_color: Used for :class:`ColorPolicy.custom` policy, custom foreground
+            color as "#RRGGBBAA" color string (RGB+alpha)
+        background_policy:
+        custom_bg_color: Used for :class:`BackgroundPolicy.custom` policy, custom
+            background color as "#RRGGBBAA" color string (RGB+alpha)
+        lineweight_policy:
 
     """
 
-    pdsize: Optional[int]
-    pdmode: Optional[int]
-    measurement: Optional[Measurement]
-    show_defpoints: bool
-    proxy_graphic_policy: ProxyGraphicPolicy
-    line_policy: LinePolicy
-    hatch_policy: HatchPolicy
-    infinite_line_length: float
-    lineweight_scaling: float
-    min_lineweight: Optional[float]
-    min_dash_length: float
-    max_flattening_distance: float
-    circle_approximation_count: int
-    hatching_timeout: float
+    pdsize: Optional[int] = None  # use $PDSIZE from HEADER section
+    pdmode: Optional[int] = None  # use $PDMODE from HEADER section
+    measurement: Optional[Measurement] = None
+    show_defpoints: bool = False
+    proxy_graphic_policy: ProxyGraphicPolicy = ProxyGraphicPolicy.SHOW
+    line_policy: LinePolicy = LinePolicy.ACCURATE
+    hatch_policy: HatchPolicy = HatchPolicy.SHOW_APPROXIMATE_PATTERN
+    infinite_line_length: float = 20
+    lineweight_scaling: float = 1.0
+    min_lineweight: Optional[float] = None
+    min_dash_length: float = 0.1
+    max_flattening_distance: float = disassemble.Primitive.max_flattening_distance
+    circle_approximation_count: int = 128
+    hatching_timeout: float = 30.0
+    color_policy: ColorPolicy = ColorPolicy.COLOR
+    custom_fg_color: Color = "#000000"
+    background_policy: BackgroundPolicy = BackgroundPolicy.DEFAULT
+    custom_bg_color: Color = "#ffffff"
+    lineweight_policy: LineweightPolicy = LineweightPolicy.ABSOLUTE
 
     @staticmethod
-    def defaults() -> "Configuration":
-        return Configuration(
-            pdsize=None,  # use $PDSIZE from HEADER section
-            pdmode=None,  # use $PDMODE from HEADER section
-            measurement=None,  # use $MEASUREMENT from HEADER section
-            show_defpoints=False,
-            proxy_graphic_policy=ProxyGraphicPolicy.SHOW,
-            line_policy=LinePolicy.APPROXIMATE,
-            hatch_policy=HatchPolicy.SHOW_APPROXIMATE_PATTERN,
-            infinite_line_length=20,
-            lineweight_scaling=1.0,
-            min_lineweight=None,
-            min_dash_length=0.1,
-            max_flattening_distance=disassemble.Primitive.max_flattening_distance,
-            circle_approximation_count=128,
-            hatching_timeout=30.0,
+    def defaults() -> Configuration:
+        warnings.warn(
+            "use Configuration() instead of Configuration.defaults()",
+            DeprecationWarning,
         )
+        return Configuration()
 
-    def with_changes(self, **kwargs) -> "Configuration":
+    def with_changes(self, **kwargs) -> Configuration:
+        """Returns a new frozen :class:`Configuration` object with modified values."""
         params = dataclasses.asdict(self)
         for k, v in kwargs.items():
             params[k] = v
         return Configuration(**params)
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/debug_backend.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/debug_backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """The basic backend has no draw_path() support and approximates all curves
     by lines.
     """
 
     def __init__(self):
         super().__init__()
         self.collector = []
-        self.configure(Configuration.defaults())
+        self.configure(Configuration())
 
     def draw_point(self, pos: AnyVec, properties: BackendProperties) -> None:
         self.collector.append(("point", pos, properties))
 
     def draw_line(
         self, start: AnyVec, end: AnyVec, properties: BackendProperties
     ) -> None:
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/debug_utils.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/debug_utils.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/frontend.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/frontend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2022, Matthew Broadway
+# Copyright (c) 2020-2023, Matthew Broadway
 # License: MIT License
 from __future__ import annotations
 import math
 from typing import (
     Iterable,
     Iterator,
     cast,
@@ -29,16 +29,19 @@
 from ezdxf.addons.drawing.properties import (
     RenderContext,
     VIEWPORT_COLOR,
     OLE2FRAME_COLOR,
     Properties,
     Filling,
     LayoutProperties,
+    BackendProperties,
+    hex_to_rgb,
+    rgb_to_hex,
 )
-from ezdxf.addons.drawing.config import LinePolicy
+from ezdxf.addons.drawing.config import LinePolicy, BackgroundPolicy, ColorPolicy
 from ezdxf.addons.drawing.text import simplified_text_chunks
 from ezdxf.addons.drawing.type_hints import FilterFunc
 from ezdxf.addons.drawing.gfxproxy import DXFGraphicProxy
 from ezdxf.addons.drawing.mtext_complex import complex_mtext_renderer
 from ezdxf.addons.drawing.unified_text_renderer import UnifiedTextRenderer
 from ezdxf.entities import (
     DXFEntity,
@@ -78,14 +81,16 @@
 from ezdxf.tools.text import (
     has_inline_formatting_codes,
     replace_non_printable_characters,
 )
 from ezdxf.lldxf import const
 from ezdxf.render import hatching
 from ezdxf.fonts import fonts
+from ezdxf.colors import luminance
+from .type_hints import Color
 
 
 __all__ = ["Frontend"]
 
 
 TDispatchTable: TypeAlias = Dict[str, Callable[[DXFGraphic, Properties], None]]
 PatternKey: TypeAlias = Tuple[str, float]
@@ -115,15 +120,15 @@
 
     """
 
     def __init__(
         self,
         ctx: RenderContext,
         out: BackendInterface,
-        config: Configuration = Configuration.defaults(),
+        config: Configuration = Configuration(),
         bbox_cache: Optional[ezdxf.bbox.Cache] = None,
     ):
         # RenderContext contains all information to resolve resources for a
         # specific DXF document.
         self.ctx = ctx
         self.out = out
         self.config = ctx.update_configuration(config)
@@ -235,15 +240,15 @@
         """
         if layout_properties is not None:
             # TODO: this does not work, layer properties have to be re-evaluated!
             self.ctx.current_layout_properties = layout_properties
         else:
             self.ctx.set_current_layout(layout)
         # set background before drawing entities
-        self.out.set_background(self.ctx.current_layout_properties.background_color)
+        self.set_background(self.ctx.current_layout_properties.background_color)
         self.parent_stack = []
         handle_mapping = list(layout.get_redraw_order())
         if handle_mapping:
             self.draw_entities(
                 reorder.ascending(layout, handle_mapping),
                 filter_func=filter_func,
             )
@@ -251,14 +256,28 @@
             self.draw_entities(
                 layout,
                 filter_func=filter_func,
             )
         if finalize:
             self.out.finalize()
 
+    def set_background(self, color: Color) -> None:
+        policy = self.config.background_policy
+        if policy == BackgroundPolicy.DEFAULT:
+            pass
+        elif policy == BackgroundPolicy.OFF:
+            color = "#ffffff00"  # white, fully transparent
+        elif policy == BackgroundPolicy.BLACK:
+            color = "#000000"
+        elif policy == BackgroundPolicy.WHITE:
+            color = "#ffffff"
+        elif policy == BackgroundPolicy.CUSTOM:
+            color = self.config.custom_bg_color
+        self.out.set_background(color)
+
     def draw_entities(
         self,
         entities: Iterable[DXFGraphic],
         *,
         filter_func: Optional[FilterFunc] = None,
     ) -> None:
         """Draw the given `entities`. The method skips invisible entities
@@ -272,14 +291,17 @@
 
         Args:
             entity: DXF entity inherited from DXFGraphic()
             properties: resolved entity properties
 
         """
         self.out.enter_entity(entity, properties)
+        if not entity.is_virtual:
+            # top level entity
+            self._designer.set_current_entity_handle(entity.dxf.handle)
         if (
             entity.proxy_graphic
             and self.config.proxy_graphic_policy == ProxyGraphicPolicy.PREFER
         ):
             self.draw_proxy_graphic(entity.proxy_graphic, entity.doc)
         else:
             draw_method = self._dispatch.get(entity.dxftype(), None)
@@ -532,15 +554,15 @@
             return
 
         if external_paths:
             self._designer.draw_filled_paths(
                 ignore_text_boxes(external_paths), holes, properties
             )
         elif holes:
-            # The first path is considered the exterior path, everything else is
+            # The first path is considered the exterior path, everything else are
             # holes.
             self._designer.draw_filled_paths([holes[0]], holes[1:], properties)
 
     def draw_mpolygon_entity(self, entity: DXFGraphic, properties: Properties):
         def resolve_fill_color() -> str:
             return self.ctx.resolve_aci_color(entity.dxf.fill_color, properties.layer)
 
@@ -581,27 +603,21 @@
         properties.color = self.ctx.current_layout_properties.background_color
         path = wipeout.boundary_path_wcs()
         self._designer.draw_filled_polygon(path, properties)
 
     def draw_viewport_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         assert isinstance(entity, Viewport)
         vp = entity
-        # Special VIEWPORT id == 1, this viewport defines the "active viewport"
-        # which is the area currently shown in the layout tab by the CAD
-        # application.
-        # BricsCAD set id to -1 if the viewport is off and 'status' (group
-        # code 68) is not present.
-        if vp.dxf.id < 2 or vp.dxf.status < 1:
+        if vp.dxf.get("status", 0) < 2:  # 0= off; 1= "active viewport"
             return
+
         if not vp.is_top_view:
             self.log_message("Cannot render non top-view viewports")
             return
-        if not self._designer.draw_viewport(vp, self.ctx, self._bbox_cache):
-            # viewports are not supported by the backend
-            self._draw_filled_rect(vp.clipping_rect_corners(), VIEWPORT_COLOR)
+        self._designer.draw_viewport(vp, self.ctx, self._bbox_cache)
 
     def draw_ole2frame_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         ole2frame = cast(OLE2Frame, entity)
         bbox = ole2frame.bbox()
         if not bbox.is_empty:
             self._draw_filled_rect(bbox.rect_vertices(), OLE2FRAME_COLOR)
 
@@ -748,63 +764,82 @@
 
 class Designer:
     """The designer is placed between the frontend and the backend
     and adds this features:
 
         - automatically linetype rendering
         - VIEWPORT rendering
+        - foreground color mapping according Frontend.config.color_policy
 
     """
 
     def __init__(self, frontend: Frontend, backend: BackendInterface):
         self.frontend = frontend
         self.backend = backend
         self.config = frontend.config
         self.pattern_cache: dict[PatternKey, Sequence[float]] = dict()
         self.text_engine = UnifiedTextRenderer()
         self.default_font_face = fonts.FontFace()
         self.clipper = ClippingRect()
         self.current_vp_scale = 1.0
+        self._current_entity_handle: str = ""
+        self._color_mapping: dict[str, str] = dict()
 
     @property
     def vp_ltype_scale(self) -> float:
         """The linetype pattern should look the same in all viewports
-        independent of the viewport scaling.
+        regardless of the viewport scale.
         """
         return 1.0 / max(self.current_vp_scale, 0.0001)  # max out at 1:10000
 
+    def get_backend_properties(self, properties: Properties) -> BackendProperties:
+        try:
+            color = self._color_mapping[properties.color]
+        except KeyError:
+            color = apply_color_policy(
+                properties.color, self.config.color_policy, self.config.custom_fg_color
+            )
+            self._color_mapping[properties.color] = color
+        return BackendProperties(
+            color,
+            properties.lineweight,
+            properties.layer,
+            properties.pen,
+            self._current_entity_handle,
+        )
+
+    def set_current_entity_handle(self, handle: str) -> None:
+        assert handle is not None
+        self._current_entity_handle = handle
+
     def draw_viewport(
         self,
         vp: Viewport,
         layout_ctx: RenderContext,
         bbox_cache: Optional[ezdxf.bbox.Cache] = None,
-    ) -> bool:
+    ) -> None:
         """Draw the content of the given viewport current viewport.
         Returns ``False`` if the backend doesn't support viewports.
         """
         if vp.doc is None:
-            return False
+            return
         try:
             msp_limits = vp.get_modelspace_limits()
         except ValueError:  # modelspace limits not detectable
-            return False
+            return
         if self.enter_viewport(vp):
             _draw_entities(
                 self.frontend,
                 layout_ctx.from_viewport(vp),
                 filter_vp_entities(vp.doc.modelspace(), msp_limits, bbox_cache),
             )
             self.exit_viewport()
-            return True
-        return False
 
     def enter_viewport(self, vp: Viewport) -> bool:
-        """Set current viewport. Returns ``False`` if the backend doesn't
-        support viewports.
-        """
+        """Set current viewport, returns ``True`` for valid viewports."""
         self.current_vp_scale = vp.get_scale()
         m = vp.get_transformation_matrix()
         clipping_path = make_path(vp)
         if len(clipping_path):
             self.clipper.push(clipping_path, m)
             return True
         return False
@@ -815,58 +850,60 @@
 
     def draw_point(self, pos: AnyVec, properties: Properties) -> None:
         if self.clipper.is_active:
             point = self.clipper.clip_point(pos)
             if point is None:
                 return
             pos = point
-        self.backend.draw_point(pos, properties.backend_properties)
+        self.backend.draw_point(pos, self.get_backend_properties(properties))
 
     def draw_line(self, start: AnyVec, end: AnyVec, properties: Properties):
         if (
             self.config.line_policy == LinePolicy.SOLID
             or len(properties.linetype_pattern) < 2  # CONTINUOUS
         ):
             if self.clipper.is_active:
                 points = self.clipper.clip_line(start, end)
-                if points:
-                    self.backend.draw_line(start, end, properties.backend_properties)
-            else:
-                self.backend.draw_line(start, end, properties.backend_properties)
+                if len(points) != 2:
+                    return
+                start, end = points
+            self.backend.draw_line(start, end, self.get_backend_properties(properties))
         else:
             renderer = linetypes.LineTypeRenderer(self.pattern(properties))
-            self.draw_solid_lines(  # including transformation
+            self.draw_solid_lines(  # includes transformation
                 ((s, e) for s, e in renderer.line_segment(start, end)),
                 properties,
             )
 
     def draw_solid_lines(
         self, lines: Iterable[tuple[AnyVec, AnyVec]], properties: Properties
     ) -> None:
         if self.clipper.is_active:
             clipped_lines: list[Sequence[AnyVec]] = []
             for start, end in lines:
                 points = self.clipper.clip_line(start, end)
                 if points:
                     clipped_lines.append(points)
             lines = clipped_lines  # type: ignore
-        self.backend.draw_solid_lines(lines, properties.backend_properties)
+        self.backend.draw_solid_lines(lines, self.get_backend_properties(properties))
 
     def draw_path(self, path: Path | Path2d, properties: Properties):
         if (
             self.config.line_policy == LinePolicy.SOLID
             or len(properties.linetype_pattern) < 2  # CONTINUOUS
         ):
             if self.clipper.is_active:
                 for clipped_path in self.clipper.clip_paths(
                     [path], self.config.max_flattening_distance
                 ):
-                    self.backend.draw_path(clipped_path, properties.backend_properties)
+                    self.backend.draw_path(
+                        clipped_path, self.get_backend_properties(properties)
+                    )
                 return
-            self.backend.draw_path(path, properties.backend_properties)
+            self.backend.draw_path(path, self.get_backend_properties(properties))
         else:
             renderer = linetypes.LineTypeRenderer(self.pattern(properties))
             vertices = path.flattening(self.config.max_flattening_distance, segments=16)
             self.draw_solid_lines(
                 ((s, e) for s, e in renderer.line_segments(vertices)),
                 properties,
             )
@@ -874,30 +911,29 @@
     def draw_filled_paths(
         self,
         paths: Iterable[Path | Path2d],
         holes: Iterable[Path | Path2d],
         properties: Properties,
     ) -> None:
         if self.clipper.is_active:
-            m = self.clipper.m
             max_sagitta = self.config.max_flattening_distance
-            paths = self.clipper.clip_filled_paths(
-                (p.transform(m) for p in paths), max_sagitta
-            )
-            holes = self.clipper.clip_filled_paths(
-                (h.transform(m) for h in holes), max_sagitta
-            )
-        self.backend.draw_filled_paths(paths, holes, properties.backend_properties)
+            paths = self.clipper.clip_filled_paths(paths, max_sagitta)
+            holes = self.clipper.clip_filled_paths(holes, max_sagitta)
+        self.backend.draw_filled_paths(
+            paths, holes, self.get_backend_properties(properties)
+        )
 
     def draw_filled_polygon(
         self, points: Iterable[AnyVec], properties: Properties
     ) -> None:
         if self.clipper.is_active:
             points = self.clipper.clip_polygon(points)
-        self.backend.draw_filled_polygon(points, properties.backend_properties)
+        self.backend.draw_filled_polygon(
+            points, self.get_backend_properties(properties)
+        )
 
     def pattern(self, properties: Properties) -> Sequence[float]:
         """Get pattern - implements pattern caching."""
         if self.config.line_policy == LinePolicy.SOLID:
             scale = 0.0
         else:
             scale = properties.linetype_scale * self.vp_ltype_scale
@@ -937,15 +973,15 @@
         font_face = properties.font
         if font_face is None:
             font_face = self.default_font_face
         try:
             text_path = self.text_engine.get_text_path(text, font_face, cap_height)
         except (RuntimeError, ValueError):
             return
-        
+
         transformed_path = text_path.transform(transform)
         if self.text_engine.is_stroke_font(font_face):
             self.draw_path(transformed_path, properties)
             return
         polygons = fast_bbox_detection(single_paths([transformed_path]))  # type: ignore
         external_paths, holes = winding_deconstruction(polygons)  # type: ignore
         if properties.filling is None:
@@ -1045,7 +1081,52 @@
         text = text.replace("\t", "?")
     elif dxftype == "MTEXT":
         text = replace_non_printable_characters(text, replacement="▯")
         text = text.replace("\t", "        ")
     else:
         raise TypeError(dxftype)
     return text
+
+
+def invert_color(color: Color) -> Color:
+    r, g, b = hex_to_rgb(color)
+    return rgb_to_hex((255 - r, 255 - g, 255 - b))
+
+
+def swap_bw(color: str) -> Color:
+    color = color.lower()
+    if color == "#000000":
+        return "#ffffff"
+    if color == "#ffffff":
+        return "#000000"
+    return color
+
+
+def color_to_monochrome(color: Color, invert=False) -> Color:
+    lum = luminance(hex_to_rgb(color))
+    if invert:
+        gray = round((1.0 - lum) * 255)
+    else:
+        gray = round(lum * 255)
+    return rgb_to_hex((gray, gray, gray))
+
+
+def apply_color_policy(color: Color, policy: ColorPolicy, custom_color: Color) -> Color:
+    alpha = color[7:9]
+    color = color[:7]
+    if policy == ColorPolicy.COLOR_SWAP_BW:
+        color = swap_bw(color)
+    elif policy == ColorPolicy.COLOR_NEGATIVE:
+        color = invert_color(color)
+    elif policy == ColorPolicy.MONOCHROME_WHITE_BG:
+        color = color_to_monochrome(color, invert=True)
+    elif policy == ColorPolicy.MONOCHROME_BLACK_BG:
+        color = color_to_monochrome(color, invert=False)
+    elif policy == ColorPolicy.BLACK:
+        color = "#000000"
+    elif policy == ColorPolicy.WHITE:
+        color = "#ffffff"
+    elif policy == ColorPolicy.CUSTOM:
+        fg = custom_color
+        color = fg[:7]
+        alpha = fg[7:9]
+    return color + alpha
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/gfxproxy.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/gfxproxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/matplotlib.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/matplotlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,15 @@
     import matplotlib
 
     # Set the backend to prevent warnings about GUIs being opened from a thread
     # other than the main thread.
     old_backend = matplotlib.get_backend()
     matplotlib.use(backend)
     if config is None:
-        config = Configuration.defaults()
+        config = Configuration()
 
     try:
         fig: plt.Figure = plt.figure(dpi=dpi)
         ax: plt.Axes = fig.add_axes((0, 0, 1, 1))
         ctx = RenderContext(layout.doc)
         layout_properties = LayoutProperties.from_layout(layout)
         if bg is not None:
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/mtext_complex.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/mtext_complex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/properties.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,17 @@
 class Properties:
     """An implementation agnostic representation of DXF entity properties like
     color and linetype. These properties represent the actual values after
     resolving all DXF specific rules like "by layer", "by block" and so on.
     """
 
     def __init__(self) -> None:
-        self.color: str = "#ffffff"  # format #RRGGBB or #RRGGBBAA
+        # color string format "#RRGGBB" or "#RRGGBBAA"
+        # alpha channel AA: 0x00 = transparent; 0xff = opaque
+        self.color: str = "#ffffff"
         self.pen = 7  # equals the ACI (1-255), for pen based backends like plotters
 
         # Linetype rendering is done by the frontend, the backend receives only solid
         # lines.
         self.linetype_name: str = "CONTINUOUS"
 
         # Simplified DXF linetype definition:
@@ -159,25 +161,22 @@
         return hex_to_rgb(self.color[:7])  # ignore alpha if present
 
     @property
     def luminance(self) -> float:
         """Returns perceived color luminance in range [0, 1] from dark to light."""
         return luminance(self.rgb)
 
-    @property
-    def backend_properties(self) -> BackendProperties:
-        return BackendProperties(self.color, self.lineweight, self.layer, self.pen)
-
 
 class BackendProperties(NamedTuple):
     """The backend receives a condensed version of the entity properties."""
     color: Color = "#000000"
     lineweight: float = 0.25  # in mm
     layer: str = "0"  # maybe useful to group entities (SVG, PDF)
     pen: int = 1  # equals the ACI (1-255), for pen based backends like plotters
+    handle: str = ""  # top level entity handle
 
     @property
     def rgb(self) -> RGB:
         """Returns color as RGB tuple."""
         return hex_to_rgb(self.color[:7])  # ignore alpha if present
 
     @property
@@ -734,19 +733,16 @@
         else:
             return self.current_layout_properties.default_color  # unknown / invalid
 
     def _aci_to_true_color(self, aci: int) -> Color:
         """Returns the `aci` value (AutoCAD Color Index) as rgb value in
         hex format: "#RRGGBB".
         """
-        if aci == 7:  # black/white; todo: this bypasses the plot style table
-            if self.current_layout_properties.has_dark_background:
-                return "#ffffff"
-            else:
-                return "#000000"
+        if aci == 7:  # black/white
+            return self.current_layout_properties.default_color
         else:
             return rgb_to_hex(self.plot_styles[aci].color)
 
     def resolve_linetype(
         self, entity: DXFGraphic, *, resolved_layer: Optional[str] = None
     ) -> tuple[str, Sequence[float]]:
         """Resolve the linetype of `entity`. Returns a tuple of the linetype
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/pyqt.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/pyqt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # Copyright (c) 2020-2023, Matthew Broadway
 # License: MIT License
 # mypy: ignore_errors=True
 from __future__ import annotations
-from typing import Optional, Iterable, Tuple
-from typing_extensions import TypeAlias
+from typing import Optional, Iterable
+import abc
 import math
 
 from ezdxf.addons.xqt import QtCore as qc, QtGui as qg, QtWidgets as qw
 from ezdxf.addons.drawing.backend import Backend
 from ezdxf.addons.drawing.config import Configuration
 from ezdxf.addons.drawing.type_hints import Color
 from ezdxf.addons.drawing.properties import BackendProperties
 from ezdxf.math import Vec3, Matrix44
 from ezdxf.path import Path, to_qpainter_path
 
-PatternKey: TypeAlias = Tuple[str, float]
-
 
 class _Point(qw.QAbstractGraphicsShapeItem):
     """A dimensionless point which is drawn 'cosmetically' (scale depends on
     view)
     """
 
     def __init__(self, x: float, y: float, brush: qg.QBrush):
@@ -41,136 +39,97 @@
         painter.setPen(qc.Qt.NoPen)
         painter.drawEllipse(self.location, radius, radius)
 
     def boundingRect(self) -> qc.QRectF:
         return qc.QRectF(self.location, qc.QSizeF(1, 1))
 
 
-class ViewportGroup(qw.QGraphicsItemGroup):
-    def __init__(self, clipping_path: Path):
-        super().__init__()
-        self.setFlag(
-            qw.QGraphicsItemGroup.GraphicsItemFlag.ItemClipsChildrenToShape,
-            True,
-        )
-        self._clipping_path = to_qpainter_path([clipping_path])
-
-    def shape(self):
-        return self._clipping_path
-
-
 # The key used to store the dxf entity corresponding to each graphics element
 CorrespondingDXFEntity = qc.Qt.UserRole + 0  # type: ignore
 CorrespondingDXFParentStack = qc.Qt.UserRole + 1  # type: ignore
 
 
-class PyQtBackend(Backend):
+class _PyQtBackend(Backend):
     """
-    Backend which uses the :mod:`PySide6` package to implement an interactive
-    viewer. The :mod:`PyQt5` package can be used as fallback if the :mod:`PySide6`
-    package is not available.
-
-    Args:
-        scene: drawing canvas of type :class:`QtWidgets.QGraphicsScene`,
-            if ``None`` a new canvas will be created
-        extra_lineweight_scaling: compared to other backends,
-            PyQt draws lines which appear thinner
+    Abstract PyQt backend which uses the :mod:`PySide6` package to implement an
+    interactive viewer. The :mod:`PyQt5` package can be used as fallback if the
+    :mod:`PySide6` package is not available.
     """
 
-    def __init__(
-        self,
-        scene: Optional[qw.QGraphicsScene] = None,
-        *,
-        debug_draw_rect: bool = False,
-        extra_lineweight_scaling: float = 2.0,
-    ):
+    def __init__(self, scene: qw.QGraphicsScene):
         super().__init__()
-        self._scene = scene or qw.QGraphicsScene()  # avoids many type errors
+        self._scene = scene
         self._color_cache: dict[Color, qg.QColor] = {}
-        self._pattern_cache: dict[PatternKey, int] = {}
         self._no_line = qg.QPen(qc.Qt.NoPen)
         self._no_fill = qg.QBrush(qc.Qt.NoBrush)
-        self._extra_lineweight_scaling = extra_lineweight_scaling
-        self._debug_draw_rect = debug_draw_rect
 
     def configure(self, config: Configuration) -> None:
         if config.min_lineweight is None:
             config = config.with_changes(min_lineweight=0.24)
         super().configure(config)
 
-    def set_scene(self, scene: qw.QGraphicsScene):
+    def set_scene(self, scene: qw.QGraphicsScene) -> None:
         self._scene = scene
 
-    def _add_item(self, item):
-        self._set_item_data(item)
+    def _add_item(self, item: qw.QGraphicsItem, entity_handle: str) -> None:
+        self.set_item_data(item, entity_handle)
         self._scene.addItem(item)
 
+    @abc.abstractmethod
+    def set_item_data(self, item: qw.QGraphicsItem, entity_handle: str) -> None:
+        ...
+
     def _get_color(self, color: Color) -> qg.QColor:
-        qt_color = self._color_cache.get(color, None)
-        if qt_color is None:
-            if len(color) == 7:
-                qt_color = qg.QColor(color)  # '#RRGGBB'
-            elif len(color) == 9:
-                rgb = color[1:7]
-                alpha = color[7:9]
-                qt_color = qg.QColor(f"#{alpha}{rgb}")  # '#AARRGGBB'
-            else:
-                raise TypeError(color)
+        try:
+            return self._color_cache[color]
+        except KeyError:
+            pass
+        if len(color) == 7:
+            qt_color = qg.QColor(color)  # '#RRGGBB'
+        elif len(color) == 9:
+            rgb = color[1:7]
+            alpha = color[7:9]
+            qt_color = qg.QColor(f"#{alpha}{rgb}")  # '#AARRGGBB'
+        else:
+            raise TypeError(color)
 
-            self._color_cache[color] = qt_color
+        self._color_cache[color] = qt_color
         return qt_color
 
     def _get_pen(self, properties: BackendProperties) -> qg.QPen:
         """Returns a cosmetic pen with applied lineweight but without line type
         support.
         """
-        px = (
-            properties.lineweight
-            / 0.3527
-            * self.config.lineweight_scaling
-            * self._extra_lineweight_scaling
-        )
+        px = properties.lineweight / 0.3527 * self.config.lineweight_scaling
         pen = qg.QPen(self._get_color(properties.color), px)
         # Use constant width in pixel:
         pen.setCosmetic(True)
         pen.setJoinStyle(qc.Qt.RoundJoin)
         return pen
 
     def _get_fill_brush(self, color: Color) -> qg.QBrush:
         return qg.QBrush(self._get_color(color), qc.Qt.SolidPattern)  # type: ignore
 
-    def _set_item_data(self, item: qw.QGraphicsItem) -> None:
-        parent_stack = tuple(e for e, props in self.entity_stack[:-1])
-        current_entity = self.current_entity
-        if isinstance(item, list):
-            for item_ in item:
-                item_.setData(CorrespondingDXFEntity, current_entity)
-                item_.setData(CorrespondingDXFParentStack, parent_stack)
-        else:
-            item.setData(CorrespondingDXFEntity, current_entity)
-            item.setData(CorrespondingDXFParentStack, parent_stack)
-
     def set_background(self, color: Color):
         self._scene.setBackgroundBrush(qg.QBrush(self._get_color(color)))
 
     def draw_point(self, pos: Vec3, properties: BackendProperties) -> None:
         """Draw a real dimensionless point."""
         brush = self._get_fill_brush(properties.color)
         item = _Point(pos.x, pos.y, brush)
-        self._set_item_data(item)
-        self._add_item(item)
+        self._add_item(item, properties.handle)
 
     def draw_line(self, start: Vec3, end: Vec3, properties: BackendProperties) -> None:
         # PyQt draws a long line for a zero-length line:
         if start.isclose(end):
             self.draw_point(start, properties)
         else:
             item = qw.QGraphicsLineItem(start.x, start.y, end.x, end.y)
             item.setPen(self._get_pen(properties))
-            self._add_item(item)
+            self._add_item(item, properties.handle)
 
     def draw_solid_lines(
         self,
         lines: Iterable[tuple[Vec3, Vec3]],
         properties: BackendProperties,
     ):
         """Fast method to draw a bunch of solid lines with the same properties."""
@@ -178,21 +137,21 @@
         add_line = self._add_item
         for s, e in lines:
             if s.isclose(e):
                 self.draw_point(s, properties)
             else:
                 item = qw.QGraphicsLineItem(s.x, s.y, e.x, e.y)
                 item.setPen(pen)
-                add_line(item)
+                add_line(item, properties.handle)
 
     def draw_path(self, path: Path, properties: BackendProperties) -> None:
         item = qw.QGraphicsPathItem(to_qpainter_path([path]))
         item.setPen(self._get_pen(properties))
         item.setBrush(self._no_fill)
-        self._add_item(item)
+        self._add_item(item, properties.handle)
 
     def draw_filled_paths(
         self,
         paths: Iterable[Path],
         holes: Iterable[Path],
         properties: BackendProperties,
     ) -> None:
@@ -210,42 +169,89 @@
                 continue
             oriented_paths.append(path)
         if len(oriented_paths) == 0:
             return
         item = _CosmeticPath(to_qpainter_path(oriented_paths))
         item.setPen(self._get_pen(properties))
         item.setBrush(self._get_fill_brush(properties.color))
-        self._add_item(item)
+        self._add_item(item, properties.handle)
 
     def draw_filled_polygon(
         self, points: Iterable[Vec3], properties: BackendProperties
     ) -> None:
         brush = self._get_fill_brush(properties.color)
         polygon = qg.QPolygonF()
         for p in points:
             polygon.append(qc.QPointF(p.x, p.y))
         item = _CosmeticPolygon(polygon)
         item.setPen(self._no_line)
         item.setBrush(brush)
-        self._add_item(item)
+        self._add_item(item, properties.handle)
 
     def clear(self) -> None:
         self._scene.clear()
 
     def finalize(self) -> None:
         super().finalize()
         self._scene.setSceneRect(self._scene.itemsBoundingRect())
-        if self._debug_draw_rect:
-            properties = BackendProperties()
-            properties.color = "#000000"
-            self._scene.addRect(
-                self._scene.sceneRect(),
-                self._get_pen(properties),
-                self._no_fill,
-            )
+
+
+class PyQtBackend(_PyQtBackend):
+    """
+    Backend which uses the :mod:`PySide6` package to implement an interactive
+    viewer. The :mod:`PyQt5` package can be used as fallback if the :mod:`PySide6`
+    package is not available.
+
+    Args:
+        scene: drawing canvas of type :class:`QtWidgets.QGraphicsScene`,
+            if ``None`` a new canvas will be created
+    """
+
+    def __init__(
+        self,
+        scene: Optional[qw.QGraphicsScene] = None,
+    ):
+        super().__init__(scene or qw.QGraphicsScene())
+    # This implementation keeps all virtual entities alive by attaching references
+    # to entities to the graphic scene items.
+
+    def set_item_data(self, item: qw.QGraphicsItem, entity_handle: str) -> None:
+        parent_stack = tuple(e for e, props in self.entity_stack[:-1])
+        current_entity = self.current_entity
+        item.setData(CorrespondingDXFEntity, current_entity)
+        item.setData(CorrespondingDXFParentStack, parent_stack)
+
+
+class PyQtPlaybackBackend(_PyQtBackend):
+    """
+    Backend which uses the :mod:`PySide6` package to implement an interactive
+    viewer. The :mod:`PyQt5` package can be used as fallback if the :mod:`PySide6`
+    package is not available.
+
+    This backend can be used a playback backend for the :meth:`replay` method of the
+    :class:`Player` class
+
+    Args:
+        scene: drawing canvas of type :class:`QtWidgets.QGraphicsScene`,
+            if ``None`` a new canvas will be created
+    """
+
+    def __init__(
+        self,
+        scene: Optional[qw.QGraphicsScene] = None,
+    ):
+        super().__init__(scene or qw.QGraphicsScene())
+
+    # The backend recorder does not record enter_entity() and exit_entity() events.
+    # This implementation attaches only entity handles (str) to the graphic scene items.
+    # Each item references the top level entity e.g. all items of a block reference
+    # references the handle of the INSERT entity.
+
+    def set_item_data(self, item: qw.QGraphicsItem, entity_handle: str) -> None:
+        item.setData(CorrespondingDXFEntity, entity_handle)
 
 
 class _CosmeticPath(qw.QGraphicsPathItem):
     def paint(
         self,
         painter: qg.QPainter,
         option: qw.QStyleOptionGraphicsItem,
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/qtviewer.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/analyze.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,453 +1,576 @@
-#!/usr/bin/env python3
-# Copyright (c) 2020-2022, Matthew Broadway
+# Copyright (c) 2021-2022, Manfred Moitzi
 # License: MIT License
-# mypy: ignore_errors=True
+# Debugging tools to analyze DXF entities.
 from __future__ import annotations
-from typing import Iterable, Sequence
-import math
-import os
-import time
-
-from ezdxf.addons.xqt import QtWidgets as qw, QtCore as qc, QtGui as qg
-from ezdxf.addons.xqt import Slot, QAction, Signal
+from typing import Iterable, Sequence, Optional
+import textwrap
 
 import ezdxf
-import ezdxf.bbox
-from ezdxf import recover
-from ezdxf.addons import odafc
-from ezdxf.addons.drawing import Frontend, RenderContext
-from ezdxf.addons.drawing.config import Configuration
-
-from ezdxf.addons.drawing.properties import (
-    is_dark_color,
-    set_layers_state,
-    LayerProperties,
-)
-from ezdxf.addons.drawing.pyqt import (
-    _get_x_scale,
-    PyQtBackend,
-    CorrespondingDXFEntity,
-    CorrespondingDXFParentStack,
+from ezdxf import colors
+from ezdxf.math import Vec2
+from ezdxf.lldxf import const
+from ezdxf.enums import TextEntityAlignment
+from ezdxf.tools.debug import print_bitmask
+from ezdxf.render.mleader import MLeaderStyleOverride, OVERRIDE_FLAG
+from ezdxf.entities import (
+    EdgePath,
+    PolylinePath,
+    LineEdge,
+    ArcEdge,
+    EllipseEdge,
+    SplineEdge,
+    mleader,
 )
-from ezdxf.audit import Auditor
-from ezdxf.document import Drawing
-from ezdxf.entities import DXFGraphic
-from ezdxf.lldxf.const import DXFStructureError
+from ezdxf.entities.polygon import DXFPolygon
 
+EDGE_START_MARKER = "EDGE_START_MARKER"
+EDGE_END_MARKER = "EDGE_END_MARKER"
+HATCH_LAYER = "HATCH"
+POLYLINE_LAYER = "POLYLINE_MARKER"
+LINE_LAYER = "LINE_MARKER"
+ARC_LAYER = "ARC_MARKER"
+ELLIPSE_LAYER = "ELLIPSE_MARKER"
+SPLINE_LAYER = "SPLINE_MARKER"
 
-class CADGraphicsView(qw.QGraphicsView):
+
+class HatchAnalyzer:
     def __init__(
         self,
         *,
-        view_buffer: float = 0.2,
-        zoom_per_scroll_notch: float = 0.2,
-        loading_overlay: bool = True,
+        marker_size: float = 1.0,
+        angle: float = 45,
     ):
-        super().__init__()
-        self._zoom = 1.0
-        self._default_zoom = 1.0
-        self._zoom_limits = (0.5, 100)
-        self._zoom_per_scroll_notch = zoom_per_scroll_notch
-        self._view_buffer = view_buffer
-        self._loading_overlay = loading_overlay
-        self._is_loading = False
-
-        self.setTransformationAnchor(qw.QGraphicsView.AnchorUnderMouse)
-        self.setResizeAnchor(qw.QGraphicsView.AnchorUnderMouse)
-        self.setVerticalScrollBarPolicy(qc.Qt.ScrollBarAlwaysOff)
-        self.setHorizontalScrollBarPolicy(qc.Qt.ScrollBarAlwaysOff)
-        self.setDragMode(qw.QGraphicsView.ScrollHandDrag)
-        self.setFrameShape(qw.QFrame.NoFrame)
-        self.setRenderHints(
-            qg.QPainter.Antialiasing
-            | qg.QPainter.TextAntialiasing
-            | qg.QPainter.SmoothPixmapTransform
-        )
-
-    def clear(self):
-        pass
-
-    def begin_loading(self):
-        self._is_loading = True
-        self.scene().invalidate(qc.QRectF(), qw.QGraphicsScene.AllLayers)
-        qw.QApplication.processEvents()
-
-    def end_loading(self, new_scene: qw.QGraphicsScene):
-        self.setScene(new_scene)
-        self._is_loading = False
-        self.buffer_scene_rect()
-        self.scene().invalidate(qc.QRectF(), qw.QGraphicsScene.AllLayers)
-
-    def buffer_scene_rect(self):
-        scene = self.scene()
-        r = scene.sceneRect()
-        bx, by = (
-            r.width() * self._view_buffer / 2,
-            r.height() * self._view_buffer / 2,
-        )
-        scene.setSceneRect(r.adjusted(-bx, -by, bx, by))
-
-    def fit_to_scene(self):
-        self.fitInView(self.sceneRect(), qc.Qt.KeepAspectRatio)
-        self._default_zoom = _get_x_scale(self.transform())
-        self._zoom = 1
-
-    def _get_zoom_amount(self) -> float:
-        return _get_x_scale(self.transform()) / self._default_zoom
-
-    def wheelEvent(self, event: qg.QWheelEvent) -> None:
-        # dividing by 120 gets number of notches on a typical scroll wheel.
-        # See QWheelEvent documentation
-        delta_notches = event.angleDelta().y() / 120
-        direction = math.copysign(1, delta_notches)
-        factor = (1.0 + self._zoom_per_scroll_notch * direction) ** abs(
-            delta_notches
-        )
-        resulting_zoom = self._zoom * factor
-        if resulting_zoom < self._zoom_limits[0]:
-            factor = self._zoom_limits[0] / self._zoom
-        elif resulting_zoom > self._zoom_limits[1]:
-            factor = self._zoom_limits[1] / self._zoom
-        self.scale(factor, factor)
-        self._zoom *= factor
-
-    def drawForeground(self, painter: qg.QPainter, rect: qc.QRectF) -> None:
-        if self._is_loading and self._loading_overlay:
-            painter.save()
-            painter.fillRect(rect, qg.QColor("#aa000000"))
-            painter.setWorldMatrixEnabled(False)
-            r = self.viewport().rect()
-            painter.setBrush(qc.Qt.NoBrush)
-            painter.setPen(qc.Qt.white)
-            painter.drawText(r.center(), "Loading...")
-            painter.restore()
-
-
-class CADGraphicsViewWithOverlay(CADGraphicsView):
-
-    mouse_moved = Signal(qc.QPointF)
-    element_selected = Signal(object, int)
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self._selected_items: list[qw.QGraphicsItem] = []
-        self._selected_index = None
-
-    def clear(self):
-        super().clear()
-        self._selected_items = None
-        self._selected_index = None
-
-    def begin_loading(self):
-        self.clear()
-        super().begin_loading()
-
-    def drawForeground(self, painter: qg.QPainter, rect: qc.QRectF) -> None:
-        super().drawForeground(painter, rect)
-        if self._selected_items:
-            item = self._selected_items[self._selected_index]
-            r = item.sceneTransform().mapRect(item.boundingRect())
-            painter.fillRect(r, qg.QColor(0, 255, 0, 100))
-
-    def mouseMoveEvent(self, event: qg.QMouseEvent) -> None:
-        super().mouseMoveEvent(event)
-        pos = self.mapToScene(event.pos())
-        self.mouse_moved.emit(pos)
-        selected_items = self.scene().items(pos)
-        if selected_items != self._selected_items:
-            self._selected_items = selected_items
-            self._selected_index = 0 if self._selected_items else None
-            self._emit_selected()
-
-    def mouseReleaseEvent(self, event: qg.QMouseEvent) -> None:
-        super().mouseReleaseEvent(event)
-        if event.button() == qc.Qt.LeftButton and self._selected_items:
-            self._selected_index = (self._selected_index + 1) % len(
-                self._selected_items
+        self.marker_size = marker_size
+        self.angle = angle
+        self.doc = ezdxf.new()
+        self.msp = self.doc.modelspace()
+        self.init_layers()
+        self.init_markers()
+
+    def init_layers(self):
+        self.doc.layers.add(POLYLINE_LAYER, color=colors.YELLOW)
+        self.doc.layers.add(LINE_LAYER, color=colors.RED)
+        self.doc.layers.add(ARC_LAYER, color=colors.GREEN)
+        self.doc.layers.add(ELLIPSE_LAYER, color=colors.MAGENTA)
+        self.doc.layers.add(SPLINE_LAYER, color=colors.CYAN)
+        self.doc.layers.add(HATCH_LAYER)
+
+    def init_markers(self):
+        blk = self.doc.blocks.new(EDGE_START_MARKER)
+        attribs = {"layer": "0"}  # from INSERT
+        radius = self.marker_size / 2.0
+        height = radius
+
+        # start marker: 0-- name
+        blk.add_circle(
+            center=(0, 0),
+            radius=radius,
+            dxfattribs=attribs,
+        )
+        text_start = radius * 4
+        blk.add_line(
+            start=(radius, 0),
+            end=(text_start - radius / 2.0, 0),
+            dxfattribs=attribs,
+        )
+        text = blk.add_attdef(
+            tag="NAME",
+            dxfattribs=attribs,
+        )
+        text.dxf.height = height
+        text.set_placement(
+            (text_start, 0), align=TextEntityAlignment.MIDDLE_LEFT
+        )
+
+        # end marker: name --X
+        blk = self.doc.blocks.new(EDGE_END_MARKER)
+        attribs = {"layer": "0"}  # from INSERT
+        blk.add_line(
+            start=(-radius, -radius),
+            end=(radius, radius),
+            dxfattribs=attribs,
+        )
+        blk.add_line(
+            start=(-radius, radius),
+            end=(radius, -radius),
+            dxfattribs=attribs,
+        )
+        text_start = -radius * 4
+        blk.add_line(
+            start=(-radius, 0),
+            end=(text_start + radius / 2.0, 0),
+            dxfattribs=attribs,
+        )
+        text = blk.add_attdef(
+            tag="NAME",
+            dxfattribs=attribs,
+        )
+        text.dxf.height = height
+        text.set_placement(
+            (text_start, 0), align=TextEntityAlignment.MIDDLE_RIGHT
+        )
+
+    def export(self, name: str) -> None:
+        self.doc.saveas(name)
+
+    def add_hatch(self, hatch: DXFPolygon) -> None:
+        hatch.dxf.discard("extrusion")
+        hatch.dxf.layer = HATCH_LAYER
+        self.msp.add_foreign_entity(hatch)
+
+    def add_boundary_markers(self, hatch: DXFPolygon) -> None:
+        hatch.dxf.discard("extrusion")
+        path_num: int = 0
+
+        for p in hatch.paths:
+            path_num += 1
+            if isinstance(p, PolylinePath):
+                self.add_polyline_markers(p, path_num)
+            elif isinstance(p, EdgePath):
+                self.add_edge_markers(p, path_num)
+            else:
+                raise TypeError(f"unknown boundary path type: {type(p)}")
+
+    def add_start_marker(self, location: Vec2, name: str, layer: str) -> None:
+        self.add_marker(EDGE_START_MARKER, location, name, layer)
+
+    def add_end_marker(self, location: Vec2, name: str, layer: str) -> None:
+        self.add_marker(EDGE_END_MARKER, location, name, layer)
+
+    def add_marker(
+        self, blk_name: str, location: Vec2, name: str, layer: str
+    ) -> None:
+        blkref = self.msp.add_blockref(
+            name=blk_name,
+            insert=location,
+            dxfattribs={
+                "layer": layer,
+                "rotation": self.angle,
+            },
+        )
+        blkref.add_auto_attribs({"NAME": name})
+
+    def add_polyline_markers(self, p: PolylinePath, num: int) -> None:
+        self.add_start_marker(
+            Vec2(p.vertices[0]), f"Poly-S({num})", POLYLINE_LAYER
+        )
+        self.add_end_marker(
+            Vec2(p.vertices[0]), f"Poly-E({num})", POLYLINE_LAYER
+        )
+
+    def add_edge_markers(self, p: EdgePath, num: int) -> None:
+        edge_num: int = 0
+        for edge in p.edges:
+            edge_num += 1
+            name = f"({num}.{edge_num})"
+            if isinstance(
+                edge,
+                LineEdge,
+            ):
+                self.add_line_edge_markers(edge, name)
+            elif isinstance(edge, ArcEdge):
+                self.add_arc_edge_markers(edge, name)
+            elif isinstance(edge, EllipseEdge):
+                self.add_ellipse_edge_markers(edge, name)
+            elif isinstance(edge, SplineEdge):
+                self.add_spline_edge_markers(edge, name)
+            else:
+                raise TypeError(f"unknown edge type: {type(edge)}")
+
+    def add_line_edge_markers(self, line: LineEdge, name: str) -> None:
+        self.add_start_marker(line.start, "Line-S" + name, LINE_LAYER)
+        self.add_end_marker(line.end, "Line-E" + name, LINE_LAYER)
+
+    def add_arc_edge_markers(self, arc: ArcEdge, name: str) -> None:
+        self.add_start_marker(arc.start_point, "Arc-S" + name, ARC_LAYER)
+        self.add_end_marker(arc.end_point, "Arc-E" + name, ARC_LAYER)
+
+    def add_ellipse_edge_markers(self, ellipse: EllipseEdge, name: str) -> None:
+        self.add_start_marker(
+            ellipse.start_point, "Ellipse-S" + name, ELLIPSE_LAYER
+        )
+        self.add_end_marker(
+            ellipse.end_point, "Ellipse-E" + name, ELLIPSE_LAYER
+        )
+
+    def add_spline_edge_markers(self, spline: SplineEdge, name: str) -> None:
+        if len(spline.control_points):
+            # Assuming a clamped B-spline, because this is the only practical
+            # usable B-spline for edges.
+            self.add_start_marker(
+                spline.start_point, "SplineS" + name, SPLINE_LAYER
+            )
+            self.add_end_marker(
+                spline.end_point, "SplineE" + name, SPLINE_LAYER
             )
-            self._emit_selected()
 
-    def _emit_selected(self):
-        self.element_selected.emit(self._selected_items, self._selected_index)
-        self.scene().invalidate(
-            self.sceneRect(), qw.QGraphicsScene.ForegroundLayer
-        )
-
-
-class CadViewer(qw.QMainWindow):
-    def __init__(self, config: Configuration = Configuration.defaults()):
-        super().__init__()
-        self._config = config
-        # Avoid using Optional[...], otherwise mypy requires None checks
-        # everywhere!
-        self.doc: Drawing = None  # type: ignore
-        self._render_context: RenderContext = None  # type: ignore
-        self._visible_layers: set[str] = set()
-        self._current_layout: str = "Model"
-        self._reset_backend()
-        self._bbox_cache = ezdxf.bbox.Cache()
-
-        self.view = CADGraphicsViewWithOverlay()
-        self.view.setScene(qw.QGraphicsScene())
-        self.view.scale(1, -1)  # so that +y is up
-        self.view.element_selected.connect(self._on_element_selected)
-        self.view.mouse_moved.connect(self._on_mouse_moved)
-
-        menu = self.menuBar()
-        select_doc_action = QAction("Select Document", self)
-        select_doc_action.triggered.connect(self._select_doc)
-        menu.addAction(select_doc_action)
-        self.select_layout_menu = menu.addMenu("Select Layout")
-
-        toggle_sidebar_action = QAction("Toggle Sidebar", self)
-        toggle_sidebar_action.triggered.connect(self._toggle_sidebar)
-        menu.addAction(toggle_sidebar_action)
-
-        self.sidebar = qw.QSplitter(qc.Qt.Vertical)
-        self.layers = qw.QListWidget()
-        self.layers.setStyleSheet(
-            "QListWidget {font-size: 12pt;} "
-            "QCheckBox {font-size: 12pt; padding-left: 5px;}"
-        )
-        self.sidebar.addWidget(self.layers)
-        info_container = qw.QWidget()
-        info_layout = qw.QVBoxLayout()
-        info_layout.setContentsMargins(0, 0, 0, 0)
-        self.selected_info = qw.QPlainTextEdit()
-        self.selected_info.setReadOnly(True)
-        info_layout.addWidget(self.selected_info)
-        self.mouse_pos = qw.QLabel()
-        info_layout.addWidget(self.mouse_pos)
-        info_container.setLayout(info_layout)
-        self.sidebar.addWidget(info_container)
-
-        container = qw.QSplitter()
-        self.setCentralWidget(container)
-        container.addWidget(self.view)
-        container.addWidget(self.sidebar)
-        container.setCollapsible(0, False)
-        container.setCollapsible(1, True)
-        w = container.width()
-        container.setSizes([int(3 * w / 4), int(w / 4)])
-
-        self.setWindowTitle("CAD Viewer")
-        self.resize(1600, 900)
-        self.show()
-
-    def _reset_backend(self):
-        # clear caches
-        self._backend = PyQtBackend()
-
-    def _select_doc(self):
-        path, _ = qw.QFileDialog.getOpenFileName(
-            self,
-            caption="Select CAD Document",
-            filter="CAD Documents (*.dxf *.DXF *.dwg *.DWG)",
-        )
-        if path:
-            try:
-                if os.path.splitext(path)[1].lower() == ".dwg":
-                    doc = odafc.readfile(path)
-                    auditor = doc.audit()
-                else:
-                    try:
-                        doc = ezdxf.readfile(path)
-                    except ezdxf.DXFError:
-                        doc, auditor = recover.readfile(path)
-                    else:
-                        auditor = doc.audit()
-                self.set_document(doc, auditor)
-            except IOError as e:
-                qw.QMessageBox.critical(self, "Loading Error", str(e))
-            except DXFStructureError as e:
-                qw.QMessageBox.critical(
-                    self,
-                    "DXF Structure Error",
-                    f'Invalid DXF file "{path}": {str(e)}',
-                )
+    @staticmethod
+    def report(hatch: DXFPolygon) -> list[str]:
+        return hatch_report(hatch)
+
+    @staticmethod
+    def print_report(hatch: DXFPolygon) -> None:
+        print("\n".join(hatch_report(hatch)))
+
+
+def hatch_report(hatch: DXFPolygon) -> list[str]:
+    dxf = hatch.dxf
+    style = const.ISLAND_DETECTION[dxf.hatch_style]
+    pattern_type = const.HATCH_PATTERN_TYPE[dxf.pattern_type]
+    text = [
+        f"{str(hatch)}",
+        f"   solid fill: {bool(dxf.solid_fill)}",
+        f"   pattern type: {pattern_type}",
+        f"   pattern name: {dxf.pattern_name}",
+        f"   associative: {bool(dxf.associative)}",
+        f"   island detection: {style}",
+        f"   has pattern data: {hatch.pattern is not None}",
+        f"   has gradient data: {hatch.gradient is not None}",
+        f"   seed value count: {len(hatch.seeds)}",
+        f"   boundary path count: {len(hatch.paths)}",
+    ]
+    num = 0
+    for path in hatch.paths:
+        num += 1
+        if isinstance(path, PolylinePath):
+            text.extend(polyline_path_report(path, num))
+        elif isinstance(path, EdgePath):
+            text.extend(edge_path_report(path, num))
+    return text
+
+
+def polyline_path_report(p: PolylinePath, num: int) -> list[str]:
+    path_type = ", ".join(const.boundary_path_flag_names(p.path_type_flags))
+    return [
+        f"{num}. Polyline Path, vertex count: {len(p.vertices)}",
+        f"   path type:                      {path_type}",
+    ]
+
+
+def edge_path_report(p: EdgePath, num: int) -> list[str]:
+    closed = False
+    connected = False
+    path_type = ", ".join(const.boundary_path_flag_names(p.path_type_flags))
+    edges = p.edges
+    if len(edges):
+        closed = edges[0].start_point.isclose(edges[-1].end_point)
+        connected = all(
+            e1.end_point.isclose(e2.start_point)
+            for e1, e2 in zip(edges, edges[1:])
+        )
 
-    def set_document(
+    return [
+        f"{num}. Edge Path, edge count: {len(p.edges)}",
+        f"   path type:                      {path_type}",
+        f"   continuously connected edges:   {connected}",
+        f"   closed edge loop:               {closed}",
+    ]
+
+
+MULTILEADER = "MULTILEADER_MARKER"
+POINT_MARKER = "POINT_MARKER"
+
+
+class MultileaderAnalyzer:
+    """Multileader can not be added as foreign entity to a new document.
+    Annotations have to be added to the source document.
+
+    """
+
+    def __init__(
         self,
-        document: Drawing,
-        auditor: Auditor,
+        multileader: mleader.MultiLeader,
         *,
-        layout: str = "Model",
+        marker_size: float = 1.0,
+        report_width: int = 79,
     ):
-        error_count = len(auditor.errors)
-        if error_count > 0:
-            ret = qw.QMessageBox.question(
-                self,
-                "Found DXF Errors",
-                f'Found {error_count} errors in file "{document.filename}"\n'
-                f"Load file anyway? ",
+        self.marker_size = marker_size
+        self.report_width = report_width
+        self.multileader = multileader
+        assert self.multileader.doc is not None, "valid DXF document required"
+        self.doc = self.multileader.doc
+        self.msp = self.doc.modelspace()
+        self.init_layers()
+        self.init_markers()
+
+    def init_layers(self):
+        if self.doc.layers.has_entry(MULTILEADER):
+            return
+        self.doc.layers.add(MULTILEADER, color=colors.RED)
+
+    def init_markers(self):
+        if POINT_MARKER not in self.doc.blocks:
+            blk = self.doc.blocks.new(POINT_MARKER)
+            attribs = {"layer": "0"}  # from INSERT
+            size = self.marker_size
+            size_2 = size / 2.0
+            radius = size / 4.0
+            blk.add_circle(
+                center=(0, 0),
+                radius=radius,
+                dxfattribs=attribs,
             )
-            if ret == qw.QMessageBox.No:
-                auditor.print_error_report(auditor.errors)
-                return
-
-        self.doc = document
-        # initialize bounding box cache for faste paperspace drawing
-        self._bbox_cache = ezdxf.bbox.Cache()
-        self._render_context = self._make_render_context(document)
-        self._reset_backend()
-        self._visible_layers = set()
-        self._current_layout = None
-        self._populate_layouts()
-        self._populate_layer_list()
-        self.draw_layout(layout)
-        self.setWindowTitle("CAD Viewer - " + str(document.filename))
-
-    def _make_render_context(self, doc) -> RenderContext:
-        def update_layers_state(layers: Sequence[LayerProperties]):
-            if self._visible_layers:
-                set_layers_state(layers, self._visible_layers, state=True)
-
-        render_context = RenderContext(doc)
-        render_context.set_layer_properties_override(update_layers_state)
-        return render_context
-
-    def _populate_layer_list(self):
-        self.layers.blockSignals(True)
-        self.layers.clear()
-        for layer in self._render_context.layers.values():
-            name = layer.layer
-            item = qw.QListWidgetItem()
-            self.layers.addItem(item)
-            checkbox = qw.QCheckBox(name)
-            checkbox.setCheckState(
-                qc.Qt.Checked if layer.is_visible else qc.Qt.Unchecked
+            blk.add_line((-size_2, 0), (size_2, 0), dxfattribs=attribs)
+            blk.add_line((0, -size_2), (0, size_2), dxfattribs=attribs)
+
+    @property
+    def context(self) -> mleader.MLeaderContext:
+        return self.multileader.context
+
+    @property
+    def mleaderstyle(self) -> Optional[mleader.MLeaderStyle]:
+        handle = self.multileader.dxf.get("style_handle")
+        return self.doc.entitydb.get(handle)  # type: ignore
+
+    def divider_line(self, symbol="-") -> str:
+        return symbol * self.report_width
+
+    def shorten_lines(self, lines: Iterable[str]) -> list[str]:
+        return [
+            textwrap.shorten(line, width=self.report_width) for line in lines
+        ]
+
+    def report(self) -> list[str]:
+        report = [
+            str(self.multileader),
+            self.divider_line(),
+            "Existing DXF attributes:",
+            self.divider_line(),
+        ]
+        report.extend(self.multileader_attributes())
+        report.extend(self.context_attributes())
+        if self.context.mtext is not None:
+            report.extend(self.mtext_attributes())
+        if self.context.block is not None:
+            report.extend(self.block_attributes())
+            if self.multileader.block_attribs:
+                report.extend(self.block_reference_attribs())
+        if self.multileader.context.leaders:
+            report.extend(self.leader_attributes())
+        if self.multileader.arrow_heads:
+            report.extend(self.arrow_heads())
+        return self.shorten_lines(report)
+
+    def print_report(self) -> None:
+        width = self.report_width
+        print()
+        print("=" * width)
+        print("\n".join(self.report()))
+        print("=" * width)
+
+    def print_overridden_properties(self):
+        print("\n".join(self.overridden_attributes()))
+
+    def overridden_attributes(self) -> list[str]:
+        multileader = self.multileader
+        style = self.mleaderstyle
+        if style is not None:
+            report = [
+                self.divider_line(),
+                f"Override attributes of {str(style)}: '{style.dxf.name}'",
+                self.divider_line(),
+            ]
+
+            override = MLeaderStyleOverride(style, multileader)
+            for name in OVERRIDE_FLAG.keys():
+                if override.is_overridden(name):
+                    report.append(f"{name}: {override.get(name)}")
+            if override.use_mtext_default_content:
+                report.append("use_mtext_default_content: 1")
+        else:
+            handle = self.multileader.dxf.get("style_handle")
+            report = [
+                self.divider_line(),
+                f"MLEADERSTYLE(#{handle}) not found",
+            ]
+        return report
+
+    def multileader_attributes(self) -> list[str]:
+        attribs = self.multileader.dxf.all_existing_dxf_attribs()
+        keys = sorted(attribs.keys())
+        return [f"{key}: {attribs[key]}" for key in keys]
+
+    def print_override_state(self):
+        flags = self.multileader.dxf.property_override_flags
+        print(f"\nproperty_override_flags:")
+        print(f"dec: {flags}")
+        print(f"hex: {hex(flags)}")
+        print_bitmask(flags)
+
+    def print_context_attributes(self):
+        print("\n".join(self.context_attributes()))
+
+    def context_attributes(self) -> list[str]:
+        context = self.context
+        if context is None:
+            return []
+        report = [
+            self.divider_line(),
+            "CONTEXT object attributes:",
+            self.divider_line(),
+            f"has MTEXT content: {yes_or_no(context.mtext)}",
+            f"has BLOCK content: {yes_or_no(context.block)}",
+            self.divider_line(),
+        ]
+        keys = [
+            key
+            for key in context.__dict__.keys()
+            if key not in ("mtext", "block", "leaders")
+        ]
+        attributes = [f"{name}: {getattr(context, name)}" for name in keys]
+        attributes.sort()
+        report.extend(attributes)
+        return self.shorten_lines(report)
+
+    def print_mtext_attributes(self):
+        print("\n".join(self.mtext_attributes()))
+
+    def mtext_attributes(self) -> list[str]:
+        report = [
+            self.divider_line(),
+            "MTEXT content attributes:",
+            self.divider_line(),
+        ]
+        mtext = self.context.mtext
+        if mtext is not None:
+            report.extend(_content_attributes(mtext))
+        return self.shorten_lines(report)
+
+    def print_block_attributes(self):
+        print("\n".join(self.block_attributes()))
+
+    def block_attributes(self) -> list[str]:
+        report = [
+            self.divider_line(),
+            "BLOCK content attributes:",
+            self.divider_line(),
+        ]
+        block = self.context.block
+        if block is not None:
+            report.extend(_content_attributes(block))
+        return self.shorten_lines(report)
+
+    def print_leader_attributes(self):
+        print("\n".join(self.leader_attributes()))
+
+    def leader_attributes(self) -> list[str]:
+        report = []
+        leaders = self.context.leaders
+        if leaders is not None:
+            for index, leader in enumerate(leaders):
+                report.extend(self._leader_attributes(index, leader))
+        return self.shorten_lines(report)
+
+    def _leader_attributes(
+        self, index: int, leader: mleader.LeaderData
+    ) -> list[str]:
+        report = [
+            self.divider_line(),
+            f"{index+1}. LEADER attributes:",
+            self.divider_line(),
+        ]
+        report.extend(_content_attributes(leader, exclude=("lines", "breaks")))
+        s = ", ".join(map(str, leader.breaks))
+        report.append(f"breaks: [{s}]")
+        if leader.lines:
+            report.extend(self._leader_lines(leader.lines))
+        return report
+
+    def _leader_lines(self, lines) -> list[str]:
+        report = []
+        for num, line in enumerate(lines):
+            report.extend(
+                [
+                    self.divider_line(),
+                    f"{num + 1}. LEADER LINE attributes:",
+                    self.divider_line(),
+                ]
             )
-            checkbox.stateChanged.connect(self._layers_updated)
-            text_color = (
-                "#FFFFFF" if is_dark_color(layer.color, 0.4) else "#000000"
+            for name, value in line.__dict__.items():
+                if name in ("vertices", "breaks"):
+                    vstr = ""
+                    if value is not None:
+                        vstr = ", ".join(map(str, value))
+                    vstr = f"[{vstr}]"
+                else:
+                    vstr = str(value)
+                report.append(f"{name}: {vstr}")
+        return report
+
+    def print_block_attribs(self):
+        print("\n".join(self.block_reference_attribs()))
+
+    def block_reference_attribs(self) -> list[str]:
+        report = [
+            self.divider_line(),
+            f"BLOCK reference attributes:",
+            self.divider_line(),
+        ]
+        for index, attr in enumerate(self.multileader.block_attribs):
+            report.extend(
+                [
+                    f"{index+1}. Attributes",
+                    self.divider_line(),
+                ]
             )
-            checkbox.setStyleSheet(
-                f"color: {text_color}; background-color: {layer.color}"
+            report.append(f"handle: {attr.handle}")
+            report.append(f"index: {attr.index}")
+            report.append(f"width: {attr.width}")
+            report.append(f"text: {attr.text}")
+        return report
+
+    def arrow_heads(self) -> list[str]:
+        report = [
+            self.divider_line(),
+            f"ARROW HEAD attributes:",
+            self.divider_line(),
+        ]
+        for index, attr in enumerate(self.multileader.arrow_heads):
+            report.extend(
+                [
+                    f"{index+1}. Arrow Head",
+                    self.divider_line(),
+                ]
             )
-            self.layers.setItemWidget(item, checkbox)
-        self.layers.blockSignals(False)
-
-    def _populate_layouts(self):
-        def draw_layout(name: str):
-            def run():
-                self.draw_layout(name, reset_view=True)
-
-            return run
-
-        self.select_layout_menu.clear()
-        for layout_name in self.doc.layout_names_in_taborder():
-            action = QAction(layout_name, self)
-            action.triggered.connect(draw_layout(layout_name))
-            self.select_layout_menu.addAction(action)
-
-    def draw_layout(
-        self,
-        layout_name: str,
-        reset_view: bool = True,
-    ):
-        print(f"drawing {layout_name}")
-        self._current_layout = layout_name
-        self.view.begin_loading()
-        new_scene = qw.QGraphicsScene()
-        self._backend.set_scene(new_scene)
-        layout = self.doc.layout(layout_name)
-        self._update_render_context(layout)
-        try:
-            start = time.perf_counter()
-            self.create_frontend().draw_layout(layout)
-            duration = time.perf_counter() - start
-            print(f"took {duration:.4f} seconds")
-        except DXFStructureError as e:
-            qw.QMessageBox.critical(
-                self,
-                "DXF Structure Error",
-                f'Abort rendering of layout "{layout_name}": {str(e)}',
+            report.append(f"handle: {attr.handle}")
+            report.append(f"index: {attr.index}")
+        return report
+
+    def print_mleaderstyle(self):
+        print("\n".join(self.mleaderstyle_attributes()))
+
+    def mleaderstyle_attributes(self) -> list[str]:
+        report = []
+        style = self.mleaderstyle
+        if style is not None:
+            report.extend(
+                [
+                    self.divider_line("="),
+                    str(style),
+                    self.divider_line("="),
+                ]
             )
-        finally:
-            self._backend.finalize()
-        self.view.end_loading(new_scene)
-        self.view.buffer_scene_rect()
-        if reset_view:
-            self.view.fit_to_scene()
-
-    def create_frontend(self):
-        return Frontend(
-            ctx=self._render_context,
-            out=self._backend,
-            config=self._config,
-            bbox_cache=self._bbox_cache
-        )
-
-    def _update_render_context(self, layout):
-        assert self._render_context is not None
-        self._render_context.set_current_layout(layout)
-
-    def resizeEvent(self, event: qg.QResizeEvent) -> None:
-        self.view.fit_to_scene()
-
-    def _layer_checkboxes(self) -> Iterable[tuple[int, qw.QCheckBox]]:
-        for i in range(self.layers.count()):
-            item = self.layers.itemWidget(self.layers.item(i))
-            yield i, item  # type: ignore
-
-    @Slot(int)  # type: ignore
-    def _layers_updated(self, item_state: qc.Qt.CheckState):
-        shift_held = qw.QApplication.keyboardModifiers() & qc.Qt.ShiftModifier
-        if shift_held:
-            for i, item in self._layer_checkboxes():
-                item.blockSignals(True)
-                item.setCheckState(item_state)
-                item.blockSignals(False)
-
-        self._visible_layers = set()
-        for i, layer in self._layer_checkboxes():
-            if layer.checkState() == qc.Qt.Checked:
-                self._visible_layers.add(layer.text())
-        self.draw_layout(self._current_layout, reset_view=False)
-
-    @Slot()
-    def _toggle_sidebar(self):
-        self.sidebar.setHidden(not self.sidebar.isHidden())
-
-    @Slot(qc.QPointF)
-    def _on_mouse_moved(self, mouse_pos: qc.QPointF):
-        self.mouse_pos.setText(
-            f"mouse position: {mouse_pos.x():.4f}, {mouse_pos.y():.4f}\n"
-        )
-
-    @Slot(object, int)
-    def _on_element_selected(
-        self, elements: list[qw.QGraphicsItem], index: int
-    ):
-        if not elements:
-            text = "No element selected"
+            attribs = style.dxf.all_existing_dxf_attribs()
+            keys = sorted(attribs.keys())
+            report.extend([f"{name}: {attribs[name]}" for name in keys])
         else:
-            text = (
-                f"Selected: {index + 1} / {len(elements)}    (click to cycle)\n"
-            )
-            element = elements[index]
-            dxf_entity = element.data(CorrespondingDXFEntity)
-            if dxf_entity is None:
-                text += "No data"
-            else:
-                text += (
-                    f"Selected Entity: {dxf_entity}\n"
-                    f"Layer: {dxf_entity.dxf.layer}\n\nDXF Attributes:\n"
-                )
-                text += _entity_attribs_string(dxf_entity)
-
-                dxf_parent_stack = element.data(CorrespondingDXFParentStack)
-                if dxf_parent_stack:
-                    text += "\nParents:\n"
-                    for entity in reversed(dxf_parent_stack):
-                        text += f"- {entity}\n"
-                        text += _entity_attribs_string(entity, indent="    ")
-
-        self.selected_info.setPlainText(text)
-
-
-def _entity_attribs_string(dxf_entity: DXFGraphic, indent: str = "") -> str:
-    text = ""
-    for key, value in dxf_entity.dxf.all_existing_dxf_attribs().items():
-        text += f"{indent}- {key}: {value}\n"
-    return text
+            handle = self.multileader.dxf.get("style_handle")
+            report.append(f"MLEADERSTYLE(#{handle}) not found")
+        return self.shorten_lines(report)
+
+
+def _content_attributes(
+    entity, exclude: Optional[Sequence[str]] = None
+) -> list[str]:
+    exclude = exclude or []
+    if entity is not None:
+        return [
+            f"{name}: {value}"
+            for name, value in entity.__dict__.items()
+            if name not in exclude
+        ]
+    return []
+
+
+def yes_or_no(data) -> str:
+    return "yes" if data else "no"
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/recorder.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/recorder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
-from typing import Iterable, Any, Iterator
+from typing import Iterable, Any, Iterator, Callable, Optional, NamedTuple
+from typing_extensions import Self, TypeAlias
+import copy
 import enum
 import dataclasses
 
 from ezdxf.math import AnyVec, BoundingBox2d, Matrix44
 from ezdxf.path import Path, Path2d
 from ezdxf import npshapes
 from ezdxf.tools import take2
@@ -23,65 +25,78 @@
     FILLED_PATHS = enum.auto()
 
 
 @dataclasses.dataclass
 class DataRecord:
     type: RecordType
     property_hash: int
+    handle: str  # top-level entity handle
     data: Any
 
 
 class Recorder(BackendInterface):
+    """Records the output of the Frontend class."""
+
     def __init__(self) -> None:
-        self.config = Configuration.defaults()
+        self.config = Configuration()
         self.background: Color = "#000000"
         self.records: list[DataRecord] = []
         self.properties: dict[int, BackendProperties] = dict()
-        self._bbox = BoundingBox2d()
 
-    def bbox(self) -> BoundingBox2d:
-        """Returns the bounding box of all recorded shapes as
-        :class:`~ezdxf.math.BoundingBox2d`.
+    def __copy__(self) -> Self:
+        recorder = self.__class__()
+        # config is a frozen dataclass:
+        recorder.config = self.config
+        recorder.background = self.background
+        # mutable - recordings are transformed inplace:
+        recorder.records = copy.deepcopy(self.records)
+        # hashes and BackendProperties are immutable, the properties dict may grow, but
+        # entries will never be removed:
+        recorder.properties = self.properties
+        return recorder
+
+    def copy_player(self) -> Player:
+        """Returns a :class:`Player` instance with a copy of the recordings, this player
+        needs more memory, but does not modify the original recordings.
         """
-        if not self._bbox.has_data:
-            self.update_bbox()
-        return self._bbox
+        return Player(self.__copy__(), shared_recordings=False)
 
-    def update_bbox(self) -> None:
-        points: list[AnyVec] = []
-        for record in self.records:
-            if record.type == RecordType.FILLED_PATHS:
-                for path in record.data[0]:  # only add paths, ignore holes
-                    points.extend(path.extends())
-            else:
-                points.extend(record.data.extends())
-        self._bbox = BoundingBox2d(points)
+    def shared_player(self) -> Player:
+        """Returns a :class:`Player` instance with the original recordings! This player
+        is faster to create and needs less memory but is dangerous because it may modify
+        the original recordings.
+        """
+        return Player(self, shared_recordings=True)
 
     def configure(self, config: Configuration) -> None:
         self.config = config
 
     def set_background(self, color: Color) -> None:
         self.background = color
 
     def store(
         self, type_: RecordType, properties: BackendProperties, data: Any
     ) -> None:
-        prop_hash = hash(properties)
-        self.records.append(DataRecord(type=type_, property_hash=prop_hash, data=data))
+        # exclude top-level entity handle to reduce the variance:
+        # color, lineweight, layer, pen
+        prop_hash = hash(properties[:4])
+        self.records.append(
+            DataRecord(
+                type=type_, property_hash=prop_hash, handle=properties.handle, data=data
+            )
+        )
         self.properties[prop_hash] = properties
 
     def draw_point(self, pos: AnyVec, properties: BackendProperties) -> None:
         self.store(RecordType.POINTS, properties, npshapes.NumpyPoints2d((pos,)))
 
     def draw_line(
         self, start: AnyVec, end: AnyVec, properties: BackendProperties
     ) -> None:
-        self.store(
-            RecordType.POINTS, properties, npshapes.NumpyPoints2d((start, end))
-        )
+        self.store(RecordType.POINTS, properties, npshapes.NumpyPoints2d((start, end)))
 
     def draw_solid_lines(
         self, lines: Iterable[tuple[AnyVec, AnyVec]], properties: BackendProperties
     ) -> None:
         def flatten() -> Iterator[AnyVec]:
             for s, e in lines:
                 yield s
@@ -105,38 +120,74 @@
         holes: Iterable[Path | Path2d],
         properties: BackendProperties,
     ) -> None:
         _paths = tuple(npshapes.NumpyPath2d(p) for p in paths)
         _holes = tuple(npshapes.NumpyPath2d(p) for p in holes)
         self.store(RecordType.FILLED_PATHS, properties, (_paths, _holes))
 
-    def transform(self, m: Matrix44) -> None:
-        """Transforms the recordings by a transformation matrix `m` of type
-        :class:`~ezdxf.math.Matrix44`.
-        """
-        for record in self.records:
-            if record.type == RecordType.FILLED_PATHS:
-                for p in record.data[0]:
-                    p.transform_inplace(m)
-                for p in record.data[1]:
-                    p.transform_inplace(m)
-            else:
-                record.data.transform_inplace(m)
+    def enter_entity(self, entity, properties) -> None:
+        pass
 
-        if self._bbox.has_data:
-            # fast, but maybe inaccurate update
-            self._bbox = BoundingBox2d(m.fast_2d_transform(self._bbox.rect_vertices()))
+    def exit_entity(self, entity) -> None:
+        pass
+
+    def clear(self) -> None:
+        raise NotImplementedError()
+
+    def finalize(self) -> None:
+        pass
+
+
+class Override(NamedTuple):
+    """Represents the override state for a data record.
+
+    Attributes:
+        properties: original or modified :class:`BackendProperties`
+        is_visible: override visibility e.g. switch layers on/off
+
+    """
+    properties: BackendProperties
+    is_visible: bool = True
+
+
+OverrideFunc: TypeAlias = Callable[[BackendProperties], Override]
+
+
+class Player:
+    """Plays the recordings of the :class:`Recorder` backend on another backend."""
+
+    def __init__(self, recorder: Recorder, shared_recordings: bool) -> None:
+        self.config = recorder.config
+        self.background: Color = recorder.background
+        self.records: list[DataRecord] = recorder.records
+        self.properties: dict[int, BackendProperties] = recorder.properties
+        self._bbox = BoundingBox2d()
+        self.has_shared_recordings: bool = shared_recordings
+
+    def replay(
+        self, backend: BackendInterface, override: Optional[OverrideFunc] = None
+    ) -> None:
+        """Replay the recording on another backend that implements the
+        :class:`BackendInterface`. The optional `override` function can be used to
+        override the properties and state of data records, it gets the :class:`BackendProperties`
+        as input and must return an :class:`Override` instance.
+        """
 
-    def replay(self, backend: BackendInterface) -> None:
-        """Replay the recording on another backend."""
         backend.configure(self.config)
         backend.set_background(self.background)
         props = self.properties
         for record in self.records:
-            properties = props[record.property_hash]
+            properties = BackendProperties(
+                *props[record.property_hash][:4], record.handle
+            )
+            if override:
+                state = override(properties)
+                if not state.is_visible:
+                    continue
+                properties = state.properties
             t = record.type
             if t == RecordType.POINTS:
                 vertices = record.data.vertices()
                 if len(vertices) == 1:
                     backend.draw_point(vertices[0], properties)
                 elif len(vertices) == 2:
                     backend.draw_line(vertices[0], vertices[1], properties)
@@ -148,18 +199,42 @@
                 backend.draw_path(record.data.to_path2d(), properties)
             elif t == RecordType.FILLED_PATHS:
                 paths = [p.to_path2d() for p in record.data[0]]
                 holes = [p.to_path2d() for p in record.data[1]]
                 backend.draw_filled_paths(paths, holes, properties)
         backend.finalize()
 
-    def enter_entity(self, entity, properties) -> None:
-        pass
+    def transform(self, m: Matrix44) -> None:
+        """Transforms the recordings inplace by a transformation matrix `m` of type
+        :class:`~ezdxf.math.Matrix44`.
+        """
+        for record in self.records:
+            if record.type == RecordType.FILLED_PATHS:
+                for p in record.data[0]:
+                    p.transform_inplace(m)
+                for p in record.data[1]:
+                    p.transform_inplace(m)
+            else:
+                record.data.transform_inplace(m)
 
-    def exit_entity(self, entity) -> None:
-        pass
+        if self._bbox.has_data:
+            # works for 90-, 180- and 270-degree rotation
+            self._bbox = BoundingBox2d(m.fast_2d_transform(self._bbox.rect_vertices()))
 
-    def clear(self) -> None:
-        raise NotImplementedError()
+    def bbox(self) -> BoundingBox2d:
+        """Returns the bounding box of all records as :class:`~ezdxf.math.BoundingBox2d`."""
+        if not self._bbox.has_data:
+            self.update_bbox()
+        return self._bbox
 
-    def finalize(self) -> None:
-        pass
+    def update_bbox(self) -> None:
+        points: list[AnyVec] = []
+        for record in self.records:
+            try:
+                if record.type == RecordType.FILLED_PATHS:
+                    for path in record.data[0]:  # only add paths, ignore holes
+                        points.extend(path.extents())
+                else:
+                    points.extend(record.data.extents())
+            except npshapes.EmptyShapeError:
+                pass
+        self._bbox = BoundingBox2d(points)
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/text.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/text_renderer.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/text_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/unified_text_renderer.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/unified_text_renderer.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 
     """
 
     def __init__(self) -> None:
         self._font_cache: dict[str, fonts.AbstractFont] = dict()
 
     def get_font(self, font_face: fonts.FontFace) -> fonts.AbstractFont:
+        if not font_face.filename and font_face.family:
+            found = fonts.find_best_match(
+                family=font_face.family,
+                weight=700 if font_face.is_bold else 400,
+                italic=font_face.is_italic,
+            )
+            if found is not None:
+                font_face = found
         key = font_face.filename.lower()
         try:
             return self._font_cache[key]
         except KeyError:
             pass
         abstract_font = fonts.make_font(font_face.filename, 1.0)
         self._font_cache[key] = abstract_font
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/dwg/classes_section.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/dwg/classes_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/dwg/const.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/dwg/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/dwg/crc.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/dwg/crc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/dwg/fileheader.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/dwg/fileheader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/dwg/header_section.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/dwg/header_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/dwg/loader.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/dwg/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/api.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import ezdxf
 from ezdxf.document import Drawing
 from ezdxf import zoom
 
 from .tokenizer import hpgl2_commands
 from .plotter import Plotter
 from .interpreter import Interpreter
-from .backend import Recorder, placement_matrix
+from .backend import Recorder, placement_matrix, Player
 from .dxf_backend import DXFBackend, ColorMode
 from .svg_backend import SVGBackend
 from .pdf_backend import PDFBackend, pdf_is_supported
 
 
 DEBUG = False
 ENTER_HPGL2_MODE = b"%1B"
@@ -93,28 +93,28 @@
     """
     if rotation not in (0, 90, 180, 270):
         raise ValueError("invalid rotation angle: should be 0, 90, 180, or 270")
 
     # 1st pass records output of the plotting commands and detects the bounding box
     doc = ezdxf.new()
     try:
-        recorder = record_plotter_output(b, rotation, sx, sy, merge_control)
+        player = record_plotter_output(b, rotation, sx, sy, merge_control)
     except Hpgl2Error:
         return doc
 
     msp = doc.modelspace()
     dxf_backend = DXFBackend(
         msp,
         color_mode=color_mode,
         map_black_rgb_to_white_rgb=map_black_rgb_to_white_rgb,
     )
     # 2nd pass replays the plotting commands to plot the DXF
-    recorder.replay(dxf_backend)
-    bbox = recorder.bbox()
-    del recorder
+    player.replay(dxf_backend)
+    bbox = player.bbox()
+    del player
 
     if bbox.has_data:  # non-empty page
         zoom.window(msp, bbox.extmin, bbox.extmax)
         _update_doc(doc, bbox)
     return doc
 
 
@@ -163,22 +163,22 @@
     Returns: SVG content as ``str``
 
     """
     if rotation not in (0, 90, 180, 270):
         raise ValueError("invalid rotation angle: should be 0, 90, 180, or 270")
     # 1st pass records output of the plotting commands and detects the bounding box
     try:
-        recorder = record_plotter_output(b, rotation, sx, sy, merge_control)
+        player = record_plotter_output(b, rotation, sx, sy, merge_control)
     except Hpgl2Error:
         return ""
 
     # 2nd pass replays the plotting commands to plot the SVG
-    svg_backend = SVGBackend(recorder.bbox())
-    recorder.replay(svg_backend)
-    del recorder
+    svg_backend = SVGBackend(player.bbox())
+    player.replay(svg_backend)
+    del player
     return svg_backend.get_string()
 
 
 def to_pdf(
     b: bytes,
     *,
     rotation: int = 0,
@@ -213,21 +213,21 @@
         print("Python module PyMuPDF is required: https://pypi.org/project/PyMuPDF/")
         return b""
 
     if rotation not in (0, 90, 180, 270):
         raise ValueError("invalid rotation angle: should be 0, 90, 180, or 270")
     # 1st pass records output of the plotting commands and detects the bounding box
     try:
-        recorder = record_plotter_output(b, rotation, sx, sy, merge_control)
+        player = record_plotter_output(b, rotation, sx, sy, merge_control)
     except Hpgl2Error:
         return b""
     # 2nd pass replays the plotting commands to plot the SVG
-    pdf_backend = PDFBackend(recorder.bbox())
-    recorder.replay(pdf_backend)
-    del recorder
+    pdf_backend = PDFBackend(player.bbox())
+    player.replay(pdf_backend)
+    del player
     return pdf_backend.get_bytes()
 
 
 def print_interpreter_log(interpreter: Interpreter) -> None:
     print("HPGL/2 interpreter log:")
     print(f"unsupported commands: {interpreter.not_implemented_commands}")
     if interpreter.errors:
@@ -238,33 +238,34 @@
 
 def record_plotter_output(
     b: bytes,
     rotation: int,
     sx: float,
     sy: float,
     merge_control: MergeControl,
-) -> Recorder:
+) -> Player:
     commands = hpgl2_commands(b)
     if len(commands) == 0:
         print("HPGL2 data not found.")
         raise Hpgl2DataNotFound
 
     recorder = Recorder()
     plotter = Plotter(recorder)
     interpreter = Interpreter(plotter)
     interpreter.run(commands)
     if DEBUG:
         print_interpreter_log(interpreter)
-    bbox = recorder.bbox()
+    player = recorder.player()
+    bbox = player.bbox()
     if not bbox.has_data:
         raise EmptyDrawing
     m = placement_matrix(bbox, sx, sy, rotation)
-    recorder.transform(m)
+    player.transform(m)
 
     if merge_control == MergeControl.AUTO:
         if plotter.has_merge_control:
             merge_control = MergeControl.LUMINANCE  # type: ignore
     if merge_control == MergeControl.LUMINANCE:
         if DEBUG:
             print("merge control on: sorting filled polygons by luminance")
-        recorder.sort_filled_polygons()
-    return recorder
+        player.sort_filled_polygons()
+    return player
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/backend.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/backend.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
-from typing import Sequence, NamedTuple, Any
+from typing import Sequence, NamedTuple, Any, Iterator
+from typing_extensions import Self
 import abc
+import copy
 import enum
 import math
 from .deps import (
     Vec2,
     Path,
     luminance,
     Matrix44,
@@ -72,77 +74,114 @@
 class DataRecord(NamedTuple):
     type: RecordType
     property_hash: int
     data: Any
 
 
 class Recorder(Backend):
-    """The :class:`Recorder` class records the output of the :class:`Plotter` and
-    can replay this recording on another backend. The class can modify the recorded
-    output.
-    """
+    """The :class:`Recorder` class records the output of the :class:`Plotter` class."""
 
     def __init__(self) -> None:
-        self.records: list[DataRecord] = []
-        self.properties: dict[int, Properties] = {}
+        self._records: list[DataRecord] = []
+        self._properties: dict[int, Properties] = {}
+        self._pens: Sequence[Pen] = []
+
+    def player(self) -> Player:
+        """Returns a :class:`Player` instance with the original recordings. Make a copy
+        of this player to protect the original recordings from being modified::
+
+            safe_player = recorder.player().copy()
+
+        """
+        return Player(self._records, self._properties)
+
+    def draw_polyline(self, properties: Properties, points: Sequence[Vec2]) -> None:
+        self.store(RecordType.POLYLINE, properties, NumpyPoints2d(points))
+
+    def draw_filled_polygon(
+        self, properties: Properties, paths: Sequence[Path]
+    ) -> None:
+        data = tuple(NumpyPath2d(p) for p in paths)
+        self.store(RecordType.FILLED_POLYGON, properties, data)
+
+    def store(self, record_type: RecordType, properties: Properties, args) -> None:
+        prop_hash = properties.hash()
+        if prop_hash not in self._properties:
+            self._properties[prop_hash] = properties.copy()
+        self._records.append(DataRecord(record_type, prop_hash, args))
+        if len(self._pens) != len(properties.pen_table):
+            self._pens = list(properties.pen_table.values())
+
+
+class Player:
+    """This class replays the recordings of the :class:`Recorder` class on another
+    backend. The class can modify the recorded output.
+    """
+    def __init__(self, records: list[DataRecord], properties: dict[int, Properties]):
+        self._records: list[DataRecord] = records
+        self._properties: dict[int, Properties] = properties
         self._bbox = BoundingBox2d()
-        self.pens: Sequence[Pen] = []
+
+    def __copy__(self) -> Self:
+        """Returns a new :class:`Player` instance with a copy of recordings."""
+        records = copy.deepcopy(self._records)
+        player = self.__class__(records, self._properties)
+        player._bbox = self._bbox.copy()
+        return player
+
+    copy = __copy__
+
+    def recordings(self) -> Iterator[tuple[RecordType, Properties, Any]]:
+        """Yields all recordings as [RecordType, Properties, Any] tuples.
+
+        The last field is the data field and depends on :class:`RecordType`:
+
+        - :attr:`RecordType.POLYLINE` returns a :class:`NumpyPoints2d` instance
+        - :attr:`RecordType.FILLED_POLYGON` returns a tuple of :class:`NumpyPath2d` instances
+
+        """
+        props = self._properties
+        for record in self._records:
+            yield record.type, props[record.property_hash], record.data
 
     def bbox(self) -> BoundingBox2d:
         """Returns the bounding box of all recorded polylines and polygons as
         :class:`~ezdxf.math.BoundingBox2d`.
         """
         if not self._bbox.has_data:
             self.update_bbox()
         return self._bbox
 
     def update_bbox(self) -> None:
         points: list[Vec2] = []
-        for record in self.records:
+        for record in self._records:
             if record.type == RecordType.POLYLINE:
                 points.extend(record.data.extents())
             else:
                 for path in record.data:
                     points.extend(path.extents())
         self._bbox = BoundingBox2d(points)
 
-    def draw_polyline(self, properties: Properties, points: Sequence[Vec2]) -> None:
-        self.store(RecordType.POLYLINE, properties, NumpyPoints2d(points))
-
-    def draw_filled_polygon(
-        self, properties: Properties, paths: Sequence[Path]
-    ) -> None:
-        data = tuple(NumpyPath2d(p) for p in paths)
-        self.store(RecordType.FILLED_POLYGON, properties, data)
-
-    def store(self, record_type: RecordType, properties: Properties, args) -> None:
-        prop_hash = properties.hash()
-        if prop_hash not in self.properties:
-            self.properties[prop_hash] = properties.copy()
-        self.records.append(DataRecord(record_type, prop_hash, args))
-        if len(self.pens) != len(properties.pen_table):
-            self.pens = list(properties.pen_table.values())
-
     def replay(self, backend: Backend) -> None:
         """Replay the recording on another backend."""
         current_props = Properties()
-        props = self.properties
-        for record in self.records:
+        props = self._properties
+        for record in self._records:
             current_props = props.get(record.property_hash, current_props)
             if record.type == RecordType.POLYLINE:
                 backend.draw_polyline(current_props, record.data.vertices())
             else:
                 paths = [p.to_path2d() for p in record.data]
                 backend.draw_filled_polygon(current_props, paths)
 
     def transform(self, m: Matrix44) -> None:
         """Transforms the recordings by a transformation matrix `m` of type
         :class:`~ezdxf.math.Matrix44`.
         """
-        for record in self.records:
+        for record in self._records:
             if record.type == RecordType.POLYLINE:
                 record.data.transform_inplace(m)
             else:
                 for path in record.data:
                     path.transform_inplace(m)
 
         if self._bbox.has_data:
@@ -154,27 +193,27 @@
 
         This also changes the plot order in the way that all filled polygons are plotted
         before the polylines.
         """
         polygons = []
         polylines = []
         current = Properties()
-        props = self.properties
-        for record in self.records:
+        props = self._properties
+        for record in self._records:
             if record.type == RecordType.FILLED_POLYGON:
                 current = props.get(record.property_hash, current)
                 key = luminance(current.resolve_fill_color())
                 polygons.append((key, record))
             else:
                 polylines.append(record)
 
         polygons.sort(key=lambda r: r[0], reverse=True)
         records = [sort_rec[1] for sort_rec in polygons]
         records.extend(polylines)
-        self.records = records
+        self._records = records
 
 
 def placement_matrix(
     bbox: BoundingBox2d, sx: float = 1.0, sy: float = 1.0, rotation: float = 0.0
 ) -> Matrix44:
     """Returns a matrix to place the bbox in the first quadrant of the coordinate
     system (+x, +y).
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/compiler.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/compiler.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/deps.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/deps.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/dxf_backend.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/dxf_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/interpreter.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/interpreter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/page.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/page.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/pdf_backend.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/pdf_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/plotter.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/plotter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/polygon_buffer.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/polygon_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/properties.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/svg_backend.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/svg_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/tokenizer.py` & `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/tokenizer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/acad_proxy_entity.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/acad_table.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/acis.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/appdata.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/appid.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/appid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/arc.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/attrib.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/block.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/blockrecord.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/blockrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/boundary_paths.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/circle.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/dictionary.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/dimension.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/dimstyle.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/dimstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/dimstyleoverride.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/dimstyleoverride.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/dxfclass.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/dxfentity.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/dxfgfx.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/dxfgroups.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/dxfns.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/dxfns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/dxfobj.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/ellipse.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/factory.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/geodata.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/geodata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/gradient.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/gradient.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/hatch.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/hatch.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/helix.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/idbuffer.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/idbuffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/image.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/image.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/insert.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/layer.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/layout.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/leader.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/light.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/line.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/ltype.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/lwpolyline.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/lwpolyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/material.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/mesh.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/mleader.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/mline.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/mpolygon.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/mtext.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/mtext_columns.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/objectcollection.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/objectcollection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/oleframe.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/oleframe.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/pattern.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/point.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/polygon.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/polygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/polyline.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/shape.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/solid.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/spline.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/subentity.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/subentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/sun.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/table.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/text.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/textstyle.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/textstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/tolerance.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/ucs.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/underlay.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/view.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/view.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/viewport.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/viewport.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,23 +297,23 @@
         """Thaw `layer_name` in this viewport."""
         index = self._layer_index(layer_name)
         if index != -1:
             del self._frozen_layers[index]
 
     @property
     def is_visible(self) -> bool:
-        # Special VIEWPORT id == 1, this viewport defines the "active viewport"
+        # VIEWPORT id == 1 or status == 1, this viewport defines the "active viewport"
         # which is the area currently shown in the layout tab by the CAD
         # application.
         # BricsCAD set id to -1 if the viewport is off and 'status' (group
         # code 68) is not present.
-        # status: -1 is off-screen, 0 is off
-        if self.dxf.id < 2 or self.dxf.status < 1:
-            return False
-        return True
+        # status: -1= off-screen, 0= off, 1= "active viewport"
+        if self.dxf.hasattr("status"):
+            return self.dxf.status > 0
+        return self.dxf.id > 1
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
         if processor:
             tags = processor.fast_load_dxfattribs(
@@ -594,22 +594,18 @@
             Vec2(cx + width2, cy - height2),
             Vec2(cx + width2, cy + height2),
             Vec2(cx - width2, cy + height2),
         ]
 
     def clipping_rect(self) -> tuple[Vec2, Vec2]:
         """Returns the lower left and the upper right corner of the clipping
-        rectangle.
+        rectangle in paperspace coordinates.
         """
-        center = self.dxf.center
-        cx = center.x
-        cy = center.y
-        width2 = self.dxf.width / 2
-        height2 = self.dxf.height / 2
-        return Vec2(cx - width2, cy - height2), Vec2(cx + width2, cy + height2)
+        corners = self.clipping_rect_corners()
+        return corners[0], corners[2]
 
     @property
     def has_extended_clipping_path(self) -> bool:
         """Returns ``True`` if a non-rectangular clipping path is defined."""
         _flag = self.dxf.flags & const.VSF_NON_RECTANGULAR_CLIPPING
         if _flag:
             handle = self.dxf.clipping_boundary_handle
@@ -626,20 +622,29 @@
 
     @property
     def is_top_view(self) -> bool:
         """Returns ``True`` if the viewport is a top view."""
         view_direction: Vec3 = self.dxf.view_direction_vector
         return view_direction.is_null or view_direction.isclose(Z_AXIS)
 
+    def get_view_center_point(self) -> Vec3:
+        # TODO: Is there a flag or attribute that determines which of these points is
+        #  the center point?
+        center_point = Vec3(self.dxf.view_center_point)
+        if center_point.is_null:
+            center_point = Vec3(self.dxf.view_target_point)
+        return center_point
+
     def get_transformation_matrix(self) -> Matrix44:
-        """Returns the transformation matrix from modelspace to viewport."""
-        # supports only top-view viewports yet!
+        """Returns the transformation matrix from modelspace to paperspace coordinates.
+        """
+        # supports only top-view viewports!
         scale = self.get_scale()
         rotation_angle: float = self.dxf.view_twist_angle
-        msp_center_point: Vec3 = self.dxf.view_center_point
+        msp_center_point: Vec3 = self.get_view_center_point()
         offset: Vec3 = self.dxf.center - (msp_center_point * scale)
         m = Matrix44.scale(scale)
         if rotation_angle:
             m @= Matrix44.z_rotate(math.radians(rotation_angle))
         return m @ Matrix44.translate(offset.x, offset.y, 0)
 
     def get_aspect_ratio(self) -> float:
@@ -651,15 +656,15 @@
         except ZeroDivisionError:
             return 0.0
 
     def get_modelspace_limits(self) -> tuple[float, float, float, float]:
         """Returns the limits of the modelspace to view in drawing units
         as tuple (min_x, min_y, max_x, max_y).
         """
-        msp_center_point: Vec3 = self.dxf.view_center_point
+        msp_center_point: Vec3 = self.get_view_center_point()
         msp_height: float = self.dxf.view_height
         rotation_angle: float = self.dxf.view_twist_angle
         ratio = self.get_aspect_ratio()
         if ratio == 0.0:
             raise ValueError("invalid viewport parameters width or height")
 
         w2 = msp_height * ratio * 0.5
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/visualstyle.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/visualstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/vport.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/vport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/xdata.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/xdict.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/xdict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/xline.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/entities/__init__.py` & `ezdxf-1.1.0b2/src/ezdxf/entities/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/fonts/fonts.py` & `ezdxf-1.1.0b2/src/ezdxf/fonts/fonts.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 import enum
 import logging
 import sys
 import pathlib
 
 from ezdxf import options
 from .font_face import FontFace
-from .font_manager import FontManager, SUPPORTED_TTF_TYPES, FontNotFoundError
+from .font_manager import (
+    FontManager,
+    SUPPORTED_TTF_TYPES,
+    FontNotFoundError,
+    UnsupportedFont,
+)
 from .font_measurements import FontMeasurements
 from .glyphs import GlyphPath, Glyphs
 
 if TYPE_CHECKING:
     from ezdxf.document import Drawing
     from ezdxf.entities import DXFEntity, Textstyle
     from ezdxf.path import Path2d
@@ -234,15 +239,16 @@
     family: str = "sans-serif",
     style: str = "Regular",
     weight: int = 400,
     width: int = 5,
     italic: Optional[bool] = False,
 ) -> Optional[FontFace]:
     """Returns a :class:`FontFace` that matches the given properties best. The search
-    is based the descriptive properties and not on comparing glyph shapes.
+    is based the descriptive properties and not on comparing glyph shapes. Returns
+    ``None`` if no font was found.
 
     Args:
         family: font family name e.g. "sans-serif", "Liberation Sans"
         style: font style e.g. "Regular", "Italic", "Bold"
         weight: weight in the range from 1-1000 (usWeightClass)
         width: width in the range from 1-9 (usWidthClass)
         italic: ``True``, ``False`` or ``None`` to ignore this flag
@@ -504,15 +510,20 @@
         from .ttfonts import TTFontRenderer
 
         key = pathlib.Path(ttf).name.lower()
         try:
             return self._glyph_caches[key]
         except KeyError:
             pass
-        cache = TTFontRenderer(font_manager.get_ttf_font(ttf))
+        try:
+            cache = TTFontRenderer(font_manager.get_ttf_font(ttf))
+        except UnsupportedFont:
+            fallback_font_name = font_manager.fallback_font_name()
+            logger.info(f"replacing unsupported font '{ttf}' by '{fallback_font_name}'")
+            cache = TTFontRenderer(font_manager.get_ttf_font(fallback_font_name))
         self._glyph_caches[key] = cache
         return cache
 
 
 class ShapeFileFont(_CachedFont):
     """Represents a shapefile font (.shx, .shp). Font measurement and glyph rendering is
     done by the ezdxf.fonts.shapefile module. The given cap height and width factor are
@@ -581,36 +592,41 @@
     if font_name == MONOSPACE:
         return MonospaceFont(cap_height, width_factor)
     ext = pathlib.Path(font_name).suffix
     last_resort = MonospaceFont(cap_height, width_factor)
     if ext in SUPPORTED_TTF_TYPES:
         try:
             return TrueTypeFont(font_name, cap_height, width_factor)
-        except FontNotFoundError:
+        except FontNotFoundError as e:
+            logger.warning(f"no default font found: {str(e)}")
             return last_resort
     elif ext == ".shx" or ext == ".shp":
         try:
             return ShapeFileFont(font_name, cap_height, width_factor)
         except FontNotFoundError:
-            pass  # no shape file fonts available
+            pass
+        except UnsupportedFont:
+            # change name - the font exists but is not supported
+            font_name = font_manager.fallback_font_name()
     elif ext == ".lff":
         try:
             return LibreCadFont(font_name, cap_height, width_factor)
         except FontNotFoundError:
-            pass  # no libreCAD fonts available
+            pass
     elif ext == "":  # e.g. "TXT"
         font_face = font_manager.find_best_match(
             family=font_name, style=".shx", italic=None
         )
         if font_face is not None:
             return make_font(font_face.filename, cap_height, width_factor)
     # return default TrueType font
     try:
         return TrueTypeFont(font_name, cap_height, width_factor)
-    except FontNotFoundError:
+    except FontNotFoundError as e:
+        logger.warning(f"no default font found: {str(e)}")
         return last_resort
 
 
 def get_entity_font_face(entity: DXFEntity, doc: Optional[Drawing] = None) -> FontFace:
     """Returns the :class:`FontFace` defined by the associated text style.
     Returns the default font face if the `entity` does not have or support
     the DXF attribute "style". Supports the extended font information stored in
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/fonts/font_face.py` & `ezdxf-1.1.0b2/src/ezdxf/fonts/font_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/fonts/font_manager.py` & `ezdxf-1.1.0b2/src/ezdxf/fonts/font_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pathlib
 from typing import Iterable, NamedTuple, Optional, Sequence
 import os
 import platform
 import json
 
 from pathlib import Path
-from fontTools.ttLib import TTFont
+from fontTools.ttLib import TTFont, TTLibError
 from .font_face import FontFace
 from . import shapefile, lff
 
 WINDOWS = "Windows"
 LINUX = "Linux"
 MACOS = "Darwin"
 
@@ -176,14 +176,33 @@
                 entry.font_face.width,
             )
             for entry in self._cache.values()
         ]
         data = {"version": CURRENT_CACHE_VERSION, "font-faces": faces}
         return json.dumps(data, indent=2)
 
+    def print_available_fonts(self, verbose=False) -> None:
+        for entry in self._cache.values():
+            print(f"{entry.file_path}")
+            if not verbose:
+                continue
+            font_type = entry.file_path.suffix.lower()
+            ff = entry.font_face
+            if font_type in (".shx", ".shp"):
+                print(f"  Shape font file: '{ff.filename}'")
+            elif font_type == ".lff":
+                print(f"  LibreCAD font file: '{ff.filename}'")
+            else:
+                print(f"  TrueType/OpenType font file: '{ff.filename}'")
+                print(f"  family: {ff.family}")
+                print(f"  style: {ff.style}")
+                print(f"  weight: {ff.weight}, {ff.weight_str}")
+                print(f"  width: {ff.width}, {ff.width_str}")
+        print(f"\nfound {len(self._cache)} fonts")
+
 
 def filter_family(family: str, entries: Iterable[CacheEntry]) -> list[CacheEntry]:
     key = str(family).lower()
     return [e for e in entries if e.font_face.family.lower().startswith(key)]
 
 
 def filter_style(style: str, entries: Iterable[CacheEntry]) -> list[CacheEntry]:
@@ -201,25 +220,33 @@
 FALLBACK_LFF = ["standard.lff", "iso.lff", "simplex.lff"]
 
 
 class FontNotFoundError(Exception):
     pass
 
 
+class UnsupportedFont(Exception):
+    pass
+
+
 class FontManager:
     def __init__(self) -> None:
         self.platform = platform.system()
         self._font_cache: FontCache = FontCache()
+        self._match_cache: dict[int, Optional[FontFace]] = dict()
         self._loaded_ttf_fonts: dict[str, TTFont] = dict()
         self._loaded_shape_file_glyph_caches: dict[str, shapefile.GlyphCache] = dict()
         self._loaded_lff_glyph_caches: dict[str, lff.GlyphCache] = dict()
         self._fallback_font_name = ""
         self._fallback_shape_file = ""
         self._fallback_lff = ""
 
+    def print_available_fonts(self, verbose=False) -> None:
+        self._font_cache.print_available_fonts(verbose=verbose)
+
     def has_font(self, font_name: str) -> bool:
         return font_name in self._font_cache
 
     def clear(self) -> None:
         self._font_cache = FontCache()
         self._loaded_ttf_fonts.clear()
         self._fallback_font_name = ""
@@ -270,14 +297,16 @@
         try:
             font = TTFont(
                 self._font_cache.get(font_name, fallback_name).file_path,
                 fontNumber=font_number,
             )
         except IOError as e:
             raise FontNotFoundError(str(e))
+        except TTLibError as e:
+            raise FontNotFoundError(str(e))
         self._loaded_ttf_fonts[font_name] = font
         return font
 
     def ttf_font_from_font_face(self, font_face: FontFace) -> TTFont:
         return self.get_ttf_font(Path(font_face.filename).name)
 
     def get_shapefile_glyph_cache(self, font_name: str) -> shapefile.GlyphCache:
@@ -290,14 +319,16 @@
             file_path = self._font_cache.get(font_name, fallback_name).file_path
         except KeyError:
             raise FontNotFoundError(f"shape font '{font_name}' not found")
         try:
             file = shapefile.readfile(str(file_path))
         except IOError:
             raise FontNotFoundError(f"shape file '{file_path}' not found")
+        except shapefile.UnsupportedShapeFile as e:
+            raise UnsupportedFont(f"unsupported font'{file_path}': {str(e)}")
         glyph_cache = shapefile.GlyphCache(file)
         self._loaded_shape_file_glyph_caches[font_name] = glyph_cache
         return glyph_cache
 
     def get_lff_glyph_cache(self, font_name: str) -> lff.GlyphCache:
         try:
             return self._loaded_lff_glyph_caches[font_name]
@@ -325,15 +356,24 @@
         self,
         family: str = "sans-serif",
         style: str = "Regular",
         weight=400,
         width=5,
         italic: Optional[bool] = False,
     ) -> Optional[FontFace]:
-        return self._font_cache.find_best_match_ex(family, style, weight, width, italic)
+        key = hash((family, style, weight, width, italic))
+        try:
+            return self._match_cache[key]
+        except KeyError:
+            pass
+        font_face = self._font_cache.find_best_match_ex(
+            family, style, weight, width, italic
+        )
+        self._match_cache[key] = font_face
+        return font_face
 
     def find_font_name(self, font_face: FontFace) -> str:
         """Returns the font file name of the font without parent directories
         e.g. "LiberationSans-Regular.ttf".
         """
         font_face = self._font_cache.find_best_match(font_face)  # type: ignore
         if font_face is None:
@@ -359,15 +399,21 @@
         else:
             dirs = FONT_DIRECTORIES.get(self.platform, LINUX_FONT_DIRS)
         self.scan_all(dirs + list(options.support_dirs))
 
     def scan_all(self, folders: Iterable[str]) -> None:
         for folder in folders:
             folder = folder.strip("'\"")  # strip quotes
-            self.scan_folder(Path(folder).expanduser())
+            if not folder:
+                continue
+            try:
+                self.scan_folder(Path(folder).expanduser())
+            except PermissionError as e:
+                print(str(e))
+                continue
 
     def scan_folder(self, folder: Path):
         if not folder.exists():
             return
         for file in folder.iterdir():
             if file.is_dir():
                 self.scan_folder(file)
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/fonts/font_measurements.py` & `ezdxf-1.1.0b2/src/ezdxf/fonts/font_measurements.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/fonts/glyphs.py` & `ezdxf-1.1.0b2/src/ezdxf/fonts/glyphs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/fonts/lff.py` & `ezdxf-1.1.0b2/src/ezdxf/fonts/lff.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/fonts/shapefile.py` & `ezdxf-1.1.0b2/src/ezdxf/fonts/shapefile.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/fonts/ttfonts.py` & `ezdxf-1.1.0b2/src/ezdxf/fonts/ttfonts.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #  License: MIT License
 from __future__ import annotations
 from typing import Any, no_type_check
 from fontTools.pens.basePen import BasePen
 from fontTools.ttLib import TTFont
 
 from ezdxf.math import Matrix44, UVec, BoundingBox2d
-from .font_manager import FontManager
+from .font_manager import FontManager, UnsupportedFont
 from .font_measurements import FontMeasurements
 from .glyphs import GlyphPath, Glyphs
 
 UNICODE_WHITE_SQUARE = 9633  # U+25A1
 UNICODE_REPLACEMENT_CHAR = 65533  # U+FFFD
 
 font_manager = FontManager()
@@ -71,14 +71,16 @@
 class TTFontRenderer(Glyphs):
     def __init__(self, font: TTFont, kerning=False):
         self._glyph_path_cache: dict[str, GlyphPath] = dict()
         self._generic_glyph_cache: dict[str, Any] = dict()
         self._glyph_width_cache: dict[str, float] = dict()
         self.font = font
         self.cmap = self.font.getBestCmap()
+        if self.cmap is None:
+            raise UnsupportedFont(f"font '{self.font_name}' has no character map.")
         self.glyph_set = self.font.getGlyphSet()
         self.kerning = NoKerning()
         if kerning:
             try:
                 self.kerning = KerningTable(self.font, self.cmap)
             except KeyError:  # kerning table does not exist
                 pass
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/layouts/base.py` & `ezdxf-1.1.0b2/src/ezdxf/layouts/base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/layouts/blocklayout.py` & `ezdxf-1.1.0b2/src/ezdxf/layouts/blocklayout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/layouts/layout.py` & `ezdxf-1.1.0b2/src/ezdxf/layouts/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,14 +265,25 @@
         dxf = self.dxf_layout.dxf
         dxf.plot_window_x1 = x1
         dxf.plot_window_y1 = y1
         dxf.plot_window_x2 = x2
         dxf.plot_window_y2 = y2
         self.set_plot_type(4)
 
+    def get_plot_unit_scale_factor(self) -> float:
+        denom = self.dxf.scale_denominator
+        numerator = self.dxf.scale_numerator
+        scale = 1.0
+        if denom:
+            scale = numerator / denom
+        if self.dxf.plot_paper_units == 1:
+            return scale  # mm
+        else:
+            return scale * 25.4  # inch
+
     # plot layout flags setter
     def plot_viewport_borders(self, state: bool = True) -> None:
         self.set_plot_flags(self.PLOT_VIEWPORT_BORDERS, state)
 
     def show_plot_styles(self, state: bool = True) -> None:
         self.set_plot_flags(self.SHOW_PLOT_STYLES, state)
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf/layouts/layouts.py` & `ezdxf-1.1.0b2/src/ezdxf/layouts/layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/lldxf/attributes.py` & `ezdxf-1.1.0b2/src/ezdxf/lldxf/attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/lldxf/const.py` & `ezdxf-1.1.0b2/src/ezdxf/lldxf/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/lldxf/encoding.py` & `ezdxf-1.1.0b2/src/ezdxf/lldxf/encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/lldxf/extendedtags.py` & `ezdxf-1.1.0b2/src/ezdxf/lldxf/extendedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/lldxf/fileindex.py` & `ezdxf-1.1.0b2/src/ezdxf/lldxf/fileindex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/lldxf/hdrvars.py` & `ezdxf-1.1.0b2/src/ezdxf/lldxf/hdrvars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/lldxf/loader.py` & `ezdxf-1.1.0b2/src/ezdxf/lldxf/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/lldxf/packedtags.py` & `ezdxf-1.1.0b2/src/ezdxf/lldxf/packedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/lldxf/repair.py` & `ezdxf-1.1.0b2/src/ezdxf/lldxf/repair.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/lldxf/tagger.py` & `ezdxf-1.1.0b2/src/ezdxf/lldxf/tagger.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/lldxf/tags.py` & `ezdxf-1.1.0b2/src/ezdxf/lldxf/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/lldxf/tagwriter.py` & `ezdxf-1.1.0b2/src/ezdxf/lldxf/tagwriter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/lldxf/types.py` & `ezdxf-1.1.0b2/src/ezdxf/lldxf/types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/lldxf/validator.py` & `ezdxf-1.1.0b2/src/ezdxf/lldxf/validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/arc.py` & `ezdxf-1.1.0b2/src/ezdxf/math/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/bbox.py` & `ezdxf-1.1.0b2/src/ezdxf/math/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/bezier.py` & `ezdxf-1.1.0b2/src/ezdxf/math/bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/bezier_interpolation.py` & `ezdxf-1.1.0b2/src/ezdxf/math/bezier_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/box.py` & `ezdxf-1.1.0b2/src/ezdxf/math/box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/bspline.py` & `ezdxf-1.1.0b2/src/ezdxf/math/bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/bulge.py` & `ezdxf-1.1.0b2/src/ezdxf/math/bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/circle.py` & `ezdxf-1.1.0b2/src/ezdxf/math/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/clipping.py` & `ezdxf-1.1.0b2/src/ezdxf/math/clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/clustering.py` & `ezdxf-1.1.0b2/src/ezdxf/math/clustering.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/construct2d.py` & `ezdxf-1.1.0b2/src/ezdxf/math/construct2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/construct3d.py` & `ezdxf-1.1.0b2/src/ezdxf/math/construct3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/cspline.py` & `ezdxf-1.1.0b2/src/ezdxf/math/cspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/curvetools.py` & `ezdxf-1.1.0b2/src/ezdxf/math/curvetools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/ellipse.py` & `ezdxf-1.1.0b2/src/ezdxf/math/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/eulerspiral.py` & `ezdxf-1.1.0b2/src/ezdxf/math/eulerspiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/linalg.py` & `ezdxf-1.1.0b2/src/ezdxf/math/linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/line.py` & `ezdxf-1.1.0b2/src/ezdxf/math/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/offset2d.py` & `ezdxf-1.1.0b2/src/ezdxf/math/offset2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/parametrize.py` & `ezdxf-1.1.0b2/src/ezdxf/math/parametrize.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/perlin.py` & `ezdxf-1.1.0b2/src/ezdxf/math/perlin.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/polyline.py` & `ezdxf-1.1.0b2/src/ezdxf/math/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/rtree.py` & `ezdxf-1.1.0b2/src/ezdxf/math/rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/shape.py` & `ezdxf-1.1.0b2/src/ezdxf/math/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/surfaces.py` & `ezdxf-1.1.0b2/src/ezdxf/math/surfaces.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/transformtools.py` & `ezdxf-1.1.0b2/src/ezdxf/math/transformtools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/triangulation.py` & `ezdxf-1.1.0b2/src/ezdxf/math/triangulation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/ucs.py` & `ezdxf-1.1.0b2/src/ezdxf/math/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/_bezier3p.py` & `ezdxf-1.1.0b2/src/ezdxf/math/_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/_bezier4p.py` & `ezdxf-1.1.0b2/src/ezdxf/math/_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/_bspline.py` & `ezdxf-1.1.0b2/src/ezdxf/math/_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/_construct.py` & `ezdxf-1.1.0b2/src/ezdxf/math/_construct.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/_ctypes.py` & `ezdxf-1.1.0b2/src/ezdxf/math/_ctypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/_mapbox_earcut.py` & `ezdxf-1.1.0b2/src/ezdxf/math/_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/_matrix44.py` & `ezdxf-1.1.0b2/src/ezdxf/math/_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/_vector.py` & `ezdxf-1.1.0b2/src/ezdxf/math/_vector.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/math/__init__.py` & `ezdxf-1.1.0b2/src/ezdxf/math/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/path/commands.py` & `ezdxf-1.1.0b2/src/ezdxf/path/commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/path/converter.py` & `ezdxf-1.1.0b2/src/ezdxf/path/converter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/path/nesting.py` & `ezdxf-1.1.0b2/src/ezdxf/path/nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/path/path.py` & `ezdxf-1.1.0b2/src/ezdxf/path/path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/path/shapes.py` & `ezdxf-1.1.0b2/src/ezdxf/path/shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/path/tools.py` & `ezdxf-1.1.0b2/src/ezdxf/path/tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.css` & `ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.css`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.html` & `ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.html`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.js` & `ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.js`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.py` & `ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/pp/pprint.py` & `ezdxf-1.1.0b2/src/ezdxf/pp/pprint.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.css` & `ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.css`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.py` & `ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/pp/reflinks.py` & `ezdxf-1.1.0b2/src/ezdxf/pp/reflinks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/abstract_mtext_renderer.py` & `ezdxf-1.1.0b2/src/ezdxf/render/abstract_mtext_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/arrows.py` & `ezdxf-1.1.0b2/src/ezdxf/render/arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/curves.py` & `ezdxf-1.1.0b2/src/ezdxf/render/curves.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/dimension.py` & `ezdxf-1.1.0b2/src/ezdxf/render/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/dim_base.py` & `ezdxf-1.1.0b2/src/ezdxf/render/dim_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/dim_curved.py` & `ezdxf-1.1.0b2/src/ezdxf/render/dim_curved.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/dim_diameter.py` & `ezdxf-1.1.0b2/src/ezdxf/render/dim_diameter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/dim_linear.py` & `ezdxf-1.1.0b2/src/ezdxf/render/dim_linear.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/dim_ordinate.py` & `ezdxf-1.1.0b2/src/ezdxf/render/dim_ordinate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/dim_radius.py` & `ezdxf-1.1.0b2/src/ezdxf/render/dim_radius.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/forms.py` & `ezdxf-1.1.0b2/src/ezdxf/render/forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/hatching.py` & `ezdxf-1.1.0b2/src/ezdxf/render/hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/leader.py` & `ezdxf-1.1.0b2/src/ezdxf/render/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/linetypes.py` & `ezdxf-1.1.0b2/src/ezdxf/render/linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/mesh.py` & `ezdxf-1.1.0b2/src/ezdxf/render/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/mleader.py` & `ezdxf-1.1.0b2/src/ezdxf/render/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/mline.py` & `ezdxf-1.1.0b2/src/ezdxf/render/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/point.py` & `ezdxf-1.1.0b2/src/ezdxf/render/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/polyline.py` & `ezdxf-1.1.0b2/src/ezdxf/render/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/r12spline.py` & `ezdxf-1.1.0b2/src/ezdxf/render/r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/trace.py` & `ezdxf-1.1.0b2/src/ezdxf/render/trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/_linetypes.py` & `ezdxf-1.1.0b2/src/ezdxf/render/_linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/render/__init__.py` & `ezdxf-1.1.0b2/src/ezdxf/render/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/16x16.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/16x16.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/24x24.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/24x24.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/256x256.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/256x256.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/32x32.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/32x32.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/48x48.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/48x48.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/64x64.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/64x64.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/icon-copy-64px.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/icon-copy-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/icon-find-64px.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/icon-find-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-bookmark-64px.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-handle-64px.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-handle-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-line-64px.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-line-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/icon-left-arrow-64px.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/icon-left-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/icon-next-entity-64px.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/icon-next-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/icon-prev-entity-64px.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/icon-prev-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/icon-right-arrow-64px.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/icon-right-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/icon-show-in-tree-64px.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/icon-show-in-tree-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/resources/icon-store-bookmark-64px.png` & `ezdxf-1.1.0b2/src/ezdxf/resources/icon-store-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/sections/acdsdata.py` & `ezdxf-1.1.0b2/src/ezdxf/sections/acdsdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/sections/blocks.py` & `ezdxf-1.1.0b2/src/ezdxf/sections/blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/sections/classes.py` & `ezdxf-1.1.0b2/src/ezdxf/sections/classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/sections/entities.py` & `ezdxf-1.1.0b2/src/ezdxf/sections/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/sections/header.py` & `ezdxf-1.1.0b2/src/ezdxf/sections/header.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/sections/headervars.py` & `ezdxf-1.1.0b2/src/ezdxf/sections/headervars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/sections/objects.py` & `ezdxf-1.1.0b2/src/ezdxf/sections/objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/sections/table.py` & `ezdxf-1.1.0b2/src/ezdxf/sections/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/sections/tables.py` & `ezdxf-1.1.0b2/src/ezdxf/sections/tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/binarydata.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/binarydata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/codepage.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/codepage.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/complex_ltype.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/complex_ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/crypt.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/debug.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/debug.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/difftags.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/handle.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/indexing.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/juliandate.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/pattern.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/rawloader.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/rawloader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/standards.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/standards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/strip.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/strip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/test.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/test.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/text.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/text_layout.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/text_size.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/zipmanager.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/zipmanager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/_iso_pattern.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/_iso_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf/tools/__init__.py` & `ezdxf-1.1.0b2/src/ezdxf/tools/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/src/ezdxf.egg-info/PKG-INFO` & `ezdxf-1.1.0b2/src/ezdxf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.1.0b1
+Version: 1.1.0b2
 Summary: A Python package to create/manipulate DXF drawings.
 Home-page: https://ezdxf.mozman.at
 Author: Manfred Moitzi
 Author-email: me@mozman.at
 License: MIT License
 Download-URL: https://pypi.org/project/ezdxf/
 Keywords: DXF,CAD
@@ -211,29 +211,30 @@
 Feedback is greatly appreciated.
 
 Manfred
 
 News
 ====
 
-Version 1.1.0b0 - dev
+Version 1.1.0b2 - dev
 ---------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-1.html
 - WARNING: The font support changed drastically in this version, if you use the 
   `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
   v1.0.3 in your `requirements.txt` file to use the previous version!
 - NEW: `numpy` is a hard dependency, requires Python version >= 3.8
 - NEW: `fontTools` is a hard dependency
 - NEW: `ezdxf.path.Path2d()` class, `Path` class with `Vec2` vertices
 - NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
-- NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG
-- NEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF
-- NEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG
-- NEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF
+- NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF, SVG, PDF, PNG
+- NEW: `ezdxf hpgl` command to view and/or convert HPGL/2 plot files to various formats: DXF, SVG, PDF
+- NEW: native `SVG` backend for the `drawing` add-on
+- NEW: `ColorPolicy` and `BackgroundPolicy` configuration settings for the `drawing` 
+  add-on to change/override foreground- and background color by the frontend 
 - NEW: support for measuring and rendering of .shx, .shp and .lff fonts, the basic 
   stroke fonts included in CAD applications
 - NEW: added setter to `BlockLayout.base_point` property
 - CHANGED: moved font related modules into a new subpackage `ezdxf.fonts` 
   including a big refactoring
 - CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
   renamed to `width` and is also an int value (1-9) now
```

## Comparing `ezdxf-1.1.0b1/src/ezdxf.egg-info/SOURCES.txt` & `ezdxf-1.1.0b2/src/ezdxf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 integration_tests/test_document_guid.py
 integration_tests/test_document_page_setup.py
 integration_tests/test_dxf_info_scanning.py
 integration_tests/test_entities_iterator.py
 integration_tests/test_fix_dulicate_handles.py
 integration_tests/test_geo.py
 integration_tests/test_groups.py
+integration_tests/test_hpgl2_addon.py
 integration_tests/test_ignore_junk_beyond_EOF.py
 integration_tests/test_launcher.py
 integration_tests/test_leica_disto_r12.py
 integration_tests/test_load_dxf_unicode_notation.py
 integration_tests/test_mapbox_earcut.py
 integration_tests/test_mtext_columns.py
 integration_tests/test_mtext_explode_addon.py
@@ -52,14 +53,15 @@
 integration_tests/test_write_fixed_meta_data.py
 integration_tests/test_write_without_handles.py
 integration_tests/test_xref_detach.py
 integration_tests/data/AC1003_LINE_Example.dxf
 integration_tests/data/ASCII_R12.dxf
 integration_tests/data/Leica_Disto_S910.dxf
 integration_tests/data/MODEL.dxf
+integration_tests/data/PLOTFILE.plt
 integration_tests/data/POLI-ALL210_12.DXF
 integration_tests/data/R12_with_trash_beyond_EOF.dxf
 integration_tests/data/XRECORD_0.bin
 integration_tests/data/XRECORD_1.bin
 integration_tests/data/XRECORD_2.bin
 integration_tests/data/acad_table_with_blk_ref.dxf
 integration_tests/data/bin_dxf_r12.dxf
@@ -175,14 +177,15 @@
 src/ezdxf/addons/openscad.py
 src/ezdxf/addons/pycsg.py
 src/ezdxf/addons/r12export.py
 src/ezdxf/addons/r12writer.py
 src/ezdxf/addons/sierpinski_pyramid.py
 src/ezdxf/addons/tablepainter.py
 src/ezdxf/addons/text2path.py
+src/ezdxf/addons/xplayer.py
 src/ezdxf/addons/xqt.py
 src/ezdxf/addons/acisbrowser/__init__.py
 src/ezdxf/addons/acisbrowser/browser.py
 src/ezdxf/addons/acisbrowser/data.py
 src/ezdxf/addons/browser/__init__.py
 src/ezdxf/addons/browser/bookmarks.py
 src/ezdxf/addons/browser/browser.py
@@ -196,20 +199,22 @@
 src/ezdxf/addons/drawing/backend.py
 src/ezdxf/addons/drawing/clipper.py
 src/ezdxf/addons/drawing/config.py
 src/ezdxf/addons/drawing/debug_backend.py
 src/ezdxf/addons/drawing/debug_utils.py
 src/ezdxf/addons/drawing/frontend.py
 src/ezdxf/addons/drawing/gfxproxy.py
+src/ezdxf/addons/drawing/layout.py
 src/ezdxf/addons/drawing/matplotlib.py
 src/ezdxf/addons/drawing/mtext_complex.py
 src/ezdxf/addons/drawing/properties.py
 src/ezdxf/addons/drawing/pyqt.py
 src/ezdxf/addons/drawing/qtviewer.py
 src/ezdxf/addons/drawing/recorder.py
+src/ezdxf/addons/drawing/svg.py
 src/ezdxf/addons/drawing/text.py
 src/ezdxf/addons/drawing/text_renderer.py
 src/ezdxf/addons/drawing/type_hints.py
 src/ezdxf/addons/drawing/unified_text_renderer.py
 src/ezdxf/addons/dwg/__init__.py
 src/ezdxf/addons/dwg/classes_section.py
 src/ezdxf/addons/dwg/const.py
@@ -227,14 +232,15 @@
 src/ezdxf/addons/hpgl2/page.py
 src/ezdxf/addons/hpgl2/pdf_backend.py
 src/ezdxf/addons/hpgl2/plotter.py
 src/ezdxf/addons/hpgl2/polygon_buffer.py
 src/ezdxf/addons/hpgl2/properties.py
 src/ezdxf/addons/hpgl2/svg_backend.py
 src/ezdxf/addons/hpgl2/tokenizer.py
+src/ezdxf/addons/hpgl2/viewer.py
 src/ezdxf/entities/__init__.py
 src/ezdxf/entities/acad_proxy_entity.py
 src/ezdxf/entities/acad_table.py
 src/ezdxf/entities/acis.py
 src/ezdxf/entities/appdata.py
 src/ezdxf/entities/appid.py
 src/ezdxf/entities/arc.py
@@ -774,18 +780,21 @@
 tests/test_08_addons/test_817_genetic_algorithm.py
 tests/test_08_addons/test_818_meshex.py
 tests/test_08_addons/test_819_menger_sponge.py
 tests/test_08_addons/test_820_openscad.py
 tests/test_08_addons/test_821_hpgl2.py
 tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
 tests/test_08_addons/test_822_clipper.py
+tests/test_08_addons/test_823_drawing_layout.py
+tests/test_08_addons/test_824_svg_drawing_backend.py
 tests/test_09_cython_acceleration/test_901_acc_vec2.py
 tests/test_09_cython_acceleration/test_902_acc_vec3.py
 tests/test_09_cython_acceleration/test_903_acc_matrix44.py
 tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
 tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
 tests/test_09_cython_acceleration/test_906_acc_bspline.py
 tests/test_10_issues/test_issue_414_bbox_calculation.py
 tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
 tests/test_10_issues/test_issue_574_flattening_error.py
 tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
-tests/test_10_issues/test_issue_749_text_layout.py
+tests/test_10_issues/test_issue_749_text_layout.py
+tests/test_10_issues/test_issue_873_circle_inverted_normal.py
```

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_010_binary_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_012_crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_013_juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_016_encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_018_handle.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_018_handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_024_render_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_040_tags.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_040_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_041_group_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py` & `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_101_dxfnamespace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_102_appdata.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_102_appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_103_reactors.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_103_reactors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_104_extension_dict.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_104_extension_dict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_105_xdata.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_105_xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_110_dxfentity.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_110_dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_112a_dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_112b_dxfobj.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_112b_dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_113_dxfclass.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_113_dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_114_factory.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_114_factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_115_new_empty_drawing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_116_dictionary.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_116_dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_117_layer_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_119_ucs_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_120_style_table_entry.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_120_style_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_121_ltype_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_123_view_table_entry.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_123_view_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_125_image_def.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_125_image_def.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_126_image_def_reactor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_127_raster_variables.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_127_raster_variables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_128_pdf_definition.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_128_pdf_definition.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_129_xrecord.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_129_xrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_130_id_buffer.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_130_id_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_131_field_list.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_131_field_list.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_132_layer_filter.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_132_layer_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_133_sun.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_133_sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_134_material.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_134_material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_135_geo_data.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_135_geo_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_136_vba_project.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_136_vba_project.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_137_sortentstable.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_137_sortentstable.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_138_setup_visual_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_139_user_record.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_139_user_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_140_block_record.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_140_block_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py` & `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_141_layer_vp_override.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/conftest.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_200_line.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_200_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_201_point.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_201_point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_202_circle.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_202_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_203_arc.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_203_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_204_shape.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_204_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_205_solid.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_205_solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_206_text.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_206_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_207_attdef.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_207_attdef.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_208_attrib.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_208_attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_209_vertex.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_209_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_1.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_2.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_211_viewport.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_211_viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_212_insert.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_212_insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_213_minsert.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_213_minsert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_214_block.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_214_block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_215_dimension.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_215_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_216_dimlines_R12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_221_ellipse.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_221_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_222_xline.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_222_xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_223_ray.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_223_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_224_group.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_224_group.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_225_mtext.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_225_mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_226_spline.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_226_spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_228_mesh.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_228_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229b_hatch_extended.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_231_underlay.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_231_underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_231_underlay_2.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_231_underlay_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_acis.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_acis_2.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_acis_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_surface.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_surface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_233_helix.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_233_helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_234_light.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_234_light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_235_leader.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_235_leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_236_multileader.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_236_multileader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_237_mline.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_237_mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_238_tolerance.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_238_tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_239_proxy_graphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_240_arc_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_241_hyperlink.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_241_hyperlink.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_242_random_transform.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_242_random_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_243_replace_entity.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_243_replace_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_245_wipeout.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_245_wipeout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_246_spline_audit.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_246_spline_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_248_mpolygon.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_248_mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_249_boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_251_upright.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_251_upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_253_ole2frame.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_253_ole2frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_254_get_font_name.py` & `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_254_get_font_name.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_300_layout.py` & `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_300_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py` & `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_302_block_references.py` & `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_302_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py` & `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_303_auto_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py` & `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_304_new_entity_space.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py` & `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py` & `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_307_groupby.py` & `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_307_groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_308_query.py` & `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_308_query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_309_query_parser.py` & `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_309_query_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py` & `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py` & `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_312_virtual_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_313_redraw_order.py` & `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_313_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_401_headersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_402_classessection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_403_entity_database.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_404a_tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_405_classes.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_405_classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_407_entity_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_408_objects_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_409_create_objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_410_table.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_410_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_411_acds_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_415_layout_management.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_417_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_424_audit.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_424_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_427_appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py` & `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/conftest.py` & `ezdxf-1.1.0b2/tests/test_05_tools/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_500_units.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_500_units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_501_truecolor.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_501_truecolor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_502_raw_color.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_502_raw_color.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_503_indexing.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_503_indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_504_suppress_zeros.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_504_suppress_zeros.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_507_dxf_pretty_printer.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_507_dxf_pretty_printer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_508_read_zip.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_508_read_zip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_509_comments.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_509_comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_510_byte_stream.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_510_byte_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_511_bit_stream.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_511_bit_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_512_pattern.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_512_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_513_reorder_entities.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_513_reorder_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_514_text.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_514_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_515a_fonts_truetype.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_515a_fonts_truetype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_515b_fonts_shapefiles.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_515b_fonts_shapefiles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_515c_fonts_lff.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_515c_fonts_lff.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_516_zoom.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_516_zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_517_text_layout.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_517_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_519_mtext_editor.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_519_mtext_editor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_520_mtext_context.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_520_mtext_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_521_mtext_parser.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_521_mtext_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_522_text_scanner.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_522_text_scanner.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_523_text_size.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_523_text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_524_block_reference_manager.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_524_block_reference_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_525_transparency.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_525_transparency.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_526_explode.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_526_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_527_gfxattribs.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_527_gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_528_difftags.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_528_difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_529_acis_sat.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_529_acis_sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_530_acis_sab.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_530_acis_sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_531_acis_entities.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_531_acis_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_532_acis_mesh.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_532_acis_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_533_shapefiles.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_533_shapefiles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_534_dwg_info.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_534_dwg_info.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_535_xref_basic.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_535_xref_basic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_536_xref_conflict.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_536_xref_conflict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_537_transform.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_537_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_538_scale_mtext_inline_commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_539_npshapes.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_539_npshapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_05_tools/test_540_lff_parser.py` & `ezdxf-1.1.0b2/tests/test_05_tools/test_540_lff_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/conftest.py` & `ezdxf-1.1.0b2/tests/test_06_math/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_600_base.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_600_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_601_bulge.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_601_bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_602_vec3.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_602_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_603_vec2.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_603_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_604_banded_matrix.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_604_banded_matrix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_604_linalg.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_604_linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_605_matrix44.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_605_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_606_convexhull.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_606_convexhull.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_607_perlin_noise.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_607_perlin_noise.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_608_intersection_line_line_2d.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_608_intersection_line_line_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_609_point_on_line.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_609_point_on_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_610_ocs.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_610_ocs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_611_ucs.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_611_ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_612_ucs_pass_trough.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_612_ucs_pass_trough.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_613_point_in_poygon.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_613_point_in_poygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_614_construct_3d.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_614_construct_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_615_rytz_axis.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_615_rytz_axis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_616_plane.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_616_plane.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_617_clockwise_orientation.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_617_clockwise_orientation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_618_clipping.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_618_clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_619_greiner_hormann.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_619_greiner_hormann.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_620_knot.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_620_knot.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_621_bspline.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_621_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_622_bsplineu.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_622_bsplineu.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_623_rbspline.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_623_rbspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_624_global_bspline_interpolation.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_624_global_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_626_local_bspline_interpolation.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_626_local_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_627_bspline_basis.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_627_bspline_basis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_629_bezier.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_629_bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_630a_bezier4p_base.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_630a_bezier4p_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_630b_bezier4p_functions.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_630b_bezier4p_functions.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_631_euler_spiral.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_631_euler_spiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_632_bezier3p.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_632_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_640_bbox.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_640_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_641_construction_ray.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_641_construction_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_642_construction_line.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_642_construction_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_643_construction_box.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_643_construction_box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_644_construction_circle.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_644_construction_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_645_construction_arc.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_645_construction_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_646_offset_vertices_2d.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_646_offset_vertices_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_647_transform_tools.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_647_transform_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_648_construction_ellipse.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_648_construction_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_650_elliptic_arc_span.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_650_elliptic_arc_span.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_651_construction_polyline.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_651_construction_polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_652_approx_param_t.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_652_approx_param_t.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_653_polyline_intersection.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_653_polyline_intersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_654_rtree.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_654_rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_655_dbscan.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_655_dbscan.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_656_k_means.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_656_k_means.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_657_mapbox_earcut.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_657_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_658_bevel_tools.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_658_bevel_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_659_intersection_line_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_660_intersection_ray_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_06_math/test_662_is_convex_polygon_2d.py` & `ezdxf-1.1.0b2/tests/test_06_math/test_662_is_convex_polygon_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_701_arrows.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_701_arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_702_render_forms.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_702_render_forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_703_mesh_builder.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_703_mesh_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_704_render_linear_dimension.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_704_render_linear_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_705_shape.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_705_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_707_trace.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_707_trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_708a_path.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_708a_path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_708b_path_tools.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_708b_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_708c_matplotlib_path_tools.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_708c_matplotlib_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_708d_qpainter_path_tools.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_708d_qpainter_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_708e_path_shapes.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_708e_path_shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_708f_path_nesting.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_708f_path_nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_709_linetype_renderer.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_709_linetype_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_711_points.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_711_points.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_712_render_curved_dimension.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_712_render_curved_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_713_mleader_builder.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_713_mleader_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_714_mleader_render_engine.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_714_mleader_render_engine.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_715_hatching.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_715_hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py` & `ezdxf-1.1.0b2/tests/test_07_render/test_715_issue_747_explode_3d_dim.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_800_mtext_surrogate.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_800_mtext_surrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_801_r12spline.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_801_r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_802_table_painter.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_802_table_painter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_803_entities_to_code.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_803_entities_to_code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_804_importer.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_804_importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_805_pycsg.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_805_pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_806_acadctb.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_806_acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_807_dwg_loader_basics.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_807_dwg_loader_basics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_810_drawing_properties.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_810_drawing_properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_811a_drawing_frontend.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_811a_drawing_frontend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_812_drawing_graphic_proxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_813_geo_interface.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_813_geo_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_814_text2path.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_814_text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_815_dxf_browser.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_815_dxf_browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_816_bin_packing.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_816_bin_packing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_817_genetic_algorithm.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_817_genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_818_meshex.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_818_meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_819_menger_sponge.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_819_menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_820_openscad.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_820_openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_821_hpgl2.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_821_hpgl2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_08_addons/test_822_clipper.py` & `ezdxf-1.1.0b2/tests/test_08_addons/test_822_clipper.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py` & `ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_901_acc_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py` & `ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_902_acc_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py` & `ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_903_acc_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py` & `ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py` & `ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py` & `ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_906_acc_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_10_issues/test_issue_414_bbox_calculation.py` & `ezdxf-1.1.0b2/tests/test_10_issues/test_issue_414_bbox_calculation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py` & `ezdxf-1.1.0b2/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_10_issues/test_issue_574_flattening_error.py` & `ezdxf-1.1.0b2/tests/test_10_issues/test_issue_574_flattening_error.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py` & `ezdxf-1.1.0b2/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b1/tests/test_10_issues/test_issue_749_text_layout.py` & `ezdxf-1.1.0b2/tests/test_10_issues/test_issue_749_text_layout.py`

 * *Files identical despite different names*

