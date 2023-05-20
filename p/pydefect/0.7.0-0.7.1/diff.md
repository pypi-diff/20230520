# Comparing `tmp/pydefect-0.7.0.tar.gz` & `tmp/pydefect-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydefect-0.7.0.tar", last modified: Wed Jan  4 05:29:11 2023, max compression
+gzip compressed data, was "dist/pydefect-0.7.1.tar", last modified: Sat May 20 00:06:15 2023, max compression
```

## Comparing `pydefect-0.7.0.tar` & `pydefect-0.7.1.tar`

### file list

```diff
@@ -1,218 +1,272 @@
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:11.140972 pydefect-0.7.0/
--rw-r--r--   0 kumagai    (501) staff       (20)       54 2021-03-12 02:40:59.000000 pydefect-0.7.0/MANIFEST.in
--rw-r--r--   0 kumagai    (501) staff       (20)      397 2023-01-04 05:29:11.140474 pydefect-0.7.0/PKG-INFO
--rw-r--r--   0 kumagai    (501) staff       (20)     4563 2022-08-17 09:42:29.000000 pydefect-0.7.0/README.md
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.816954 pydefect-0.7.0/pydefect/
--rw-r--r--   0 kumagai    (501) staff       (20)       21 2023-01-04 05:28:36.000000 pydefect-0.7.0/pydefect/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.846063 pydefect-0.7.0/pydefect/analyzer/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.0/pydefect/analyzer/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2840 2021-04-02 01:38:50.000000 pydefect-0.7.0/pydefect/analyzer/_defect_charge_distribution.py
--rw-r--r--   0 kumagai    (501) staff       (20)    11522 2022-12-13 08:07:02.000000 pydefect-0.7.0/pydefect/analyzer/band_edge_states.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1334 2021-05-01 01:17:09.000000 pydefect-0.7.0/pydefect/analyzer/calc_results.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2426 2021-05-26 07:04:12.000000 pydefect-0.7.0/pydefect/analyzer/calc_summary.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.858220 pydefect-0.7.0/pydefect/analyzer/dash_components/
--rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-08-21 04:26:43.000000 pydefect-0.7.0/pydefect/analyzer/dash_components/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5094 2021-08-15 04:39:32.000000 pydefect-0.7.0/pydefect/analyzer/dash_components/cpd_energy_dash.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1754 2021-05-27 10:09:51.000000 pydefect-0.7.0/pydefect/analyzer/dash_components/cpd_energy_dash_demo.py
--rw-r--r--   0 kumagai    (501) staff       (20)      929 2021-05-27 09:07:43.000000 pydefect-0.7.0/pydefect/analyzer/dash_components/cpd_plotter_main.py
--rw-r--r--   0 kumagai    (501) staff       (20)     8866 2021-04-04 05:43:59.000000 pydefect-0.7.0/pydefect/analyzer/dash_components/main.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6859 2021-04-04 05:43:59.000000 pydefect-0.7.0/pydefect/analyzer/dash_components/scenes_from_volumetric_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4716 2021-08-06 10:14:07.000000 pydefect-0.7.0/pydefect/analyzer/defect_charge_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)    11874 2022-12-08 06:24:14.000000 pydefect-0.7.0/pydefect/analyzer/defect_energy.py
--rw-r--r--   0 kumagai    (501) staff       (20)     9898 2022-11-19 05:32:10.000000 pydefect-0.7.0/pydefect/analyzer/defect_energy_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1280 2022-11-15 04:48:53.000000 pydefect-0.7.0/pydefect/analyzer/defect_energy_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7741 2022-09-30 05:43:38.000000 pydefect-0.7.0/pydefect/analyzer/defect_structure_comparator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6577 2022-11-19 06:17:42.000000 pydefect-0.7.0/pydefect/analyzer/defect_structure_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10186 2021-06-04 06:03:27.000000 pydefect-0.7.0/pydefect/analyzer/eigenvalue_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2420 2021-08-06 10:11:01.000000 pydefect-0.7.0/pydefect/analyzer/grids.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7225 2022-11-22 05:43:00.000000 pydefect-0.7.0/pydefect/analyzer/make_band_edge_states.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1571 2021-05-26 07:04:53.000000 pydefect-0.7.0/pydefect/analyzer/make_calc_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2270 2021-08-06 10:11:46.000000 pydefect-0.7.0/pydefect/analyzer/make_defect_energy_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1578 2021-06-03 10:27:09.000000 pydefect-0.7.0/pydefect/analyzer/make_defect_energy_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6480 2022-11-19 06:15:43.000000 pydefect-0.7.0/pydefect/analyzer/make_defect_structure_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)      787 2022-12-08 07:12:16.000000 pydefect-0.7.0/pydefect/analyzer/pinning_levels.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1575 2021-04-27 05:43:07.000000 pydefect-0.7.0/pydefect/analyzer/refine_defect_structure.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2279 2022-11-16 04:21:58.000000 pydefect-0.7.0/pydefect/analyzer/transition_levels.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2006 2022-11-16 04:21:59.000000 pydefect-0.7.0/pydefect/analyzer/transition_levels_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1266 2021-04-25 05:17:40.000000 pydefect-0.7.0/pydefect/analyzer/unitcell.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.884230 pydefect-0.7.0/pydefect/chem_pot_diag/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.0/pydefect/chem_pot_diag/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)    15678 2023-01-04 05:04:29.000000 pydefect-0.7.0/pydefect/chem_pot_diag/chem_pot_diag.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10577 2022-10-10 09:09:15.000000 pydefect-0.7.0/pydefect/chem_pot_diag/cpd_plotter.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.894089 pydefect-0.7.0/pydefect/cli/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.0/pydefect/cli/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)    15165 2022-12-09 00:57:36.000000 pydefect-0.7.0/pydefect/cli/main.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10213 2022-12-09 00:59:11.000000 pydefect-0.7.0/pydefect/cli/main_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)      289 2022-12-13 08:11:13.000000 pydefect-0.7.0/pydefect/cli/main_print_json.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2248 2022-12-13 08:19:12.000000 pydefect-0.7.0/pydefect/cli/main_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5861 2022-12-08 07:20:06.000000 pydefect-0.7.0/pydefect/cli/main_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3663 2022-12-08 07:20:43.000000 pydefect-0.7.0/pydefect/cli/main_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4923 2021-05-02 06:20:14.000000 pydefect-0.7.0/pydefect/cli/make_defect_vesta_file.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.910439 pydefect-0.7.0/pydefect/cli/vasp/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-26 08:41:03.000000 pydefect-0.7.0/pydefect/cli/vasp/__init__.py
--rwxr-xr-x   0 kumagai    (501) staff       (20)     1017 2021-04-29 04:10:12.000000 pydefect-0.7.0/pydefect/cli/vasp/get_defect_charge_state.py
--rw-r--r--   0 kumagai    (501) staff       (20)     9144 2022-11-22 04:59:04.000000 pydefect-0.7.0/pydefect/cli/vasp/main_vasp.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6879 2023-01-04 04:53:30.000000 pydefect-0.7.0/pydefect/cli/vasp/main_vasp_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4785 2021-08-06 10:11:01.000000 pydefect-0.7.0/pydefect/cli/vasp/main_vasp_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3523 2021-08-06 10:14:07.000000 pydefect-0.7.0/pydefect/cli/vasp/main_vasp_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4770 2022-11-22 05:00:35.000000 pydefect-0.7.0/pydefect/cli/vasp/make_band_edge_orbital_infos.py
--rw-r--r--   0 kumagai    (501) staff       (20)      690 2021-04-13 03:41:39.000000 pydefect-0.7.0/pydefect/cli/vasp/make_calc_results.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2221 2021-06-04 02:29:24.000000 pydefect-0.7.0/pydefect/cli/vasp/make_composition_energies_from_mp.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2754 2021-05-24 05:42:28.000000 pydefect-0.7.0/pydefect/cli/vasp/make_defect_charge_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3564 2022-05-20 02:48:51.000000 pydefect-0.7.0/pydefect/cli/vasp/make_efnv_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2398 2020-11-25 07:07:18.000000 pydefect-0.7.0/pydefect/cli/vasp/make_gkfo_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)    18748 2022-10-24 06:34:05.000000 pydefect-0.7.0/pydefect/cli/vasp/make_local_extrema.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1349 2021-08-06 10:14:07.000000 pydefect-0.7.0/pydefect/cli/vasp/make_perfect_band_edge_state.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2471 2023-01-04 04:53:30.000000 pydefect-0.7.0/pydefect/cli/vasp/make_poscars_from_query.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1156 2021-04-25 05:20:51.000000 pydefect-0.7.0/pydefect/cli/vasp/make_unitcell.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.915274 pydefect-0.7.0/pydefect/cli/vasp/molecules/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.916919 pydefect-0.7.0/pydefect/cli/vasp/molecules/H2/
--rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-12-04 01:34:20.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/H2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/H2/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.918927 pydefect-0.7.0/pydefect/cli/vasp/molecules/H2O/
--rw-r--r--   0 kumagai    (501) staff       (20)      618 2020-05-15 22:52:05.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/H2O/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/H2O/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.920632 pydefect-0.7.0/pydefect/cli/vasp/molecules/N2/
--rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/N2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/N2/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.922419 pydefect-0.7.0/pydefect/cli/vasp/molecules/NH3/
--rw-r--r--   0 kumagai    (501) staff       (20)      733 2020-05-15 22:52:05.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/NH3/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/NH3/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.924039 pydefect-0.7.0/pydefect/cli/vasp/molecules/NO2/
--rw-r--r--   0 kumagai    (501) staff       (20)      623 2020-05-15 22:52:05.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/NO2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/NO2/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.925743 pydefect-0.7.0/pydefect/cli/vasp/molecules/O2/
--rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/O2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       49 2020-05-15 22:52:05.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/O2/prior_info.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-26 08:59:11.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)      729 2020-05-15 22:52:05.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/molecule_data.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      417 2020-05-26 08:59:40.000000 pydefect-0.7.0/pydefect/cli/vasp/molecules/molecules.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.934354 pydefect-0.7.0/pydefect/corrections/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.0/pydefect/corrections/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)      523 2021-04-26 01:51:45.000000 pydefect-0.7.0/pydefect/corrections/abstract_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2100 2021-04-14 04:22:43.000000 pydefect-0.7.0/pydefect/corrections/efnv_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4802 2020-06-06 00:50:29.000000 pydefect-0.7.0/pydefect/corrections/ewald.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2875 2020-11-26 00:07:11.000000 pydefect-0.7.0/pydefect/corrections/gkfo_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     9586 2021-06-03 10:30:08.000000 pydefect-0.7.0/pydefect/corrections/site_potential_plotter.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.938748 pydefect-0.7.0/pydefect/database/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.0/pydefect/database/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)      808 2021-04-28 23:15:40.000000 pydefect-0.7.0/pydefect/database/database.py
--rw-r--r--   0 kumagai    (501) staff       (20)      985 2020-05-15 01:50:57.000000 pydefect-0.7.0/pydefect/database/electronegativity.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      467 2021-05-08 04:43:11.000000 pydefect-0.7.0/pydefect/database/oxidation_state.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1073 2020-05-15 01:46:44.000000 pydefect-0.7.0/pydefect/database/rcore.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     2982 2021-06-10 06:38:20.000000 pydefect-0.7.0/pydefect/defaults.py
--rw-r--r--   0 kumagai    (501) staff       (20)      138 2020-05-13 06:54:40.000000 pydefect-0.7.0/pydefect/error.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.951017 pydefect-0.7.0/pydefect/input_maker/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:45:24.000000 pydefect-0.7.0/pydefect/input_maker/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2252 2022-11-04 06:49:00.000000 pydefect-0.7.0/pydefect/input_maker/append_interstitial.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1509 2022-09-30 06:02:01.000000 pydefect-0.7.0/pydefect/input_maker/defect.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5794 2022-09-30 06:04:45.000000 pydefect-0.7.0/pydefect/input_maker/defect_entries_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4655 2022-09-30 06:27:37.000000 pydefect-0.7.0/pydefect/input_maker/defect_entry.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1464 2022-07-01 01:20:02.000000 pydefect-0.7.0/pydefect/input_maker/defect_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3918 2020-11-23 04:55:46.000000 pydefect-0.7.0/pydefect/input_maker/defect_set_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2305 2021-08-06 10:14:07.000000 pydefect-0.7.0/pydefect/input_maker/local_extrema.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3880 2021-03-05 09:52:57.000000 pydefect-0.7.0/pydefect/input_maker/supercell.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3915 2021-04-28 11:22:39.000000 pydefect-0.7.0/pydefect/input_maker/supercell_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4644 2021-08-01 05:39:19.000000 pydefect-0.7.0/pydefect/input_maker/supercell_maker.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.953052 pydefect-0.7.0/pydefect/tests/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 pydefect-0.7.0/pydefect/tests/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:11.067513 pydefect-0.7.0/pydefect/tests/analyzer/
--rw-r--r--   0 kumagai    (501) staff       (20)     1983 2022-09-30 04:57:26.000000 pydefect-0.7.0/pydefect/tests/analyzer/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-08-03 11:12:30.000000 pydefect-0.7.0/pydefect/tests/analyzer/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.806870 pydefect-0.7.0/pydefect/tests/analyzer/dash_components/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.807745 pydefect-0.7.0/pydefect/tests/analyzer/dash_components/mgo_defects/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:11.068368 pydefect-0.7.0/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_0/
--rw-r--r--   0 kumagai    (501) staff       (20)     7233 2020-06-26 09:34:37.000000 pydefect-0.7.0/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_0/POSCAR
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:11.069533 pydefect-0.7.0/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_2/
--rw-r--r--   0 kumagai    (501) staff       (20)     7233 2020-06-26 09:34:37.000000 pydefect-0.7.0/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)     7450 2022-09-30 03:57:34.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_band_edge_states.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1022 2021-08-06 10:14:07.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_calc_results.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2402 2021-05-26 07:04:12.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_calc_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2915 2021-05-03 01:56:28.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_defect_charge_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7507 2022-12-08 06:25:11.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_defect_energy.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2466 2022-11-15 07:29:49.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_defect_energy_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1540 2022-11-15 04:49:34.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_defect_energy_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7391 2022-09-30 04:57:30.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_defect_structure_comparator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4373 2021-08-04 10:39:43.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_defect_structure_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2636 2021-05-02 08:25:54.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_eigenvalue_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2648 2021-08-06 10:14:07.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_grids.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7215 2022-11-22 05:40:58.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_make_band_edge_states.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1786 2021-08-06 10:14:07.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_make_calc_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2067 2021-08-06 10:14:07.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_make_defect_energy_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1609 2021-05-01 06:02:47.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_make_defect_energy_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1665 2022-09-30 05:50:49.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_make_defect_structure_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1465 2022-12-08 07:12:16.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_pinning_levels.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4262 2022-05-20 02:54:43.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_refine_defect_structure.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1796 2022-11-16 04:14:17.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_transition_levels.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1539 2022-11-16 04:16:01.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_transition_levels_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1111 2021-04-25 05:19:09.000000 pydefect-0.7.0/pydefect/tests/analyzer/test_unitcell.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:11.070273 pydefect-0.7.0/pydefect/tests/chem_pot_diag/
--rw-r--r--   0 kumagai    (501) staff       (20)      169 2020-11-30 07:08:52.000000 pydefect-0.7.0/pydefect/tests/chem_pot_diag/cpd.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:11.075811 pydefect-0.7.0/pydefect/tests/cli/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.0/pydefect/tests/cli/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10053 2022-12-12 23:52:07.000000 pydefect-0.7.0/pydefect/tests/cli/test_main.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10292 2022-11-22 05:02:01.000000 pydefect-0.7.0/pydefect/tests/cli/test_main_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1980 2022-10-10 09:24:54.000000 pydefect-0.7.0/pydefect/tests/cli/test_main_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4911 2022-11-15 04:58:26.000000 pydefect-0.7.0/pydefect/tests/cli/test_main_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4459 2022-12-09 00:53:29.000000 pydefect-0.7.0/pydefect/tests/cli/test_main_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3011 2021-05-15 12:24:21.000000 pydefect-0.7.0/pydefect/tests/cli/test_make_defect_vesta_file.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:11.089161 pydefect-0.7.0/pydefect/tests/cli/vasp/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/__init__.py
--rwxr-xr-x   0 kumagai    (501) staff       (20)     1671 2021-08-06 10:14:07.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_get_defect_charge_state.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4907 2022-11-22 04:59:59.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_main_vasp.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10097 2022-12-04 04:30:27.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_main_vasp_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2748 2021-04-30 03:32:19.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_main_vasp_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5028 2021-08-06 10:14:07.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_main_vasp_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7333 2022-11-22 01:50:04.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_band_edge_orbital_infos.py
--rw-r--r--   0 kumagai    (501) staff       (20)      848 2021-04-13 03:41:26.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_calc_results.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2702 2021-06-04 02:28:26.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_composition_energies_from_mp.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2164 2021-08-06 10:10:20.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_defect_charge_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2385 2021-03-05 09:52:57.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_efnv_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1619 2021-04-12 08:07:10.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_gkfo_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2178 2021-04-29 04:12:46.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_local_extrema.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1404 2021-04-01 02:01:36.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_perfect_band_edge_state.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1557 2022-05-20 02:54:43.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_poscars_from_query.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1513 2021-04-23 05:08:48.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_unitcell.py
--rw-r--r--   0 kumagai    (501) staff       (20)      216 2021-04-23 05:16:53.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/unitcell.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.809993 pydefect-0.7.0/pydefect/tests/cli/vasp/vasp_files/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:11.090148 pydefect-0.7.0/pydefect/tests/cli/vasp/vasp_files/KInO2_Va_O_2/
--rw-r--r--   0 kumagai    (501) staff       (20)       18 2020-05-31 08:54:40.000000 pydefect-0.7.0/pydefect/tests/cli/vasp/vasp_files/KInO2_Va_O_2/pydefect.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)    14270 2022-11-15 03:25:39.000000 pydefect-0.7.0/pydefect/tests/conftest.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:11.095483 pydefect-0.7.0/pydefect/tests/corrections/
--rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-06-14 07:43:24.000000 pydefect-0.7.0/pydefect/tests/corrections/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1723 2021-04-26 01:56:50.000000 pydefect-0.7.0/pydefect/tests/corrections/test_efnv_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)      963 2020-06-05 00:53:04.000000 pydefect-0.7.0/pydefect/tests/corrections/test_efnv_performance.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3613 2021-03-02 02:40:28.000000 pydefect-0.7.0/pydefect/tests/corrections/test_ewald.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2549 2020-11-25 07:07:18.000000 pydefect-0.7.0/pydefect/tests/corrections/test_gkfo_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2395 2020-11-25 07:22:27.000000 pydefect-0.7.0/pydefect/tests/corrections/test_site_potential_plotter.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:11.096685 pydefect-0.7.0/pydefect/tests/helpers/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 pydefect-0.7.0/pydefect/tests/helpers/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:11.130772 pydefect-0.7.0/pydefect/tests/input_maker/
--rw-r--r--   0 kumagai    (501) staff       (20)      347 2020-08-05 23:35:58.000000 pydefect-0.7.0/pydefect/tests/input_maker/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:46:18.000000 pydefect-0.7.0/pydefect/tests/input_maker/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2704 2021-04-28 11:25:22.000000 pydefect-0.7.0/pydefect/tests/input_maker/test_append_interstitial.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1230 2022-09-30 06:02:25.000000 pydefect-0.7.0/pydefect/tests/input_maker/test_defect.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5834 2021-08-06 10:14:07.000000 pydefect-0.7.0/pydefect/tests/input_maker/test_defect_entries_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4367 2022-09-30 06:12:21.000000 pydefect-0.7.0/pydefect/tests/input_maker/test_defect_entry.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1551 2022-07-01 01:20:10.000000 pydefect-0.7.0/pydefect/tests/input_maker/test_defect_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2139 2020-12-23 03:22:55.000000 pydefect-0.7.0/pydefect/tests/input_maker/test_defect_set_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4174 2021-08-06 10:11:01.000000 pydefect-0.7.0/pydefect/tests/input_maker/test_local_extrema.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3571 2021-03-05 09:52:57.000000 pydefect-0.7.0/pydefect/tests/input_maker/test_supercell.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3301 2021-04-28 11:22:26.000000 pydefect-0.7.0/pydefect/tests/input_maker/test_supercell_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5471 2022-07-05 00:40:37.000000 pydefect-0.7.0/pydefect/tests/input_maker/test_supercell_maker.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:11.139284 pydefect-0.7.0/pydefect/util/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-26 03:04:22.000000 pydefect-0.7.0/pydefect/util/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)      245 2021-04-06 09:47:19.000000 pydefect-0.7.0/pydefect/util/coords.py
--rw-r--r--   0 kumagai    (501) staff       (20)      287 2020-05-26 12:22:43.000000 pydefect-0.7.0/pydefect/util/error_classes.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2333 2023-01-04 05:27:12.000000 pydefect-0.7.0/pydefect/util/mp_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3052 2022-11-15 07:39:58.000000 pydefect-0.7.0/pydefect/util/prepare_names.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2727 2021-04-26 23:23:36.000000 pydefect-0.7.0/pydefect/util/structure_tools.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-01-04 05:29:10.820829 pydefect-0.7.0/pydefect.egg-info/
--rw-r--r--   0 kumagai    (501) staff       (20)      397 2023-01-04 05:29:10.000000 pydefect-0.7.0/pydefect.egg-info/PKG-INFO
--rw-r--r--   0 kumagai    (501) staff       (20)     7662 2023-01-04 05:29:10.000000 pydefect-0.7.0/pydefect.egg-info/SOURCES.txt
--rw-r--r--   0 kumagai    (501) staff       (20)        1 2023-01-04 05:29:10.000000 pydefect-0.7.0/pydefect.egg-info/dependency_links.txt
--rw-r--r--   0 kumagai    (501) staff       (20)      256 2023-01-04 05:29:10.000000 pydefect-0.7.0/pydefect.egg-info/entry_points.txt
--rw-r--r--   0 kumagai    (501) staff       (20)      164 2023-01-04 05:29:10.000000 pydefect-0.7.0/pydefect.egg-info/requires.txt
--rw-r--r--   0 kumagai    (501) staff       (20)        9 2023-01-04 05:29:10.000000 pydefect-0.7.0/pydefect.egg-info/top_level.txt
--rw-r--r--   0 kumagai    (501) staff       (20)       38 2023-01-04 05:29:11.141137 pydefect-0.7.0/setup.cfg
--rw-r--r--   0 kumagai    (501) staff       (20)     1335 2021-08-06 00:13:51.000000 pydefect-0.7.0/setup.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.152753 pydefect-0.7.1/
+-rw-r--r--   0 kumagai    (501) staff       (20)       54 2021-03-12 02:40:59.000000 pydefect-0.7.1/MANIFEST.in
+-rw-r--r--   0 kumagai    (501) staff       (20)      397 2023-05-20 00:06:15.152455 pydefect-0.7.1/PKG-INFO
+-rw-r--r--   0 kumagai    (501) staff       (20)     4563 2022-08-17 09:42:29.000000 pydefect-0.7.1/README.md
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.010738 pydefect-0.7.1/pydefect/
+-rw-r--r--   0 kumagai    (501) staff       (20)       21 2023-05-20 00:05:58.000000 pydefect-0.7.1/pydefect/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.037593 pydefect-0.7.1/pydefect/analyzer/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.1/pydefect/analyzer/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2840 2021-04-02 01:38:50.000000 pydefect-0.7.1/pydefect/analyzer/_defect_charge_distribution.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    11690 2023-02-21 04:23:52.000000 pydefect-0.7.1/pydefect/analyzer/band_edge_states.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1334 2021-05-01 01:17:09.000000 pydefect-0.7.1/pydefect/analyzer/calc_results.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2426 2021-05-26 07:04:12.000000 pydefect-0.7.1/pydefect/analyzer/calc_summary.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.040948 pydefect-0.7.1/pydefect/analyzer/concentration/
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2023-01-30 01:05:15.000000 pydefect-0.7.1/pydefect/analyzer/concentration/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5631 2023-02-08 05:36:42.000000 pydefect-0.7.1/pydefect/analyzer/concentration/concentration.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2973 2023-02-01 00:50:27.000000 pydefect-0.7.1/pydefect/analyzer/concentration/degeneracy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      385 2023-01-30 01:10:12.000000 pydefect-0.7.1/pydefect/analyzer/concentration/distribution_function.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7772 2023-02-08 07:02:02.000000 pydefect-0.7.1/pydefect/analyzer/concentration/make_concentration.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2462 2023-03-09 04:26:39.000000 pydefect-0.7.1/pydefect/analyzer/concentration/plot_concentration.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.044379 pydefect-0.7.1/pydefect/analyzer/dash_components/
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-08-21 04:26:43.000000 pydefect-0.7.1/pydefect/analyzer/dash_components/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5094 2021-08-15 04:39:32.000000 pydefect-0.7.1/pydefect/analyzer/dash_components/cpd_energy_dash.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1754 2021-05-27 10:09:51.000000 pydefect-0.7.1/pydefect/analyzer/dash_components/cpd_energy_dash_demo.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      929 2021-05-27 09:07:43.000000 pydefect-0.7.1/pydefect/analyzer/dash_components/cpd_plotter_main.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     8866 2021-04-04 05:43:59.000000 pydefect-0.7.1/pydefect/analyzer/dash_components/main.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6859 2021-04-04 05:43:59.000000 pydefect-0.7.1/pydefect/analyzer/dash_components/scenes_from_volumetric_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4716 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/analyzer/defect_charge_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    12944 2023-03-12 22:54:57.000000 pydefect-0.7.1/pydefect/analyzer/defect_energy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     9945 2023-01-31 04:11:38.000000 pydefect-0.7.1/pydefect/analyzer/defect_energy_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1280 2022-11-15 04:48:53.000000 pydefect-0.7.1/pydefect/analyzer/defect_energy_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7741 2022-09-30 05:43:38.000000 pydefect-0.7.1/pydefect/analyzer/defect_structure_comparator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6536 2023-01-28 01:55:02.000000 pydefect-0.7.1/pydefect/analyzer/defect_structure_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10186 2021-06-04 06:03:27.000000 pydefect-0.7.1/pydefect/analyzer/eigenvalue_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2420 2021-08-06 10:11:01.000000 pydefect-0.7.1/pydefect/analyzer/grids.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7225 2022-11-22 05:43:00.000000 pydefect-0.7.1/pydefect/analyzer/make_band_edge_states.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1571 2021-05-26 07:04:53.000000 pydefect-0.7.1/pydefect/analyzer/make_calc_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2270 2021-08-06 10:11:46.000000 pydefect-0.7.1/pydefect/analyzer/make_defect_energy_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1716 2023-02-11 23:51:37.000000 pydefect-0.7.1/pydefect/analyzer/make_defect_energy_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6480 2022-11-19 06:15:43.000000 pydefect-0.7.1/pydefect/analyzer/make_defect_structure_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      787 2022-12-08 07:12:16.000000 pydefect-0.7.1/pydefect/analyzer/pinning_levels.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1575 2021-04-27 05:43:07.000000 pydefect-0.7.1/pydefect/analyzer/refine_defect_structure.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2279 2022-11-16 04:21:58.000000 pydefect-0.7.1/pydefect/analyzer/transition_levels.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2006 2022-11-16 04:21:59.000000 pydefect-0.7.1/pydefect/analyzer/transition_levels_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2128 2023-03-26 01:17:24.000000 pydefect-0.7.1/pydefect/analyzer/unitcell.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.046070 pydefect-0.7.1/pydefect/chem_pot_diag/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.1/pydefect/chem_pot_diag/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    15678 2023-01-04 05:04:29.000000 pydefect-0.7.1/pydefect/chem_pot_diag/chem_pot_diag.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10577 2022-10-10 09:09:15.000000 pydefect-0.7.1/pydefect/chem_pot_diag/cpd_plotter.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.050461 pydefect-0.7.1/pydefect/cli/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.1/pydefect/cli/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    15399 2023-03-05 01:50:27.000000 pydefect-0.7.1/pydefect/cli/main.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10546 2023-05-19 23:36:53.000000 pydefect-0.7.1/pydefect/cli/main_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      289 2022-12-13 08:11:13.000000 pydefect-0.7.1/pydefect/cli/main_print_json.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2248 2023-04-06 01:32:45.000000 pydefect-0.7.1/pydefect/cli/main_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10042 2023-03-09 23:27:38.000000 pydefect-0.7.1/pydefect/cli/main_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6818 2023-03-09 23:26:07.000000 pydefect-0.7.1/pydefect/cli/main_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4923 2021-05-02 06:20:14.000000 pydefect-0.7.1/pydefect/cli/make_defect_vesta_file.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.058388 pydefect-0.7.1/pydefect/cli/vasp/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-26 08:41:03.000000 pydefect-0.7.1/pydefect/cli/vasp/__init__.py
+-rwxr-xr-x   0 kumagai    (501) staff       (20)     1017 2021-04-29 04:10:12.000000 pydefect-0.7.1/pydefect/cli/vasp/get_defect_charge_state.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     9144 2022-11-22 04:59:04.000000 pydefect-0.7.1/pydefect/cli/vasp/main_vasp.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6954 2023-03-26 01:11:16.000000 pydefect-0.7.1/pydefect/cli/vasp/main_vasp_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5648 2023-03-05 02:05:12.000000 pydefect-0.7.1/pydefect/cli/vasp/main_vasp_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4282 2023-03-05 02:05:12.000000 pydefect-0.7.1/pydefect/cli/vasp/main_vasp_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4770 2022-11-22 05:00:35.000000 pydefect-0.7.1/pydefect/cli/vasp/make_band_edge_orbital_infos.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      690 2021-04-13 03:41:39.000000 pydefect-0.7.1/pydefect/cli/vasp/make_calc_results.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2221 2021-06-04 02:29:24.000000 pydefect-0.7.1/pydefect/cli/vasp/make_composition_energies_from_mp.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2754 2021-05-24 05:42:28.000000 pydefect-0.7.1/pydefect/cli/vasp/make_defect_charge_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3728 2023-03-24 00:21:35.000000 pydefect-0.7.1/pydefect/cli/vasp/make_efnv_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2398 2020-11-25 07:07:18.000000 pydefect-0.7.1/pydefect/cli/vasp/make_gkfo_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    18748 2022-10-24 06:34:05.000000 pydefect-0.7.1/pydefect/cli/vasp/make_local_extrema.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1349 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/cli/vasp/make_perfect_band_edge_state.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2471 2023-01-04 04:53:30.000000 pydefect-0.7.1/pydefect/cli/vasp/make_poscars_from_query.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1156 2021-04-25 05:20:51.000000 pydefect-0.7.1/pydefect/cli/vasp/make_unitcell.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.059832 pydefect-0.7.1/pydefect/cli/vasp/molecules/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.060735 pydefect-0.7.1/pydefect/cli/vasp/molecules/H2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-12-04 01:34:20.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/H2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/H2/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.061706 pydefect-0.7.1/pydefect/cli/vasp/molecules/H2O/
+-rw-r--r--   0 kumagai    (501) staff       (20)      618 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/H2O/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/H2O/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.062542 pydefect-0.7.1/pydefect/cli/vasp/molecules/N2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/N2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/N2/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.063381 pydefect-0.7.1/pydefect/cli/vasp/molecules/NH3/
+-rw-r--r--   0 kumagai    (501) staff       (20)      733 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/NH3/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/NH3/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.064335 pydefect-0.7.1/pydefect/cli/vasp/molecules/NO2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      623 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/NO2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/NO2/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.065353 pydefect-0.7.1/pydefect/cli/vasp/molecules/O2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/O2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       49 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/O2/prior_info.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-26 08:59:11.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      729 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/molecule_data.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      417 2020-05-26 08:59:40.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/molecules.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.068090 pydefect-0.7.1/pydefect/corrections/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.1/pydefect/corrections/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      523 2021-04-26 01:51:45.000000 pydefect-0.7.1/pydefect/corrections/abstract_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2042 2023-05-10 06:23:17.000000 pydefect-0.7.1/pydefect/corrections/efnv_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4802 2020-06-06 00:50:29.000000 pydefect-0.7.1/pydefect/corrections/ewald.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2875 2020-11-26 00:07:11.000000 pydefect-0.7.1/pydefect/corrections/gkfo_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     9656 2023-03-29 07:34:00.000000 pydefect-0.7.1/pydefect/corrections/site_potential_plotter.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.070382 pydefect-0.7.1/pydefect/database/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.1/pydefect/database/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      808 2021-04-28 23:15:40.000000 pydefect-0.7.1/pydefect/database/database.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      985 2020-05-15 01:50:57.000000 pydefect-0.7.1/pydefect/database/electronegativity.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      467 2021-05-08 04:43:11.000000 pydefect-0.7.1/pydefect/database/oxidation_state.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)     1073 2020-05-15 01:46:44.000000 pydefect-0.7.1/pydefect/database/rcore.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)     2982 2021-06-10 06:38:20.000000 pydefect-0.7.1/pydefect/defaults.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      138 2020-05-13 06:54:40.000000 pydefect-0.7.1/pydefect/error.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.077411 pydefect-0.7.1/pydefect/input_maker/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:45:24.000000 pydefect-0.7.1/pydefect/input_maker/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2252 2022-11-04 06:49:00.000000 pydefect-0.7.1/pydefect/input_maker/append_interstitial.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2011 2023-03-13 01:10:20.000000 pydefect-0.7.1/pydefect/input_maker/complex_defect_entries_make.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1178 2023-03-12 23:38:44.000000 pydefect-0.7.1/pydefect/input_maker/complex_defect_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1509 2022-09-30 06:02:01.000000 pydefect-0.7.1/pydefect/input_maker/defect.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5794 2022-09-30 06:04:45.000000 pydefect-0.7.1/pydefect/input_maker/defect_entries_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4655 2022-09-30 06:27:37.000000 pydefect-0.7.1/pydefect/input_maker/defect_entry.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1464 2022-07-01 01:20:02.000000 pydefect-0.7.1/pydefect/input_maker/defect_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3918 2020-11-23 04:55:46.000000 pydefect-0.7.1/pydefect/input_maker/defect_set_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2305 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/input_maker/local_extrema.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3149 2023-01-28 01:22:10.000000 pydefect-0.7.1/pydefect/input_maker/manual_supercell_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3938 2023-01-28 00:19:05.000000 pydefect-0.7.1/pydefect/input_maker/supercell.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4242 2023-01-28 01:11:46.000000 pydefect-0.7.1/pydefect/input_maker/supercell_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4727 2023-05-18 07:33:28.000000 pydefect-0.7.1/pydefect/input_maker/supercell_maker.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.078243 pydefect-0.7.1/pydefect/tests/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 pydefect-0.7.1/pydefect/tests/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.094353 pydefect-0.7.1/pydefect/tests/analyzer/
+-rw-r--r--   0 kumagai    (501) staff       (20)     1983 2022-09-30 04:57:26.000000 pydefect-0.7.1/pydefect/tests/analyzer/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-08-03 11:12:30.000000 pydefect-0.7.1/pydefect/tests/analyzer/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.097026 pydefect-0.7.1/pydefect/tests/analyzer/concentration/
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2023-01-30 01:05:35.000000 pydefect-0.7.1/pydefect/tests/analyzer/concentration/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3177 2023-02-02 23:17:57.000000 pydefect-0.7.1/pydefect/tests/analyzer/concentration/test_concentration.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1723 2023-02-01 00:50:07.000000 pydefect-0.7.1/pydefect/tests/analyzer/concentration/test_degeneracy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      469 2023-01-30 01:09:25.000000 pydefect-0.7.1/pydefect/tests/analyzer/concentration/test_distribution_function.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3239 2023-03-05 02:07:50.000000 pydefect-0.7.1/pydefect/tests/analyzer/concentration/test_make_concentration.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      975 2023-02-08 06:50:25.000000 pydefect-0.7.1/pydefect/tests/analyzer/concentration/test_plot_concentration.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.003173 pydefect-0.7.1/pydefect/tests/analyzer/dash_components/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.003650 pydefect-0.7.1/pydefect/tests/analyzer/dash_components/mgo_defects/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.097571 pydefect-0.7.1/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_0/
+-rw-r--r--   0 kumagai    (501) staff       (20)     7233 2020-06-26 09:34:37.000000 pydefect-0.7.1/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_0/POSCAR
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.098235 pydefect-0.7.1/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_2/
+-rw-r--r--   0 kumagai    (501) staff       (20)     7233 2020-06-26 09:34:37.000000 pydefect-0.7.1/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)     7450 2022-09-30 03:57:34.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_band_edge_states.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1022 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_calc_results.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2402 2021-05-26 07:04:12.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_calc_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2915 2021-05-03 01:56:28.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_defect_charge_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     8302 2023-03-05 02:36:13.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_defect_energy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2466 2022-11-15 07:29:49.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_defect_energy_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1540 2022-11-15 04:49:34.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_defect_energy_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7391 2022-09-30 04:57:30.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_defect_structure_comparator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4373 2023-01-29 23:13:01.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_defect_structure_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2636 2021-05-02 08:25:54.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_eigenvalue_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2648 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_grids.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7215 2022-11-22 05:40:58.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_make_band_edge_states.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1786 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_make_calc_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2067 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_make_defect_energy_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1609 2021-05-01 06:02:47.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_make_defect_energy_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1665 2022-09-30 05:50:49.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_make_defect_structure_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1465 2022-12-08 07:12:16.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_pinning_levels.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4262 2022-05-20 02:54:43.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_refine_defect_structure.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1796 2022-11-16 04:14:17.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_transition_levels.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1539 2022-11-16 04:16:01.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_transition_levels_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2014 2023-05-10 06:40:55.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_unitcell.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.100873 pydefect-0.7.1/pydefect/tests/chem_pot_diag/
+-rw-r--r--   0 kumagai    (501) staff       (20)      169 2020-11-30 07:08:52.000000 pydefect-0.7.1/pydefect/tests/chem_pot_diag/cpd.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.106560 pydefect-0.7.1/pydefect/tests/cli/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.1/pydefect/tests/cli/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10308 2023-01-28 00:50:06.000000 pydefect-0.7.1/pydefect/tests/cli/test_main.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    11140 2023-03-05 02:10:01.000000 pydefect-0.7.1/pydefect/tests/cli/test_main_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1980 2022-10-10 09:24:54.000000 pydefect-0.7.1/pydefect/tests/cli/test_main_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4986 2023-03-05 02:12:51.000000 pydefect-0.7.1/pydefect/tests/cli/test_main_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5290 2023-03-09 23:26:49.000000 pydefect-0.7.1/pydefect/tests/cli/test_main_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3011 2021-05-15 12:24:21.000000 pydefect-0.7.1/pydefect/tests/cli/test_make_defect_vesta_file.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.122265 pydefect-0.7.1/pydefect/tests/cli/vasp/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/__init__.py
+-rwxr-xr-x   0 kumagai    (501) staff       (20)     1671 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_get_defect_charge_state.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4907 2022-11-22 04:59:59.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10280 2023-05-10 06:37:49.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2748 2021-04-30 03:32:19.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5028 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7333 2022-11-22 01:50:04.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_band_edge_orbital_infos.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      873 2023-03-26 01:11:16.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_calc_results.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2702 2021-06-04 02:28:26.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_composition_energies_from_mp.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2164 2021-08-06 10:10:20.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_defect_charge_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2385 2021-03-05 09:52:57.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_efnv_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1619 2021-04-12 08:07:10.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_gkfo_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2178 2021-04-29 04:12:46.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_local_extrema.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1429 2023-03-26 01:11:16.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_perfect_band_edge_state.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1557 2022-05-20 02:54:43.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_poscars_from_query.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1538 2023-03-26 01:11:16.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_unitcell.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      216 2021-04-23 05:16:53.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/unitcell.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.005209 pydefect-0.7.1/pydefect/tests/cli/vasp/vasp_files/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.123025 pydefect-0.7.1/pydefect/tests/cli/vasp/vasp_files/KInO2_Va_O_2/
+-rw-r--r--   0 kumagai    (501) staff       (20)       18 2020-05-31 08:54:40.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/vasp_files/KInO2_Va_O_2/pydefect.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)    14382 2023-05-10 00:54:37.000000 pydefect-0.7.1/pydefect/tests/conftest.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.128009 pydefect-0.7.1/pydefect/tests/corrections/
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-06-14 07:43:24.000000 pydefect-0.7.1/pydefect/tests/corrections/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1723 2021-04-26 01:56:50.000000 pydefect-0.7.1/pydefect/tests/corrections/test_efnv_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      963 2020-06-05 00:53:04.000000 pydefect-0.7.1/pydefect/tests/corrections/test_efnv_performance.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3613 2021-03-02 02:40:28.000000 pydefect-0.7.1/pydefect/tests/corrections/test_ewald.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2549 2020-11-25 07:07:18.000000 pydefect-0.7.1/pydefect/tests/corrections/test_gkfo_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2395 2020-11-25 07:22:27.000000 pydefect-0.7.1/pydefect/tests/corrections/test_site_potential_plotter.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.128445 pydefect-0.7.1/pydefect/tests/helpers/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 pydefect-0.7.1/pydefect/tests/helpers/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.138244 pydefect-0.7.1/pydefect/tests/input_maker/
+-rw-r--r--   0 kumagai    (501) staff       (20)      347 2020-08-05 23:35:58.000000 pydefect-0.7.1/pydefect/tests/input_maker/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:46:18.000000 pydefect-0.7.1/pydefect/tests/input_maker/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2704 2021-04-28 11:25:22.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_append_interstitial.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1923 2023-03-13 01:10:15.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_complex_defect_entries_make.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      810 2023-03-13 00:52:36.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_complex_defect_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1230 2022-09-30 06:02:25.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_defect.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5834 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_defect_entries_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4367 2022-09-30 06:12:21.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_defect_entry.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1551 2022-07-01 01:20:10.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_defect_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2139 2020-12-23 03:22:55.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_defect_set_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4174 2021-08-06 10:11:01.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_local_extrema.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2368 2023-01-28 01:19:23.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_manual_supercell_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3571 2021-03-05 09:52:57.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_supercell.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4443 2023-01-27 05:27:59.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_supercell_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5393 2023-05-19 23:41:13.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_supercell_maker.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.007077 pydefect-0.7.1/pydefect/tests/test_data_files/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.138808 pydefect-0.7.1/pydefect/tests/test_data_files/Na3AgO2/
+-rw-r--r--   0 kumagai    (501) staff       (20)     3145 2023-01-31 23:38:38.000000 pydefect-0.7.1/pydefect/tests/test_data_files/Na3AgO2/degeneracies.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.151776 pydefect-0.7.1/pydefect/util/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-26 03:04:22.000000 pydefect-0.7.1/pydefect/util/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      245 2021-04-06 09:47:19.000000 pydefect-0.7.1/pydefect/util/coords.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      287 2020-05-26 12:22:43.000000 pydefect-0.7.1/pydefect/util/error_classes.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2333 2023-01-04 05:27:12.000000 pydefect-0.7.1/pydefect/util/mp_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3052 2022-11-15 07:39:58.000000 pydefect-0.7.1/pydefect/util/prepare_names.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2727 2021-04-26 23:23:36.000000 pydefect-0.7.1/pydefect/util/structure_tools.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:14.993460 pydefect-0.7.1/pydefect-0.7.0/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:14.996014 pydefect-0.7.1/pydefect-0.7.0/pydefect/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:14.993732 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:14.993945 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.011265 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.012364 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/H2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-12-04 01:34:20.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/H2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/H2/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.013419 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/H2O/
+-rw-r--r--   0 kumagai    (501) staff       (20)      618 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/H2O/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/H2O/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.014378 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/N2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/N2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/N2/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.015440 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/NH3/
+-rw-r--r--   0 kumagai    (501) staff       (20)      733 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/NH3/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/NH3/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.016562 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/NO2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      623 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/NO2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/NO2/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.017619 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/O2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/O2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       49 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/O2/prior_info.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      729 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/molecule_data.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.019166 pydefect-0.7.1/pydefect-0.7.0/pydefect/database/
+-rw-r--r--   0 kumagai    (501) staff       (20)      985 2020-05-15 01:50:57.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/database/electronegativity.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      467 2021-05-08 04:43:11.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/database/oxidation_state.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)     1073 2020-05-15 01:46:44.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/database/rcore.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:14.996213 pydefect-0.7.1/pydefect-0.7.0/pydefect/tests/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.019690 pydefect-0.7.1/pydefect-0.7.0/pydefect/tests/analyzer/
+-rw-r--r--   0 kumagai    (501) staff       (20)     1983 2022-09-30 04:57:26.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/tests/analyzer/POSCAR
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.022575 pydefect-0.7.1/pydefect.egg-info/
+-rw-r--r--   0 kumagai    (501) staff       (20)      397 2023-05-20 00:06:14.000000 pydefect-0.7.1/pydefect.egg-info/PKG-INFO
+-rw-r--r--   0 kumagai    (501) staff       (20)     9663 2023-05-20 00:06:14.000000 pydefect-0.7.1/pydefect.egg-info/SOURCES.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)        1 2023-05-20 00:06:14.000000 pydefect-0.7.1/pydefect.egg-info/dependency_links.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)      256 2023-05-20 00:06:14.000000 pydefect-0.7.1/pydefect.egg-info/entry_points.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)      164 2023-05-20 00:06:14.000000 pydefect-0.7.1/pydefect.egg-info/requires.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)        9 2023-05-20 00:06:14.000000 pydefect-0.7.1/pydefect.egg-info/top_level.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)       38 2023-05-20 00:06:15.152846 pydefect-0.7.1/setup.cfg
+-rw-r--r--   0 kumagai    (501) staff       (20)     1335 2021-08-06 00:13:51.000000 pydefect-0.7.1/setup.py
```

### Comparing `pydefect-0.7.0/README.md` & `pydefect-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/_defect_charge_distribution.py` & `pydefect-0.7.1/pydefect/analyzer/_defect_charge_distribution.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/band_edge_states.py` & `pydefect-0.7.1/pydefect/analyzer/band_edge_states.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
     occupation: float
     participation_ratio: float = None
 
 
 @dataclass
 class BandEdgeOrbitalInfos(MSONable, ToJsonFileMixIn):
     orbital_infos: List[List[List["OrbitalInfo"]]]  # [spin, k-idx, band-idx]
-    kpt_coords: List[Coords]
+    kpt_coords: List[GenCoords]
     kpt_weights: List[float]
-    lowest_band_index: int
+    lowest_band_index: int  # python convention starting from 0.
     fermi_level: float
 
     def kpt_idx(self, kpt_coord):
         for i, orig_kpt in enumerate(self.kpt_coords):
             if sum(abs(k - l) for k, l in zip(orig_kpt, kpt_coord)) < 1e-5:
                 return i
         raise ValueError(f"{kpt_coord} not in kpt_coords {self.kpt_coords}.")
@@ -133,14 +133,21 @@
     ave_energy: float
     occupation: float
     orbitals: Dict[str, List[float]]
     participation_ratio: Optional[float] = None
     radius: Optional[float] = None
     center: Optional[GenCoords] = None
 
+    @property
+    def band_index(self):
+        return self.band_idx
+
+    @property
+    def eigenvalue(self):
+        return self.ave_energy
 
 @dataclass
 class EdgeInfo(MSONable):
     """Information for a particular band edge, namely VBM or CBM."""
     band_idx: int
     kpt_coord: Coords
     orbital_info: "OrbitalInfo"
@@ -193,16 +200,16 @@
     """
 
     vbm_info: EdgeInfo
     cbm_info: EdgeInfo
     vbm_orbital_diff: float  # Difference from those of perfect supercell.
     cbm_orbital_diff: float
     localized_orbitals: List[LocalizedOrbital]
-    vbm_hole_occupation: float = None
-    cbm_electron_occupation: float = None
+    vbm_hole_occupation: float
+    cbm_electron_occupation: float
 
     @property
     def is_shallow(self):
         return self.has_donor_phs or self.has_acceptor_phs
 
     @property
     def has_donor_phs(self):
```

### Comparing `pydefect-0.7.0/pydefect/analyzer/calc_results.py` & `pydefect-0.7.1/pydefect/analyzer/calc_results.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/calc_summary.py` & `pydefect-0.7.1/pydefect/analyzer/calc_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/dash_components/cpd_energy_dash.py` & `pydefect-0.7.1/pydefect/analyzer/dash_components/cpd_energy_dash.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/dash_components/cpd_energy_dash_demo.py` & `pydefect-0.7.1/pydefect/analyzer/dash_components/cpd_energy_dash_demo.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/dash_components/cpd_plotter_main.py` & `pydefect-0.7.1/pydefect/analyzer/dash_components/cpd_plotter_main.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/dash_components/main.py` & `pydefect-0.7.1/pydefect/analyzer/dash_components/main.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/dash_components/scenes_from_volumetric_data.py` & `pydefect-0.7.1/pydefect/analyzer/dash_components/scenes_from_volumetric_data.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/defect_charge_info.py` & `pydefect-0.7.1/pydefect/analyzer/defect_charge_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/defect_energy.py` & `pydefect-0.7.1/pydefect/analyzer/defect_energy.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,24 +89,28 @@
     """ The base Fermi level is set at the VBM."""
 
     def __post_init__(self):
         if self.supercell_cbm < self.cbm - 0.01:
             logger.warning(f"Supercell CBM {self.supercell_cbm} is lower in "
                            f"energy than the unitcell CBM {self.cbm}")
 
-    def screened_defect_energies(self, allow_shallow: bool
+    def screened_defect_energies(self,
+                                 allow_shallow: bool,
+                                 excluded_defects: List[str] = None
                                  ) -> Dict[str, DefectEnergies]:
         result = {}
         for name, des in self.defect_energies.items():
             charges, defect_energies = [], []
-            for c, de in zip(des.charges, des.defect_energies):
-                if allow_shallow or \
-                        (allow_shallow is False and de.is_shallow is False):
-                    charges.append(c)
-                    defect_energies.append(de)
+            for charge, de in zip(des.charges, des.defect_energies):
+                if allow_shallow is False and de.is_shallow is True:
+                    continue
+                if excluded_defects and f"{name}_{charge}" in excluded_defects:
+                    continue
+                charges.append(charge)
+                defect_energies.append(de)
             result[name] = DefectEnergies(des.atom_io, charges, defect_energies)
         return result
 
     def __str__(self):
         lines = [f"title: {numbers_to_lowercases(self.title)}",
                  "rel_chem_pots:"]
         chem_pot = []
@@ -160,16 +164,19 @@
             if charge_energies:
                 charge_energies_dict[k] = SingleChargeEnergies(charge_energies)
 
         if not charge_energies_dict:
             logger.warning(f"No defect data is available. Try to switch on "
                            f"allow_shallow flag.")
 
-        return ChargeEnergies(prettify_names(charge_energies_dict, name_style),
-                              e_range[0], e_range[1])
+        if name_style is not False:
+            charge_energies_dict = \
+                prettify_names(charge_energies_dict, name_style)
+
+        return ChargeEnergies(charge_energies_dict, e_range[0], e_range[1])
 
     @property
     def latexified_title(self):
         return latexify(self.title)
 
 
 @dataclass
@@ -228,17 +235,32 @@
 
     def energy_range(self, space: float) -> List[float]:
         candidates = []
         for cp in self.cross_point_dicts.values():
             candidates.extend(cp.t_all_sorted_points[1])
         return [min(candidates) - space, max(candidates) + space]
 
+    @property
+    def pinning_levels(self) -> Dict[str, List[float]]:
+        result = {}
+        for k, v in self.charge_energies_dict.items():
+            pl = v.pinning_level(self.e_min, self.e_max)
+            lower = pl[0][0] if pl[0] else None
+            upper = pl[1][0] if pl[1] else None
+            result[k] = [lower, upper]
+        return result
+
 
 @dataclass
 class SingleChargeEnergies(MSONable):
+    """
+    charge_energies store the energy at each charge state at the E_F=0 in the
+    situation where the VBM is set to 0.
+
+    """
     charge_energies: List[Tuple[int, float]]
 
     def pinning_level(self, e_min, e_max
                       ) -> Tuple[Tuple[float, Optional[int]],
                                  Tuple[float, Optional[int]]]:
         """
         :return: ((Lower pinning, its charge), (Upper pinning, its charge))
@@ -261,14 +283,23 @@
 
         if upper_charge is None or upper_pinning > e_max:
             upper = None
         else:
             upper = (upper_pinning, upper_charge)
         return lower, upper
 
+    def charge_energies_at_ef(self, ef: float) -> List[Tuple[int, float]]:
+        """
+        :return: (Lowest energy, its charge)
+        """
+        result = []
+        for charge, energy in self.charge_energies:
+            result.append((charge, energy + charge * ef))
+        return result
+
     def energy_at_ef(self, ef: float) -> Tuple[float, int]:
         """
         :return: (Lowest energy, its charge)
         """
         result_e, result_charge = float("inf"), None
         for charge, energy in self.charge_energies:
             energy = energy + charge * ef
```

### Comparing `pydefect-0.7.0/pydefect/analyzer/defect_energy_plotter.py` & `pydefect-0.7.1/pydefect/analyzer/defect_energy_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         tls.to_json_file()
 
         # charge_energies needs to be run again to change name to mpl style.
         # Need refactoring in the future.
         charge_energies = defect_energy_summary.charge_energies(
             chem_pot_label, allow_shallow, with_corrections, self._x_range,
             name_style)
+        self.charge_energies = charge_energies
         self.with_corrections = with_corrections
         self._cross_points = charge_energies.cross_point_dicts
         self._e_min_max_energies_dict = charge_energies.e_min_max_energies_dict
         self._y_range = y_range or charge_energies.energy_range(space=0.2)
         self._vline_threshold = vline_threshold
         self._x_unit = x_unit
         self._y_unit = y_unit
```

### Comparing `pydefect-0.7.0/pydefect/analyzer/defect_energy_util.py` & `pydefect-0.7.1/pydefect/analyzer/defect_energy_util.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/defect_structure_comparator.py` & `pydefect-0.7.1/pydefect/analyzer/defect_structure_comparator.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/defect_structure_info.py` & `pydefect-0.7.1/pydefect/analyzer/defect_structure_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         lines.append(f"Neighbor max distance {cutoff:5.3f}")
 
         lines.append("Displacements")
         idxs = [[i, d] for i, d in enumerate(self.displacements)
                 if d is not None]
         table = [["Elem", "Dist", "Displace", "Angle", "Index",
                   "Initial site", "", "Final site", "Neighbor"]]
-        print(self.neighbor_atom_indices)
+
         for final_idx, d in sorted(idxs,
                                    key=lambda y: y[1].distance_from_defect):
             is_neighbor = "T" if final_idx in self.neighbor_atom_indices else ""
             if d.distance_from_defect > defaults.show_structure_cutoff:
                 break
             i_pos = pretty_coords(d.original_pos)
             f_pos = pretty_coords(d.final_pos)
```

### Comparing `pydefect-0.7.0/pydefect/analyzer/eigenvalue_plotter.py` & `pydefect-0.7.1/pydefect/analyzer/eigenvalue_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/grids.py` & `pydefect-0.7.1/pydefect/analyzer/grids.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/make_band_edge_states.py` & `pydefect-0.7.1/pydefect/analyzer/make_band_edge_states.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/make_calc_summary.py` & `pydefect-0.7.1/pydefect/analyzer/make_calc_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/make_defect_energy_info.py` & `pydefect-0.7.1/pydefect/analyzer/make_defect_energy_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/make_defect_energy_summary.py` & `pydefect-0.7.1/pydefect/analyzer/make_defect_energy_summary.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,20 @@
     key = lambda x: x.name
     # MUST NEED SORTED.
     for _, grouped_es in groupby(sorted(energy_infos, key=key), key=key):
         grouped_es = list(grouped_es)
         name, atom_io = grouped_es[0].name, grouped_es[0].atom_io
         charges, des = [], []
         for es in grouped_es:
-            assert atom_io == es.atom_io
+            try:
+                assert sorted(atom_io) == sorted(es.atom_io)
+            except AssertionError:
+                print(atom_io, es.atom_io)
+                raise
+
             charges.append(es.charge)
             des.append(es.defect_energy)
         defect_energies[name] = DefectEnergies(atom_io, charges, des)
 
     return DefectEnergySummary(title=unitcell.system,
                                defect_energies=defect_energies,
                                rel_chem_pots=target_vertices.chem_pots,
```

### Comparing `pydefect-0.7.0/pydefect/analyzer/make_defect_structure_info.py` & `pydefect-0.7.1/pydefect/analyzer/make_defect_structure_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/pinning_levels.py` & `pydefect-0.7.1/pydefect/analyzer/pinning_levels.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/refine_defect_structure.py` & `pydefect-0.7.1/pydefect/analyzer/refine_defect_structure.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/transition_levels.py` & `pydefect-0.7.1/pydefect/analyzer/transition_levels.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/transition_levels_plotter.py` & `pydefect-0.7.1/pydefect/analyzer/transition_levels_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/analyzer/unitcell.py` & `pydefect-0.7.1/pydefect/analyzer/unitcell.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,14 +22,42 @@
 @dataclass
 class Unitcell(MSONable):
     system: str
     vbm: float
     cbm: float
     ele_dielectric_const: List[List[float]]
     ion_dielectric_const: List[List[float]]
+    electron_mass: List[List[float]] = None
+    hole_mass: List[List[float]] = None
+
+    @property
+    def effective_ionic_diele_const(self):
+        e_inf = np.array(self.ele_dielectric_const)
+        e_sum = np.array(self.dielectric_constant)
+        return np.nan_to_num((e_sum * e_inf) / (e_sum - e_inf)).tolist()
+
+    @property
+    def ave_ele_diele(self):
+        matrix = np.array(self.ele_dielectric_const)
+        return np.average(matrix.diagonal())
+
+    @property
+    def ave_diele(self):
+        matrix = np.array(self.dielectric_constant)
+        return np.average(matrix.diagonal())
+
+    @property
+    def ave_ele_mass(self):
+        matrix = np.array(self.electron_mass)
+        return np.average(matrix.diagonal())
+
+    @property
+    def ave_hole_mass(self):
+        matrix = np.array(self.hole_mass)
+        return np.average(matrix.diagonal())
 
     @property
     def dielectric_constant(self):
         total = (np.array(self.ele_dielectric_const)
                  + np.array(self.ion_dielectric_const))
         return total.tolist()
```

### Comparing `pydefect-0.7.0/pydefect/chem_pot_diag/chem_pot_diag.py` & `pydefect-0.7.1/pydefect/chem_pot_diag/chem_pot_diag.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/chem_pot_diag/cpd_plotter.py` & `pydefect-0.7.1/pydefect/chem_pot_diag/cpd_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/main.py` & `pydefect-0.7.1/pydefect/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,14 @@
             help="defect_energy_summary.json file path.")
         result.add_argument(
             "--allow_shallow", action="store_true",
             help="Set when the energies of shallow defects are allowed.")
         result.add_argument(
             "--no_corrections", dest="with_corrections", action="store_false",
             help="Set when corrections are switched off.")
-    elif name == "defect_energy_label":
         result.add_argument(
             "-l", "--label", type=str, required=True,
             help="Label in the chemical potential diagram")
     else:
         raise ValueError
     return result
 
@@ -98,15 +97,14 @@
 
     unitcell_parser = add_sub_parser(argparse, name="unitcell")
     si_parser = add_sub_parser(argparse, name="supercell_info")
     pcr_parser = add_sub_parser(argparse, name="perfect_calc_results")
     pbes_parser = add_sub_parser(argparse, name="perfect_band_edge_state")
     no_calc_results = add_sub_parser(argparse, name="no_calc_results_check")
     defect_e_sum_parser = add_sub_parser(argparse, name="defect_energy_summary")
-    defect_e_label = add_sub_parser(argparse, name="defect_energy_label")
 
     # -- make_standard_and_relative_energies -----------------------------------
     parser_make_standard_and_relative_energies = subparsers.add_parser(
         name="standard_and_relative_energies",
         description="",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         aliases=['sre'])
@@ -166,14 +164,21 @@
              "1, 3 or 9 components are accepted.")
     parser_supercell.add_argument(
         "--min_atoms", dest="min_num_atoms", default=50, type=int,
         help="Minimum number of atoms")
     parser_supercell.add_argument(
         "--max_atoms", dest="max_num_atoms", default=300, type=int,
         help="Maximum number of atoms")
+    parser_supercell.add_argument(
+        "--no_symmetry_analysis", dest="analyze_symmetry", action="store_false",
+        help="Set if symmetry is not analyzed. If set, sites.yaml file is "
+             "required.")
+    parser_supercell.add_argument(
+        "-s", "--sites_yaml_filename", type=str,
+        help="e.g., sites.yaml")
 
     parser_supercell.set_defaults(func=make_supercell)
 
     # -- append_interstitial ------------------------------------------------
     parser_append_interstitial = subparsers.add_parser(
         name="append_interstitial",
         description="Append interstitial information to supercell_info.yaml",
@@ -313,30 +318,30 @@
     parser_calc_summary.set_defaults(
         func=make_calc_summary_main_func)
 
     # -- plot defect formation energy ------------------------------------------
     parser_plot_energy = subparsers.add_parser(
         name="plot_defect_formation_energy",
         description="Show and plot defect formation energies.",
-        parents=[defect_e_label, defect_e_sum_parser],
+        parents=[defect_e_sum_parser],
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         aliases=['pe'])
 
     parser_plot_energy.add_argument(
         "-y", "--y_range", nargs=2, type=float,
         help="Energy range in y-axis")
     parser_plot_energy.add_argument(
         "--no_label_line", dest="label_line", action="store_false",
         help="Set the labels not to locate on the lines.")
     parser_plot_energy.add_argument(
         "--no_add_charges", dest="add_charges", action="store_false",
         help="Set the charges not to appear.")
     parser_plot_energy.add_argument(
         "--plot_all_energies", dest="plot_all_energies", action="store_true",
-        help="Set the charges not to appear.")
+        help="Plot energies of all charge states including unstable ones.")
     parser_plot_energy.set_defaults(func=plot_defect_energy)
     # ------------------------------------------------------------------------
     return parser.parse_args(args)
 
 
 def main():
     args = parse_args_main(sys.argv[1:])
```

### Comparing `pydefect-0.7.0/pydefect/cli/main_functions.py` & `pydefect-0.7.1/pydefect/cli/main_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 #  Copyright (c) 2020 Kumagai group.
 from pathlib import Path
 from typing import Union
 
+from matplotlib import pyplot as plt
 from monty.serialization import loadfn
 from pydefect.analyzer.calc_results import CalcResults, NoElectronicConvError, \
     NoIonicConvError
 from pydefect.analyzer.defect_energy import DefectEnergyInfo
 from pydefect.analyzer.defect_energy_plotter import DefectEnergyMplPlotter
 from pydefect.analyzer.make_band_edge_states import make_band_edge_states
 from pydefect.analyzer.make_calc_summary import make_calc_summary
@@ -20,19 +21,20 @@
 from pydefect.chem_pot_diag.cpd_plotter import ChemPotDiag2DMplPlotter, \
     ChemPotDiag3DMplPlotter
 from pydefect.cli.main_tools import sanitize_matrix, parse_dirs
 from pydefect.cli.vasp.make_efnv_correction import make_efnv_correction
 from pydefect.corrections.site_potential_plotter import SitePotentialMplPlotter
 from pydefect.input_maker.append_interstitial import append_interstitial
 from pydefect.input_maker.defect_set_maker import DefectSetMaker
+from pydefect.input_maker.manual_supercell_maker import ManualSupercellMaker, \
+    make_sites_from_yaml_file
 from pydefect.input_maker.supercell_maker import SupercellMaker
 from pymatgen.analysis.phase_diagram import PDPlotter
 from pymatgen.core import Composition
 from vise.util.logger import get_logger
-from matplotlib import pyplot as plt
 
 logger = get_logger(__name__)
 
 
 def get_calc_results(d: Path, check: bool) -> Union[CalcResults, bool]:
     if check:
         try:
@@ -103,24 +105,30 @@
 
     plt = plotter.draw_diagram()
     plt.savefig(fname="cpd.pdf")
     plt.show()
 
 
 def make_supercell(args):
+    kwargs = {}
+    if args.analyze_symmetry:
+        supercell_maker = SupercellMaker
+    else:
+        supercell_maker = ManualSupercellMaker
+        kwargs["sites"] = make_sites_from_yaml_file(args.sites_yaml_filename)
+
     if args.matrix:
         matrix = sanitize_matrix(args.matrix)
-        maker = SupercellMaker(args.unitcell, matrix)
+        maker = supercell_maker(args.unitcell, matrix=matrix, **kwargs)
     else:
-        kwargs = {}
         if args.min_num_atoms:
             kwargs["min_num_atoms"] = args.min_num_atoms
         if args.max_num_atoms:
             kwargs["max_num_atoms"] = args.max_num_atoms
-        maker = SupercellMaker(args.unitcell, **kwargs)
+        maker = supercell_maker(args.unitcell, **kwargs)
 
     maker.supercell.structure.to(filename="SPOSCAR")
     maker.supercell_info.to_json_file()
 
 
 def append_interstitial_to_supercell_info(args):
     supercell_info = append_interstitial(args.supercell_info,
@@ -265,9 +273,10 @@
         chem_pot_label=args.label,
         y_range=args.y_range,
         allow_shallow=args.allow_shallow,
         with_corrections=args.with_corrections,
         label_line=args.label_line,
         add_charges=args.add_charges,
         add_thin_lines=args.plot_all_energies)
+
     plotter.construct_plot()
     plotter.plt.savefig(f"energy_{args.label}.pdf")
```

### Comparing `pydefect-0.7.0/pydefect/cli/main_tools.py` & `pydefect-0.7.1/pydefect/cli/main_tools.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/make_defect_vesta_file.py` & `pydefect-0.7.1/pydefect/cli/make_defect_vesta_file.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/get_defect_charge_state.py` & `pydefect-0.7.1/pydefect/cli/vasp/get_defect_charge_state.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/main_vasp.py` & `pydefect-0.7.1/pydefect/cli/vasp/main_vasp.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/main_vasp_functions.py` & `pydefect-0.7.1/pydefect/cli/vasp/main_vasp_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,24 +124,24 @@
 
 
 def make_calc_results(args):
     file_name = "calc_results.json"
 
     def _inner(_dir: Path):
         calc_results = make_calc_results_from_vasp(
-            vasprun=Vasprun(_dir / defaults.vasprun),
+            vasprun=Vasprun(_dir / defaults.vasprun, parse_potcar_file=False),
             outcar=Outcar(_dir / defaults.outcar))
         calc_results.to_json_file(str(_dir / file_name))
 
     parse_dirs(args.dirs, _inner, args.verbose, file_name)
 
 
 def make_perfect_band_edge_state(args):
     procar = Procar(args.dir / defaults.procar)
-    vasprun = Vasprun(args.dir / defaults.vasprun)
+    vasprun = Vasprun(args.dir / defaults.vasprun, parse_potcar_file=False)
     outcar = Outcar(args.dir / defaults.outcar)
     perfect_band_edge_state = \
         make_perfect_band_edge_state_from_vasp(procar, vasprun, outcar)
     perfect_band_edge_state.to_json_file(
         args.dir / "perfect_band_edge_state.json")
 
 
@@ -154,15 +154,15 @@
     def _inner(_dir: Path):
         try:
             defect_entry = loadfn(_dir / "defect_entry.json")
             title = defect_entry.name
         except FileNotFoundError:
             title = "No name"
         procar = Procar(_dir / defaults.procar)
-        vasprun = Vasprun(_dir / defaults.vasprun)
+        vasprun = Vasprun(_dir / defaults.vasprun, parse_potcar_file=False)
 
         str_info = None
         if args.no_participation_ratio is False:
             str_info = loadfn(_dir / "defect_structure_info.json")
 
         band_edge_orb_infos = make_band_edge_orbital_infos(
             procar, vasprun, supercell_vbm, supercell_cbm, str_info)
```

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/main_vasp_util.py` & `pydefect-0.7.1/pydefect/cli/vasp/main_vasp_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,29 +8,31 @@
 
 from monty.serialization import loadfn
 from pydefect.analyzer.grids import Grids
 from pydefect.cli.main import epilog, description, add_sub_parser
 from pydefect.cli.vasp.main_vasp_util_functions import \
     make_parchg_dir, make_refine_defect_poscar, \
     calc_charge_state, make_defect_entry_main, calc_grids, \
-    make_defect_charge_info_main
+    make_defect_charge_info_main, make_total_dos
 from pymatgen.core import Structure
-from pymatgen.io.vasp import Chgcar
+from pymatgen.io.vasp import Chgcar, Vasprun, Outcar
 from pymatgen.io.vasp.inputs import UnknownPotcarWarning
+from vise.defaults import defaults
 
 warnings.simplefilter('ignore', UnknownPotcarWarning)
 
 
 def parse_args_main_vasp_util(args):
     parser = argparse.ArgumentParser(epilog=epilog,
                                      description=description + """      
     This command provides some utilities related to the VASP calculations""")
 
     subparsers = parser.add_subparsers()
     dir_parser = add_sub_parser(argparse, name="dir")
+    vasprun_parser = add_sub_parser(argparse, name="dir")
 
     # -- calc charge state -----------------------------------------------------
     parser_calc_charge_state = subparsers.add_parser(
         name="calc_charge_state",
         description="Calc defect charge states from INCAR, POSCAR and POTCAR"
                     "files.",
         parents=[dir_parser],
@@ -107,14 +109,28 @@
     parser_calc_def_charge_info.add_argument(
         "-b", "--bin_interval", type=float, default=0.2)
     parser_calc_def_charge_info.add_argument(
         "-g", "--grids", type=Grids.from_file, required=True)
 
     parser_calc_def_charge_info.set_defaults(func=make_defect_charge_info_main)
 
+    # -- make total dos for defect and carrier density -------------------------
+    parser_make_total_dos = subparsers.add_parser(
+        name="make_total_dos",
+        description="make total dos for defect and carrier density.",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        aliases=['mtd'])
+    parser_make_total_dos.add_argument(
+        "-v", "--vasprun", type=Vasprun, default=defaults.vasprun,
+        help="vasprun.xml file name.")
+    parser_make_total_dos.add_argument(
+        "-o", "--outcar", type=Outcar, default=defaults.outcar,
+        help="OUTCAR file name.")
+    parser_make_total_dos.set_defaults(func=make_total_dos)
+    # ----------------------------------------------------------------
     return parser.parse_args(args)
 
 
 def main():
     args = parse_args_main_vasp_util(sys.argv[1:])
     args.func(args)
```

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/main_vasp_util_functions.py` & `pydefect-0.7.1/pydefect/cli/vasp/main_vasp_util_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # -*- coding: utf-8 -*-
 #  Copyright (c) 2020 Kumagai group.
 import os
 from pathlib import Path
 
 from monty.serialization import loadfn
 from pydefect.analyzer.calc_results import CalcResults
+from pydefect.analyzer.concentration.make_concentration import TotalDos
 from pydefect.analyzer.grids import Grids
 from pydefect.analyzer.refine_defect_structure import refine_defect_structure
 from pydefect.cli.vasp.make_defect_charge_info import make_defect_charge_info
 from pydefect.cli.vasp.get_defect_charge_state import get_defect_charge_state
 from pydefect.input_maker.defect_entry import make_defect_entry
 from pymatgen.core import Structure
+from pymatgen.electronic_structure.core import Spin
 from pymatgen.io.vasp import Chgcar
+from vise.analyzer.vasp.band_edge_properties import VaspBandEdgeProperties
 from vise.input_set.incar import ViseIncar
 from vise.util.file_transfer import FileLink
 from vise.util.logger import get_logger
 from pymatgen.io.vasp.inputs import Poscar, Incar, Potcar
 
 logger = get_logger(__name__)
 
@@ -91,7 +94,18 @@
     defect_charge_info = make_defect_charge_info(
         parchgs, band_idxs, args.bin_interval, args.grids)
     defect_charge_info.to_json_file()
     plt = defect_charge_info.show_dist()
     plt.savefig("dist.pdf")
 
 
+def make_total_dos(args):
+    if Spin.down in args.vasprun.complete_dos.densities:
+        raise ValueError("Spin polarization is not supported yet.")
+    band_edge = VaspBandEdgeProperties(args.vasprun, args.outcar)
+    vbm, cbm = band_edge.vbm_info.energy, band_edge.cbm_info.energy
+
+    total_dos = TotalDos(args.vasprun.complete_dos.energies.tolist(),
+                         args.vasprun.complete_dos.densities[Spin.up].tolist(),
+                         args.vasprun.structures[0].volume,
+                         vbm, cbm)
+    total_dos.to_json_file()
```

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/make_band_edge_orbital_infos.py` & `pydefect-0.7.1/pydefect/cli/vasp/make_band_edge_orbital_infos.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/make_calc_results.py` & `pydefect-0.7.1/pydefect/cli/vasp/make_calc_results.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/make_composition_energies_from_mp.py` & `pydefect-0.7.1/pydefect/cli/vasp/make_composition_energies_from_mp.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/make_defect_charge_info.py` & `pydefect-0.7.1/pydefect/cli/vasp/make_defect_charge_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/make_efnv_correction.py` & `pydefect-0.7.1/pydefect/cli/vasp/make_efnv_correction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # -*- coding: utf-8 -*-
 #  Copyright (c) 2020. Distributed under the terms of the MIT License.
+from typing import Optional
 
 import numpy as np
 from numpy import dot, cross
 from numpy.linalg import norm
 
 from pydefect.analyzer.calc_results import CalcResults
 from pydefect.analyzer.defect_structure_comparator import \
     DefectStructureComparator
 from pydefect.corrections.efnv_correction import \
     ExtendedFnvCorrection, PotentialSite
 from pydefect.corrections.ewald import Ewald
 from pydefect.defaults import defaults
 from pydefect.util.error_classes import SupercellError
 from vise.util.logger import get_logger
-
+from vise.util.typing import Coords
 
 logger = get_logger(__name__)
 
 
-def make_efnv_correction(charge: int,
+def make_efnv_correction(charge: float,
                          calc_results: CalcResults,
                          perfect_calc_results: CalcResults,
                          dielectric_tensor: np.array,
+                         defect_coords: Optional[Coords] = None,
                          accuracy: float = defaults.ewald_accuracy,
                          unit_conversion: float = 180.95128169876497):
     """
     Notes:
     (1) The formula written in YK2014 need to be divided by 4pi in the SI unit.
     (2) When assuming an element charge locate at the defect_coords and
         angstrom for length, relative dielectric tensor, Multiply
@@ -35,15 +37,16 @@
     """
     if calc_results.structure.lattice != perfect_calc_results.structure.lattice:
         raise SupercellError("The lattice constants for defect and perfect "
                              "models are different")
 
     structure_analyzer = DefectStructureComparator(
         calc_results.structure, perfect_calc_results.structure)
-    defect_coords = structure_analyzer.defect_center_coord
+    if defect_coords is None:
+        defect_coords = structure_analyzer.defect_center_coord
     lattice = calc_results.structure.lattice
     ewald = Ewald(lattice.matrix, dielectric_tensor, accuracy=accuracy)
     point_charge_correction = \
         0.0 if not charge else - ewald.lattice_energy * charge ** 2
 
     defect_region_radius = calc_max_sphere_radius(lattice.matrix)
```

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/make_gkfo_correction.py` & `pydefect-0.7.1/pydefect/cli/vasp/make_gkfo_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/make_local_extrema.py` & `pydefect-0.7.1/pydefect/cli/vasp/make_local_extrema.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/make_perfect_band_edge_state.py` & `pydefect-0.7.1/pydefect/cli/vasp/make_perfect_band_edge_state.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/make_poscars_from_query.py` & `pydefect-0.7.1/pydefect/cli/vasp/make_poscars_from_query.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/make_unitcell.py` & `pydefect-0.7.1/pydefect/cli/vasp/make_unitcell.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/molecules/H2O/POSCAR` & `pydefect-0.7.1/pydefect/cli/vasp/molecules/H2O/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/molecules/NH3/POSCAR` & `pydefect-0.7.1/pydefect/cli/vasp/molecules/NH3/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/molecules/NO2/POSCAR` & `pydefect-0.7.1/pydefect/cli/vasp/molecules/NO2/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/cli/vasp/molecules/molecule_data.yaml` & `pydefect-0.7.1/pydefect/cli/vasp/molecules/molecule_data.yaml`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/corrections/abstract_correction.py` & `pydefect-0.7.1/pydefect/corrections/abstract_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/corrections/efnv_correction.py` & `pydefect-0.7.1/pydefect/corrections/efnv_correction.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,26 +8,25 @@
 from pydefect.corrections.abstract_correction import Correction
 from tabulate import tabulate
 
 
 @dataclass
 class ExtendedFnvCorrection(Correction):
     """
-    species: Species except for the defect. e.g., ["Mg", "Mg", ..., "O", ..]
-    atomic_coords: Fractional coordinates except for the defect.
-    pc_pot (list of float):
-        List of point-charge potential from the defect for all the
-        atomic sites.
+    charge: Defect charge
+    point_charge_correction: Correction energy for point charge interactions
     defect_region_radius (float):
         Maximum radius of a sphere touching to the lattice plane, used
         for defining the outside region of the defect.
+    sites: Site potentials
+    defect_coords: Position of defect site in fractional coordinates
 
     Add units of length and potential
     """
-    charge: int
+    charge: float
     point_charge_correction: float
     defect_region_radius: float
     sites: List["PotentialSite"]
     defect_coords: Tuple[float, float, float]
 
     def __str__(self):
         d = [["charge", self.charge],
```

### Comparing `pydefect-0.7.0/pydefect/corrections/ewald.py` & `pydefect-0.7.1/pydefect/corrections/ewald.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/corrections/gkfo_correction.py` & `pydefect-0.7.1/pydefect/corrections/gkfo_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/corrections/site_potential_plotter.py` & `pydefect-0.7.1/pydefect/corrections/site_potential_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,34 +52,36 @@
 class SitePotentialPlotter:
     def __init__(self,
                  title: str,
                  sites: List[PotentialSite],
                  defect_region_radius: float,
                  ave_pot_diff: float,
                  x_unit: Optional[str] = "Å",
-                 y_unit: Optional[str] = "V"):
+                 y_unit: Optional[str] = "V",
+                 **kwargs):
         self._title = title
         self.sites = sites
         self.defect_region_radius = defect_region_radius
         self.ave_pot_diff = ave_pot_diff
 
         self._x_unit = x_unit
         self._y_unit = y_unit
 
     @classmethod
     def from_efnv_corr(cls,
                        title,
                        efnv_correction: ExtendedFnvCorrection,
                        x_unit: Optional[str] = "Å",
-                       y_unit: Optional[str] = "V"):
+                       y_unit: Optional[str] = "V",
+                       **kwargs):
         return cls(title=title,
                    sites=efnv_correction.sites,
                    defect_region_radius=efnv_correction.defect_region_radius,
                    ave_pot_diff=efnv_correction.average_potential_diff,
-                   x_unit=x_unit, y_unit=y_unit)
+                   x_unit=x_unit, y_unit=y_unit, **kwargs)
 
     @classmethod
     def from_gkfo_corr(cls,
                        title,
                        gkfo_correction: GkfoCorrection,
                        x_unit: Optional[str] = "Å",
                        y_unit: Optional[str] = "V"):
```

### Comparing `pydefect-0.7.0/pydefect/database/database.py` & `pydefect-0.7.1/pydefect/database/database.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/database/electronegativity.yaml` & `pydefect-0.7.1/pydefect/database/electronegativity.yaml`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/database/rcore.yaml` & `pydefect-0.7.1/pydefect/database/rcore.yaml`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/defaults.py` & `pydefect-0.7.1/pydefect/defaults.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/input_maker/append_interstitial.py` & `pydefect-0.7.1/pydefect/input_maker/append_interstitial.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/input_maker/defect.py` & `pydefect-0.7.1/pydefect/input_maker/defect.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/input_maker/defect_entries_maker.py` & `pydefect-0.7.1/pydefect/input_maker/defect_entries_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/input_maker/defect_entry.py` & `pydefect-0.7.1/pydefect/input_maker/defect_entry.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/input_maker/defect_set.py` & `pydefect-0.7.1/pydefect/input_maker/defect_set.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/input_maker/defect_set_maker.py` & `pydefect-0.7.1/pydefect/input_maker/defect_set_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/input_maker/local_extrema.py` & `pydefect-0.7.1/pydefect/input_maker/local_extrema.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/input_maker/supercell.py` & `pydefect-0.7.1/pydefect/input_maker/supercell.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 
         self.supercells = []
         matrix = np.eye(3, dtype=int)
         for i in range(50):
             if det(matrix) > max_det:
                 break
             if det(matrix) > min_det:
-                self.supercells.append(Supercell(input_structure, matrix))
+                self.supercells.append(Supercell(input_structure,
+                                                 matrix.tolist()))
             matrix = self.incremented_matrix(matrix)
 
     def incremented_matrix(self, matrix: np.ndarray):
         abc = (self.input_structure * matrix).lattice.lengths
         min_indices = [i for i, val in enumerate(abc) if val == min(abc)]
         new_matrix = deepcopy(matrix)
         for index in min_indices:
```

### Comparing `pydefect-0.7.0/pydefect/input_maker/supercell_info.py` & `pydefect-0.7.1/pydefect/input_maker/supercell_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #  Copyright (c) 2020. Distributed under the terms of the MIT License.
 from dataclasses import dataclass, field
-from typing import List, Dict
+from typing import List, Dict, Optional, Union
 
 from monty.json import MSONable
 from numpy.linalg import det
 from pydefect.database.database import electronegativity, oxidation_state
 from pydefect.util.structure_tools import Distances
 from pymatgen.core import IStructure
 from vise.util.logger import get_logger
@@ -14,36 +14,53 @@
 
 logger = get_logger(__name__)
 
 
 @dataclass(frozen=True)
 class Interstitial(MSONable):
     frac_coords: List[float]
-    site_symmetry: str
+    site_symmetry: str = None
     info: str = None
 
 
+@dataclass
+class SimpleSite(MSONable):
+    element: str
+    site_index: int
+    site_symmetry: str = None
+    wyckoff_letter: str = None
+
+    @property
+    def pprint_equiv_atoms(self):
+        return None
+
+    @property
+    def equivalent_atoms(self):
+        return [self.site_index]
+
+
 @dataclass(frozen=True)
 class SupercellInfo(MSONable, ToJsonFileMixIn):
     structure: IStructure
     space_group: str
     transformation_matrix: List[List[int]]
-    sites: Dict[str, Site]
+    sites: Dict[str, Union[Site, SimpleSite]]
     interstitials: List[Interstitial] = field(default_factory=list)
     unitcell_structure: IStructure = None
 
     @classmethod
     def from_dict(cls, d):
         if "transform_matrix" in d:
             d["transformation_matrix"] = d.pop("transform_matrix")
         return super().from_dict(d)
 
     def coords(self, name):
         site = self.sites[name]
-        coord = list(self.structure[site.equivalent_atoms[0]].frac_coords)
+        site_idx = site.equivalent_atoms[0]
+        coord = list(self.structure[site_idx].frac_coords)
         distances = Distances(self.structure, coord)
         return distances.coordination()
 
     def interstitial_coords(self, idx: int):
         interstitial = self.interstitials[idx]
         distances = Distances(self.structure, interstitial.frac_coords)
         return distances.coordination(include_on_site=True)
@@ -57,25 +74,21 @@
         return '  '.join(str(x) for x in self.transformation_matrix)
 
     def _frac_coords(self, site):
         repr_atom_idx = site.equivalent_atoms[0]
         frac_coords = self.structure[repr_atom_idx].frac_coords
         return "{0[0]:9.7f}  {0[1]:9.7f}  {0[2]:9.7f}".format(frac_coords)
 
-    @staticmethod
-    def _stripe_numbers(name):
-        return ''.join([i for i in name if i.isalpha()])
-
     def __str__(self):
         lines = [f"Space group: {self.space_group}",
                  f"Transformation matrix: {self._transform_matrix_str}",
                  f"Cell multiplicity: {self.multiplicity}", ""]
 
         for name, site in self.sites.items():
-            elem = self._stripe_numbers(name)
+            elem = stripe_numbers(name)
             coordination = self.coords(name).distance_dict
             lines.append(f"   Irreducible element: {name}")
             lines.append(f"        Wyckoff letter: {site.wyckoff_letter}")
             lines.append(f"         Site symmetry: {site.site_symmetry}")
             lines.append(f"         Cutoff radius: {self.coords(name).cutoff}")
             lines.append(f"          Coordination: {coordination}")
             lines.append(f"      Equivalent atoms: {site.pprint_equiv_atoms}")
@@ -96,7 +109,11 @@
                 "{0[0]:9.7f}  {0[1]:9.7f}  {0[2]:9.7f}".format(site.frac_coords)
             lines.append(f"Fractional coordinates: {frac}")
             lines.append(f"         Site symmetry: {site.site_symmetry}")
             lines.append(f"          Coordination: {coordination}")
             lines.append("")
 
         return "\n".join(lines)
+
+
+def stripe_numbers(name):
+    return ''.join([i for i in name if i.isalpha()])
```

### Comparing `pydefect-0.7.0/pydefect/input_maker/supercell_maker.py` & `pydefect-0.7.1/pydefect/input_maker/supercell_maker.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,29 +17,31 @@
 
 logger = get_logger(__name__)
 
 
 class SupercellMaker:
     def __init__(self,
                  primitive_structure: IStructure,
-                 matrix_to_conv_cell: Optional[List[List[int]]] = None,
+                 # matrix_to_conv_cell
+                 matrix: Optional[List[List[int]]] = None,
                  symprec: float = defaults.symmetry_length_tolerance,
                  angle_tolerance: float = defaults.symmetry_angle_tolerance,
                  raise_error: bool = True,
                  **supercell_kwargs):
 
         self.primitive_structure = primitive_structure
         self.symmetrizer = StructureSymmetrizer(primitive_structure,
-                                           symprec=symprec,
-                                           angle_tolerance=angle_tolerance)
+                                                symprec=symprec,
+                                                angle_tolerance=angle_tolerance)
         if primitive_structure != self.symmetrizer.primitive:
             logger.warning(
                 "The input structure is different from the primitive one,"
                 "which might be due to the difference of symprec used in"
-                "the pydefect and unitcell conversion.")
+                "the pydefect and unitcell conversion. Please construct"
+                "the unitcell using vise.")
             logger.warning("\n".join([
                 "Input lattice:",
                 f"{primitive_structure.lattice}", "",
                 "Primitive structure lattice:",
                 f"{self.symmetrizer.primitive.lattice}", "",
                 "Input structure:",
                 f"{primitive_structure}", "",
@@ -52,15 +54,15 @@
         self.conv_structure = self.symmetrizer.conventional
         crystal_system, center = str(self.symmetrizer.bravais)
 
         centering = Centering(center)
         self.conv_multiplicity = centering.conv_multiplicity
         self.conv_trans_mat = centering.primitive_to_conv
 
-        self._matrix = matrix_to_conv_cell
+        self._matrix = matrix
         self._supercell_kwargs = supercell_kwargs
 
         self._generate_supercell(crystal_system)
         self._generate_supercell_info()
 
     def _generate_supercell(self, crystal_system):
         if self._matrix:
```

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/POSCAR` & `pydefect-0.7.1/pydefect/tests/analyzer/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_0/POSCAR` & `pydefect-0.7.1/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_0/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_2/POSCAR` & `pydefect-0.7.1/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_2/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_band_edge_states.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_band_edge_states.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_calc_results.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_calc_results.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_calc_summary.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_calc_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_defect_charge_info.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_defect_charge_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_defect_energy.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_defect_energy.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,14 +124,25 @@
         chem_pot_label="A", allow_shallow=True, with_corrections=True, e_range=(0.0, 2.0))
     expected = ChargeEnergies(
         charge_energies_dict={"Va_O": SingleChargeEnergies([(0, 2.0), (1, 3.0), (2, 4.0)])},
         e_min=0.0, e_max=2.0)
     assert actual == expected
 
 
+def test_defect_energy_summary_exclude_defects(defect_energy_summary):
+    actual = defect_energy_summary.screened_defect_energies(
+        allow_shallow=True, excluded_defects=["Va_O1_2"])
+    expected = {"Va_O1":
+                    DefectEnergies(
+                        {"O": -1}, charges=[0, 1],
+                        defect_energies=[DefectEnergy(1.0, {"corr": 2.0}, is_shallow=False),
+                                         DefectEnergy(2.0, {"corr": 2.0}, is_shallow=False)])}
+    assert actual == expected
+
+
 def test_cross_points_e_max_energies_dicts():
     charge_energies = ChargeEnergies(
         charge_energies_dict={"Va_Mg": SingleChargeEnergies([(0, 2.0)]),
                               "Va_O": SingleChargeEnergies([(1, 1.0)])},
         e_min=0.0, e_max=2.0)
     actual = charge_energies.cross_point_dicts
     expected = {"Va_Mg": CrossPoints(inner_cross_points=[],
@@ -141,14 +152,22 @@
     assert actual == expected
 
     actual = charge_energies.e_min_max_energies_dict
     expected = {"Va_Mg": [[2.0, 2.0]], "Va_O": [[1.0, 3.0]]}
     assert actual == expected
 
 
+def test_charge_energies_pinning_levels():
+    charge_energies = ChargeEnergies(
+        charge_energies_dict=
+        {"Va_O1": SingleChargeEnergies([(1, -1), (-1, 1.5)])},
+        e_min=0.0, e_max=2.0)
+    assert charge_energies.pinning_levels == {"Va_O1": [1.0, 1.5]}
+
+
 def test_defect_energy_summary_latexified_title(defect_energy_summary):
     actual = defect_energy_summary.latexified_title
     expected = "MgAl$_{2}$O$_{4}$"
     assert actual == expected
 
 
 @pytest.fixture
```

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_defect_energy_plotter.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_defect_energy_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_defect_energy_util.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_defect_energy_util.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_defect_structure_comparator.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_defect_structure_comparator.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_defect_structure_info.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_defect_structure_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_eigenvalue_plotter.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_eigenvalue_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_grids.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_grids.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_make_band_edge_states.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_make_band_edge_states.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_make_calc_summary.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_make_calc_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_make_defect_energy_info.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_make_defect_energy_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_make_defect_energy_summary.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_make_defect_energy_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_make_defect_structure_info.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_make_defect_structure_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_pinning_levels.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_pinning_levels.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_refine_defect_structure.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_refine_defect_structure.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_transition_levels.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_transition_levels.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/analyzer/test_transition_levels_plotter.py` & `pydefect-0.7.1/pydefect/tests/analyzer/test_transition_levels_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/cli/test_main.py` & `pydefect-0.7.1/pydefect/tests/cli/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,31 +44,37 @@
     parsed_args = parse_args_main(["s", "-p", "POSCAR-tmp"])
     # func is a pointer so need to point the same address.
     expected = Namespace(
         unitcell=mock.from_file.return_value,
         matrix=None,
         min_num_atoms=50,
         max_num_atoms=300,
+        analyze_symmetry=True,
+        sites_yaml_filename=None,
         func=parsed_args.func)
     assert parsed_args == expected
 
 
 def test_make_supercell_w_options(mocker):
     mock = mocker.patch("pydefect.cli.main.IStructure")
     parsed_args = parse_args_main(["s",
                                    "-p", "POSCAR-tmp",
                                    "--matrix", "1", "2", "3",
+                                   "--no_symmetry_analysis",
+                                   "-s", "sites.yaml",
                                    "--min_atoms", "1000",
                                    "--max_atoms", "2000"])
     # func is a pointer so need to point the same address.
     expected = Namespace(
         unitcell=mock.from_file.return_value,
         matrix=[1, 2, 3],
         min_num_atoms=1000,
         max_num_atoms=2000,
+        analyze_symmetry=False,
+        sites_yaml_filename="sites.yaml",
         func=parsed_args.func)
     assert parsed_args == expected
     mock.from_file.assert_called_once_with("POSCAR-tmp")
 
 
 def test_append_interstitial(mocker):
```

### Comparing `pydefect-0.7.0/pydefect/tests/cli/test_main_functions.py` & `pydefect-0.7.1/pydefect/tests/cli/test_main_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,33 +86,56 @@
     plot_chem_pot_diag(args)
 
 
 def test_make_supercell_from_matrix(simple_cubic, simple_cubic_2x1x1, tmpdir):
     tmpdir.chdir()
     matrix = [2, 1, 1]
     args = Namespace(unitcell=simple_cubic, matrix=matrix,
+                     analyze_symmetry=True,
+                     sites_yaml_filename=None,
                      min_num_atoms=None, max_num_atoms=None)
     make_supercell(args)
     info = loadfn("supercell_info.json")
     assert IStructure.from_file("SPOSCAR") == simple_cubic_2x1x1
     assert info.structure == simple_cubic_2x1x1
     assert info.transformation_matrix == [[2, 0, 0], [0, 1, 0], [0, 0, 1]]
 
 
 def test_make_recommended_supercell(simple_cubic, simple_cubic_2x2x2, tmpdir):
     tmpdir.chdir()
     args = Namespace(unitcell=simple_cubic, matrix=None,
+                     analyze_symmetry=True,
+                     sites_yaml_filename=None,
                      min_num_atoms=8, max_num_atoms=8)
     make_supercell(args)
     info = loadfn("supercell_info.json")
     assert IStructure.from_file("SPOSCAR") == simple_cubic_2x2x2
     assert info.structure == simple_cubic_2x2x2
     assert info.transformation_matrix == [[2, 0, 0], [0, 2, 0], [0, 0, 2]]
 
 
+def test_make_recommended_supercell2(simple_cubic, simple_cubic_2x2x2, tmpdir):
+    tmpdir.chdir()
+    Path("sites.yaml").write_text("""
+H1:
+  site_index: 0
+  site_symmetry: P1
+""")
+    args = Namespace(unitcell=simple_cubic, matrix=None,
+                     analyze_symmetry=False,
+                     sites_yaml_filename="sites.yaml",
+                     min_num_atoms=8, max_num_atoms=8)
+    make_supercell(args)
+    info = loadfn("supercell_info.json")
+    print(info)
+    assert IStructure.from_file("SPOSCAR") == simple_cubic_2x2x2
+    assert info.structure == simple_cubic_2x2x2
+    assert info.transformation_matrix == [[2, 0, 0], [0, 2, 0], [0, 0, 2]]
+
+
 def test_add_interstitials(mocker):
     mock_1 = mocker.Mock()
     mock_2 = mocker.Mock()
     mock_3 = mocker.Mock()
     mock_4 = mocker.Mock()
     args = Namespace(supercell_info=mock_1, base_structure=mock_2,
                      frac_coords=mock_3, info=mock_4)
```

### Comparing `pydefect-0.7.0/pydefect/tests/cli/test_main_tools.py` & `pydefect-0.7.1/pydefect/tests/cli/test_main_tools.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/cli/test_main_util.py` & `pydefect-0.7.1/pydefect/tests/cli/test_main_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,20 +34,22 @@
 
     # because add_sub_parser is imported from main, patch to loadfn should be
     # done in main.
     mocker.patch("pydefect.cli.main.loadfn", side_effect=side_effect)
     parsed_args = parse_args_main_util(["u",
                                         "-d", "defect_energy_summary.json",
                                         "--allow_shallow",
-                                        "--no_corrections"])
+                                        "--no_corrections",
+                                        "--label", "A"])
 
     expected = Namespace(
         defect_energy_summary=mock_summary,
         allow_shallow=True,
         with_corrections=False,
+        label="A",
         func=parsed_args.func)
     assert parsed_args == expected
 
 
 def test_add_interstitials_from_local_extrema(mocker):
 
     mock_loadfn_main = mocker.patch("pydefect.cli.main.loadfn")
```

### Comparing `pydefect-0.7.0/pydefect/tests/cli/test_main_util_functions.py` & `pydefect-0.7.1/pydefect/tests/cli/test_main_util_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # -*- coding: utf-8 -*-
 #  Copyright (c) 2020. Distributed under the terms of the MIT License.
 from argparse import Namespace
 from pathlib import Path
 
 import pytest
+from monty.serialization import loadfn
 from pydefect.analyzer.calc_results import CalcResults
+from pydefect.analyzer.concentration.degeneracy import Degeneracies
 from pydefect.analyzer.defect_energy import DefectEnergySummary, DefectEnergies, \
     DefectEnergy
 from pydefect.chem_pot_diag.chem_pot_diag import CompositionEnergies, \
     CompositionEnergy
 from pydefect.cli.main_util_functions import composition_energies_from_mp, \
     make_gkfo_correction_from_vasp, add_interstitials_from_local_extrema, \
-    make_defect_vesta_file, show_u_values, show_pinning_levels
+    make_defect_vesta_file, show_u_values, show_pinning_levels, \
+    calc_defect_concentrations
 from pydefect.corrections.efnv_correction import ExtendedFnvCorrection
 from pymatgen.core import Composition
 
 
 def test_composition_energies_from_mp(mocker, tmpdir):
     tmpdir.chdir()
     args = Namespace(elements=["H"], atom_energy_yaml="a.yaml")
@@ -114,7 +117,22 @@
         additional_charge=1,
         final_calc_results=mock_f_calc_results,
         initial_calc_results=mock_i_calc_results,
         diele_tensor=mock_unitcell.dielectric_constant,
         ion_clamped_diele_tensor=mock_unitcell.ele_dielectric_const)
 
 
+def test_calc_defect_concentrations(tmpdir, test_data_files):
+    tmpdir.chdir()
+    test_dir = test_data_files / "Na3AgO2"
+    summary = loadfn(test_dir / "defect_energy_summary.json")
+    degeneracies = Degeneracies.from_yaml(test_dir / "degeneracies.yaml")
+    args = Namespace(defect_energy_summary=summary,
+                     label="A",
+                     allow_shallow=False,
+                     with_corrections=True,
+                     total_dos=loadfn(test_dir / "total_dos.json"),
+                     degeneracies=degeneracies,
+                     T=300,
+                     con_by_Ef=None,
+                     net_abs_ratio=0.001)
+    calc_defect_concentrations(args)
```

### Comparing `pydefect-0.7.0/pydefect/tests/cli/test_make_defect_vesta_file.py` & `pydefect-0.7.1/pydefect/tests/cli/test_make_defect_vesta_file.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_get_defect_charge_state.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_get_defect_charge_state.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_main_vasp.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_main_vasp_functions.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,16 @@
     mock_vasprun = mocker.patch("pydefect.cli.vasp.main_vasp_functions.Vasprun")
     mock_outcar = mocker.patch("pydefect.cli.vasp.main_vasp_functions.Outcar")
     mock_calc_results = mocker.Mock(spec=CalcResults)
     mock.return_value = mock_calc_results
     args = Namespace(dirs=[Path("a")], verbose=False)
     make_calc_results(args)
 
-    mock_vasprun.assert_called_with(Path("a") / defaults.vasprun)
+    mock_vasprun.assert_called_with(Path("a") / defaults.vasprun,
+                                    parse_potcar_file=False)
     mock_outcar.assert_called_with(Path("a") / defaults.outcar)
     mock.assert_called_with(vasprun=mock_vasprun.return_value,
                             outcar=mock_outcar.return_value)
     mock_calc_results.to_json_file.assert_called_with("a/calc_results.json")
 
 
 def test_make_perfect_band_edge_state(mocker):
@@ -175,15 +176,16 @@
     mock_outcar = mocker.patch("pydefect.cli.vasp.main_vasp_functions.Outcar")
     mock_make_perf_be_state = mocker.patch(
         "pydefect.cli.vasp.main_vasp_functions.make_perfect_band_edge_state_from_vasp")
 
     args = Namespace(dir=Path("perfect"))
     make_perfect_band_edge_state(args)
 
-    mock_vasprun.assert_called_with(Path("perfect") / defaults.vasprun)
+    mock_vasprun.assert_called_with(Path("perfect") / defaults.vasprun,
+                                    parse_potcar_file=False)
     mock_procar.assert_called_with(Path("perfect") / defaults.procar)
     mock_outcar.assert_called_with(Path("perfect") / defaults.outcar)
     mock_make_perf_be_state.assert_called_with(mock_procar.return_value,
                                                mock_vasprun.return_value,
                                                mock_outcar.return_value)
 
 
@@ -221,15 +223,16 @@
                      p_state=mock_p_state,
                      y_range=[0.0, 1.0],
                      no_participation_ratio=False,
                      verbose=False)
     make_band_edge_orb_infos_and_eigval_plot(args)
 
     mock_procar.assert_called_with(Path("Va_O1_2") / defaults.procar)
-    mock_vasprun.assert_called_with(Path("Va_O1_2") / defaults.vasprun)
+    mock_vasprun.assert_called_with(Path("Va_O1_2") / defaults.vasprun,
+                                    parse_potcar_file=False)
 
     mock_make_orbital_infos.assert_called_with(
         mock_procar.return_value, mock_vasprun.return_value, 10, 20,
         mock_structure_info)
 
     mock_loadfn.assert_any_call(Path("Va_O1_2") / "defect_entry.json")
```

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_main_vasp_util.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp_util.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_main_vasp_util_functions.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp_util_functions.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_band_edge_orbital_infos.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_band_edge_orbital_infos.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_calc_results.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_calc_results.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #  Copyright (c) 2020. Distributed under the terms of the MIT License.
 from pydefect.cli.vasp.make_calc_results import make_calc_results_from_vasp
 from pymatgen.core import Structure
 from pymatgen.io.vasp import Vasprun, Outcar
 
 
 def test_make_calc_results_from_vasp_results(vasp_files):
-    vasprun = Vasprun(vasp_files / "MgO_conv_Va_O_0" / "vasprun.xml")
+    vasprun = Vasprun(vasp_files / "MgO_conv_Va_O_0" / "vasprun.xml", parse_potcar_file=False)
     outcar = Outcar(vasp_files / "MgO_conv_Va_O_0" / "OUTCAR")
     results = make_calc_results_from_vasp(vasprun, outcar)
 
     expected_structure = \
         Structure.from_file(vasp_files / "MgO_conv_Va_O_0" / "CONTCAR")
     assert results.structure == expected_structure
     assert results.energy == -34.91084360
```

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_composition_energies_from_mp.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_composition_energies_from_mp.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_defect_charge_info.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_defect_charge_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_efnv_correction.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_efnv_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_gkfo_correction.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_gkfo_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_local_extrema.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_local_extrema.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_perfect_band_edge_state.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_perfect_band_edge_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pydefect.cli.vasp.make_perfect_band_edge_state import \
     make_perfect_band_edge_state_from_vasp
 from pymatgen.io.vasp import Procar, Vasprun, Outcar
 
 
 def test_make_perfect_band_edge_state_from_vasp(vasp_files):
     procar = Procar(vasp_files / "MgO_2x2x2_perfect" / "PROCAR")
-    vasprun = Vasprun(vasp_files / "MgO_2x2x2_perfect" / "vasprun.xml")
+    vasprun = Vasprun(vasp_files / "MgO_2x2x2_perfect" / "vasprun.xml", parse_potcar_file=False)
     outcar = Outcar(vasp_files / "MgO_2x2x2_perfect" / "OUTCAR")
     actual = make_perfect_band_edge_state_from_vasp(procar, vasprun, outcar)
 
     vbm_info = EdgeInfo(
         band_idx=127, kpt_coord=(0.25, 0.25, 0.25),
         orbital_info=OrbitalInfo(energy=2.7746,
                                  orbitals={'Mg': [0.0, 0.0, 0.0, 0.0],
```

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_poscars_from_query.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_poscars_from_query.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/cli/vasp/test_make_unitcell.py` & `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_unitcell.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
           -0.000000     1.255879     0.000000
           -0.000000     0.000000     1.255879
  ------------------------------------------------------
     """
 
     path = vasp_files / "unitcell_Ne_solid"
     unitcell = make_unitcell_from_vasp(
-        vasprun_band=Vasprun(path / "vasprun-band.xml"),
+        vasprun_band=Vasprun(path / "vasprun-band.xml", parse_potcar_file=False),
         outcar_band=Outcar(path / "OUTCAR-band"),
         outcar_dielectric_clamped=Outcar(path / "OUTCAR-dielectric"),
         outcar_dielectric_ionic=Outcar(path / "OUTCAR-dielectric"),
         )
 
     assert unitcell.system == "Ne"
     assert unitcell.vbm == -10.3168
```

### Comparing `pydefect-0.7.0/pydefect/tests/conftest.py` & `pydefect-0.7.1/pydefect/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,22 @@
     ExtendedFnvCorrection
 from pydefect.input_maker.local_extrema import VolumetricDataAnalyzeParams
 from pydefect.input_maker.supercell_info import Site, SupercellInfo, \
     Interstitial
 from pymatgen.core import Lattice, IStructure, Structure
 
 sys.path.append(os.path.join(os.path.dirname(__file__), 'helpers'))
-# Need the following the share the fixture
+
+
+# Need the following to share the fixture
+
+
+@pytest.fixture(scope="session")
+def test_data_files():
+    return Path(__file__).parent / "test_data_files"
 
 
 @pytest.fixture(scope="session")
 def vasp_files():
     return Path(__file__).parent / "cli" / "vasp" / "vasp_files"
```

### Comparing `pydefect-0.7.0/pydefect/tests/corrections/test_efnv_correction.py` & `pydefect-0.7.1/pydefect/tests/corrections/test_efnv_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/corrections/test_efnv_performance.py` & `pydefect-0.7.1/pydefect/tests/corrections/test_efnv_performance.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/corrections/test_ewald.py` & `pydefect-0.7.1/pydefect/tests/corrections/test_ewald.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/corrections/test_gkfo_correction.py` & `pydefect-0.7.1/pydefect/tests/corrections/test_gkfo_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/corrections/test_site_potential_plotter.py` & `pydefect-0.7.1/pydefect/tests/corrections/test_site_potential_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/input_maker/test_append_interstitial.py` & `pydefect-0.7.1/pydefect/tests/input_maker/test_append_interstitial.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/input_maker/test_defect.py` & `pydefect-0.7.1/pydefect/tests/input_maker/test_defect.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/input_maker/test_defect_entries_maker.py` & `pydefect-0.7.1/pydefect/tests/input_maker/test_defect_entries_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/input_maker/test_defect_entry.py` & `pydefect-0.7.1/pydefect/tests/input_maker/test_defect_entry.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/input_maker/test_defect_set.py` & `pydefect-0.7.1/pydefect/tests/input_maker/test_defect_set.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/input_maker/test_defect_set_maker.py` & `pydefect-0.7.1/pydefect/tests/input_maker/test_defect_set_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/input_maker/test_local_extrema.py` & `pydefect-0.7.1/pydefect/tests/input_maker/test_local_extrema.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/input_maker/test_supercell.py` & `pydefect-0.7.1/pydefect/tests/input_maker/test_supercell.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/tests/input_maker/test_supercell_info.py` & `pydefect-0.7.1/pydefect/tests/input_maker/test_supercell_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 #  Copyright (c) 2020. Distributed under the terms of the MIT License.
 
 import pytest
 from pydefect.defaults import defaults
 
-from pydefect.input_maker.supercell_info import Interstitial, SupercellInfo
+from pydefect.input_maker.supercell_info import Interstitial, SupercellInfo, \
+    SimpleSite
 from pydefect.util.structure_tools import Coordination
 from vise.tests.helpers.assertion import assert_msonable, assert_json_roundtrip
 
 
 @pytest.fixture
 def interstitial():
     return Interstitial(frac_coords=[0.25, 0.25, 0.25],
@@ -81,14 +82,51 @@
       Equivalent atoms: 4..7
 Fractional coordinates: 0.0000000  0.0000000  0.5000000
      Electronegativity: None
        Oxidation state: 0
 
 -- interstitials
 #1
+                  Info: test
+Fractional coordinates: 0.2500000  0.2500000  0.2500000
+         Site symmetry: yy
+          Coordination: {'H': [2.62, 2.62, 2.62, 2.62], 'He': [2.62, 2.62, 2.62, 2.62]}
+"""
+    assert str(supercell_info) == expected
+
+
+def test_supercell_info_wo_symmetry_info(supercell_info: SupercellInfo):
+    supercell_info.sites["H1"] = SimpleSite("H", 0)
+    print(supercell_info)
+    expected = """Space group: Fmmm
+Transformation matrix: [1, 0, 0]  [0, 1, 0]  [0, 0, 1]
+Cell multiplicity: 1
+
+   Irreducible element: H1
+        Wyckoff letter: None
+         Site symmetry: None
+         Cutoff radius: 3.25
+          Coordination: {'He': [2.5, 3.0]}
+      Equivalent atoms: None
+Fractional coordinates: 0.0000000  0.0000000  0.0000000
+     Electronegativity: 2.2
+       Oxidation state: 1
+
+   Irreducible element: He1
+        Wyckoff letter: b
+         Site symmetry: mmm
+         Cutoff radius: 3.25
+          Coordination: {'H': [2.5, 3.0]}
+      Equivalent atoms: 4..7
+Fractional coordinates: 0.0000000  0.0000000  0.5000000
+     Electronegativity: None
+       Oxidation state: 0
+
+-- interstitials
+#1
                   Info: test
 Fractional coordinates: 0.2500000  0.2500000  0.2500000
          Site symmetry: yy
           Coordination: {'H': [2.62, 2.62, 2.62, 2.62], 'He': [2.62, 2.62, 2.62, 2.62]}
 """
     assert str(supercell_info) == expected
```

### Comparing `pydefect-0.7.0/pydefect/tests/input_maker/test_supercell_maker.py` & `pydefect-0.7.1/pydefect/tests/input_maker/test_supercell_maker.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,24 +33,24 @@
 def test_create_supercell_raise_not_primitive_error(bcc):
     with pytest.raises(NotPrimitiveError):
         SupercellMaker(primitive_structure=bcc)
 
 
 def test_create_supercell_matrix(a_centered_orthorhombic):
     matrix = [[2, 0, 0], [0, 1, 0], [0, 0, 1]]
-    cs = SupercellMaker(a_centered_orthorhombic, matrix_to_conv_cell=matrix)
+    cs = SupercellMaker(a_centered_orthorhombic, matrix=matrix)
     actual = cs.supercell.matrix
     np.testing.assert_array_equal(actual, matrix)
 
     expected = [[2, 0, 0], [0, 1, -1], [0, 1, 1]]
     np.testing.assert_array_equal(cs.transformation_matrix, expected)
 
 
 def test_create_supercell_generate_supercell_info(simple_cubic):
-    cs = SupercellMaker(simple_cubic, matrix_to_conv_cell=[[2, 0, 0], [0, 2, 0], [0, 0, 2]])
+    cs = SupercellMaker(simple_cubic, matrix=[[2, 0, 0], [0, 2, 0], [0, 0, 2]])
     info = cs.supercell_info
     assert info.transformation_matrix == [[2, 0, 0], [0, 2, 0], [0, 0, 2]]
     assert info.sites["H1"].wyckoff_letter == "a"
     assert info.sites["H1"].equivalent_atoms == list(range(8))
     assert info.unitcell_structure == simple_cubic
 
 
@@ -102,20 +102,20 @@
 4 
 direct
 0.000000 0.500000 0.250000 Si
 0.500000 1.000000 0.750000 Si
 0.000000 0.000000 0.000000 Si
 0.500000 0.500000 0.500000 Si""", fmt="poscar")
 
-    matrix_to_conv_cell = [[3, 0, 0], [0, 3, 0], [0, 0, 2]]
+    matrix = [[3, 0, 0], [0, 3, 0], [0, 0, 2]]
     sm = SupercellMaker(structure,
-                        matrix_to_conv_cell=matrix_to_conv_cell,
+                        matrix=matrix,
                         symprec=0.01)
     actual = structure * sm.transformation_matrix
-    expected = conv_structure * matrix_to_conv_cell
+    expected = conv_structure * matrix
     assert_structure_almost_same(actual, expected)
 
 
 def test_rhombohedral_supercell_info():
     """There is a bug in spglib to find the inequivalent sites in supercell"""
     structure = Structure.from_str("""    Ba4 Nb2 W1 O12
 1.00000000000000
```

### Comparing `pydefect-0.7.0/pydefect/util/mp_tools.py` & `pydefect-0.7.1/pydefect/util/mp_tools.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/util/prepare_names.py` & `pydefect-0.7.1/pydefect/util/prepare_names.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect/util/structure_tools.py` & `pydefect-0.7.1/pydefect/util/structure_tools.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.0/pydefect.egg-info/SOURCES.txt` & `pydefect-0.7.1/pydefect.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 MANIFEST.in
 README.md
 setup.py
 pydefect/__init__.py
 pydefect/defaults.py
 pydefect/error.py
+pydefect-0.7.0/pydefect/cli/vasp/molecules/molecule_data.yaml
+pydefect-0.7.0/pydefect/cli/vasp/molecules/H2/POSCAR
+pydefect-0.7.0/pydefect/cli/vasp/molecules/H2/prior_info.yaml
+pydefect-0.7.0/pydefect/cli/vasp/molecules/H2O/POSCAR
+pydefect-0.7.0/pydefect/cli/vasp/molecules/H2O/prior_info.yaml
+pydefect-0.7.0/pydefect/cli/vasp/molecules/N2/POSCAR
+pydefect-0.7.0/pydefect/cli/vasp/molecules/N2/prior_info.yaml
+pydefect-0.7.0/pydefect/cli/vasp/molecules/NH3/POSCAR
+pydefect-0.7.0/pydefect/cli/vasp/molecules/NH3/prior_info.yaml
+pydefect-0.7.0/pydefect/cli/vasp/molecules/NO2/POSCAR
+pydefect-0.7.0/pydefect/cli/vasp/molecules/NO2/prior_info.yaml
+pydefect-0.7.0/pydefect/cli/vasp/molecules/O2/POSCAR
+pydefect-0.7.0/pydefect/cli/vasp/molecules/O2/prior_info.yaml
+pydefect-0.7.0/pydefect/database/electronegativity.yaml
+pydefect-0.7.0/pydefect/database/oxidation_state.yaml
+pydefect-0.7.0/pydefect/database/rcore.yaml
+pydefect-0.7.0/pydefect/tests/analyzer/POSCAR
 pydefect.egg-info/PKG-INFO
 pydefect.egg-info/SOURCES.txt
 pydefect.egg-info/dependency_links.txt
 pydefect.egg-info/entry_points.txt
 pydefect.egg-info/requires.txt
 pydefect.egg-info/top_level.txt
 pydefect/analyzer/__init__.py
@@ -29,14 +46,20 @@
 pydefect/analyzer/make_defect_energy_summary.py
 pydefect/analyzer/make_defect_structure_info.py
 pydefect/analyzer/pinning_levels.py
 pydefect/analyzer/refine_defect_structure.py
 pydefect/analyzer/transition_levels.py
 pydefect/analyzer/transition_levels_plotter.py
 pydefect/analyzer/unitcell.py
+pydefect/analyzer/concentration/__init__.py
+pydefect/analyzer/concentration/concentration.py
+pydefect/analyzer/concentration/degeneracy.py
+pydefect/analyzer/concentration/distribution_function.py
+pydefect/analyzer/concentration/make_concentration.py
+pydefect/analyzer/concentration/plot_concentration.py
 pydefect/analyzer/dash_components/__init__.py
 pydefect/analyzer/dash_components/cpd_energy_dash.py
 pydefect/analyzer/dash_components/cpd_energy_dash_demo.py
 pydefect/analyzer/dash_components/cpd_plotter_main.py
 pydefect/analyzer/dash_components/main.py
 pydefect/analyzer/dash_components/scenes_from_volumetric_data.py
 pydefect/chem_pot_diag/__init__.py
@@ -90,20 +113,23 @@
 pydefect/database/__init__.py
 pydefect/database/database.py
 pydefect/database/electronegativity.yaml
 pydefect/database/oxidation_state.yaml
 pydefect/database/rcore.yaml
 pydefect/input_maker/__init__.py
 pydefect/input_maker/append_interstitial.py
+pydefect/input_maker/complex_defect_entries_make.py
+pydefect/input_maker/complex_defect_set.py
 pydefect/input_maker/defect.py
 pydefect/input_maker/defect_entries_maker.py
 pydefect/input_maker/defect_entry.py
 pydefect/input_maker/defect_set.py
 pydefect/input_maker/defect_set_maker.py
 pydefect/input_maker/local_extrema.py
+pydefect/input_maker/manual_supercell_maker.py
 pydefect/input_maker/supercell.py
 pydefect/input_maker/supercell_info.py
 pydefect/input_maker/supercell_maker.py
 pydefect/tests/__init__.py
 pydefect/tests/conftest.py
 pydefect/tests/analyzer/POSCAR
 pydefect/tests/analyzer/__init__.py
@@ -124,14 +150,20 @@
 pydefect/tests/analyzer/test_make_defect_energy_summary.py
 pydefect/tests/analyzer/test_make_defect_structure_info.py
 pydefect/tests/analyzer/test_pinning_levels.py
 pydefect/tests/analyzer/test_refine_defect_structure.py
 pydefect/tests/analyzer/test_transition_levels.py
 pydefect/tests/analyzer/test_transition_levels_plotter.py
 pydefect/tests/analyzer/test_unitcell.py
+pydefect/tests/analyzer/concentration/__init__.py
+pydefect/tests/analyzer/concentration/test_concentration.py
+pydefect/tests/analyzer/concentration/test_degeneracy.py
+pydefect/tests/analyzer/concentration/test_distribution_function.py
+pydefect/tests/analyzer/concentration/test_make_concentration.py
+pydefect/tests/analyzer/concentration/test_plot_concentration.py
 pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_0/POSCAR
 pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_2/POSCAR
 pydefect/tests/chem_pot_diag/cpd.yaml
 pydefect/tests/cli/__init__.py
 pydefect/tests/cli/test_main.py
 pydefect/tests/cli/test_main_functions.py
 pydefect/tests/cli/test_main_tools.py
@@ -162,22 +194,26 @@
 pydefect/tests/corrections/test_ewald.py
 pydefect/tests/corrections/test_gkfo_correction.py
 pydefect/tests/corrections/test_site_potential_plotter.py
 pydefect/tests/helpers/__init__.py
 pydefect/tests/input_maker/POSCAR
 pydefect/tests/input_maker/__init__.py
 pydefect/tests/input_maker/test_append_interstitial.py
+pydefect/tests/input_maker/test_complex_defect_entries_make.py
+pydefect/tests/input_maker/test_complex_defect_set.py
 pydefect/tests/input_maker/test_defect.py
 pydefect/tests/input_maker/test_defect_entries_maker.py
 pydefect/tests/input_maker/test_defect_entry.py
 pydefect/tests/input_maker/test_defect_set.py
 pydefect/tests/input_maker/test_defect_set_maker.py
 pydefect/tests/input_maker/test_local_extrema.py
+pydefect/tests/input_maker/test_manual_supercell_maker.py
 pydefect/tests/input_maker/test_supercell.py
 pydefect/tests/input_maker/test_supercell_info.py
 pydefect/tests/input_maker/test_supercell_maker.py
+pydefect/tests/test_data_files/Na3AgO2/degeneracies.yaml
 pydefect/util/__init__.py
 pydefect/util/coords.py
 pydefect/util/error_classes.py
 pydefect/util/mp_tools.py
 pydefect/util/prepare_names.py
 pydefect/util/structure_tools.py
```

### Comparing `pydefect-0.7.0/setup.py` & `pydefect-0.7.1/setup.py`

 * *Files identical despite different names*

