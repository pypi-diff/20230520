# Comparing `tmp/gdsfactory-6.96.0.tar.gz` & `tmp/gdsfactory-6.97.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdsfactory-6.96.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gdsfactory-6.97.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gdsfactory-6.96.0.tar` & `gdsfactory-6.97.0.tar`

### file list

```diff
@@ -1,693 +1,693 @@
--rw-r--r--   0        0        0     1072 2023-05-19 04:20:22.281426 gdsfactory-6.96.0/LICENSE
--rw-r--r--   0        0        0    14319 2023-05-19 04:20:22.281426 gdsfactory-6.96.0/README.md
--rw-r--r--   0        0        0     3566 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/__init__.py
--rw-r--r--   0        0        0     2104 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_keepout.py
--rw-r--r--   0        0        0    12629 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_labels.py
--rw-r--r--   0        0        0     3711 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_loopback.py
--rw-r--r--   0        0        0     5054 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_padding.py
--rw-r--r--   0        0        0    15639 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_pins.py
--rw-r--r--   0        0        0    14700 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_ports.py
--rw-r--r--   0        0        0     2884 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_tapers.py
--rw-r--r--   0        0        0     2257 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_tapers_cross_section.py
--rw-r--r--   0        0        0     1831 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_termination.py
--rw-r--r--   0        0        0     1856 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/asserts.py
--rw-r--r--   0        0        0    12272 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/cell.py
--rw-r--r--   0        0        0    16040 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/circuitviz.py
--rw-r--r--   0        0        0     5718 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/cli.py
--rw-r--r--   0        0        0   102063 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/component.py
--rw-r--r--   0        0        0    23424 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/component_layout.py
--rw-r--r--   0        0        0    29879 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/component_reference.py
--rw-r--r--   0        0        0     1205 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/C.py
--rw-r--r--   0        0        0     1144 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/L.py
--rw-r--r--   0        0        0    20964 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/__init__.py
--rw-r--r--   0        0        0     2621 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/add_fiducials.py
--rw-r--r--   0        0        0    14087 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/add_grating_couplers.py
--rw-r--r--   0        0        0     2014 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/add_trenches.py
--rw-r--r--   0        0        0     3207 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/align.py
--rw-r--r--   0        0        0     2622 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/array_component.py
--rw-r--r--   0        0        0     4705 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/array_with_fanout.py
--rw-r--r--   0        0        0     4322 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/array_with_via.py
--rw-r--r--   0        0        0     4042 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/awg.py
--rw-r--r--   0        0        0     1269 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/bbox.py
--rw-r--r--   0        0        0     2851 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/bend_circular.py
--rw-r--r--   0        0        0     2649 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/bend_circular_heater.py
--rw-r--r--   0        0        0     7903 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/bend_euler.py
--rw-r--r--   0        0        0     2682 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/bend_port.py
--rw-r--r--   0        0        0     3664 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/bend_s.py
--rw-r--r--   0        0        0     5373 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/bezier.py
--rw-r--r--   0        0        0     1605 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cavity.py
--rw-r--r--   0        0        0     5766 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cdc.py
--rw-r--r--   0        0        0     2929 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cdsem_all.py
--rw-r--r--   0        0        0     1788 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cdsem_bend180.py
--rw-r--r--   0        0        0     1631 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cdsem_coupler.py
--rw-r--r--   0        0        0     1412 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cdsem_straight.py
--rw-r--r--   0        0        0     1565 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cdsem_straight_density.py
--rw-r--r--   0        0        0      793 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/circle.py
--rw-r--r--   0        0        0     5722 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coh_rx_dual_pol.py
--rw-r--r--   0        0        0     8922 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coh_rx_single_pol.py
--rw-r--r--   0        0        0     5043 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coh_tx_dual_pol.py
--rw-r--r--   0        0        0     6118 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coh_tx_single_pol.py
--rw-r--r--   0        0        0     2548 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/compass.py
--rw-r--r--   0        0        0     9876 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/component_lattice.py
--rw-r--r--   0        0        0     7174 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/component_sequence.py
--rw-r--r--   0        0        0      812 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/copy_layers.py
--rw-r--r--   0        0        0     3460 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler.py
--rw-r--r--   0        0        0     2113 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler90.py
--rw-r--r--   0        0        0     1802 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler90bend.py
--rw-r--r--   0        0        0     4666 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler_adiabatic.py
--rw-r--r--   0        0        0     1909 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler_asymmetric.py
--rw-r--r--   0        0        0     3970 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler_full.py
--rw-r--r--   0        0        0     3414 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler_ring.py
--rw-r--r--   0        0        0     1060 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler_straight.py
--rw-r--r--   0        0        0     1164 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler_straight_asymmetric.py
--rw-r--r--   0        0        0     2192 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler_symmetric.py
--rw-r--r--   0        0        0     1848 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cross.py
--rw-r--r--   0        0        0    12873 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/crossing_waveguide.py
--rw-r--r--   0        0        0      500 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
--rw-r--r--   0        0        0     1014 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
--rw-r--r--   0        0        0    19749 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
--rw-r--r--   0        0        0    19751 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
--rw-r--r--   0        0        0    19749 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
--rw-r--r--   0        0        0    19751 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
--rw-r--r--   0        0        0    19775 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
--rw-r--r--   0        0        0     3143 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
--rw-r--r--   0        0        0     5272 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cutback_2x2.py
--rw-r--r--   0        0        0     6450 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cutback_bend.py
--rw-r--r--   0        0        0     3765 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cutback_component.py
--rw-r--r--   0        0        0     2721 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cutback_splitter.py
--rw-r--r--   0        0        0     2971 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/dbr.py
--rw-r--r--   0        0        0     4288 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/dbr_tapered.py
--rw-r--r--   0        0        0     2486 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/delay_snake.py
--rw-r--r--   0        0        0     3177 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/delay_snake2.py
--rw-r--r--   0        0        0     3245 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/delay_snake3.py
--rw-r--r--   0        0        0     4319 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/delay_snake_sbend.py
--rw-r--r--   0        0        0     1226 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/dicing_lane.py
--rw-r--r--   0        0        0     3471 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/die.py
--rw-r--r--   0        0        0     2975 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/die_bbox.py
--rw-r--r--   0        0        0     2863 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/die_bbox_frame.py
--rw-r--r--   0        0        0     8015 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/disk.py
--rw-r--r--   0        0        0     4112 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/edge_coupler_array.py
--rw-r--r--   0        0        0     1214 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ellipse.py
--rw-r--r--   0        0        0     1800 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/extend_ports_list.py
--rw-r--r--   0        0        0     7988 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/extension.py
--rw-r--r--   0        0        0      981 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/fiber.py
--rw-r--r--   0        0        0     1432 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/fiber_array.py
--rw-r--r--   0        0        0      722 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/fiducial_squares.py
--rw-r--r--   0        0        0     3290 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ge_detector_straight_si_contacts.py
--rw-r--r--   0        0        0     1063 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_array.py
--rw-r--r--   0        0        0     4682 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_dual_pol.py
--rw-r--r--   0        0        0     7110 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical.py
--rw-r--r--   0        0        0     7221 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
--rw-r--r--   0        0        0     4960 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py
--rw-r--r--   0        0        0     4592 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical_trenches.py
--rw-r--r--   0        0        0     1773 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_functions.py
--rw-r--r--   0        0        0     9058 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_loss.py
--rw-r--r--   0        0        0     1786 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_loss_fiber_single.py
--rw-r--r--   0        0        0     4142 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_rectangular.py
--rw-r--r--   0        0        0     4685 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
--rw-r--r--   0        0        0     3887 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
--rw-r--r--   0        0        0     1578 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_tree.py
--rw-r--r--   0        0        0     8811 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/greek_cross.py
--rw-r--r--   0        0        0     1019 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/hline.py
--rw-r--r--   0        0        0     3687 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/interdigital_capacitor.py
--rw-r--r--   0        0        0     1825 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/litho_calipers.py
--rw-r--r--   0        0        0     1244 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/litho_ruler.py
--rw-r--r--   0        0        0     1304 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/litho_steps.py
--rw-r--r--   0        0        0      650 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/logo.py
--rw-r--r--   0        0        0     1679 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/loop_mirror.py
--rw-r--r--   0        0        0     3873 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mmi1x2.py
--rw-r--r--   0        0        0     2814 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mmi1x2_with_sbend.py
--rw-r--r--   0        0        0     3858 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mmi2x2.py
--rw-r--r--   0        0        0     3299 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mmi2x2_with_sbend.py
--rw-r--r--   0        0        0     4947 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mmi_90degree_hybrid.py
--rw-r--r--   0        0        0     3265 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mode_converter.py
--rw-r--r--   0        0        0     7579 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzi.py
--rw-r--r--   0        0        0     2499 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzi_arm.py
--rw-r--r--   0        0        0     5835 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzi_arms.py
--rw-r--r--   0        0        0    12214 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzi_lattice.py
--rw-r--r--   0        0        0     4025 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzi_pads_center.py
--rw-r--r--   0        0        0     1064 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzi_phase_shifter.py
--rw-r--r--   0        0        0     6342 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzit.py
--rw-r--r--   0        0        0     3502 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzit_lattice.py
--rw-r--r--   0        0        0     6047 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzm.py
--rw-r--r--   0        0        0     3518 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/nxn.py
--rw-r--r--   0        0        0     1940 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/optimal_90deg.py
--rw-r--r--   0        0        0     3876 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/optimal_hairpin.py
--rw-r--r--   0        0        0     6131 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/optimal_step.py
--rw-r--r--   0        0        0     6327 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/pack_doe.py
--rw-r--r--   0        0        0     3860 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/pad.py
--rw-r--r--   0        0        0     1890 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/pad_gsg.py
--rw-r--r--   0        0        0     1157 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/pads_shorted.py
--rw-r--r--   0        0        0     3833 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/polarization_splitter_rotator.py
--rw-r--r--   0        0        0     1147 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ramp.py
--rw-r--r--   0        0        0     1508 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/rectangle.py
--rw-r--r--   0        0        0     2972 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/rectangle_with_slits.py
--rw-r--r--   0        0        0     1508 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/regular_polygon.py
--rw-r--r--   0        0        0     3302 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/resistance_meander.py
--rw-r--r--   0        0        0     2642 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/resistance_sheet.py
--rw-r--r--   0        0        0     1273 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring.py
--rw-r--r--   0        0        0     4143 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_crow.py
--rw-r--r--   0        0        0     3272 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_crow_couplers.py
--rw-r--r--   0        0        0     2267 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_double.py
--rw-r--r--   0        0        0     2846 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_double_bend_coupler.py
--rw-r--r--   0        0        0     3846 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_double_heater.py
--rw-r--r--   0        0        0     7757 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_double_pn.py
--rw-r--r--   0        0        0    12137 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_section_based.py
--rw-r--r--   0        0        0     2740 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_single.py
--rw-r--r--   0        0        0     1968 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_single_array.py
--rw-r--r--   0        0        0     6868 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_single_bend_coupler.py
--rw-r--r--   0        0        0     2714 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_single_dut.py
--rw-r--r--   0        0        0     4018 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_single_heater.py
--rw-r--r--   0        0        0     5267 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_single_pn.py
--rw-r--r--   0        0        0     2282 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/seal_ring.py
--rw-r--r--   0        0        0     3758 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/snspd.py
--rw-r--r--   0        0        0     2059 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/spiral_double.py
--rw-r--r--   0        0        0     5871 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/spiral_external_io.py
--rw-r--r--   0        0        0    16692 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/spiral_heater.py
--rw-r--r--   0        0        0     9181 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/spiral_inner_io.py
--rw-r--r--   0        0        0     1733 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/splitter_chain.py
--rw-r--r--   0        0        0     5327 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/splitter_tree.py
--rw-r--r--   0        0        0     2526 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight.py
--rw-r--r--   0        0        0     1033 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_array.py
--rw-r--r--   0        0        0     7914 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_heater_doped_rib.py
--rw-r--r--   0        0        0     1922 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_heater_doped_strip.py
--rw-r--r--   0        0        0     7891 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_heater_meander.py
--rw-r--r--   0        0        0     8090 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_heater_meander_doped.py
--rw-r--r--   0        0        0     5686 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_heater_metal.py
--rw-r--r--   0        0        0     2809 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_pin.py
--rw-r--r--   0        0        0     3974 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_pin_slot.py
--rw-r--r--   0        0        0      655 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_rib.py
--rw-r--r--   0        0        0      820 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/switch_tree.py
--rw-r--r--   0        0        0     7730 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/taper.py
--rw-r--r--   0        0        0     3530 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/taper_adiabatic.py
--rw-r--r--   0        0        0     2457 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/taper_cross_section.py
--rw-r--r--   0        0        0     2363 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/taper_from_csv.py
--rw-r--r--   0        0        0     1215 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/taper_parabolic.py
--rw-r--r--   0        0        0     1635 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/terminator.py
--rw-r--r--   0        0        0     2913 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/text.py
--rw-r--r--   0        0        0     3821 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/text_freetype.py
--rw-r--r--   0        0        0     3160 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/text_rectangular.py
--rw-r--r--   0        0        0     3943 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/text_rectangular_font.py
--rw-r--r--   0        0        0     2536 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/triangles.py
--rw-r--r--   0        0        0      715 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/verniers.py
--rw-r--r--   0        0        0     2468 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/version_stamp.py
--rw-r--r--   0        0        0     2436 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/via.py
--rw-r--r--   0        0        0     3060 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/via_corner.py
--rw-r--r--   0        0        0     5342 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/via_cutback.py
--rw-r--r--   0        0        0    15612 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/via_stack.py
--rw-r--r--   0        0        0     4430 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/via_stack_slot.py
--rw-r--r--   0        0        0     4944 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/via_stack_with_offset.py
--rw-r--r--   0        0        0     1088 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/wafer.py
--rw-r--r--   0        0        0     2542 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/wire.py
--rw-r--r--   0        0        0      978 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/wire_sbend.py
--rw-r--r--   0        0        0     8145 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/config.py
--rw-r--r--   0        0        0      481 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/conftest.py
--rw-r--r--   0        0        0    38409 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/constants.py
--rw-r--r--   0        0        0     1476 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/containers.py
--rw-r--r--   0        0        0    82893 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/cross_section.py
--rw-r--r--   0        0        0     2982 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/decorators.py
--rw-r--r--   0        0        0     7312 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/difftest.py
--rw-r--r--   0        0        0     1020 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/events.py
--rw-r--r--   0        0        0      204 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/export/__init__.py
--rw-r--r--   0        0        0     3353 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/export/to_3d.py
--rw-r--r--   0        0        0     1940 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/export/to_np.py
--rw-r--r--   0        0        0     3058 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/export/to_stl.py
--rw-r--r--   0        0        0     7445 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/export/write_gerbers.py
--rw-r--r--   0        0        0     2976 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/filestorage.py
--rw-r--r--   0        0        0    11890 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/fill.py
--rw-r--r--   0        0        0     7799 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/font.py
--rw-r--r--   0        0        0     8073 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/functions.py
--rw-r--r--   0        0        0       20 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/.gitattributes
--rw-r--r--   0        0        0       83 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/.gitconfig
--rw-r--r--   0        0        0       72 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/__init__.py
--rw-r--r--   0        0        0     1069 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/gds_diff_git.py
--rw-r--r--   0        0        0     2935 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/gdsdiff.py
--rw-r--r--   0        0        0      708 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/install.py
--rw-r--r--   0        0        0      271 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/sample.py
--rw-r--r--   0        0        0     1059 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/test_xor.py
--rw-r--r--   0        0        0     1100 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/README.md
--rw-r--r--   0        0        0     1722 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/__init__.py
--rw-r--r--   0        0        0      169 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/generic_tech.sh
--rw-r--r--   0        0        0     8142 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/get_klayout_pyxs.py
--rw-r--r--   0        0        0      161 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/README.md
--rw-r--r--   0        0        0      104 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/drc/Makefile
--rw-r--r--   0        0        0        0 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/drc/__init__.py
--rw-r--r--   0        0        0     2842 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/drc/errors.py
--rw-r--r--   0        0        0     6193 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/grain.xml
--rw-r--r--   0        0        0    10140 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/icon_128x128.png
--rw-r--r--   0        0        0     4248 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/icon_64x64.png
--rw-r--r--   0        0        0       27 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/.gitignore
--rw-r--r--   0        0        0      494 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/Makefile
--rw-r--r--   0        0        0     4062 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/README.md
--rw-r--r--   0        0        0     2419 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
--rw-r--r--   0        0        0     9696 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
--rw-r--r--   0        0        0    12379 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
--rw-r--r--   0        0        0     7235 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
--rw-r--r--   0        0        0     3446 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
--rw-r--r--   0        0        0      479 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
--rw-r--r--   0        0        0      582 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
--rw-r--r--   0        0        0      108 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
--rw-r--r--   0        0        0      186 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
--rw-r--r--   0        0        0      398 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
--rw-r--r--   0        0        0      574 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
--rw-r--r--   0        0        0     6034 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
--rw-r--r--   0        0        0    10704 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
--rw-r--r--   0        0        0      477 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
--rw-r--r--   0        0        0     4337 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
--rw-r--r--   0        0        0      926 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
--rw-r--r--   0        0        0    10945 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
--rw-r--r--   0        0        0      710 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
--rw-r--r--   0        0        0      538 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
--rw-r--r--   0        0        0        0 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/python/__init__.py
--rw-r--r--   0        0        0      114 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
--rw-r--r--   0        0        0     4311 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
--rw-r--r--   0        0        0      269 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/Makefile
--rw-r--r--   0        0        0     1854 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25
--rw-r--r--   0        0        0     1519 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack
--rw-r--r--   0        0        0    41073 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
--rw-r--r--   0        0        0    40616 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/layers.lyp
--rw-r--r--   0        0        0     5977 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/tech.lyt
--rw-r--r--   0        0        0     4258 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
--rw-r--r--   0        0        0     4537 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
--rw-r--r--   0        0        0     4690 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
--rw-r--r--   0        0        0     5508 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
--rw-r--r--   0        0        0     1883 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/layer_map.py
--rw-r--r--   0        0        0     6511 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/layer_stack.py
--rw-r--r--   0        0        0    10780 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/layer_views.yaml
--rw-r--r--   0        0        0      158 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/simulation_settings.py
--rw-r--r--   0        0        0     1431 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/__init__.py
--rw-r--r--   0        0        0     4917 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/boolean.py
--rw-r--r--   0        0        0     3814 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/boolean_klayout.py
--rw-r--r--   0        0        0     1904 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/boolean_polygons.py
--rw-r--r--   0        0        0      598 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/check_duplicated_cells.py
--rw-r--r--   0        0        0     2719 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/check_exclusion.py
--rw-r--r--   0        0        0     2829 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/check_inclusion.py
--rw-r--r--   0        0        0     3566 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/check_space.py
--rw-r--r--   0        0        0     1904 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/check_width.py
--rw-r--r--   0        0        0     5015 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/fill_klayout.py
--rw-r--r--   0        0        0     7084 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/fill_tiled.py
--rw-r--r--   0        0        0     1697 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/fillet.py
--rw-r--r--   0        0        0     6664 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/functions.py
--rw-r--r--   0        0        0     2167 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/invert.py
--rw-r--r--   0        0        0     3685 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/layer_priority.py
--rw-r--r--   0        0        0     3054 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/manhattanize.py
--rw-r--r--   0        0        0     4192 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/maskprep.py
--rw-r--r--   0        0        0     4812 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/maskprep_flat.py
--rw-r--r--   0        0        0     3250 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/offset.py
--rw-r--r--   0        0        0     3842 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/outline.py
--rw-r--r--   0        0        0     2510 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/trim.py
--rw-r--r--   0        0        0     2948 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/union.py
--rw-r--r--   0        0        0     1898 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/write_connectivity.py
--rw-r--r--   0        0        0    10532 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/write_drc.py
--rw-r--r--   0        0        0     1783 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/xor_diff.py
--rw-r--r--   0        0        0     1158 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/get_factories.py
--rw-r--r--   0        0        0    23569 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/get_netlist.py
--rw-r--r--   0        0        0    14446 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/get_netlist_flat.py
--rw-r--r--   0        0        0      682 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/get_netlist_klayout.py
--rw-r--r--   0        0        0     9745 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/grid.py
--rw-r--r--   0        0        0     4393 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/install.py
--rw-r--r--   0        0        0     1970 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/klive.py
--rw-r--r--   0        0        0      585 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/labels/__init__.py
--rw-r--r--   0        0        0     3563 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/labels/add_label_yaml.py
--rw-r--r--   0        0        0     3847 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/labels/ehva.py
--rw-r--r--   0        0        0     3810 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/labels/merge_test_metadata.py
--rw-r--r--   0        0        0     4668 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/labels/siepic.py
--rw-r--r--   0        0        0     4847 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/labels/write_labels.py
--rw-r--r--   0        0        0     1149 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/materials.py
--rw-r--r--   0        0        0     5247 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/name.py
--rw-r--r--   0        0        0    11586 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/pack.py
--rw-r--r--   0        0        0    50930 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/path.py
--rw-r--r--   0        0        0    27294 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/pdk.py
--rw-r--r--   0        0        0     6220 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/picmodel.py
--rw-r--r--   0        0        0     5068 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/pixelate.py
--rw-r--r--   0        0        0        0 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/dagster/__init__.py
--rw-r--r--   0        0        0      976 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/dagster/workflow.py
--rw-r--r--   0        0        0      566 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/database/README.md
--rw-r--r--   0        0        0        0 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/database/__init__.py
--rw-r--r--   0        0        0     6216 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/database/db_upload.py
--rw-r--r--   0        0        0    16143 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/database/models.py
--rw-r--r--   0        0        0       32 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/web/Makefile
--rw-r--r--   0        0        0       23 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/web/__init__.py
--rw-r--r--   0        0        0     4080 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/web/main.py
--rwxr-xr-x   0        0        0     7511 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/web/server.py
--rwxr-xr-x   0        0        0      594 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/web/server_jupyter.py
--rw-r--r--   0        0        0     1299 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/web/static/client.css
--rw-r--r--   0        0        0    32235 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/port.py
--rw-r--r--   0        0        0    37817 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/quickplotter.py
--rw-r--r--   0        0        0      696 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/__init__.py
--rw-r--r--   0        0        0     1639 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/from_dphox.py
--rw-r--r--   0        0        0     1285 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/from_gdspaths.py
--rw-r--r--   0        0        0     1953 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/from_np.py
--rw-r--r--   0        0        0     2813 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/from_phidl.py
--rw-r--r--   0        0        0    38082 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/from_yaml.py
--rw-r--r--   0        0        0     5897 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/from_yaml_template.py
--rw-r--r--   0        0        0     5688 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/import_gds.py
--rw-r--r--   0        0        0     3407 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/labels.py
--rw-r--r--   0        0        0     3769 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/__init__.py
--rw-r--r--   0        0        0     2920 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/add_electrical_pads_shortest.py
--rw-r--r--   0        0        0     3015 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/add_electrical_pads_top.py
--rw-r--r--   0        0        0     3035 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/add_electrical_pads_top_dc.py
--rw-r--r--   0        0        0     8715 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/add_fiber_array.py
--rw-r--r--   0        0        0    10624 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/add_fiber_single.py
--rw-r--r--   0        0        0     8967 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/add_pads.py
--rw-r--r--   0        0        0    38948 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/all_angle.py
--rw-r--r--   0        0        0     3916 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/auto_taper.py
--rw-r--r--   0        0        0      982 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/factories.py
--rw-r--r--   0        0        0     4415 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/fanout.py
--rw-r--r--   0        0        0     2800 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/fanout2x2.py
--rw-r--r--   0        0        0    24342 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_bundle.py
--rw-r--r--   0        0        0     8652 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_bundle_corner.py
--rw-r--r--   0        0        0     6910 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_bundle_from_steps.py
--rw-r--r--   0        0        0    12949 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_bundle_from_waypoints.py
--rw-r--r--   0        0        0     5284 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_bundle_path_length_match.py
--rw-r--r--   0        0        0     1937 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_bundle_sbend.py
--rw-r--r--   0        0        0    17064 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_bundle_u.py
--rw-r--r--   0        0        0     1510 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_input_labels.py
--rw-r--r--   0        0        0     9233 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_route.py
--rw-r--r--   0        0        0    10872 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_route_astar.py
--rw-r--r--   0        0        0     6119 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_route_from_steps.py
--rw-r--r--   0        0        0     2766 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_route_sbend.py
--rw-r--r--   0        0        0     3311 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_routes_bend180.py
--rw-r--r--   0        0        0     1854 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_routes_straight.py
--rw-r--r--   0        0        0    34394 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/manhattan.py
--rw-r--r--   0        0        0    10081 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/path_length_matching.py
--rw-r--r--   0        0        0    22568 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/route_fiber_array.py
--rw-r--r--   0        0        0     8679 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/route_fiber_single.py
--rw-r--r--   0        0        0    18132 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/route_ports_to_side.py
--rw-r--r--   0        0        0     4379 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/route_quad.py
--rw-r--r--   0        0        0    14370 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/route_sharp.py
--rw-r--r--   0        0        0    10167 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/route_south.py
--rw-r--r--   0        0        0     5072 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/routing/sort_ports.py
--rw-r--r--   0        0        0     2477 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/routing/utils.py
--rw-r--r--   0        0        0     2897 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell.py
--rw-r--r--   0        0        0      646 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
--rw-r--r--   0        0        0     1109 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell_with_pins.py
--rw-r--r--   0        0        0      664 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
--rw-r--r--   0        0        0      347 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/02_component_autoname.py
--rw-r--r--   0        0        0      887 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/03_move.py
--rw-r--r--   0        0        0      881 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/04_connect.py
--rw-r--r--   0        0        0      710 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/05_remove_layers.py
--rw-r--r--   0        0        0      931 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/06_remapping_layers.py
--rw-r--r--   0        0        0     1082 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/07_flattening_device.py
--rw-r--r--   0        0        0      475 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/08_group.py
--rw-r--r--   0        0        0     1631 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/11_component_layout.py
--rw-r--r--   0        0        0     2245 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/12_component_refs.py
--rw-r--r--   0        0        0      955 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/13_component_netlist.py
--rw-r--r--   0        0        0     2592 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/14_component_connectivity.py
--rw-r--r--   0        0        0     1636 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/15_component_sequence1.py
--rw-r--r--   0        0        0     1680 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/16_component_sequence2.py
--rw-r--r--   0        0        0      965 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/17_ports.py
--rw-r--r--   0        0        0      489 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/18_port_markers.py
--rw-r--r--   0        0        0      361 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/19_references.py
--rw-r--r--   0        0        0      533 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/20_components.py
--rw-r--r--   0        0        0      507 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/21_add_fiber_array.py
--rw-r--r--   0        0        0      493 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/22_add_fiber_single.py
--rw-r--r--   0        0        0      569 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/22_add_pads.py
--rw-r--r--   0        0        0      848 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/23_reticle.py
--rw-r--r--   0        0        0     1588 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/23_reticle_passives.py
--rw-r--r--   0        0        0      457 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/24_doe.py
--rw-r--r--   0        0        0      687 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/24_doe_2.py
--rw-r--r--   0        0        0      692 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/24_doe_3.py
--rw-r--r--   0        0        0      306 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/25_slot_cross_section.py
--rw-r--r--   0        0        0     1363 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/30_lidar.py
--rw-r--r--   0        0        0     1412 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/30_lidar_pcell.py
--rw-r--r--   0        0        0     1943 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/30_lidar_with_pads.py
--rw-r--r--   0        0        0        0 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/__init__.py
--rw-r--r--   0        0        0     1307 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing.py
--rw-r--r--   0        0        0      558 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
--rw-r--r--   0        0        0     6062 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
--rw-r--r--   0        0        0      444 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
--rw-r--r--   0        0        0      463 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
--rw-r--r--   0        0        0     1552 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
--rw-r--r--   0        0        0     1315 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
--rw-r--r--   0        0        0      602 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
--rw-r--r--   0        0        0     3317 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
--rw-r--r--   0        0        0     1484 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
--rw-r--r--   0        0        0     3045 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
--rw-r--r--   0        0        0     3782 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
--rw-r--r--   0        0        0     1988 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/big_device.py
--rw-r--r--   0        0        0       19 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/Makefile
--rw-r--r--   0        0        0        0 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/__init__.py
--rw-r--r--   0        0        0     1129 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/benchmark/fill_demo.py
--rw-r--r--   0        0        0      343 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
--rw-r--r--   0        0        0      637 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/mask.pic.yml
--rw-r--r--   0        0        0      622 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
--rw-r--r--   0        0        0      569 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
--rw-r--r--   0        0        0      453 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/pads.pic.yml
--rw-r--r--   0        0        0      287 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/rectangles.pic.yml
--rw-r--r--   0        0        0     2260 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/drc_errors.py
--rw-r--r--   0        0        0     1014 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/drc_write.py
--rw-r--r--   0        0        0     4530 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/layers.py
--rw-r--r--   0        0        0      158 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/layers_sky130.py
--rw-r--r--   0        0        0      364 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/layers_xsection.py
--rw-r--r--   0        0        0     1062 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/lvs.py
--rw-r--r--   0        0        0      574 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/pcell.py
--rw-r--r--   0        0        0     4174 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/netlists/mzi.yml
--rw-r--r--   0        0        0     5840 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/netlists/mzi_full.yml
--rw-r--r--   0        0        0        0 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/__init__.py
--rw-r--r--   0        0        0     4235 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/fab_c.py
--rw-r--r--   0        0        0      475 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/fab_d/__init__.py
--rw-r--r--   0        0        0     1880 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py
--rw-r--r--   0        0        0     1715 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c.py
--rw-r--r--   0        0        0       50 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
--rw-r--r--   0        0        0       93 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
--rw-r--r--   0        0        0       85 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
--rw-r--r--   0        0        0      139 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
--rw-r--r--   0        0        0       90 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
--rw-r--r--   0        0        0      126 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
--rw-r--r--   0        0        0       48 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
--rw-r--r--   0        0        0     1023 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
--rw-r--r--   0        0        0     2140 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
--rw-r--r--   0        0        0     1879 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
--rw-r--r--   0        0        0     1283 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
--rw-r--r--   0        0        0     1632 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
--rw-r--r--   0        0        0     1061 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
--rw-r--r--   0        0        0     1054 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
--rw-r--r--   0        0        0     1617 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
--rw-r--r--   0        0        0     4497 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
--rw-r--r--   0        0        0     3625 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
--rw-r--r--   0        0        0     3603 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
--rw-r--r--   0        0        0     4455 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
--rw-r--r--   0        0        0      840 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
--rw-r--r--   0        0        0     2231 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
--rw-r--r--   0        0        0      316 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/schematic.py
--rw-r--r--   0        0        0    17862 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/schematic_editor.py
--rw-r--r--   0        0        0     4194 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/serialization.py
--rw-r--r--   0        0        0     1612 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/show.py
--rw-r--r--   0        0        0      724 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/__init__.py
--rw-r--r--   0        0        0     4369 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/add_simulation_markers.py
--rw-r--r--   0        0        0     2476 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/convert_sparameters.py
--rw-r--r--   0        0        0      547 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/devsim/__init__.py
--rw-r--r--   0        0        0     2559 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/devsim/doping.py
--rw-r--r--   0        0        0    11977 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/devsim/get_simulation.py
--rw-r--r--   0        0        0    23687 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/devsim/get_simulation_xsection.py
--rw-r--r--   0        0        0    19756 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/devsim/get_solver.py
--rw-r--r--   0        0        0     1644 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/devsim/test_devsim.py
--rw-r--r--   0        0        0      189 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/disable_print.py
--rw-r--r--   0        0        0       79 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/eme/__init__.py
--rw-r--r--   0        0        0    14784 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/eme/meow_eme.py
--rw-r--r--   0        0        0     1787 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/eme/test_meow_simulation.py
--rw-r--r--   0        0        0        0 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/fem/__init__.py
--rw-r--r--   0        0        0     8968 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/fem/mode_solver.py
--rw-r--r--   0        0        0     2221 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/fem/test_mode_solver.py
--rw-r--r--   0        0        0     3455 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/get_effective_indices.py
--rw-r--r--   0        0        0     3109 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/get_modes_path.py
--rw-r--r--   0        0        0     3888 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/get_sparameters_path.py
--rw-r--r--   0        0        0     2003 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/__init__.py
--rw-r--r--   0        0        0     3194 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_material.py
--rw-r--r--   0        0        0     6137 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_meep_geometry.py
--rw-r--r--   0        0        0     6054 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py
--rw-r--r--   0        0        0    11014 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_simulation.py
--rw-r--r--   0        0        0    15915 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py
--rw-r--r--   0        0        0    18182 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py
--rw-r--r--   0        0        0    12312 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py
--rw-r--r--   0        0        0    11914 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_eigenmode.py
--rw-r--r--   0        0        0      832 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_materials.py
--rw-r--r--   0        0        0    10128 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0     6642 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py
--rw-r--r--   0        0        0    10128 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0    10093 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
--rw-r--r--   0        0        0    10085 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
--rw-r--r--   0        0        0    34701 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
--rw-r--r--   0        0        0    10123 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
--rw-r--r--   0        0        0     9966 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
--rw-r--r--   0        0        0     9966 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
--rw-r--r--   0        0        0    10129 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
--rw-r--r--   0        0        0    14053 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py
--rw-r--r--   0        0        0    21281 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py
--rw-r--r--   0        0        0     8143 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py
--rw-r--r--   0        0        0     9577 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py
--rw-r--r--   0        0        0     1246 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/__init__.py
--rw-r--r--   0        0        0     6653 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/break_geometry.py
--rw-r--r--   0        0        0    11250 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/mesh.py
--rw-r--r--   0        0        0    11824 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/meshtracker.py
--rw-r--r--   0        0        0     7752 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/parse_component.py
--rw-r--r--   0        0        0     3644 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/parse_gds.py
--rw-r--r--   0        0        0     3605 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/parse_layerstack.py
--rw-r--r--   0        0        0     2990 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/refine.py
--rw-r--r--   0        0        0    10851 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py
--rw-r--r--   0        0        0     2513 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/tests/test_meshing.py
--rw-r--r--   0        0        0    14168 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py
--rw-r--r--   0        0        0     7441 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py
--rw-r--r--   0        0        0    16334 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/xyz_mesh.py
--rw-r--r--   0        0        0     1624 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/__init__.py
--rw-r--r--   0        0        0     4368 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/get_results.py
--rw-r--r--   0        0        0    20009 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/get_simulation.py
--rw-r--r--   0        0        0    21071 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py
--rw-r--r--   0        0        0     2821 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/materials.py
--rw-r--r--   0        0        0    27439 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/modes.py
--rw-r--r--   0        0        0     8941 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/sim_run.yaml
--rw-r--r--   0        0        0     8114 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml
--rw-r--r--   0        0        0     8114 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml
--rw-r--r--   0        0        0      744 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py
--rw-r--r--   0        0        0      262 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_modes/test_sweep_width.csv
--rw-r--r--   0        0        0      879 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_results.py
--rw-r--r--   0        0        0     1505 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py
--rw-r--r--   0        0        0     1270 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py
--rw-r--r--   0        0        0     9297 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv
--rw-r--r--   0        0        0     1732 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0     1224 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/utils.py
--rw-r--r--   0        0        0    10515 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/write_sparameters.py
--rw-r--r--   0        0        0     7695 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0      588 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/lumerical/__init__.py
--rw-r--r--   0        0        0    16091 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/lumerical/interconnect.py
--rw-r--r--   0        0        0     4286 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/lumerical/read.py
--rw-r--r--   0        0        0     3569 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/lumerical/settings.py
--rw-r--r--   0        0        0     2368 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/lumerical/test_read_sparameters.py
--rw-r--r--   0        0        0    19865 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py
--rw-r--r--   0        0        0     1504 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py
--rw-r--r--   0        0        0      932 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/__init__.py
--rw-r--r--   0        0        0     1618 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/coupler.py
--rw-r--r--   0        0        0     4166 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py
--rw-r--r--   0        0        0     2773 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/find_mode_dispersion.py
--rw-r--r--   0        0        0     8924 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/find_modes.py
--rwxr-xr-x   0        0        0     7032 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/find_modes_cross_section.py
--rw-r--r--   0        0        0     4458 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py
--rw-r--r--   0        0        0     2728 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/find_neff_vs_width.py
--rw-r--r--   0        0        0     7148 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py
--rwxr-xr-x   0        0        0     4462 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py
--rw-r--r--   0        0        0     5411 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/get_mode_solver_rib.py
--rw-r--r--   0        0        0     1110 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv
--rw-r--r--   0        0        0     1102 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv
--rw-r--r--   0        0        0     1110 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv
--rw-r--r--   0        0        0     8023 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/neff_convergence_test.py
--rw-r--r--   0        0        0      267 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/neff_vs_width.csv
--rw-r--r--   0        0        0     2469 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/overlap.py
--rw-r--r--   0        0        0      418 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_dw_dh.py
--rw-r--r--   0        0        0       83 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh.csv
--rw-r--r--   0        0        0      548 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
--rw-r--r--   0        0        0     1137 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_find_modes.py
--rw-r--r--   0        0        0      649 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py
--rw-r--r--   0        0        0      354 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_neff_vs_width.py
--rw-r--r--   0        0        0      113 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
--rw-r--r--   0        0        0    15492 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/types.py
--rw-r--r--   0        0        0     1169 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/waveguide.py
--rw-r--r--   0        0        0     2013 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/__init__.py
--rw-r--r--   0        0        0      597 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/coupler.py
--rw-r--r--   0        0        0      377 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/fsr.py
--rw-r--r--   0        0        0      418 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/heater.py
--rw-r--r--   0        0        0     3069 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/mzi.py
--rw-r--r--   0        0        0     2616 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/ring.py
--rw-r--r--   0        0        0     7332 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/plot.py
--rw-r--r--   0        0        0     2480 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/plot_csv.py
--rw-r--r--   0        0        0      703 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/port_symmetries.py
--rw-r--r--   0        0        0     4685 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/diffusion.py
--rw-r--r--   0        0        0     5317 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/implant_tables.py
--rw-r--r--   0        0        0     6800 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/pysrim.py
--rw-r--r--   0        0        0     2182 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/silicon.py
--rw-r--r--   0        0        0     1861 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv
--rw-r--r--   0        0        0     1050 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv
--rw-r--r--   0        0        0     1468 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/skew/boron_si_skew.csv
--rw-r--r--   0        0        0     1118 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv
--rw-r--r--   0        0        0      191 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/__init__.py
--rw-r--r--   0        0        0    14848 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/build_model.py
--rw-r--r--   0        0        0     7449 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/femwell_waveguide_model.py
--rw-r--r--   0        0        0     1571 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/interpolators.py
--rw-r--r--   0        0        0     6755 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/meep_FDTD_model.py
--rw-r--r--   0        0        0     4528 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/meow_eme_model.py
--rw-r--r--   0        0        0     5613 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/mlp.py
--rw-r--r--   0        0        0     7358 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/models.py
--rw-r--r--   0        0        0    13894 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/parameter.py
--rwxr-xr-x   0        0        0     2225 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/plot_model.py
--rw-r--r--   0        0        0     6805 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/read.py
--rw-r--r--   0        0        0     1350 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/tests/test_mzi.py
--rw-r--r--   0        0        0     2220 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py
--rw-r--r--   0        0        0     1405 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/tests/test_parameters.py
--rw-r--r--   0        0        0     1357 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/__init__.py
--rw-r--r--   0        0        0     1573 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/add_gc.py
--rw-r--r--   0        0        0     3383 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/circuit.py
--rw-r--r--   0        0        0      891 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/__init__.py
--rw-r--r--   0        0        0     1295 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/bend_circular.py
--rw-r--r--   0        0        0     1388 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/bend_euler.py
--rw-r--r--   0        0        0     2560 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler.py
--rw-r--r--   0        0        0     1046 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py
--rw-r--r--   0        0        0     1848 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_ring.py
--rw-r--r--   0        0        0     1329 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py
--rw-r--r--   0        0        0      589 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py
--rw-r--r--   0        0        0      913 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/gc.py
--rw-r--r--   0        0        0     2032 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mmi1x2.py
--rw-r--r--   0        0        0     1910 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mmi2x2.py
--rw-r--r--   0        0        0     2618 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mzi.py
--rw-r--r--   0        0        0     1759 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mzi_siepic.py
--rw-r--r--   0        0        0      487 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mzi_thermal.py
--rw-r--r--   0        0        0     2597 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_double.py
--rw-r--r--   0        0        0     1665 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py
--rw-r--r--   0        0        0     1782 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_single.py
--rw-r--r--   0        0        0     1416 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py
--rw-r--r--   0        0        0     1099 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/straight.py
--rw-r--r--   0        0        0      800 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/get_transmission.py
--rw-r--r--   0        0        0     2516 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py
--rw-r--r--   0        0        0     3841 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/model_from_sparameters.py
--rw-r--r--   0        0        0     2438 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/plot_circuit.py
--rw-r--r--   0        0        0     1798 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py
--rw-r--r--   0        0        0     2773 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/plot_model.py
--rw-r--r--   0        0        0     1261 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_circuit.py
--rw-r--r--   0        0        0       90 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_circuit/test_circuit_transmission.yml
--rw-r--r--   0        0        0     1109 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components.py
--rw-r--r--   0        0        0       66 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_mzi_.yml
--rw-r--r--   0        0        0       69 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_double_.yml
--rw-r--r--   0        0        0       69 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_single_.yml
--rw-r--r--   0        0        0       92 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_circular_.yml
--rw-r--r--   0        0        0       92 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_euler_.yml
--rw-r--r--   0        0        0      412 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_.yml
--rw-r--r--   0        0        0      412 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_ring_.yml
--rw-r--r--   0        0        0      114 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_gc1550te_.yml
--rw-r--r--   0        0        0      256 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi1x2_.yml
--rw-r--r--   0        0        0      460 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi2x2_.yml
--rw-r--r--   0        0        0      104 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_straight_.yml
--rw-r--r--   0        0        0      166 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/types.py
--rw-r--r--   0        0        0      471 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/sipann/__init__.py
--rw-r--r--   0        0        0     1376 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/sipann/bend_circular.py
--rw-r--r--   0        0        0     1465 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/sipann/bend_euler.py
--rw-r--r--   0        0        0     2508 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/sipann/coupler.py
--rw-r--r--   0        0        0     1892 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/sipann/coupler_ring.py
--rw-r--r--   0        0        0      736 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/sipann/straight.py
--rw-r--r--   0        0        0      100 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/thermal/__init__.py
--rw-r--r--   0        0        0     7789 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/thermal/heater.py
--rw-r--r--   0        0        0     1744 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/snap.py
--rw-r--r--   0        0        0     4245 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/symbols.py
--rw-r--r--   0        0        0      524 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/technology/__init__.py
--rw-r--r--   0        0        0     7607 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/technology/klayout_tech.py
--rw-r--r--   0        0        0     1078 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/technology/layer_map.py
--rw-r--r--   0        0        0    16139 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/technology/layer_stack.py
--rw-r--r--   0        0        0    42133 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/technology/layer_views.py
--rw-r--r--   0        0        0     1984 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/technology/simulation_settings.py
--rw-r--r--   0        0        0     1635 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/types.py
--rw-r--r--   0        0        0    10008 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/typings.py
--rw-r--r--   0        0        0        0 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/utils/__init__.py
--rw-r--r--   0        0        0     1342 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/utils/async_utils.py
--rw-r--r--   0        0        0      376 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/utils/color_utils.py
--rw-r--r--   0        0        0      558 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/utils/file_utils.py
--rw-r--r--   0        0        0      185 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/utils/function_utils.py
--rw-r--r--   0        0        0      684 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/utils/xml_utils.py
--rw-r--r--   0        0        0     1453 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/utils/yaml_utils.py
--rw-r--r--   0        0        0     4865 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/watch.py
--rw-r--r--   0        0        0        0 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/widgets/__init__.py
--rw-r--r--   0        0        0     7969 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/widgets/layout_viewer.py
--rw-r--r--   0        0        0     7480 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/write_cells.py
--rw-r--r--   0        0        0     5687 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/pyproject.toml
--rw-r--r--   0        0        0    18772 1970-01-01 00:00:00.000000 gdsfactory-6.96.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-19 23:05:02.442286 gdsfactory-6.97.0/LICENSE
+-rw-r--r--   0        0        0    14319 2023-05-19 23:05:02.442286 gdsfactory-6.97.0/README.md
+-rw-r--r--   0        0        0     3583 2023-05-19 23:05:02.450286 gdsfactory-6.97.0/gdsfactory/__init__.py
+-rw-r--r--   0        0        0     2104 2023-05-19 23:05:02.450286 gdsfactory-6.97.0/gdsfactory/add_keepout.py
+-rw-r--r--   0        0        0    12629 2023-05-19 23:05:02.450286 gdsfactory-6.97.0/gdsfactory/add_labels.py
+-rw-r--r--   0        0        0     3711 2023-05-19 23:05:02.450286 gdsfactory-6.97.0/gdsfactory/add_loopback.py
+-rw-r--r--   0        0        0     5054 2023-05-19 23:05:02.450286 gdsfactory-6.97.0/gdsfactory/add_padding.py
+-rw-r--r--   0        0        0    15639 2023-05-19 23:05:02.450286 gdsfactory-6.97.0/gdsfactory/add_pins.py
+-rw-r--r--   0        0        0    14700 2023-05-19 23:05:02.450286 gdsfactory-6.97.0/gdsfactory/add_ports.py
+-rw-r--r--   0        0        0     2884 2023-05-19 23:05:02.450286 gdsfactory-6.97.0/gdsfactory/add_tapers.py
+-rw-r--r--   0        0        0     2257 2023-05-19 23:05:02.450286 gdsfactory-6.97.0/gdsfactory/add_tapers_cross_section.py
+-rw-r--r--   0        0        0     1831 2023-05-19 23:05:02.450286 gdsfactory-6.97.0/gdsfactory/add_termination.py
+-rw-r--r--   0        0        0     1856 2023-05-19 23:05:02.450286 gdsfactory-6.97.0/gdsfactory/asserts.py
+-rw-r--r--   0        0        0    12988 2023-05-19 23:05:02.450286 gdsfactory-6.97.0/gdsfactory/cell.py
+-rw-r--r--   0        0        0    16040 2023-05-19 23:05:02.450286 gdsfactory-6.97.0/gdsfactory/circuitviz.py
+-rw-r--r--   0        0        0     5718 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/cli.py
+-rw-r--r--   0        0        0   101568 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/component.py
+-rw-r--r--   0        0        0    23424 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/component_layout.py
+-rw-r--r--   0        0        0    29879 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/component_reference.py
+-rw-r--r--   0        0        0     1205 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/C.py
+-rw-r--r--   0        0        0     1144 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/L.py
+-rw-r--r--   0        0        0    20964 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/__init__.py
+-rw-r--r--   0        0        0     2621 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/add_fiducials.py
+-rw-r--r--   0        0        0    14087 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/add_grating_couplers.py
+-rw-r--r--   0        0        0     2014 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/add_trenches.py
+-rw-r--r--   0        0        0     3207 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/align.py
+-rw-r--r--   0        0        0     2622 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/array_component.py
+-rw-r--r--   0        0        0     4705 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/array_with_fanout.py
+-rw-r--r--   0        0        0     4322 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/array_with_via.py
+-rw-r--r--   0        0        0     4042 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/awg.py
+-rw-r--r--   0        0        0     1269 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/bbox.py
+-rw-r--r--   0        0        0     2851 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/bend_circular.py
+-rw-r--r--   0        0        0     2649 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/bend_circular_heater.py
+-rw-r--r--   0        0        0     7903 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/bend_euler.py
+-rw-r--r--   0        0        0     2682 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/bend_port.py
+-rw-r--r--   0        0        0     3664 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/bend_s.py
+-rw-r--r--   0        0        0     5373 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/bezier.py
+-rw-r--r--   0        0        0     1605 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/cavity.py
+-rw-r--r--   0        0        0     5766 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/cdc.py
+-rw-r--r--   0        0        0     2929 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/cdsem_all.py
+-rw-r--r--   0        0        0     1788 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/cdsem_bend180.py
+-rw-r--r--   0        0        0     1631 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/cdsem_coupler.py
+-rw-r--r--   0        0        0     1412 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/cdsem_straight.py
+-rw-r--r--   0        0        0     1565 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/cdsem_straight_density.py
+-rw-r--r--   0        0        0      793 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/circle.py
+-rw-r--r--   0        0        0     5722 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/coh_rx_dual_pol.py
+-rw-r--r--   0        0        0     8922 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/coh_rx_single_pol.py
+-rw-r--r--   0        0        0     5043 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/coh_tx_dual_pol.py
+-rw-r--r--   0        0        0     6118 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/coh_tx_single_pol.py
+-rw-r--r--   0        0        0     2548 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/compass.py
+-rw-r--r--   0        0        0     9876 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/component_lattice.py
+-rw-r--r--   0        0        0     7174 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/component_sequence.py
+-rw-r--r--   0        0        0      812 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/copy_layers.py
+-rw-r--r--   0        0        0     3460 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/coupler.py
+-rw-r--r--   0        0        0     2113 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/coupler90.py
+-rw-r--r--   0        0        0     1802 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/coupler90bend.py
+-rw-r--r--   0        0        0     4666 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/coupler_adiabatic.py
+-rw-r--r--   0        0        0     1909 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/coupler_asymmetric.py
+-rw-r--r--   0        0        0     3970 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/coupler_full.py
+-rw-r--r--   0        0        0     3414 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/coupler_ring.py
+-rw-r--r--   0        0        0     1060 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/coupler_straight.py
+-rw-r--r--   0        0        0     1164 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/coupler_straight_asymmetric.py
+-rw-r--r--   0        0        0     2192 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/coupler_symmetric.py
+-rw-r--r--   0        0        0     1848 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/cross.py
+-rw-r--r--   0        0        0    12873 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/crossing_waveguide.py
+-rw-r--r--   0        0        0      500 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
+-rw-r--r--   0        0        0     1014 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
+-rw-r--r--   0        0        0    19749 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
+-rw-r--r--   0        0        0    19751 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
+-rw-r--r--   0        0        0    19749 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
+-rw-r--r--   0        0        0    19751 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
+-rw-r--r--   0        0        0    19775 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
+-rw-r--r--   0        0        0     3143 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
+-rw-r--r--   0        0        0     5272 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/cutback_2x2.py
+-rw-r--r--   0        0        0     6450 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/cutback_bend.py
+-rw-r--r--   0        0        0     3765 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/cutback_component.py
+-rw-r--r--   0        0        0     2721 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/cutback_splitter.py
+-rw-r--r--   0        0        0     2971 2023-05-19 23:05:02.454286 gdsfactory-6.97.0/gdsfactory/components/dbr.py
+-rw-r--r--   0        0        0     4288 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/dbr_tapered.py
+-rw-r--r--   0        0        0     2486 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/delay_snake.py
+-rw-r--r--   0        0        0     3177 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/delay_snake2.py
+-rw-r--r--   0        0        0     3245 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/delay_snake3.py
+-rw-r--r--   0        0        0     4319 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/delay_snake_sbend.py
+-rw-r--r--   0        0        0     1226 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/dicing_lane.py
+-rw-r--r--   0        0        0     3471 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/die.py
+-rw-r--r--   0        0        0     2975 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/die_bbox.py
+-rw-r--r--   0        0        0     2863 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/die_bbox_frame.py
+-rw-r--r--   0        0        0     8015 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/disk.py
+-rw-r--r--   0        0        0     4112 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/edge_coupler_array.py
+-rw-r--r--   0        0        0     1214 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ellipse.py
+-rw-r--r--   0        0        0     1800 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/extend_ports_list.py
+-rw-r--r--   0        0        0     7988 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/extension.py
+-rw-r--r--   0        0        0      981 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/fiber.py
+-rw-r--r--   0        0        0     1432 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/fiber_array.py
+-rw-r--r--   0        0        0      722 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/fiducial_squares.py
+-rw-r--r--   0        0        0     3290 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ge_detector_straight_si_contacts.py
+-rw-r--r--   0        0        0     1063 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/grating_coupler_array.py
+-rw-r--r--   0        0        0     4682 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/grating_coupler_dual_pol.py
+-rw-r--r--   0        0        0     7110 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/grating_coupler_elliptical.py
+-rw-r--r--   0        0        0     7222 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
+-rw-r--r--   0        0        0     4961 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py
+-rw-r--r--   0        0        0     4592 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/grating_coupler_elliptical_trenches.py
+-rw-r--r--   0        0        0     1773 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/grating_coupler_functions.py
+-rw-r--r--   0        0        0     9058 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/grating_coupler_loss.py
+-rw-r--r--   0        0        0     1786 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/grating_coupler_loss_fiber_single.py
+-rw-r--r--   0        0        0     4142 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/grating_coupler_rectangular.py
+-rw-r--r--   0        0        0     4685 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
+-rw-r--r--   0        0        0     3887 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
+-rw-r--r--   0        0        0     1579 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/grating_coupler_tree.py
+-rw-r--r--   0        0        0     8811 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/greek_cross.py
+-rw-r--r--   0        0        0     1019 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/hline.py
+-rw-r--r--   0        0        0     3687 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/interdigital_capacitor.py
+-rw-r--r--   0        0        0     1825 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/litho_calipers.py
+-rw-r--r--   0        0        0     1244 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/litho_ruler.py
+-rw-r--r--   0        0        0     1304 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/litho_steps.py
+-rw-r--r--   0        0        0      650 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/logo.py
+-rw-r--r--   0        0        0     1679 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/loop_mirror.py
+-rw-r--r--   0        0        0     3873 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mmi1x2.py
+-rw-r--r--   0        0        0     2814 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mmi1x2_with_sbend.py
+-rw-r--r--   0        0        0     3858 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mmi2x2.py
+-rw-r--r--   0        0        0     3299 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mmi2x2_with_sbend.py
+-rw-r--r--   0        0        0     4947 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mmi_90degree_hybrid.py
+-rw-r--r--   0        0        0     3265 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mode_converter.py
+-rw-r--r--   0        0        0     7579 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mzi.py
+-rw-r--r--   0        0        0     2499 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mzi_arm.py
+-rw-r--r--   0        0        0     5835 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mzi_arms.py
+-rw-r--r--   0        0        0    12214 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mzi_lattice.py
+-rw-r--r--   0        0        0     4025 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mzi_pads_center.py
+-rw-r--r--   0        0        0     1064 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mzi_phase_shifter.py
+-rw-r--r--   0        0        0     6342 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mzit.py
+-rw-r--r--   0        0        0     3502 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mzit_lattice.py
+-rw-r--r--   0        0        0     6047 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/mzm.py
+-rw-r--r--   0        0        0     3518 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/nxn.py
+-rw-r--r--   0        0        0     1940 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/optimal_90deg.py
+-rw-r--r--   0        0        0     3876 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/optimal_hairpin.py
+-rw-r--r--   0        0        0     6131 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/optimal_step.py
+-rw-r--r--   0        0        0     6327 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/pack_doe.py
+-rw-r--r--   0        0        0     3860 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/pad.py
+-rw-r--r--   0        0        0     1890 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/pad_gsg.py
+-rw-r--r--   0        0        0     1157 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/pads_shorted.py
+-rw-r--r--   0        0        0     3833 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/polarization_splitter_rotator.py
+-rw-r--r--   0        0        0     1147 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ramp.py
+-rw-r--r--   0        0        0     1508 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/rectangle.py
+-rw-r--r--   0        0        0     2972 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/rectangle_with_slits.py
+-rw-r--r--   0        0        0     1508 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/regular_polygon.py
+-rw-r--r--   0        0        0     3302 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/resistance_meander.py
+-rw-r--r--   0        0        0     2642 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/resistance_sheet.py
+-rw-r--r--   0        0        0     1273 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ring.py
+-rw-r--r--   0        0        0     4143 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ring_crow.py
+-rw-r--r--   0        0        0     3272 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ring_crow_couplers.py
+-rw-r--r--   0        0        0     2267 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ring_double.py
+-rw-r--r--   0        0        0     2846 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ring_double_bend_coupler.py
+-rw-r--r--   0        0        0     3846 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ring_double_heater.py
+-rw-r--r--   0        0        0     7757 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ring_double_pn.py
+-rw-r--r--   0        0        0    12137 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ring_section_based.py
+-rw-r--r--   0        0        0     2740 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ring_single.py
+-rw-r--r--   0        0        0     1968 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ring_single_array.py
+-rw-r--r--   0        0        0     6868 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ring_single_bend_coupler.py
+-rw-r--r--   0        0        0     2714 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ring_single_dut.py
+-rw-r--r--   0        0        0     4018 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ring_single_heater.py
+-rw-r--r--   0        0        0     5267 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/ring_single_pn.py
+-rw-r--r--   0        0        0     2282 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/seal_ring.py
+-rw-r--r--   0        0        0     3758 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/snspd.py
+-rw-r--r--   0        0        0     2059 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/spiral_double.py
+-rw-r--r--   0        0        0     5871 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/spiral_external_io.py
+-rw-r--r--   0        0        0    16692 2023-05-19 23:05:02.458286 gdsfactory-6.97.0/gdsfactory/components/spiral_heater.py
+-rw-r--r--   0        0        0     9181 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/spiral_inner_io.py
+-rw-r--r--   0        0        0     1733 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/splitter_chain.py
+-rw-r--r--   0        0        0     5327 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/splitter_tree.py
+-rw-r--r--   0        0        0     2526 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/straight.py
+-rw-r--r--   0        0        0     1033 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/straight_array.py
+-rw-r--r--   0        0        0     7914 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/straight_heater_doped_rib.py
+-rw-r--r--   0        0        0     1922 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/straight_heater_doped_strip.py
+-rw-r--r--   0        0        0     7891 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/straight_heater_meander.py
+-rw-r--r--   0        0        0     8090 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/straight_heater_meander_doped.py
+-rw-r--r--   0        0        0     5686 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/straight_heater_metal.py
+-rw-r--r--   0        0        0     2809 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/straight_pin.py
+-rw-r--r--   0        0        0     3974 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/straight_pin_slot.py
+-rw-r--r--   0        0        0      655 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/straight_rib.py
+-rw-r--r--   0        0        0      820 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/switch_tree.py
+-rw-r--r--   0        0        0     7730 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/taper.py
+-rw-r--r--   0        0        0     3530 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/taper_adiabatic.py
+-rw-r--r--   0        0        0     2457 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/taper_cross_section.py
+-rw-r--r--   0        0        0     2363 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/taper_from_csv.py
+-rw-r--r--   0        0        0     1215 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/taper_parabolic.py
+-rw-r--r--   0        0        0     1635 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/terminator.py
+-rw-r--r--   0        0        0     2913 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/text.py
+-rw-r--r--   0        0        0     3821 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/text_freetype.py
+-rw-r--r--   0        0        0     3160 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/text_rectangular.py
+-rw-r--r--   0        0        0     3943 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/text_rectangular_font.py
+-rw-r--r--   0        0        0     2536 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/triangles.py
+-rw-r--r--   0        0        0      715 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/verniers.py
+-rw-r--r--   0        0        0     2468 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/version_stamp.py
+-rw-r--r--   0        0        0     2436 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/via.py
+-rw-r--r--   0        0        0     3060 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/via_corner.py
+-rw-r--r--   0        0        0     5342 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/via_cutback.py
+-rw-r--r--   0        0        0    15612 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/via_stack.py
+-rw-r--r--   0        0        0     4430 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/via_stack_slot.py
+-rw-r--r--   0        0        0     4944 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/via_stack_with_offset.py
+-rw-r--r--   0        0        0     1088 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/wafer.py
+-rw-r--r--   0        0        0     2542 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/wire.py
+-rw-r--r--   0        0        0      978 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/components/wire_sbend.py
+-rw-r--r--   0        0        0     8145 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/config.py
+-rw-r--r--   0        0        0      481 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/conftest.py
+-rw-r--r--   0        0        0    38409 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/constants.py
+-rw-r--r--   0        0        0     1476 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/containers.py
+-rw-r--r--   0        0        0    82893 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/cross_section.py
+-rw-r--r--   0        0        0     2982 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/decorators.py
+-rw-r--r--   0        0        0     7312 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/difftest.py
+-rw-r--r--   0        0        0     1020 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/events.py
+-rw-r--r--   0        0        0      204 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/export/__init__.py
+-rw-r--r--   0        0        0     3353 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/export/to_3d.py
+-rw-r--r--   0        0        0     1940 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/export/to_np.py
+-rw-r--r--   0        0        0     3058 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/export/to_stl.py
+-rw-r--r--   0        0        0     7445 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/export/write_gerbers.py
+-rw-r--r--   0        0        0     2976 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/filestorage.py
+-rw-r--r--   0        0        0    11890 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/fill.py
+-rw-r--r--   0        0        0     7799 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/font.py
+-rw-r--r--   0        0        0     8073 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/functions.py
+-rw-r--r--   0        0        0       20 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/gdsdiff/.gitattributes
+-rw-r--r--   0        0        0       83 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/gdsdiff/.gitconfig
+-rw-r--r--   0        0        0       72 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/gdsdiff/__init__.py
+-rw-r--r--   0        0        0     1069 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/gdsdiff/gds_diff_git.py
+-rw-r--r--   0        0        0     2935 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/gdsdiff/gdsdiff.py
+-rw-r--r--   0        0        0      708 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/gdsdiff/install.py
+-rw-r--r--   0        0        0      271 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/gdsdiff/sample.py
+-rw-r--r--   0        0        0     1059 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/gdsdiff/test_xor.py
+-rw-r--r--   0        0        0     1100 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/README.md
+-rw-r--r--   0        0        0     1722 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/generic_tech.sh
+-rw-r--r--   0        0        0     8142 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/get_klayout_pyxs.py
+-rw-r--r--   0        0        0      161 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/README.md
+-rw-r--r--   0        0        0      104 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/drc/Makefile
+-rw-r--r--   0        0        0        0 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/drc/__init__.py
+-rw-r--r--   0        0        0     2842 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/drc/errors.py
+-rw-r--r--   0        0        0     6193 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/grain.xml
+-rw-r--r--   0        0        0    10140 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/icon_128x128.png
+-rw-r--r--   0        0        0     4248 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/icon_64x64.png
+-rw-r--r--   0        0        0       27 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/.gitignore
+-rw-r--r--   0        0        0      494 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/Makefile
+-rw-r--r--   0        0        0     4062 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/README.md
+-rw-r--r--   0        0        0     2419 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
+-rw-r--r--   0        0        0     9696 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
+-rw-r--r--   0        0        0    12379 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
+-rw-r--r--   0        0        0     7235 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
+-rw-r--r--   0        0        0     3446 2023-05-19 23:05:02.462286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
+-rw-r--r--   0        0        0      479 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
+-rw-r--r--   0        0        0      582 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
+-rw-r--r--   0        0        0      108 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
+-rw-r--r--   0        0        0      186 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
+-rw-r--r--   0        0        0      398 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
+-rw-r--r--   0        0        0      574 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
+-rw-r--r--   0        0        0     6034 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
+-rw-r--r--   0        0        0    10704 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
+-rw-r--r--   0        0        0      477 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
+-rw-r--r--   0        0        0     4337 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
+-rw-r--r--   0        0        0      926 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
+-rw-r--r--   0        0        0    10945 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
+-rw-r--r--   0        0        0      710 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
+-rw-r--r--   0        0        0      538 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
+-rw-r--r--   0        0        0        0 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/python/__init__.py
+-rw-r--r--   0        0        0      114 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
+-rw-r--r--   0        0        0     4311 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
+-rw-r--r--   0        0        0      269 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/Makefile
+-rw-r--r--   0        0        0     1854 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25
+-rw-r--r--   0        0        0     1519 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack
+-rw-r--r--   0        0        0    41073 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
+-rw-r--r--   0        0        0    40616 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/layers.lyp
+-rw-r--r--   0        0        0     5977 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/tech.lyt
+-rw-r--r--   0        0        0     4258 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
+-rw-r--r--   0        0        0     4537 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
+-rw-r--r--   0        0        0     4690 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
+-rw-r--r--   0        0        0     5508 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
+-rw-r--r--   0        0        0     1883 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/layer_map.py
+-rw-r--r--   0        0        0     6511 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/layer_stack.py
+-rw-r--r--   0        0        0    10780 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/layer_views.yaml
+-rw-r--r--   0        0        0      158 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/generic_tech/simulation_settings.py
+-rw-r--r--   0        0        0     1431 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/__init__.py
+-rw-r--r--   0        0        0     4917 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/boolean.py
+-rw-r--r--   0        0        0     3814 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/boolean_klayout.py
+-rw-r--r--   0        0        0     1904 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/boolean_polygons.py
+-rw-r--r--   0        0        0      598 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/check_duplicated_cells.py
+-rw-r--r--   0        0        0     2719 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/check_exclusion.py
+-rw-r--r--   0        0        0     2829 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/check_inclusion.py
+-rw-r--r--   0        0        0     3566 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/check_space.py
+-rw-r--r--   0        0        0     1904 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/check_width.py
+-rw-r--r--   0        0        0     5015 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/fill_klayout.py
+-rw-r--r--   0        0        0     7084 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/fill_tiled.py
+-rw-r--r--   0        0        0     1697 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/fillet.py
+-rw-r--r--   0        0        0     6664 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/functions.py
+-rw-r--r--   0        0        0     2167 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/invert.py
+-rw-r--r--   0        0        0     3685 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/layer_priority.py
+-rw-r--r--   0        0        0     3054 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/manhattanize.py
+-rw-r--r--   0        0        0     4192 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/maskprep.py
+-rw-r--r--   0        0        0     4812 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/maskprep_flat.py
+-rw-r--r--   0        0        0     3250 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/offset.py
+-rw-r--r--   0        0        0     3842 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/outline.py
+-rw-r--r--   0        0        0     2510 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/trim.py
+-rw-r--r--   0        0        0     2948 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/union.py
+-rw-r--r--   0        0        0     3023 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/write_connectivity.py
+-rw-r--r--   0        0        0    10532 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/write_drc.py
+-rw-r--r--   0        0        0     1783 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/geometry/xor_diff.py
+-rw-r--r--   0        0        0     1158 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/get_factories.py
+-rw-r--r--   0        0        0    23569 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/get_netlist.py
+-rw-r--r--   0        0        0    14446 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/get_netlist_flat.py
+-rw-r--r--   0        0        0      682 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/get_netlist_klayout.py
+-rw-r--r--   0        0        0     9745 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/grid.py
+-rw-r--r--   0        0        0     4393 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/install.py
+-rw-r--r--   0        0        0     1970 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/klive.py
+-rw-r--r--   0        0        0      585 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/labels/__init__.py
+-rw-r--r--   0        0        0     3563 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/labels/add_label_yaml.py
+-rw-r--r--   0        0        0     3847 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/labels/ehva.py
+-rw-r--r--   0        0        0     3810 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/labels/merge_test_metadata.py
+-rw-r--r--   0        0        0     4668 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/labels/siepic.py
+-rw-r--r--   0        0        0     4847 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/labels/write_labels.py
+-rw-r--r--   0        0        0     1149 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/materials.py
+-rw-r--r--   0        0        0     5247 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/name.py
+-rw-r--r--   0        0        0    11586 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/pack.py
+-rw-r--r--   0        0        0    50930 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/path.py
+-rw-r--r--   0        0        0    27294 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/pdk.py
+-rw-r--r--   0        0        0     6220 2023-05-19 23:05:02.466286 gdsfactory-6.97.0/gdsfactory/picmodel.py
+-rw-r--r--   0        0        0     5068 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/pixelate.py
+-rw-r--r--   0        0        0        0 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/plugins/dagster/__init__.py
+-rw-r--r--   0        0        0      976 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/plugins/dagster/workflow.py
+-rw-r--r--   0        0        0      566 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/plugins/database/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/plugins/database/__init__.py
+-rw-r--r--   0        0        0     6216 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/plugins/database/db_upload.py
+-rw-r--r--   0        0        0    16143 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/plugins/database/models.py
+-rw-r--r--   0        0        0       32 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/plugins/web/Makefile
+-rw-r--r--   0        0        0       23 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/plugins/web/__init__.py
+-rw-r--r--   0        0        0     4080 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/plugins/web/main.py
+-rwxr-xr-x   0        0        0     7511 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/plugins/web/server.py
+-rwxr-xr-x   0        0        0      594 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/plugins/web/server_jupyter.py
+-rw-r--r--   0        0        0     1299 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/plugins/web/static/client.css
+-rw-r--r--   0        0        0    32235 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/port.py
+-rw-r--r--   0        0        0    37817 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/quickplotter.py
+-rw-r--r--   0        0        0      696 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/read/__init__.py
+-rw-r--r--   0        0        0     1639 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/read/from_dphox.py
+-rw-r--r--   0        0        0     1285 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/read/from_gdspaths.py
+-rw-r--r--   0        0        0     1953 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/read/from_np.py
+-rw-r--r--   0        0        0     2813 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/read/from_phidl.py
+-rw-r--r--   0        0        0    38082 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/read/from_yaml.py
+-rw-r--r--   0        0        0     5897 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/read/from_yaml_template.py
+-rw-r--r--   0        0        0     5688 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/read/import_gds.py
+-rw-r--r--   0        0        0     3407 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/read/labels.py
+-rw-r--r--   0        0        0     3769 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/__init__.py
+-rw-r--r--   0        0        0     2920 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/add_electrical_pads_shortest.py
+-rw-r--r--   0        0        0     3015 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/add_electrical_pads_top.py
+-rw-r--r--   0        0        0     3035 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/add_electrical_pads_top_dc.py
+-rw-r--r--   0        0        0     8715 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/add_fiber_array.py
+-rw-r--r--   0        0        0    10624 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/add_fiber_single.py
+-rw-r--r--   0        0        0     8967 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/add_pads.py
+-rw-r--r--   0        0        0    38948 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/all_angle.py
+-rw-r--r--   0        0        0     3916 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/auto_taper.py
+-rw-r--r--   0        0        0      982 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/factories.py
+-rw-r--r--   0        0        0     4415 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/fanout.py
+-rw-r--r--   0        0        0     2800 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/fanout2x2.py
+-rw-r--r--   0        0        0    24342 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/get_bundle.py
+-rw-r--r--   0        0        0     8652 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/get_bundle_corner.py
+-rw-r--r--   0        0        0     6910 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/get_bundle_from_steps.py
+-rw-r--r--   0        0        0    12949 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/get_bundle_from_waypoints.py
+-rw-r--r--   0        0        0     5284 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/get_bundle_path_length_match.py
+-rw-r--r--   0        0        0     1937 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/get_bundle_sbend.py
+-rw-r--r--   0        0        0    17064 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/get_bundle_u.py
+-rw-r--r--   0        0        0     1510 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/get_input_labels.py
+-rw-r--r--   0        0        0     9233 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/get_route.py
+-rw-r--r--   0        0        0    10872 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/get_route_astar.py
+-rw-r--r--   0        0        0     6119 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/get_route_from_steps.py
+-rw-r--r--   0        0        0     2766 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/get_route_sbend.py
+-rw-r--r--   0        0        0     3311 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/get_routes_bend180.py
+-rw-r--r--   0        0        0     1854 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/get_routes_straight.py
+-rw-r--r--   0        0        0    34394 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/manhattan.py
+-rw-r--r--   0        0        0    10081 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/path_length_matching.py
+-rw-r--r--   0        0        0    22568 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/route_fiber_array.py
+-rw-r--r--   0        0        0     8679 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/route_fiber_single.py
+-rw-r--r--   0        0        0    18132 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/route_ports_to_side.py
+-rw-r--r--   0        0        0     4379 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/route_quad.py
+-rw-r--r--   0        0        0    14370 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/route_sharp.py
+-rw-r--r--   0        0        0    10167 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/route_south.py
+-rw-r--r--   0        0        0     5072 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/sort_ports.py
+-rw-r--r--   0        0        0     2477 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/routing/utils.py
+-rw-r--r--   0        0        0     2897 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/samples/01_component_pcell.py
+-rw-r--r--   0        0        0      646 2023-05-19 23:05:02.470286 gdsfactory-6.97.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
+-rw-r--r--   0        0        0     1109 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/01_component_pcell_with_pins.py
+-rw-r--r--   0        0        0      664 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
+-rw-r--r--   0        0        0      347 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/02_component_autoname.py
+-rw-r--r--   0        0        0      887 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/03_move.py
+-rw-r--r--   0        0        0      881 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/04_connect.py
+-rw-r--r--   0        0        0      710 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/05_remove_layers.py
+-rw-r--r--   0        0        0      931 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/06_remapping_layers.py
+-rw-r--r--   0        0        0     1082 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/07_flattening_device.py
+-rw-r--r--   0        0        0      475 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/08_group.py
+-rw-r--r--   0        0        0     1631 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/11_component_layout.py
+-rw-r--r--   0        0        0     2245 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/12_component_refs.py
+-rw-r--r--   0        0        0      955 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/13_component_netlist.py
+-rw-r--r--   0        0        0     2592 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/14_component_connectivity.py
+-rw-r--r--   0        0        0     1636 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/15_component_sequence1.py
+-rw-r--r--   0        0        0     1680 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/16_component_sequence2.py
+-rw-r--r--   0        0        0      965 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/17_ports.py
+-rw-r--r--   0        0        0      489 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/18_port_markers.py
+-rw-r--r--   0        0        0      361 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/19_references.py
+-rw-r--r--   0        0        0      533 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/20_components.py
+-rw-r--r--   0        0        0      507 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/21_add_fiber_array.py
+-rw-r--r--   0        0        0      493 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/22_add_fiber_single.py
+-rw-r--r--   0        0        0      569 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/22_add_pads.py
+-rw-r--r--   0        0        0      848 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/23_reticle.py
+-rw-r--r--   0        0        0     1588 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/23_reticle_passives.py
+-rw-r--r--   0        0        0      457 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/24_doe.py
+-rw-r--r--   0        0        0      687 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/24_doe_2.py
+-rw-r--r--   0        0        0      692 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/24_doe_3.py
+-rw-r--r--   0        0        0      306 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/25_slot_cross_section.py
+-rw-r--r--   0        0        0     1363 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/30_lidar.py
+-rw-r--r--   0        0        0     1412 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/30_lidar_pcell.py
+-rw-r--r--   0        0        0     1943 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/30_lidar_with_pads.py
+-rw-r--r--   0        0        0        0 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/__init__.py
+-rw-r--r--   0        0        0     1307 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing.py
+-rw-r--r--   0        0        0      558 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
+-rw-r--r--   0        0        0     6062 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
+-rw-r--r--   0        0        0      444 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
+-rw-r--r--   0        0        0      463 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
+-rw-r--r--   0        0        0     1552 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
+-rw-r--r--   0        0        0     1315 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
+-rw-r--r--   0        0        0      602 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
+-rw-r--r--   0        0        0     3317 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
+-rw-r--r--   0        0        0     1484 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
+-rw-r--r--   0        0        0     3045 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
+-rw-r--r--   0        0        0     3782 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
+-rw-r--r--   0        0        0     1988 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/big_device.py
+-rw-r--r--   0        0        0       19 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/Makefile
+-rw-r--r--   0        0        0        0 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/__init__.py
+-rw-r--r--   0        0        0     1129 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/benchmark/fill_demo.py
+-rw-r--r--   0        0        0      343 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
+-rw-r--r--   0        0        0      637 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/circuits/mask.pic.yml
+-rw-r--r--   0        0        0      622 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
+-rw-r--r--   0        0        0      569 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
+-rw-r--r--   0        0        0      453 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/circuits/pads.pic.yml
+-rw-r--r--   0        0        0      287 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/circuits/rectangles.pic.yml
+-rw-r--r--   0        0        0     2260 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/drc_errors.py
+-rw-r--r--   0        0        0     1014 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/drc_write.py
+-rw-r--r--   0        0        0     4530 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/layers.py
+-rw-r--r--   0        0        0      158 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/layers_sky130.py
+-rw-r--r--   0        0        0      364 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/layers_xsection.py
+-rw-r--r--   0        0        0     1062 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/lvs.py
+-rw-r--r--   0        0        0      574 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/demo/pcell.py
+-rw-r--r--   0        0        0     4174 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/netlists/mzi.yml
+-rw-r--r--   0        0        0     5840 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/netlists/mzi_full.yml
+-rw-r--r--   0        0        0        0 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/__init__.py
+-rw-r--r--   0        0        0     4235 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/fab_c.py
+-rw-r--r--   0        0        0      475 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/fab_d/__init__.py
+-rw-r--r--   0        0        0     1880 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py
+-rw-r--r--   0        0        0     1715 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c.py
+-rw-r--r--   0        0        0       50 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
+-rw-r--r--   0        0        0       93 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
+-rw-r--r--   0        0        0       85 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
+-rw-r--r--   0        0        0      139 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
+-rw-r--r--   0        0        0       90 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
+-rw-r--r--   0        0        0      126 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
+-rw-r--r--   0        0        0       48 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
+-rw-r--r--   0        0        0     1023 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
+-rw-r--r--   0        0        0     2140 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
+-rw-r--r--   0        0        0     1879 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
+-rw-r--r--   0        0        0     1283 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
+-rw-r--r--   0        0        0     1632 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
+-rw-r--r--   0        0        0     1061 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
+-rw-r--r--   0        0        0     1054 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
+-rw-r--r--   0        0        0     1617 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
+-rw-r--r--   0        0        0     4497 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
+-rw-r--r--   0        0        0     3625 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
+-rw-r--r--   0        0        0     3603 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
+-rw-r--r--   0        0        0     4455 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
+-rw-r--r--   0        0        0      840 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
+-rw-r--r--   0        0        0     2231 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
+-rw-r--r--   0        0        0      316 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/schematic.py
+-rw-r--r--   0        0        0    17862 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/schematic_editor.py
+-rw-r--r--   0        0        0     4194 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/serialization.py
+-rw-r--r--   0        0        0     1612 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/show.py
+-rw-r--r--   0        0        0      724 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/__init__.py
+-rw-r--r--   0        0        0     4369 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/add_simulation_markers.py
+-rw-r--r--   0        0        0     2476 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/convert_sparameters.py
+-rw-r--r--   0        0        0      547 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/devsim/__init__.py
+-rw-r--r--   0        0        0     2559 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/devsim/doping.py
+-rw-r--r--   0        0        0    11977 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/devsim/get_simulation.py
+-rw-r--r--   0        0        0    23687 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/devsim/get_simulation_xsection.py
+-rw-r--r--   0        0        0    19756 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/devsim/get_solver.py
+-rw-r--r--   0        0        0     1644 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/devsim/test_devsim.py
+-rw-r--r--   0        0        0      189 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/disable_print.py
+-rw-r--r--   0        0        0       79 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/eme/__init__.py
+-rw-r--r--   0        0        0    14784 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/eme/meow_eme.py
+-rw-r--r--   0        0        0     1787 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/eme/test_meow_simulation.py
+-rw-r--r--   0        0        0        0 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/fem/__init__.py
+-rw-r--r--   0        0        0     8968 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/fem/mode_solver.py
+-rw-r--r--   0        0        0     2221 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/fem/test_mode_solver.py
+-rw-r--r--   0        0        0     3455 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/get_effective_indices.py
+-rw-r--r--   0        0        0     3109 2023-05-19 23:05:02.474286 gdsfactory-6.97.0/gdsfactory/simulation/get_modes_path.py
+-rw-r--r--   0        0        0     3888 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/get_sparameters_path.py
+-rw-r--r--   0        0        0     2003 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/__init__.py
+-rw-r--r--   0        0        0     3194 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/get_material.py
+-rw-r--r--   0        0        0     6137 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/get_meep_geometry.py
+-rw-r--r--   0        0        0     6054 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py
+-rw-r--r--   0        0        0    11014 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/get_simulation.py
+-rw-r--r--   0        0        0    15915 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py
+-rw-r--r--   0        0        0    18182 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py
+-rw-r--r--   0        0        0    12312 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py
+-rw-r--r--   0        0        0    11914 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_eigenmode.py
+-rw-r--r--   0        0        0      832 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_materials.py
+-rw-r--r--   0        0        0    10128 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0     6642 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py
+-rw-r--r--   0        0        0    10128 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0    10093 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
+-rw-r--r--   0        0        0    10085 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    34701 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
+-rw-r--r--   0        0        0    10123 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     9966 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
+-rw-r--r--   0        0        0     9966 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    10129 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
+-rw-r--r--   0        0        0    14053 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py
+-rw-r--r--   0        0        0    21281 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py
+-rw-r--r--   0        0        0     8143 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py
+-rw-r--r--   0        0        0     9577 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py
+-rw-r--r--   0        0        0     1246 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmsh/__init__.py
+-rw-r--r--   0        0        0     6653 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmsh/break_geometry.py
+-rw-r--r--   0        0        0    11250 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmsh/mesh.py
+-rw-r--r--   0        0        0    11824 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmsh/meshtracker.py
+-rw-r--r--   0        0        0     7752 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmsh/parse_component.py
+-rw-r--r--   0        0        0     3644 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmsh/parse_gds.py
+-rw-r--r--   0        0        0     3605 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmsh/parse_layerstack.py
+-rw-r--r--   0        0        0     2990 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmsh/refine.py
+-rw-r--r--   0        0        0    10851 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py
+-rw-r--r--   0        0        0     2513 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmsh/tests/test_meshing.py
+-rw-r--r--   0        0        0    14168 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py
+-rw-r--r--   0        0        0     7441 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py
+-rw-r--r--   0        0        0    16334 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gmsh/xyz_mesh.py
+-rw-r--r--   0        0        0     1624 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/__init__.py
+-rw-r--r--   0        0        0     4368 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/get_results.py
+-rw-r--r--   0        0        0    20009 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/get_simulation.py
+-rw-r--r--   0        0        0    21071 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py
+-rw-r--r--   0        0        0     2821 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/materials.py
+-rw-r--r--   0        0        0    27439 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/modes.py
+-rw-r--r--   0        0        0     8941 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/sim_run.yaml
+-rw-r--r--   0        0        0     8114 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml
+-rw-r--r--   0        0        0     8114 2023-05-19 23:05:02.478286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml
+-rw-r--r--   0        0        0      744 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py
+-rw-r--r--   0        0        0      262 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/test_modes/test_sweep_width.csv
+-rw-r--r--   0        0        0      879 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/test_results.py
+-rw-r--r--   0        0        0     1505 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py
+-rw-r--r--   0        0        0     1270 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py
+-rw-r--r--   0        0        0     9297 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     1732 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0     1224 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/utils.py
+-rw-r--r--   0        0        0    10515 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/write_sparameters.py
+-rw-r--r--   0        0        0     7695 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0      588 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/lumerical/__init__.py
+-rw-r--r--   0        0        0    16091 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/lumerical/interconnect.py
+-rw-r--r--   0        0        0     4286 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/lumerical/read.py
+-rw-r--r--   0        0        0     3569 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/lumerical/settings.py
+-rw-r--r--   0        0        0     2368 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/lumerical/test_read_sparameters.py
+-rw-r--r--   0        0        0    19865 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py
+-rw-r--r--   0        0        0     1504 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py
+-rw-r--r--   0        0        0      932 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/__init__.py
+-rw-r--r--   0        0        0     1618 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/coupler.py
+-rw-r--r--   0        0        0     4166 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py
+-rw-r--r--   0        0        0     2773 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/find_mode_dispersion.py
+-rw-r--r--   0        0        0     8924 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/find_modes.py
+-rwxr-xr-x   0        0        0     7032 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/find_modes_cross_section.py
+-rw-r--r--   0        0        0     4458 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py
+-rw-r--r--   0        0        0     2728 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/find_neff_vs_width.py
+-rw-r--r--   0        0        0     7148 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py
+-rwxr-xr-x   0        0        0     4462 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py
+-rw-r--r--   0        0        0     5411 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/get_mode_solver_rib.py
+-rw-r--r--   0        0        0     1110 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv
+-rw-r--r--   0        0        0     1102 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv
+-rw-r--r--   0        0        0     1110 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv
+-rw-r--r--   0        0        0     8023 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/neff_convergence_test.py
+-rw-r--r--   0        0        0      267 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/neff_vs_width.csv
+-rw-r--r--   0        0        0     2469 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/overlap.py
+-rw-r--r--   0        0        0      418 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/tests/test_dw_dh.py
+-rw-r--r--   0        0        0       83 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh.csv
+-rw-r--r--   0        0        0      548 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
+-rw-r--r--   0        0        0     1137 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/tests/test_find_modes.py
+-rw-r--r--   0        0        0      649 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py
+-rw-r--r--   0        0        0      354 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/tests/test_neff_vs_width.py
+-rw-r--r--   0        0        0      113 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
+-rw-r--r--   0        0        0    15492 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/types.py
+-rw-r--r--   0        0        0     1169 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/modes/waveguide.py
+-rw-r--r--   0        0        0     2013 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/photonic_circuit_models/__init__.py
+-rw-r--r--   0        0        0      597 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/photonic_circuit_models/coupler.py
+-rw-r--r--   0        0        0      377 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/photonic_circuit_models/fsr.py
+-rw-r--r--   0        0        0      418 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/photonic_circuit_models/heater.py
+-rw-r--r--   0        0        0     3069 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/photonic_circuit_models/mzi.py
+-rw-r--r--   0        0        0     2616 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/photonic_circuit_models/ring.py
+-rw-r--r--   0        0        0     7332 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/plot.py
+-rw-r--r--   0        0        0     2480 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/plot_csv.py
+-rw-r--r--   0        0        0      703 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/port_symmetries.py
+-rw-r--r--   0        0        0     4685 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/process/diffusion.py
+-rw-r--r--   0        0        0     5317 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/process/implant_tables.py
+-rw-r--r--   0        0        0     6800 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/process/pysrim.py
+-rw-r--r--   0        0        0     2182 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/process/silicon.py
+-rw-r--r--   0        0        0     1861 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv
+-rw-r--r--   0        0        0     1050 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv
+-rw-r--r--   0        0        0     1468 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/process/skew/boron_si_skew.csv
+-rw-r--r--   0        0        0     1118 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv
+-rw-r--r--   0        0        0      191 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/sax/__init__.py
+-rw-r--r--   0        0        0    14848 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/sax/build_model.py
+-rw-r--r--   0        0        0     7449 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/sax/femwell_waveguide_model.py
+-rw-r--r--   0        0        0     1571 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/sax/interpolators.py
+-rw-r--r--   0        0        0     6755 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/sax/meep_FDTD_model.py
+-rw-r--r--   0        0        0     4528 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/sax/meow_eme_model.py
+-rw-r--r--   0        0        0     5613 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/sax/mlp.py
+-rw-r--r--   0        0        0     7358 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/sax/models.py
+-rw-r--r--   0        0        0    13894 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/sax/parameter.py
+-rwxr-xr-x   0        0        0     2225 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/sax/plot_model.py
+-rw-r--r--   0        0        0     6805 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/sax/read.py
+-rw-r--r--   0        0        0     1350 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/sax/tests/test_mzi.py
+-rw-r--r--   0        0        0     2220 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py
+-rw-r--r--   0        0        0     1405 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/sax/tests/test_parameters.py
+-rw-r--r--   0        0        0     1357 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/__init__.py
+-rw-r--r--   0        0        0     1573 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/add_gc.py
+-rw-r--r--   0        0        0     3383 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/circuit.py
+-rw-r--r--   0        0        0      891 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/__init__.py
+-rw-r--r--   0        0        0     1295 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/bend_circular.py
+-rw-r--r--   0        0        0     1388 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/bend_euler.py
+-rw-r--r--   0        0        0     2560 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/coupler.py
+-rw-r--r--   0        0        0     1046 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py
+-rw-r--r--   0        0        0     1848 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/coupler_ring.py
+-rw-r--r--   0        0        0     1329 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py
+-rw-r--r--   0        0        0      589 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py
+-rw-r--r--   0        0        0      913 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/gc.py
+-rw-r--r--   0        0        0     2032 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/mmi1x2.py
+-rw-r--r--   0        0        0     1910 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/mmi2x2.py
+-rw-r--r--   0        0        0     2618 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/mzi.py
+-rw-r--r--   0        0        0     1759 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/mzi_siepic.py
+-rw-r--r--   0        0        0      487 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/mzi_thermal.py
+-rw-r--r--   0        0        0     2597 2023-05-19 23:05:02.482286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/ring_double.py
+-rw-r--r--   0        0        0     1665 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py
+-rw-r--r--   0        0        0     1782 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/ring_single.py
+-rw-r--r--   0        0        0     1416 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py
+-rw-r--r--   0        0        0     1099 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/straight.py
+-rw-r--r--   0        0        0      800 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/get_transmission.py
+-rw-r--r--   0        0        0     2516 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py
+-rw-r--r--   0        0        0     3841 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/model_from_sparameters.py
+-rw-r--r--   0        0        0     2438 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/plot_circuit.py
+-rw-r--r--   0        0        0     1798 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py
+-rw-r--r--   0        0        0     2773 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/plot_model.py
+-rw-r--r--   0        0        0     1261 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_circuit.py
+-rw-r--r--   0        0        0       90 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_circuit/test_circuit_transmission.yml
+-rw-r--r--   0        0        0     1109 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_components.py
+-rw-r--r--   0        0        0       66 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_mzi_.yml
+-rw-r--r--   0        0        0       69 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_double_.yml
+-rw-r--r--   0        0        0       69 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_single_.yml
+-rw-r--r--   0        0        0       92 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_circular_.yml
+-rw-r--r--   0        0        0       92 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_euler_.yml
+-rw-r--r--   0        0        0      412 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_.yml
+-rw-r--r--   0        0        0      412 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_ring_.yml
+-rw-r--r--   0        0        0      114 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_gc1550te_.yml
+-rw-r--r--   0        0        0      256 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi1x2_.yml
+-rw-r--r--   0        0        0      460 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi2x2_.yml
+-rw-r--r--   0        0        0      104 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_straight_.yml
+-rw-r--r--   0        0        0      166 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/simphony/types.py
+-rw-r--r--   0        0        0      471 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/sipann/__init__.py
+-rw-r--r--   0        0        0     1376 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/sipann/bend_circular.py
+-rw-r--r--   0        0        0     1465 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/sipann/bend_euler.py
+-rw-r--r--   0        0        0     2508 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/sipann/coupler.py
+-rw-r--r--   0        0        0     1892 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/sipann/coupler_ring.py
+-rw-r--r--   0        0        0      736 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/sipann/straight.py
+-rw-r--r--   0        0        0      100 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/thermal/__init__.py
+-rw-r--r--   0        0        0     7789 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/simulation/thermal/heater.py
+-rw-r--r--   0        0        0     1744 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/snap.py
+-rw-r--r--   0        0        0     4245 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/symbols.py
+-rw-r--r--   0        0        0      524 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/technology/__init__.py
+-rw-r--r--   0        0        0     7607 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/technology/klayout_tech.py
+-rw-r--r--   0        0        0     1078 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/technology/layer_map.py
+-rw-r--r--   0        0        0    16139 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/technology/layer_stack.py
+-rw-r--r--   0        0        0    42133 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/technology/layer_views.py
+-rw-r--r--   0        0        0     1984 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/technology/simulation_settings.py
+-rw-r--r--   0        0        0     1635 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/types.py
+-rw-r--r--   0        0        0    10008 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/typings.py
+-rw-r--r--   0        0        0        0 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/utils/__init__.py
+-rw-r--r--   0        0        0     1342 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/utils/async_utils.py
+-rw-r--r--   0        0        0      376 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/utils/color_utils.py
+-rw-r--r--   0        0        0      558 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/utils/file_utils.py
+-rw-r--r--   0        0        0      185 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/utils/function_utils.py
+-rw-r--r--   0        0        0      684 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/utils/xml_utils.py
+-rw-r--r--   0        0        0     1453 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/utils/yaml_utils.py
+-rw-r--r--   0        0        0     4865 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/watch.py
+-rw-r--r--   0        0        0        0 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/widgets/__init__.py
+-rw-r--r--   0        0        0     7969 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/widgets/layout_viewer.py
+-rw-r--r--   0        0        0     7480 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/gdsfactory/write_cells.py
+-rw-r--r--   0        0        0     5687 2023-05-19 23:05:02.486286 gdsfactory-6.97.0/pyproject.toml
+-rw-r--r--   0        0        0    18772 1970-01-01 00:00:00.000000 gdsfactory-6.97.0/PKG-INFO
```

### Comparing `gdsfactory-6.96.0/LICENSE` & `gdsfactory-6.97.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/README.md` & `gdsfactory-6.97.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gdsfactory 6.96.0
+# gdsfactory 6.97.0
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![issues](https://img.shields.io/github/issues/gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/issues)
```

### Comparing `gdsfactory-6.96.0/gdsfactory/__init__.py` & `gdsfactory-6.97.0/gdsfactory/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,18 +21,19 @@
 from functools import partial
 from toolz import compose
 from gdsfactory.component_layout import Group
 from gdsfactory.path import Path
 
 
 # NOTE: import order matters. Only change the order if you know what you are doing
-from gdsfactory.component import Component, ComponentReference, declarative_component
+from gdsfactory.component import Component, ComponentReference
 from gdsfactory.config import CONF, call_if_func, PATH, logger
 from gdsfactory.port import Port
 from gdsfactory.cell import cell
+from gdsfactory.cell import declarative_cell
 from gdsfactory.cell import cell_without_validator
 from gdsfactory.cell import clear_cache
 from gdsfactory.show import show
 from gdsfactory.read.import_gds import import_gds
 from gdsfactory.cross_section import CrossSection, Section, xsection
 from gdsfactory.component_layout import Label
 from gdsfactory import decorators
@@ -88,15 +89,14 @@
         return typings
     raise AttributeError(f"No module named {name}")
 
 
 __all__ = (
     "CONF",
     "Component",
-    "declarative_component",
     "ComponentReference",
     "CrossSection",
     "Group",
     "LAYER",
     "LAYER_STACK",
     "Label",
     "Path",
@@ -109,14 +109,15 @@
     "add_ports",
     "add_tapers",
     "add_termination",
     "asserts",
     "c",
     "call_if_func",
     "cell",
+    "declarative_cell",
     "cell_without_validator",
     "clear_cache",
     "components",
     "compose",
     "cross_section",
     "decorators",
     "fill",
@@ -147,8 +148,8 @@
     "snap",
     "typings",
     "technology",
     "write_cells",
     "xsection",
     "PATH",
 )
-__version__ = "6.96.0"
+__version__ = "6.97.0"
```

### Comparing `gdsfactory-6.96.0/gdsfactory/add_keepout.py` & `gdsfactory-6.97.0/gdsfactory/add_keepout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/add_labels.py` & `gdsfactory-6.97.0/gdsfactory/add_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/add_loopback.py` & `gdsfactory-6.97.0/gdsfactory/add_loopback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/add_padding.py` & `gdsfactory-6.97.0/gdsfactory/add_padding.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/add_pins.py` & `gdsfactory-6.97.0/gdsfactory/add_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/add_ports.py` & `gdsfactory-6.97.0/gdsfactory/add_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/add_tapers.py` & `gdsfactory-6.97.0/gdsfactory/add_tapers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/add_tapers_cross_section.py` & `gdsfactory-6.97.0/gdsfactory/add_tapers_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/add_termination.py` & `gdsfactory-6.97.0/gdsfactory/add_termination.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/asserts.py` & `gdsfactory-6.97.0/gdsfactory/asserts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/cell.py` & `gdsfactory-6.97.0/gdsfactory/cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Cell decorator for functions that return a Component."""
 from __future__ import annotations
 
 import functools
 import hashlib
 import inspect
+from dataclasses import dataclass
+from functools import wraps
 from typing import Any, Callable, Dict, Optional, Tuple, TypeVar
 
 import toolz
 from pydantic import BaseModel, validate_arguments
 
 from gdsfactory.component import Component
 from gdsfactory.name import clean_name, get_name_short
@@ -290,14 +292,34 @@
             return c
 
         mzi_with_bend_decorated = gf.cell(mzi_with_bend)
 
     """
     return cell_without_validator(validate_arguments(func))
 
+def declarative_cell(cls):
+    cls = dataclass(cls)
+    @wraps(cls)
+    def cell(*args, **kwargs):
+        decl = cls(*args, **kwargs)
+        decl.instances()
+        comp = Component()
+        for k, c in vars(decl).items():
+            if not isinstance(c, Component):
+                continue
+            ref = (comp << c)
+            setattr(comp, k, ref)
+            setattr(decl, k, ref)
+        for p1, p2 in decl.connections():
+            p1.reference.connect(p1.name, p2.reference.ports[p2.name])
+        for name, p in decl.ports().items():
+            comp.add_port(name, port=p.reference.ports[p.name])
+        return comp
+    return cell
+
 
 @cell
 def wg(length: int = 3, layer: Tuple[int, int] = (1, 0)) -> Component:
     """Dummy component for testing."""
     c = Component()
     width = 0.5
     w = width / 2
```

### Comparing `gdsfactory-6.96.0/gdsfactory/circuitviz.py` & `gdsfactory-6.97.0/gdsfactory/circuitviz.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/cli.py` & `gdsfactory-6.97.0/gdsfactory/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from gdsfactory.write_cells import write_cells as write_cells_to_separate_gds
 
 try:
     import rich_click as click
 except ImportError:
     import click
 
-VERSION = "6.96.0"
+VERSION = "6.97.0"
 LAYER_LABEL = LAYER.LABEL
 
 
 def print_version(ctx: Context, param: Option, value: bool) -> None:
     """Prints the version."""
     if not value or ctx.resilient_parsing:
         return
```

### Comparing `gdsfactory-6.96.0/gdsfactory/component.py` & `gdsfactory-6.97.0/gdsfactory/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -5549,831 +5549,800 @@
 00015ac0: 2020 2020 290a 0a20 2020 2020 2020 2063      )..        c
 00015ad0: 6f6d 706f 6e65 6e74 203d 2067 662e 436f  omponent = gf.Co
 00015ae0: 6d70 6f6e 656e 7428 290a 2020 2020 2020  mponent().      
 00015af0: 2020 636f 6d70 6f6e 656e 742e 6164 645f    component.add_
 00015b00: 706f 6c79 676f 6e28 702c 206c 6179 6572  polygon(p, layer
 00015b10: 3d6c 6179 6572 290a 2020 2020 2020 2020  =layer).        
 00015b20: 7265 7475 726e 2063 6f6d 706f 6e65 6e74  return component
-00015b30: 0a0a 0a64 6566 2064 6563 6c61 7261 7469  ...def declarati
-00015b40: 7665 5f63 6f6d 706f 6e65 6e74 2863 6c73  ve_component(cls
-00015b50: 293a 0a20 2020 2064 6563 6c20 3d20 636c  ):.    decl = cl
-00015b60: 7328 290a 2020 2020 636f 6d70 203d 2043  s().    comp = C
-00015b70: 6f6d 706f 6e65 6e74 2829 0a20 2020 2066  omponent().    f
-00015b80: 6f72 206b 2c20 7620 696e 2064 6563 6c2e  or k, v in decl.
-00015b90: 5f5f 636c 6173 735f 5f2e 5f5f 6469 6374  __class__.__dict
-00015ba0: 5f5f 2e69 7465 6d73 2829 3a0a 2020 2020  __.items():.    
-00015bb0: 2020 2020 6966 206b 2e73 7461 7274 7377      if k.startsw
-00015bc0: 6974 6828 225f 2229 206f 7220 6361 6c6c  ith("_") or call
-00015bd0: 6162 6c65 2876 293a 0a20 2020 2020 2020  able(v):.       
-00015be0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-00015bf0: 2020 2020 2020 7265 6620 3d20 636f 6d70        ref = comp
-00015c00: 203c 3c20 760a 2020 2020 2020 2020 7365   << v.        se
-00015c10: 7461 7474 7228 636f 6d70 2c20 6b2c 2072  tattr(comp, k, r
-00015c20: 6566 290a 2020 2020 2020 2020 7365 7461  ef).        seta
-00015c30: 7474 7228 6465 636c 2c20 6b2c 2072 6566  ttr(decl, k, ref
-00015c40: 290a 2020 2020 666f 7220 7031 2c20 7032  ).    for p1, p2
-00015c50: 2069 6e20 6465 636c 2e63 6f6e 6e65 6374   in decl.connect
-00015c60: 696f 6e73 2829 3a0a 2020 2020 2020 2020  ions():.        
-00015c70: 7031 2e72 6566 6572 656e 6365 2e63 6f6e  p1.reference.con
-00015c80: 6e65 6374 2870 312e 6e61 6d65 2c20 7032  nect(p1.name, p2
-00015c90: 2e72 6566 6572 656e 6365 2e70 6f72 7473  .reference.ports
-00015ca0: 5b70 322e 6e61 6d65 5d29 0a20 2020 2066  [p2.name]).    f
-00015cb0: 6f72 206e 616d 652c 2070 2069 6e20 6465  or name, p in de
-00015cc0: 636c 2e70 6f72 7473 2829 2e69 7465 6d73  cl.ports().items
-00015cd0: 2829 3a0a 2020 2020 2020 2020 636f 6d70  ():.        comp
-00015ce0: 2e61 6464 5f70 6f72 7428 6e61 6d65 2c20  .add_port(name, 
-00015cf0: 706f 7274 3d70 2e72 6566 6572 656e 6365  port=p.reference
-00015d00: 2e70 6f72 7473 5b70 2e6e 616d 655d 290a  .ports[p.name]).
-00015d10: 2020 2020 7265 7475 726e 2063 6f6d 700a      return comp.
-00015d20: 0a0a 6465 6620 636f 7079 280a 2020 2020  ..def copy(.    
-00015d30: 443a 2043 6f6d 706f 6e65 6e74 2c0a 2020  D: Component,.  
-00015d40: 2020 7265 6665 7265 6e63 6573 3d4e 6f6e    references=Non
-00015d50: 652c 0a20 2020 2070 6f72 7473 3d4e 6f6e  e,.    ports=Non
-00015d60: 652c 0a20 2020 2070 6f6c 7967 6f6e 733d  e,.    polygons=
-00015d70: 4e6f 6e65 2c0a 2020 2020 7061 7468 733d  None,.    paths=
-00015d80: 4e6f 6e65 2c0a 2020 2020 6e61 6d65 3d4e  None,.    name=N
-00015d90: 6f6e 652c 0a20 2020 206c 6162 656c 733d  one,.    labels=
-00015da0: 4e6f 6e65 2c0a 2920 2d3e 2043 6f6d 706f  None,.) -> Compo
-00015db0: 6e65 6e74 3a0a 2020 2020 2222 2252 6574  nent:.    """Ret
-00015dc0: 7572 6e73 2061 2043 6f6d 706f 6e65 6e74  urns a Component
-00015dd0: 2063 6f70 792e 0a0a 2020 2020 4172 6773   copy...    Args
-00015de0: 3a0a 2020 2020 2020 2020 443a 2063 6f6d  :.        D: com
-00015df0: 706f 6e65 6e74 2074 6f20 636f 7079 2e0a  ponent to copy..
-00015e00: 2020 2020 2222 220a 2020 2020 445f 636f      """.    D_co
-00015e10: 7079 203d 2043 6f6d 706f 6e65 6e74 2829  py = Component()
-00015e20: 0a20 2020 2044 5f63 6f70 792e 696e 666f  .    D_copy.info
-00015e30: 203d 2044 2e69 6e66 6f0a 2020 2020 2320   = D.info.    # 
-00015e40: 445f 636f 7079 2e5f 6365 6c6c 203d 2044  D_copy._cell = D
-00015e50: 2e5f 6365 6c6c 2e63 6f70 7928 6e61 6d65  ._cell.copy(name
-00015e60: 3d44 5f63 6f70 792e 6e61 6d65 290a 0a20  =D_copy.name).. 
-00015e70: 2020 2066 6f72 2072 6566 2069 6e20 7265     for ref in re
-00015e80: 6665 7265 6e63 6573 2069 6620 7265 6665  ferences if refe
-00015e90: 7265 6e63 6573 2069 7320 6e6f 7420 4e6f  rences is not No
-00015ea0: 6e65 2065 6c73 6520 442e 7265 6665 7265  ne else D.refere
-00015eb0: 6e63 6573 3a0a 2020 2020 2020 2020 445f  nces:.        D_
-00015ec0: 636f 7079 2e61 6464 2863 6f70 795f 7265  copy.add(copy_re
-00015ed0: 6665 7265 6e63 6528 7265 6629 290a 2020  ference(ref)).  
-00015ee0: 2020 666f 7220 706f 7274 2069 6e20 2870    for port in (p
-00015ef0: 6f72 7473 2069 6620 706f 7274 7320 6973  orts if ports is
-00015f00: 206e 6f74 204e 6f6e 6520 656c 7365 2044   not None else D
-00015f10: 2e70 6f72 7473 292e 7661 6c75 6573 2829  .ports).values()
-00015f20: 3a0a 2020 2020 2020 2020 445f 636f 7079  :.        D_copy
-00015f30: 2e61 6464 5f70 6f72 7428 706f 7274 3d70  .add_port(port=p
-00015f40: 6f72 7429 0a20 2020 2066 6f72 2070 6f6c  ort).    for pol
-00015f50: 7920 696e 2070 6f6c 7967 6f6e 7320 6966  y in polygons if
-00015f60: 2070 6f6c 7967 6f6e 7320 6973 206e 6f74   polygons is not
-00015f70: 204e 6f6e 6520 656c 7365 2044 2e70 6f6c   None else D.pol
-00015f80: 7967 6f6e 733a 0a20 2020 2020 2020 2044  ygons:.        D
-00015f90: 5f63 6f70 792e 6164 645f 706f 6c79 676f  _copy.add_polygo
-00015fa0: 6e28 706f 6c79 290a 2020 2020 666f 7220  n(poly).    for 
-00015fb0: 7061 7468 2069 6e20 7061 7468 7320 6966  path in paths if
-00015fc0: 2070 6174 6873 2069 7320 6e6f 7420 4e6f   paths is not No
-00015fd0: 6e65 2065 6c73 6520 442e 7061 7468 733a  ne else D.paths:
-00015fe0: 0a20 2020 2020 2020 2044 5f63 6f70 792e  .        D_copy.
-00015ff0: 6164 6428 7061 7468 290a 2020 2020 666f  add(path).    fo
-00016000: 7220 6c61 6265 6c20 696e 206c 6162 656c  r label in label
-00016010: 7320 6966 206c 6162 656c 7320 6973 206e  s if labels is n
-00016020: 6f74 204e 6f6e 6520 656c 7365 2044 2e6c  ot None else D.l
-00016030: 6162 656c 733a 0a20 2020 2020 2020 2044  abels:.        D
-00016040: 5f63 6f70 792e 6164 645f 6c61 6265 6c28  _copy.add_label(
-00016050: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
-00016060: 743d 6c61 6265 6c2e 7465 7874 2c0a 2020  t=label.text,.  
-00016070: 2020 2020 2020 2020 2020 706f 7369 7469            positi
-00016080: 6f6e 3d6c 6162 656c 2e6f 7269 6769 6e2c  on=label.origin,
-00016090: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
-000160a0: 6572 3d28 6c61 6265 6c2e 6c61 7965 722c  er=(label.layer,
-000160b0: 206c 6162 656c 2e74 6578 7474 7970 6529   label.texttype)
-000160c0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-000160d0: 2069 6620 6e61 6d65 2069 7320 6e6f 7420   if name is not 
-000160e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 445f  None:.        D_
-000160f0: 636f 7079 2e6e 616d 6520 3d20 6e61 6d65  copy.name = name
-00016100: 0a0a 2020 2020 7265 7475 726e 2044 5f63  ..    return D_c
-00016110: 6f70 790a 0a0a 6465 6620 636f 7079 5f72  opy...def copy_r
-00016120: 6566 6572 656e 6365 280a 2020 2020 7265  eference(.    re
-00016130: 662c 0a20 2020 2070 6172 656e 743d 4e6f  f,.    parent=No
-00016140: 6e65 2c0a 2020 2020 636f 6c75 6d6e 733d  ne,.    columns=
-00016150: 4e6f 6e65 2c0a 2020 2020 726f 7773 3d4e  None,.    rows=N
-00016160: 6f6e 652c 0a20 2020 2073 7061 6369 6e67  one,.    spacing
-00016170: 3d4e 6f6e 652c 0a20 2020 206f 7269 6769  =None,.    origi
-00016180: 6e3d 4e6f 6e65 2c0a 2020 2020 726f 7461  n=None,.    rota
-00016190: 7469 6f6e 3d4e 6f6e 652c 0a20 2020 206d  tion=None,.    m
-000161a0: 6167 6e69 6669 6361 7469 6f6e 3d4e 6f6e  agnification=Non
-000161b0: 652c 0a20 2020 2078 5f72 6566 6c65 6374  e,.    x_reflect
-000161c0: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 6e61  ion=None,.    na
-000161d0: 6d65 3d4e 6f6e 652c 0a20 2020 2076 313d  me=None,.    v1=
-000161e0: 4e6f 6e65 2c0a 2020 2020 7632 3d4e 6f6e  None,.    v2=Non
-000161f0: 652c 0a29 202d 3e20 436f 6d70 6f6e 656e  e,.) -> Componen
-00016200: 7452 6566 6572 656e 6365 3a0a 2020 2020  tReference:.    
-00016210: 7265 7475 726e 2043 6f6d 706f 6e65 6e74  return Component
-00016220: 5265 6665 7265 6e63 6528 0a20 2020 2020  Reference(.     
-00016230: 2020 2063 6f6d 706f 6e65 6e74 3d70 6172     component=par
-00016240: 656e 7420 6f72 2072 6566 2e70 6172 656e  ent or ref.paren
-00016250: 742c 0a20 2020 2020 2020 2063 6f6c 756d  t,.        colum
-00016260: 6e73 3d63 6f6c 756d 6e73 206f 7220 7265  ns=columns or re
-00016270: 662e 636f 6c75 6d6e 732c 0a20 2020 2020  f.columns,.     
-00016280: 2020 2072 6f77 733d 726f 7773 206f 7220     rows=rows or 
-00016290: 7265 662e 726f 7773 2c0a 2020 2020 2020  ref.rows,.      
-000162a0: 2020 7370 6163 696e 673d 7370 6163 696e    spacing=spacin
-000162b0: 6720 6f72 2072 6566 2e73 7061 6369 6e67  g or ref.spacing
-000162c0: 2c0a 2020 2020 2020 2020 6f72 6967 696e  ,.        origin
-000162d0: 3d6f 7269 6769 6e20 6f72 2072 6566 2e6f  =origin or ref.o
-000162e0: 7269 6769 6e2c 0a20 2020 2020 2020 2072  rigin,.        r
-000162f0: 6f74 6174 696f 6e3d 726f 7461 7469 6f6e  otation=rotation
-00016300: 206f 7220 7265 662e 726f 7461 7469 6f6e   or ref.rotation
-00016310: 2c0a 2020 2020 2020 2020 6d61 676e 6966  ,.        magnif
-00016320: 6963 6174 696f 6e3d 6d61 676e 6966 6963  ication=magnific
-00016330: 6174 696f 6e20 6f72 2072 6566 2e6d 6167  ation or ref.mag
-00016340: 6e69 6669 6361 7469 6f6e 2c0a 2020 2020  nification,.    
-00016350: 2020 2020 785f 7265 666c 6563 7469 6f6e      x_reflection
-00016360: 3d78 5f72 6566 6c65 6374 696f 6e20 6f72  =x_reflection or
-00016370: 2072 6566 2e78 5f72 6566 6c65 6374 696f   ref.x_reflectio
-00016380: 6e2c 0a20 2020 2020 2020 206e 616d 653d  n,.        name=
-00016390: 6e61 6d65 206f 7220 7265 662e 6e61 6d65  name or ref.name
-000163a0: 2c0a 2020 2020 2020 2020 7631 3d76 3120  ,.        v1=v1 
-000163b0: 6f72 2072 6566 2e76 312c 0a20 2020 2020  or ref.v1,.     
-000163c0: 2020 2076 323d 7632 206f 7220 7265 662e     v2=v2 or ref.
-000163d0: 7632 2c0a 2020 2020 290a 0a0a 6465 6620  v2,.    )...def 
-000163e0: 7465 7374 5f67 6574 5f6c 6179 6572 7328  test_get_layers(
-000163f0: 2920 2d3e 2043 6f6d 706f 6e65 6e74 3a0a  ) -> Component:.
-00016400: 2020 2020 696d 706f 7274 2067 6473 6661      import gdsfa
-00016410: 6374 6f72 7920 6173 2067 660a 0a20 2020  ctory as gf..   
-00016420: 2063 3120 3d20 6766 2e63 6f6d 706f 6e65   c1 = gf.compone
-00016430: 6e74 732e 7374 7261 6967 6874 280a 2020  nts.straight(.  
-00016440: 2020 2020 2020 6c65 6e67 7468 3d31 302c        length=10,
-00016450: 0a20 2020 2020 2020 2077 6964 7468 3d30  .        width=0
-00016460: 2e35 2c0a 2020 2020 2020 2020 6c61 7965  .5,.        laye
-00016470: 723d 2832 2c20 3029 2c0a 2020 2020 2020  r=(2, 0),.      
-00016480: 2020 6262 6f78 5f6c 6179 6572 733d 5b28    bbox_layers=[(
-00016490: 3131 312c 2030 295d 2c0a 2020 2020 2020  111, 0)],.      
-000164a0: 2020 6262 6f78 5f6f 6666 7365 7473 3d5b    bbox_offsets=[
-000164b0: 335d 2c0a 2020 2020 2020 2020 7769 7468  3],.        with
-000164c0: 5f62 626f 783d 5472 7565 2c0a 2020 2020  _bbox=True,.    
-000164d0: 2020 2020 636c 6164 6469 6e67 5f6c 6179      cladding_lay
-000164e0: 6572 733d 4e6f 6e65 2c0a 2020 2020 2020  ers=None,.      
-000164f0: 2020 6164 645f 7069 6e73 3d4e 6f6e 652c    add_pins=None,
-00016500: 0a20 2020 2020 2020 2061 6464 5f62 626f  .        add_bbo
-00016510: 783d 4e6f 6e65 2c0a 2020 2020 290a 2020  x=None,.    ).  
-00016520: 2020 6173 7365 7274 2063 312e 6765 745f    assert c1.get_
-00016530: 6c61 7965 7273 2829 203d 3d20 7b28 322c  layers() == {(2,
-00016540: 2030 292c 2028 3131 312c 2030 297d 2c20   0), (111, 0)}, 
-00016550: 6331 2e67 6574 5f6c 6179 6572 7328 290a  c1.get_layers().
-00016560: 2020 2020 2320 7265 7475 726e 2063 310a      # return c1.
-00016570: 2020 2020 6332 203d 2063 312e 7265 6d6f      c2 = c1.remo
-00016580: 7665 5f6c 6179 6572 7328 5b28 3131 312c  ve_layers([(111,
-00016590: 2030 295d 290a 2020 2020 6173 7365 7274   0)]).    assert
-000165a0: 2063 322e 6765 745f 6c61 7965 7273 2829   c2.get_layers()
-000165b0: 203d 3d20 7b28 322c 2030 297d 2c20 6332   == {(2, 0)}, c2
-000165c0: 2e67 6574 5f6c 6179 6572 7328 290a 2020  .get_layers().  
-000165d0: 2020 7265 7475 726e 2063 320a 0a0a 6465    return c2...de
-000165e0: 6620 5f66 696c 7465 725f 706f 6c79 7328  f _filter_polys(
-000165f0: 706f 6c79 676f 6e73 2c20 6c61 7965 7273  polygons, layers
-00016600: 5f65 7863 6c29 3a0a 2020 2020 7265 7475  _excl):.    retu
-00016610: 726e 205b 0a20 2020 2020 2020 2070 6f6c  rn [.        pol
-00016620: 7967 6f6e 0a20 2020 2020 2020 2066 6f72  ygon.        for
-00016630: 2070 6f6c 7967 6f6e 2c20 6c61 7965 722c   polygon, layer,
-00016640: 2064 6174 6174 7970 6520 696e 207a 6970   datatype in zip
-00016650: 280a 2020 2020 2020 2020 2020 2020 706f  (.            po
-00016660: 6c79 676f 6e73 2e70 6f6c 7967 6f6e 732c  lygons.polygons,
-00016670: 2070 6f6c 7967 6f6e 732e 6c61 7965 7273   polygons.layers
-00016680: 2c20 706f 6c79 676f 6e73 2e64 6174 6174  , polygons.datat
-00016690: 7970 6573 0a20 2020 2020 2020 2029 0a20  ypes.        ). 
-000166a0: 2020 2020 2020 2069 6620 286c 6179 6572         if (layer
-000166b0: 2c20 6461 7461 7479 7065 2920 6e6f 7420  , datatype) not 
-000166c0: 696e 206c 6179 6572 735f 6578 636c 0a20  in layers_excl. 
-000166d0: 2020 205d 0a0a 0a64 6566 2072 6563 7572     ]...def recur
-000166e0: 7365 5f73 7472 7563 7475 7265 7328 0a20  se_structures(. 
-000166f0: 2020 2063 6f6d 706f 6e65 6e74 3a20 436f     component: Co
-00016700: 6d70 6f6e 656e 742c 0a20 2020 2069 676e  mponent,.    ign
-00016710: 6f72 655f 636f 6d70 6f6e 656e 7473 5f70  ore_components_p
-00016720: 7265 6669 783a 204f 7074 696f 6e61 6c5b  refix: Optional[
-00016730: 4c69 7374 5b73 7472 5d5d 203d 204e 6f6e  List[str]] = Non
-00016740: 652c 0a20 2020 2069 676e 6f72 655f 6675  e,.    ignore_fu
-00016750: 6e63 7469 6f6e 735f 7072 6566 6978 3a20  nctions_prefix: 
-00016760: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
-00016770: 725d 5d20 3d20 4e6f 6e65 2c0a 2920 2d3e  r]] = None,.) ->
-00016780: 2044 6963 745b 7374 722c 2041 6e79 5d3a   Dict[str, Any]:
-00016790: 0a20 2020 2022 2222 5265 6375 7273 6520  .    """Recurse 
-000167a0: 636f 6d70 6f6e 656e 7420 616e 6420 636f  component and co
-000167b0: 6d70 6f6e 656e 7473 2072 6566 6572 656e  mponents referen
-000167c0: 6365 7320 7265 6375 7273 6976 656c 792e  ces recursively.
-000167d0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-000167e0: 2020 2020 636f 6d70 6f6e 656e 743a 2063      component: c
-000167f0: 6f6d 706f 6e65 6e74 2074 6f20 7265 6375  omponent to recu
-00016800: 7273 652e 0a20 2020 2020 2020 2069 676e  rse..        ign
-00016810: 6f72 655f 636f 6d70 6f6e 656e 7473 5f70  ore_components_p
-00016820: 7265 6669 783a 206c 6973 7420 6f66 2070  refix: list of p
-00016830: 7265 6669 7820 746f 2069 676e 6f72 652e  refix to ignore.
-00016840: 0a20 2020 2020 2020 2069 676e 6f72 655f  .        ignore_
-00016850: 6675 6e63 7469 6f6e 735f 7072 6566 6978  functions_prefix
-00016860: 3a20 6c69 7374 206f 6620 7072 6566 6978  : list of prefix
-00016870: 2074 6f20 6967 6e6f 7265 2e0a 2020 2020   to ignore..    
-00016880: 2222 220a 2020 2020 6967 6e6f 7265 5f66  """.    ignore_f
-00016890: 756e 6374 696f 6e73 5f70 7265 6669 7820  unctions_prefix 
-000168a0: 3d20 6967 6e6f 7265 5f66 756e 6374 696f  = ignore_functio
-000168b0: 6e73 5f70 7265 6669 7820 6f72 205b 5d0a  ns_prefix or [].
-000168c0: 2020 2020 6967 6e6f 7265 5f63 6f6d 706f      ignore_compo
-000168d0: 6e65 6e74 735f 7072 6566 6978 203d 2069  nents_prefix = i
-000168e0: 676e 6f72 655f 636f 6d70 6f6e 656e 7473  gnore_components
-000168f0: 5f70 7265 6669 7820 6f72 205b 5d0a 0a20  _prefix or [].. 
-00016900: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-00016910: 6861 7361 7474 7228 636f 6d70 6f6e 656e  hasattr(componen
-00016920: 742c 2022 6675 6e63 7469 6f6e 5f6e 616d  t, "function_nam
-00016930: 6522 290a 2020 2020 2020 2020 616e 6420  e").        and 
-00016940: 636f 6d70 6f6e 656e 742e 6675 6e63 7469  component.functi
-00016950: 6f6e 5f6e 616d 6520 696e 2069 676e 6f72  on_name in ignor
-00016960: 655f 6675 6e63 7469 6f6e 735f 7072 6566  e_functions_pref
-00016970: 6978 0a20 2020 2029 3a0a 2020 2020 2020  ix.    ):.      
-00016980: 2020 7265 7475 726e 207b 7d0a 0a20 2020    return {}..   
-00016990: 2069 6620 6861 7361 7474 7228 636f 6d70   if hasattr(comp
-000169a0: 6f6e 656e 742c 2022 6e61 6d65 2229 2061  onent, "name") a
-000169b0: 6e64 2061 6e79 280a 2020 2020 2020 2020  nd any(.        
-000169c0: 636f 6d70 6f6e 656e 742e 6e61 6d65 2e73  component.name.s
-000169d0: 7461 7274 7377 6974 6828 6929 2066 6f72  tartswith(i) for
-000169e0: 2069 2069 6e20 6967 6e6f 7265 5f63 6f6d   i in ignore_com
-000169f0: 706f 6e65 6e74 735f 7072 6566 6978 0a20  ponents_prefix. 
-00016a00: 2020 2029 3a0a 2020 2020 2020 2020 7265     ):.        re
-00016a10: 7475 726e 207b 7d0a 0a20 2020 206f 7574  turn {}..    out
-00016a20: 7075 7420 3d20 7b63 6f6d 706f 6e65 6e74  put = {component
-00016a30: 2e6e 616d 653a 2064 6963 7428 636f 6d70  .name: dict(comp
-00016a40: 6f6e 656e 742e 7365 7474 696e 6773 297d  onent.settings)}
-00016a50: 0a20 2020 2066 6f72 2072 6566 6572 656e  .    for referen
-00016a60: 6365 2069 6e20 636f 6d70 6f6e 656e 742e  ce in component.
-00016a70: 7265 6665 7265 6e63 6573 3a0a 2020 2020  references:.    
-00016a80: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
-00016a90: 2020 2020 2069 7369 6e73 7461 6e63 6528       isinstance(
-00016aa0: 7265 6665 7265 6e63 652c 2043 6f6d 706f  reference, Compo
-00016ab0: 6e65 6e74 5265 6665 7265 6e63 6529 0a20  nentReference). 
-00016ac0: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
-00016ad0: 6566 6572 656e 6365 2e72 6566 5f63 656c  eference.ref_cel
-00016ae0: 6c2e 6e61 6d65 206e 6f74 2069 6e20 6f75  l.name not in ou
-00016af0: 7470 7574 0a20 2020 2020 2020 2029 3a0a  tput.        ):.
-00016b00: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00016b10: 7574 2e75 7064 6174 6528 7265 6375 7273  ut.update(recurs
-00016b20: 655f 7374 7275 6374 7572 6573 2872 6566  e_structures(ref
-00016b30: 6572 656e 6365 2e72 6566 5f63 656c 6c29  erence.ref_cell)
-00016b40: 290a 0a20 2020 2072 6574 7572 6e20 6f75  )..    return ou
-00016b50: 7470 7574 0a0a 0a64 6566 2066 6c61 7474  tput...def flatt
-00016b60: 656e 5f69 6e76 616c 6964 5f72 6566 735f  en_invalid_refs_
-00016b70: 7265 6375 7273 6976 6528 0a20 2020 2063  recursive(.    c
-00016b80: 6f6d 706f 6e65 6e74 3a20 436f 6d70 6f6e  omponent: Compon
-00016b90: 656e 742c 0a20 2020 2067 7269 645f 7369  ent,.    grid_si
-00016ba0: 7a65 3a20 4f70 7469 6f6e 616c 5b66 6c6f  ze: Optional[flo
-00016bb0: 6174 5d20 3d20 4e6f 6e65 2c0a 2020 2020  at] = None,.    
-00016bc0: 7570 6461 7465 645f 636f 6d70 6f6e 656e  updated_componen
-00016bd0: 7473 3d4e 6f6e 652c 0a20 2020 2074 7261  ts=None,.    tra
-00016be0: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
-00016bf0: 733d 4e6f 6e65 2c0a 293a 0a20 2020 2022  s=None,.):.    "
-00016c00: 2222 5265 6375 7273 6976 656c 7920 666c  ""Recursively fl
-00016c10: 6174 7465 6e73 2063 6f6d 706f 6e65 6e74  attens component
-00016c20: 2072 6566 6572 656e 6365 7320 7768 6963   references whic
-00016c30: 6820 6861 7665 2069 6e76 616c 6964 2074  h have invalid t
-00016c40: 7261 6e73 666f 726d 6174 696f 6e73 2028  ransformations (
-00016c50: 692e 652e 206e 6f6e 2d39 3020 6465 6720  i.e. non-90 deg 
-00016c60: 726f 7461 7469 6f6e 7320 6f72 2073 7562  rotations or sub
-00016c70: 2d67 7269 6420 7472 616e 736c 6174 696f  -grid translatio
-00016c80: 6e73 2920 616e 6420 7265 7475 726e 7320  ns) and returns 
-00016c90: 6120 636f 7079 2069 6620 616e 7920 7375  a copy if any su
-00016ca0: 6263 656c 6c73 2068 6176 6520 6265 656e  bcells have been
-00016cb0: 206d 6f64 6966 6965 642e 0a0a 2020 2020   modified...    
-00016cc0: 5741 524e 494e 473a 2074 6869 7320 6675  WARNING: this fu
-00016cd0: 6e63 7469 6f6e 2077 696c 6c20 7072 6f64  nction will prod
-00016ce0: 7563 6520 7361 6d65 2d6e 616d 6520 636f  uce same-name co
-00016cf0: 7069 6573 206f 6620 6365 6c6c 732e 2049  pies of cells. I
-00016d00: 7420 6973 2073 7472 6963 746c 7920 6d65  t is strictly me
-00016d10: 616e 7420 746f 2062 6520 7573 6564 206f  ant to be used o
-00016d20: 6e20 7772 6974 6520 6f66 2074 6865 2047  n write of the G
-00016d30: 4453 2066 696c 6520 616e 640a 2020 2020  DS file and.    
-00016d40: 7368 6f75 6c64 206e 6f74 2062 6520 6d69  should not be mi
-00016d50: 7865 6420 7769 7468 206f 7468 6572 2063  xed with other c
-00016d60: 656c 6c73 2c20 6f72 2079 6f75 2077 696c  ells, or you wil
-00016d70: 6c20 6c69 6b65 6c79 2065 7870 6572 6965  l likely experie
-00016d80: 6e63 6520 6973 7375 6573 2077 6974 6820  nce issues with 
-00016d90: 6475 706c 6963 6174 6520 6365 6c6c 730a  duplicate cells.
-00016da0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00016db0: 2020 2063 6f6d 706f 6e65 6e74 3a20 7468     component: th
-00016dc0: 6520 636f 6d70 6f6e 656e 7420 746f 2066  e component to f
-00016dd0: 6978 2028 696e 2070 6c61 6365 292e 0a20  ix (in place).. 
-00016de0: 2020 2020 2020 2067 7269 645f 7369 7a65         grid_size
-00016df0: 3a20 7468 6520 4744 5320 6772 6964 2073  : the GDS grid s
-00016e00: 697a 652c 2069 6e20 756d 2c20 6465 6661  ize, in um, defa
-00016e10: 756c 7473 2074 6f20 6163 7469 7665 2050  ults to active P
-00016e20: 444b 2e67 6574 5f67 7269 645f 7369 7a65  DK.get_grid_size
-00016e30: 2829 0a20 2020 2020 2020 2020 2020 2061  ().            a
-00016e40: 6e79 2074 7261 6e73 6c61 7469 6f6e 7320  ny translations 
-00016e50: 7769 7468 2068 6967 6865 7220 7265 736f  with higher reso
-00016e60: 6c75 7469 6f6e 2074 6861 6e20 7468 6973  lution than this
-00016e70: 2061 7265 2063 6f6e 7369 6465 7265 6420   are considered 
-00016e80: 696e 7661 6c69 642e 0a20 2020 2020 2020  invalid..       
-00016e90: 2075 7064 6174 6564 5f63 6f6d 706f 6e65   updated_compone
-00016ea0: 6e74 733a 2074 6865 2072 756e 6e69 6e67  nts: the running
-00016eb0: 2064 6963 7469 6f6e 6172 7920 6f66 2063   dictionary of c
-00016ec0: 6f6d 706f 6e65 6e74 7320 7768 6963 6820  omponents which 
-00016ed0: 6861 7665 2062 6565 6e20 6d6f 6469 6669  have been modifi
-00016ee0: 6564 2062 7920 7468 6973 2074 7261 6e73  ed by this trans
-00016ef0: 666f 726d 6174 696f 6e2e 2053 686f 756c  formation. Shoul
-00016f00: 6420 616c 7761 7973 2062 6520 4e6f 6e65  d always be None
-00016f10: 2c20 6578 6365 7074 2066 6f72 2072 6563  , except for rec
-00016f20: 7572 7369 7665 2069 6e76 6f63 6174 696f  ursive invocatio
-00016f30: 6e73 2e0a 2020 2020 2020 2020 7472 6176  ns..        trav
-00016f40: 6572 7365 645f 636f 6d70 6f6e 656e 7473  ersed_components
-00016f50: 3a20 7468 6520 7365 7420 6f66 2063 6f6d  : the set of com
-00016f60: 706f 6e65 6e74 206e 616d 6573 2077 6869  ponent names whi
-00016f70: 6368 2068 6176 6520 6265 656e 2074 7261  ch have been tra
-00016f80: 7665 7273 6564 2e20 5368 6f75 6c64 2061  versed. Should a
-00016f90: 6c77 6179 7320 6265 204e 6f6e 652c 2065  lways be None, e
-00016fa0: 7863 6570 7420 666f 7220 7265 6375 7273  xcept for recurs
-00016fb0: 6976 6520 696e 766f 6361 7469 6f6e 732e  ive invocations.
-00016fc0: 0a20 2020 2022 2222 0a20 2020 2066 726f  .    """.    fro
-00016fd0: 6d20 6764 7366 6163 746f 7279 2e64 6563  m gdsfactory.dec
-00016fe0: 6f72 6174 6f72 7320 696d 706f 7274 2069  orators import i
-00016ff0: 735f 696e 7661 6c69 645f 7265 660a 0a20  s_invalid_ref.. 
-00017000: 2020 2069 6e76 616c 6964 5f72 6566 7320     invalid_refs 
-00017010: 3d20 5b5d 0a20 2020 2072 6566 7320 3d20  = [].    refs = 
-00017020: 636f 6d70 6f6e 656e 742e 7265 6665 7265  component.refere
-00017030: 6e63 6573 0a20 2020 2073 7562 6365 6c6c  nces.    subcell
-00017040: 5f6d 6f64 6966 6965 6420 3d20 4661 6c73  _modified = Fals
-00017050: 650a 2020 2020 6966 2075 7064 6174 6564  e.    if updated
-00017060: 5f63 6f6d 706f 6e65 6e74 7320 6973 204e  _components is N
-00017070: 6f6e 653a 0a20 2020 2020 2020 2075 7064  one:.        upd
-00017080: 6174 6564 5f63 6f6d 706f 6e65 6e74 7320  ated_components 
-00017090: 3d20 7b7d 0a20 2020 2069 6620 7472 6176  = {}.    if trav
-000170a0: 6572 7365 645f 636f 6d70 6f6e 656e 7473  ersed_components
-000170b0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-000170c0: 2020 7472 6176 6572 7365 645f 636f 6d70    traversed_comp
-000170d0: 6f6e 656e 7473 203d 2073 6574 2829 0a20  onents = set(). 
-000170e0: 2020 2066 6f72 2072 6566 2069 6e20 7265     for ref in re
-000170f0: 6673 3a0a 2020 2020 2020 2020 2320 6d61  fs:.        # ma
-00017100: 726b 2061 6e79 2069 6e76 616c 6964 2072  rk any invalid r
-00017110: 6566 7320 666f 7220 666c 6174 7465 6e69  efs for flatteni
-00017120: 6e67 0a20 2020 2020 2020 2023 206f 7468  ng.        # oth
-00017130: 6572 7769 7365 2c20 6368 6563 6b20 6966  erwise, check if
-00017140: 2074 6865 7265 2061 7265 2061 6e79 206d   there are any m
-00017150: 6f64 6966 6965 6420 6365 6c6c 7320 6265  odified cells be
-00017160: 6e65 6174 6820 2877 6520 6e65 6564 206e  neath (we need n
-00017170: 6f74 2064 6f20 7468 6973 2069 6620 7468  ot do this if th
-00017180: 6520 7265 6620 7769 6c6c 2062 6520 666c  e ref will be fl
-00017190: 6174 7465 6e65 6420 616e 7977 6179 7329  attened anyways)
-000171a0: 0a20 2020 2020 2020 2069 6620 6973 5f69  .        if is_i
-000171b0: 6e76 616c 6964 5f72 6566 2872 6566 2c20  nvalid_ref(ref, 
-000171c0: 6772 6964 5f73 697a 6529 3a0a 2020 2020  grid_size):.    
-000171d0: 2020 2020 2020 2020 696e 7661 6c69 645f          invalid_
-000171e0: 7265 6673 2e61 7070 656e 6428 7265 662e  refs.append(ref.
-000171f0: 6e61 6d65 290a 2020 2020 2020 2020 656c  name).        el
-00017200: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00017210: 2320 6f74 6865 7277 6973 652c 2072 6563  # otherwise, rec
-00017220: 7572 7369 7665 6c79 2066 6c61 7474 656e  ursively flatten
-00017230: 2072 6566 7320 6966 2074 6865 2073 7562   refs if the sub
-00017240: 6365 6c6c 2068 6173 206e 6f74 2061 6c72  cell has not alr
-00017250: 6561 6479 2062 6565 6e20 7472 6176 6572  eady been traver
-00017260: 7365 640a 2020 2020 2020 2020 2020 2020  sed.            
-00017270: 6966 2072 6566 2e70 6172 656e 742e 6e61  if ref.parent.na
-00017280: 6d65 206e 6f74 2069 6e20 7472 6176 6572  me not in traver
-00017290: 7365 645f 636f 6d70 6f6e 656e 7473 3a0a  sed_components:.
-000172a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172b0: 666c 6174 7465 6e5f 696e 7661 6c69 645f  flatten_invalid_
-000172c0: 7265 6673 5f72 6563 7572 7369 7665 280a  refs_recursive(.
-000172d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172e0: 2020 2020 7265 662e 7061 7265 6e74 2c0a      ref.parent,.
-000172f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017300: 2020 2020 6772 6964 5f73 697a 653d 6772      grid_size=gr
-00017310: 6964 5f73 697a 652c 0a20 2020 2020 2020  id_size,.       
-00017320: 2020 2020 2020 2020 2020 2020 2075 7064               upd
-00017330: 6174 6564 5f63 6f6d 706f 6e65 6e74 733d  ated_components=
-00017340: 7570 6461 7465 645f 636f 6d70 6f6e 656e  updated_componen
-00017350: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
-00017360: 2020 2020 2020 2020 7472 6176 6572 7365          traverse
-00017370: 645f 636f 6d70 6f6e 656e 7473 3d74 7261  d_components=tra
-00017380: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
-00017390: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-000173a0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000173b0: 2023 206e 6f77 2c20 6966 2074 6865 2072   # now, if the r
-000173c0: 6566 2773 2063 656c 6c20 6265 656e 206d  ef's cell been m
-000173d0: 6f64 6966 6965 642c 206d 6172 6b20 6974  odified, mark it
-000173e0: 2061 7320 7375 6368 0a20 2020 2020 2020   as such.       
-000173f0: 2020 2020 2069 6620 7265 662e 7061 7265       if ref.pare
-00017400: 6e74 2e6e 616d 6520 696e 2075 7064 6174  nt.name in updat
-00017410: 6564 5f63 6f6d 706f 6e65 6e74 733a 0a20  ed_components:. 
-00017420: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017430: 7562 6365 6c6c 5f6d 6f64 6966 6965 6420  ubcell_modified 
-00017440: 3d20 5472 7565 0a20 2020 2069 6620 696e  = True.    if in
-00017450: 7661 6c69 645f 7265 6673 206f 7220 7375  valid_refs or su
-00017460: 6263 656c 6c5f 6d6f 6469 6669 6564 3a0a  bcell_modified:.
-00017470: 2020 2020 2020 2020 6e65 775f 636f 6d70          new_comp
-00017480: 6f6e 656e 7420 3d20 636f 6d70 6f6e 656e  onent = componen
-00017490: 742e 636f 7079 2829 0a20 2020 2020 2020  t.copy().       
-000174a0: 206e 6577 5f63 6f6d 706f 6e65 6e74 2e6e   new_component.n
-000174b0: 616d 6520 3d20 636f 6d70 6f6e 656e 742e  ame = component.
-000174c0: 6e61 6d65 0a20 2020 2020 2020 2023 206d  name.        # m
-000174d0: 616b 6520 7375 7265 2061 6c6c 206d 6f64  ake sure all mod
-000174e0: 6966 6965 6420 6365 6c6c 7320 6861 7665  ified cells have
-000174f0: 2074 6865 6972 2072 6566 6572 656e 6365   their reference
-00017500: 7320 7570 6461 7465 640a 2020 2020 2020  s updated.      
-00017510: 2020 6e65 775f 7265 6673 203d 206e 6577    new_refs = new
-00017520: 5f63 6f6d 706f 6e65 6e74 2e72 6566 6572  _component.refer
-00017530: 656e 6365 732e 636f 7079 2829 0a20 2020  ences.copy().   
-00017540: 2020 2020 2066 6f72 2072 6566 2069 6e20       for ref in 
-00017550: 6e65 775f 7265 6673 3a0a 2020 2020 2020  new_refs:.      
-00017560: 2020 2020 2020 6966 2072 6566 2e6e 616d        if ref.nam
-00017570: 6520 696e 2069 6e76 616c 6964 5f72 6566  e in invalid_ref
-00017580: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00017590: 2020 206e 6577 5f63 6f6d 706f 6e65 6e74     new_component
-000175a0: 2e66 6c61 7474 656e 5f72 6566 6572 656e  .flatten_referen
-000175b0: 6365 2872 6566 290a 2020 2020 2020 2020  ce(ref).        
-000175c0: 2020 2020 656c 6966 2028 0a20 2020 2020      elif (.     
-000175d0: 2020 2020 2020 2020 2020 2072 6566 2e70             ref.p
-000175e0: 6172 656e 742e 6e61 6d65 2069 6e20 7570  arent.name in up
-000175f0: 6461 7465 645f 636f 6d70 6f6e 656e 7473  dated_components
-00017600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017610: 2061 6e64 2072 6566 2e70 6172 656e 7420   and ref.parent 
-00017620: 6973 206e 6f74 2075 7064 6174 6564 5f63  is not updated_c
-00017630: 6f6d 706f 6e65 6e74 735b 7265 662e 7061  omponents[ref.pa
-00017640: 7265 6e74 2e6e 616d 655d 0a20 2020 2020  rent.name].     
-00017650: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00017660: 2020 2020 2020 2020 2020 7265 662e 7061            ref.pa
-00017670: 7265 6e74 203d 2075 7064 6174 6564 5f63  rent = updated_c
-00017680: 6f6d 706f 6e65 6e74 735b 7265 662e 7061  omponents[ref.pa
-00017690: 7265 6e74 2e6e 616d 655d 0a20 2020 2020  rent.name].     
-000176a0: 2020 2063 6f6d 706f 6e65 6e74 203d 206e     component = n
-000176b0: 6577 5f63 6f6d 706f 6e65 6e74 0a20 2020  ew_component.   
-000176c0: 2020 2020 2075 7064 6174 6564 5f63 6f6d       updated_com
-000176d0: 706f 6e65 6e74 735b 636f 6d70 6f6e 656e  ponents[componen
-000176e0: 742e 6e61 6d65 5d20 3d20 6e65 775f 636f  t.name] = new_co
-000176f0: 6d70 6f6e 656e 740a 2020 2020 7472 6176  mponent.    trav
-00017700: 6572 7365 645f 636f 6d70 6f6e 656e 7473  ersed_components
-00017710: 2e61 6464 2863 6f6d 706f 6e65 6e74 2e6e  .add(component.n
-00017720: 616d 6529 0a20 2020 2072 6574 7572 6e20  ame).    return 
-00017730: 636f 6d70 6f6e 656e 740a 0a0a 6465 6620  component...def 
-00017740: 5f63 6865 636b 5f75 6e63 6163 6865 645f  _check_uncached_
-00017750: 636f 6d70 6f6e 656e 7473 2863 6f6d 706f  components(compo
-00017760: 6e65 6e74 2c20 6d6f 6465 293a 0a20 2020  nent, mode):.   
-00017770: 2076 616c 6964 5f6d 6f64 6573 203d 205b   valid_modes = [
-00017780: 2277 6172 6e22 2c20 2265 7272 6f72 222c  "warn", "error",
-00017790: 2022 6967 6e6f 7265 225d 0a0a 2020 2020   "ignore"]..    
-000177a0: 6966 206d 6f64 6520 3d3d 2022 6967 6e6f  if mode == "igno
-000177b0: 7265 223a 0a20 2020 2020 2020 2072 6574  re":.        ret
-000177c0: 7572 6e0a 2020 2020 656c 6966 206d 6f64  urn.    elif mod
-000177d0: 6520 6e6f 7420 696e 2076 616c 6964 5f6d  e not in valid_m
-000177e0: 6f64 6573 3a0a 2020 2020 2020 2020 7261  odes:.        ra
-000177f0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
-00017800: 2020 2020 2020 2020 2020 2020 6622 7b6d              f"{m
-00017810: 6f64 657d 2069 7320 6e6f 7420 6120 7661  ode} is not a va
-00017820: 6c69 6420 7661 6c75 6520 666f 7220 6f6e  lid value for on
-00017830: 5f75 6e63 6163 6865 645f 636f 6d70 6f6e  _uncached_compon
-00017840: 656e 742e 2054 7279 206f 6e65 206f 6620  ent. Try one of 
-00017850: 7468 6573 653a 207b 7661 6c69 645f 6d6f  these: {valid_mo
-00017860: 6465 737d 2e22 0a20 2020 2020 2020 2029  des}.".        )
-00017870: 0a0a 2020 2020 666f 7220 7375 625f 636f  ..    for sub_co
-00017880: 6d70 6f6e 656e 7420 696e 2063 6f6d 706f  mponent in compo
-00017890: 6e65 6e74 2e67 6574 5f64 6570 656e 6465  nent.get_depende
-000178a0: 6e63 6965 7328 7265 6375 7273 6976 653d  ncies(recursive=
-000178b0: 5472 7565 293a 0a20 2020 2020 2020 2069  True):.        i
-000178c0: 6620 6e6f 7420 7375 625f 636f 6d70 6f6e  f not sub_compon
-000178d0: 656e 742e 5f6c 6f63 6b65 643a 0a20 2020  ent._locked:.   
-000178e0: 2020 2020 2020 2020 206d 6573 7361 6765           message
-000178f0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00017900: 2020 2020 2066 2243 6f6d 706f 6e65 6e74       f"Component
-00017910: 207b 7375 625f 636f 6d70 6f6e 656e 742e   {sub_component.
-00017920: 6e61 6d65 2172 7d20 7761 7320 4e4f 5420  name!r} was NOT 
-00017930: 7072 6f70 6572 6c79 206c 6f63 6b65 642e  properly locked.
-00017940: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00017950: 2020 2022 596f 7520 6e65 6564 2074 6f20     "You need to 
-00017960: 7772 6974 6520 6974 2069 6e74 6f20 6120  write it into a 
-00017970: 6675 6e63 7469 6f6e 2074 6861 7420 6861  function that ha
-00017980: 7320 7468 6520 4063 656c 6c20 6465 636f  s the @cell deco
-00017990: 7261 746f 722e 220a 2020 2020 2020 2020  rator.".        
-000179a0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000179b0: 2020 6966 206d 6f64 6520 3d3d 2022 7761    if mode == "wa
-000179c0: 726e 223a 0a20 2020 2020 2020 2020 2020  rn":.           
-000179d0: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-000179e0: 726e 286d 6573 7361 6765 2c20 556e 6361  rn(message, Unca
-000179f0: 6368 6564 436f 6d70 6f6e 656e 7457 6172  chedComponentWar
-00017a00: 6e69 6e67 2c20 7374 6163 6b6c 6576 656c  ning, stacklevel
-00017a10: 3d33 290a 0a20 2020 2020 2020 2020 2020  =3)..           
-00017a20: 2065 6c69 6620 6d6f 6465 203d 3d20 2265   elif mode == "e
-00017a30: 7272 6f72 223a 0a20 2020 2020 2020 2020  rror":.         
-00017a40: 2020 2020 2020 2072 6169 7365 2055 6e63         raise Unc
-00017a50: 6163 6865 6443 6f6d 706f 6e65 6e74 4572  achedComponentEr
-00017a60: 726f 7228 6d65 7373 6167 6529 0a0a 0a64  ror(message)...d
-00017a70: 6566 2074 6573 745f 7361 6d65 5f75 6964  ef test_same_uid
-00017a80: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
-00017a90: 696d 706f 7274 2067 6473 6661 6374 6f72  import gdsfactor
-00017aa0: 7920 6173 2067 660a 0a20 2020 2063 203d  y as gf..    c =
-00017ab0: 2043 6f6d 706f 6e65 6e74 2829 0a20 2020   Component().   
-00017ac0: 2063 203c 3c20 6766 2e63 6f6d 706f 6e65   c << gf.compone
-00017ad0: 6e74 732e 7265 6374 616e 676c 6528 290a  nts.rectangle().
-00017ae0: 2020 2020 6320 3c3c 2067 662e 636f 6d70      c << gf.comp
-00017af0: 6f6e 656e 7473 2e72 6563 7461 6e67 6c65  onents.rectangle
-00017b00: 2829 0a0a 2020 2020 7231 203d 2063 2e72  ()..    r1 = c.r
-00017b10: 6566 6572 656e 6365 735b 305d 2e70 6172  eferences[0].par
-00017b20: 656e 740a 2020 2020 7232 203d 2063 2e72  ent.    r2 = c.r
-00017b30: 6566 6572 656e 6365 735b 315d 2e70 6172  eferences[1].par
-00017b40: 656e 740a 0a20 2020 2061 7373 6572 7420  ent..    assert 
-00017b50: 7231 2e75 6964 203d 3d20 7232 2e75 6964  r1.uid == r2.uid
-00017b60: 2c20 6622 7b72 312e 7569 647d 206d 7573  , f"{r1.uid} mus
-00017b70: 7420 6571 7561 6c20 7b72 322e 7569 647d  t equal {r2.uid}
-00017b80: 220a 0a0a 6465 6620 7465 7374 5f6e 6574  "...def test_net
-00017b90: 6c69 7374 5f73 696d 706c 6528 2920 2d3e  list_simple() ->
-00017ba0: 204e 6f6e 653a 0a20 2020 2069 6d70 6f72   None:.    impor
-00017bb0: 7420 6764 7366 6163 746f 7279 2061 7320  t gdsfactory as 
-00017bc0: 6766 0a0a 2020 2020 6320 3d20 6766 2e43  gf..    c = gf.C
-00017bd0: 6f6d 706f 6e65 6e74 2829 0a20 2020 2063  omponent().    c
-00017be0: 3120 3d20 6320 3c3c 2067 662e 636f 6d70  1 = c << gf.comp
-00017bf0: 6f6e 656e 7473 2e73 7472 6169 6768 7428  onents.straight(
-00017c00: 6c65 6e67 7468 3d31 2c20 7769 6474 683d  length=1, width=
-00017c10: 3229 0a20 2020 2063 3220 3d20 6320 3c3c  2).    c2 = c <<
-00017c20: 2067 662e 636f 6d70 6f6e 656e 7473 2e73   gf.components.s
-00017c30: 7472 6169 6768 7428 6c65 6e67 7468 3d32  traight(length=2
-00017c40: 2c20 7769 6474 683d 3229 0a20 2020 2063  , width=2).    c
-00017c50: 322e 636f 6e6e 6563 7428 706f 7274 3d22  2.connect(port="
-00017c60: 6f31 222c 2064 6573 7469 6e61 7469 6f6e  o1", destination
-00017c70: 3d63 312e 706f 7274 735b 226f 3222 5d29  =c1.ports["o2"])
-00017c80: 0a20 2020 2063 2e61 6464 5f70 6f72 7428  .    c.add_port(
-00017c90: 226f 3122 2c20 706f 7274 3d63 312e 706f  "o1", port=c1.po
-00017ca0: 7274 735b 226f 3122 5d29 0a20 2020 2063  rts["o1"]).    c
-00017cb0: 2e61 6464 5f70 6f72 7428 226f 3222 2c20  .add_port("o2", 
-00017cc0: 706f 7274 3d63 322e 706f 7274 735b 226f  port=c2.ports["o
-00017cd0: 3222 5d29 0a20 2020 206e 6574 6c69 7374  2"]).    netlist
-00017ce0: 203d 2063 2e67 6574 5f6e 6574 6c69 7374   = c.get_netlist
-00017cf0: 2829 0a20 2020 2023 2070 7269 6e74 286e  ().    # print(n
-00017d00: 6574 6c69 7374 2e70 7265 7474 7928 2929  etlist.pretty())
-00017d10: 0a20 2020 2061 7373 6572 7420 6c65 6e28  .    assert len(
-00017d20: 6e65 746c 6973 745b 2269 6e73 7461 6e63  netlist["instanc
-00017d30: 6573 225d 2920 3d3d 2032 0a0a 0a64 6566  es"]) == 2...def
-00017d40: 2074 6573 745f 6e65 746c 6973 745f 7369   test_netlist_si
-00017d50: 6d70 6c65 5f77 6964 7468 5f6d 6973 6d61  mple_width_misma
-00017d60: 7463 685f 7468 726f 7773 5f65 7272 6f72  tch_throws_error
-00017d70: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
-00017d80: 696d 706f 7274 2070 7974 6573 740a 0a20  import pytest.. 
-00017d90: 2020 2069 6d70 6f72 7420 6764 7366 6163     import gdsfac
-00017da0: 746f 7279 2061 7320 6766 0a0a 2020 2020  tory as gf..    
-00017db0: 6320 3d20 6766 2e43 6f6d 706f 6e65 6e74  c = gf.Component
-00017dc0: 2829 0a20 2020 2063 3120 3d20 6320 3c3c  ().    c1 = c <<
-00017dd0: 2067 662e 636f 6d70 6f6e 656e 7473 2e73   gf.components.s
-00017de0: 7472 6169 6768 7428 6c65 6e67 7468 3d31  traight(length=1
-00017df0: 2c20 7769 6474 683d 3129 0a20 2020 2063  , width=1).    c
-00017e00: 3220 3d20 6320 3c3c 2067 662e 636f 6d70  2 = c << gf.comp
-00017e10: 6f6e 656e 7473 2e73 7472 6169 6768 7428  onents.straight(
-00017e20: 6c65 6e67 7468 3d32 2c20 7769 6474 683d  length=2, width=
-00017e30: 3229 0a20 2020 2063 322e 636f 6e6e 6563  2).    c2.connec
-00017e40: 7428 706f 7274 3d22 6f31 222c 2064 6573  t(port="o1", des
-00017e50: 7469 6e61 7469 6f6e 3d63 312e 706f 7274  tination=c1.port
-00017e60: 735b 226f 3222 5d29 0a20 2020 2063 2e61  s["o2"]).    c.a
-00017e70: 6464 5f70 6f72 7428 226f 3122 2c20 706f  dd_port("o1", po
-00017e80: 7274 3d63 312e 706f 7274 735b 226f 3122  rt=c1.ports["o1"
-00017e90: 5d29 0a20 2020 2063 2e61 6464 5f70 6f72  ]).    c.add_por
-00017ea0: 7428 226f 3222 2c20 706f 7274 3d63 322e  t("o2", port=c2.
-00017eb0: 706f 7274 735b 226f 3222 5d29 0a20 2020  ports["o2"]).   
-00017ec0: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
-00017ed0: 7365 7328 5661 6c75 6545 7272 6f72 293a  ses(ValueError):
-00017ee0: 0a20 2020 2020 2020 2063 2e67 6574 5f6e  .        c.get_n
-00017ef0: 6574 6c69 7374 2829 0a0a 0a64 6566 2074  etlist()...def t
-00017f00: 6573 745f 6e65 746c 6973 745f 636f 6d70  est_netlist_comp
-00017f10: 6c65 7828 2920 2d3e 204e 6f6e 653a 0a20  lex() -> None:. 
-00017f20: 2020 2069 6d70 6f72 7420 6764 7366 6163     import gdsfac
-00017f30: 746f 7279 2061 7320 6766 0a0a 2020 2020  tory as gf..    
-00017f40: 6320 3d20 6766 2e63 6f6d 706f 6e65 6e74  c = gf.component
-00017f50: 732e 6d7a 695f 6172 6d73 2829 0a20 2020  s.mzi_arms().   
-00017f60: 206e 6574 6c69 7374 203d 2063 2e67 6574   netlist = c.get
-00017f70: 5f6e 6574 6c69 7374 2829 0a20 2020 2023  _netlist().    #
-00017f80: 2070 7269 6e74 286e 6574 6c69 7374 2e70   print(netlist.p
-00017f90: 7265 7474 7928 2929 0a20 2020 2061 7373  retty()).    ass
-00017fa0: 6572 7420 6c65 6e28 6e65 746c 6973 745b  ert len(netlist[
-00017fb0: 2269 6e73 7461 6e63 6573 225d 2920 3d3d  "instances"]) ==
-00017fc0: 2034 2c20 6c65 6e28 6e65 746c 6973 745b   4, len(netlist[
-00017fd0: 2269 6e73 7461 6e63 6573 225d 290a 0a0a  "instances"])...
-00017fe0: 6465 6620 7465 7374 5f65 7874 7261 6374  def test_extract
-00017ff0: 2829 202d 3e20 436f 6d70 6f6e 656e 743a  () -> Component:
-00018000: 0a20 2020 2069 6d70 6f72 7420 6764 7366  .    import gdsf
-00018010: 6163 746f 7279 2061 7320 6766 0a0a 2020  actory as gf..  
-00018020: 2020 6320 3d20 6766 2e63 6f6d 706f 6e65    c = gf.compone
-00018030: 6e74 732e 7374 7261 6967 6874 280a 2020  nts.straight(.  
-00018040: 2020 2020 2020 6c65 6e67 7468 3d31 302c        length=10,
-00018050: 0a20 2020 2020 2020 2077 6964 7468 3d30  .        width=0
-00018060: 2e35 2c0a 2020 2020 2020 2020 6262 6f78  .5,.        bbox
-00018070: 5f6c 6179 6572 733d 5b67 662e 4c41 5945  _layers=[gf.LAYE
-00018080: 522e 5747 434c 4144 5d2c 0a20 2020 2020  R.WGCLAD],.     
-00018090: 2020 2062 626f 785f 6f66 6673 6574 733d     bbox_offsets=
-000180a0: 5b33 5d2c 0a20 2020 2020 2020 2077 6974  [3],.        wit
-000180b0: 685f 6262 6f78 3d54 7275 652c 0a20 2020  h_bbox=True,.   
-000180c0: 2020 2020 2063 6c61 6464 696e 675f 6c61       cladding_la
-000180d0: 7965 7273 3d4e 6f6e 652c 0a20 2020 2020  yers=None,.     
-000180e0: 2020 2061 6464 5f70 696e 733d 4e6f 6e65     add_pins=None
-000180f0: 2c0a 2020 2020 2020 2020 6164 645f 6262  ,.        add_bb
-00018100: 6f78 3d4e 6f6e 652c 0a20 2020 2029 0a20  ox=None,.    ). 
-00018110: 2020 2063 3220 3d20 632e 6578 7472 6163     c2 = c.extrac
-00018120: 7428 6c61 7965 7273 3d5b 6766 2e4c 4159  t(layers=[gf.LAY
-00018130: 4552 2e57 4743 4c41 445d 290a 0a20 2020  ER.WGCLAD])..   
-00018140: 2061 7373 6572 7420 6c65 6e28 632e 706f   assert len(c.po
-00018150: 6c79 676f 6e73 2920 3d3d 2032 2c20 6c65  lygons) == 2, le
-00018160: 6e28 632e 706f 6c79 676f 6e73 290a 2020  n(c.polygons).  
-00018170: 2020 6173 7365 7274 206c 656e 2863 322e    assert len(c2.
-00018180: 706f 6c79 676f 6e73 2920 3d3d 2031 2c20  polygons) == 1, 
-00018190: 6c65 6e28 6332 2e70 6f6c 7967 6f6e 7329  len(c2.polygons)
-000181a0: 0a20 2020 2061 7373 6572 7420 6766 2e4c  .    assert gf.L
-000181b0: 4159 4552 2e57 4743 4c41 4420 696e 2063  AYER.WGCLAD in c
-000181c0: 322e 6c61 7965 7273 0a20 2020 2072 6574  2.layers.    ret
-000181d0: 7572 6e20 6332 0a0a 0a64 6566 2068 6173  urn c2...def has
-000181e0: 685f 6669 6c65 2866 696c 6570 6174 6829  h_file(filepath)
-000181f0: 3a0a 2020 2020 6d64 3520 3d20 6861 7368  :.    md5 = hash
-00018200: 6c69 622e 6d64 3528 290a 2020 2020 6d64  lib.md5().    md
-00018210: 352e 7570 6461 7465 2866 696c 6570 6174  5.update(filepat
-00018220: 682e 7265 6164 5f62 7974 6573 2829 290a  h.read_bytes()).
-00018230: 2020 2020 7265 7475 726e 206d 6435 2e68      return md5.h
-00018240: 6578 6469 6765 7374 2829 0a0a 0a64 6566  exdigest()...def
-00018250: 2074 6573 745f 6262 6f78 5f72 6566 6572   test_bbox_refer
-00018260: 656e 6365 2829 202d 3e20 436f 6d70 6f6e  ence() -> Compon
-00018270: 656e 743a 0a20 2020 2069 6d70 6f72 7420  ent:.    import 
-00018280: 6764 7366 6163 746f 7279 2061 7320 6766  gdsfactory as gf
-00018290: 0a0a 2020 2020 6320 3d20 6766 2e43 6f6d  ..    c = gf.Com
-000182a0: 706f 6e65 6e74 2822 636f 6d70 6f6e 656e  ponent("componen
-000182b0: 745f 7769 7468 5f6f 6666 6772 6964 5f70  t_with_offgrid_p
-000182c0: 6f6c 7967 6f6e 7322 290a 2020 2020 6331  olygons").    c1
-000182d0: 203d 2063 203c 3c20 6766 2e63 6f6d 706f   = c << gf.compo
-000182e0: 6e65 6e74 732e 7265 6374 616e 676c 6528  nents.rectangle(
-000182f0: 7369 7a65 3d28 312e 3565 2d33 2c20 312e  size=(1.5e-3, 1.
-00018300: 3565 2d33 292c 2070 6f72 745f 7479 7065  5e-3), port_type
-00018310: 3d4e 6f6e 6529 0a20 2020 2063 3220 3d20  =None).    c2 = 
-00018320: 6320 3c3c 2067 662e 636f 6d70 6f6e 656e  c << gf.componen
-00018330: 7473 2e72 6563 7461 6e67 6c65 2873 697a  ts.rectangle(siz
-00018340: 653d 2831 2e35 652d 332c 2031 2e35 652d  e=(1.5e-3, 1.5e-
-00018350: 3329 2c20 706f 7274 5f74 7970 653d 4e6f  3), port_type=No
-00018360: 6e65 290a 2020 2020 6332 2e78 6d69 6e20  ne).    c2.xmin 
-00018370: 3d20 6331 2e78 6d61 780a 0a20 2020 2061  = c1.xmax..    a
-00018380: 7373 6572 7420 6332 2e78 7369 7a65 203d  ssert c2.xsize =
-00018390: 3d20 3265 2d33 0a20 2020 2072 6574 7572  = 2e-3.    retur
-000183a0: 6e20 6332 0a0a 0a64 6566 2074 6573 745f  n c2...def test_
-000183b0: 6262 6f78 5f63 6f6d 706f 6e65 6e74 2829  bbox_component()
-000183c0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 696d   -> None:.    im
-000183d0: 706f 7274 2067 6473 6661 6374 6f72 7920  port gdsfactory 
-000183e0: 6173 2067 660a 0a20 2020 2063 203d 2067  as gf..    c = g
-000183f0: 662e 636f 6d70 6f6e 656e 7473 2e72 6563  f.components.rec
-00018400: 7461 6e67 6c65 2873 697a 653d 2831 2e35  tangle(size=(1.5
-00018410: 652d 332c 2031 2e35 652d 3329 2c20 706f  e-3, 1.5e-3), po
-00018420: 7274 5f74 7970 653d 4e6f 6e65 290a 2020  rt_type=None).  
-00018430: 2020 6173 7365 7274 2063 2e78 7369 7a65    assert c.xsize
-00018440: 203d 3d20 3265 2d33 0a0a 0a64 6566 2074   == 2e-3...def t
-00018450: 6573 745f 7265 6d61 705f 6c61 7965 7273  est_remap_layers
-00018460: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
-00018470: 696d 706f 7274 2067 6473 6661 6374 6f72  import gdsfactor
-00018480: 7920 6173 2067 660a 0a20 2020 2063 203d  y as gf..    c =
-00018490: 2067 662e 636f 6d70 6f6e 656e 7473 2e73   gf.components.s
-000184a0: 7472 6169 6768 7428 6c61 7965 723d 2832  traight(layer=(2
-000184b0: 2c20 3029 290a 2020 2020 7265 6d61 7020  , 0)).    remap 
-000184c0: 3d20 632e 7265 6d61 705f 6c61 7965 7273  = c.remap_layers
-000184d0: 286c 6179 6572 6d61 703d 7b28 322c 2030  (layermap={(2, 0
-000184e0: 293a 2067 662e 4c41 5945 522e 5747 4e7d  ): gf.LAYER.WGN}
-000184f0: 290a 2020 2020 6861 7368 5f67 656f 6d65  ).    hash_geome
-00018500: 7472 7920 3d20 2233 3263 6431 3465 6137  try = "32cd14ea7
-00018510: 6365 3133 6366 3166 3433 3032 3737 6234  ce13cf1f430277b4
-00018520: 3530 3534 6130 6137 3930 3961 3363 3422  5054a0a7909a3c4"
-00018530: 0a0a 2020 2020 6173 7365 7274 2028 0a20  ..    assert (. 
-00018540: 2020 2020 2020 2072 656d 6170 2e68 6173         remap.has
-00018550: 685f 6765 6f6d 6574 7279 2829 203d 3d20  h_geometry() == 
-00018560: 6861 7368 5f67 656f 6d65 7472 790a 2020  hash_geometry.  
-00018570: 2020 292c 2066 2268 6173 685f 6765 6f6d    ), f"hash_geom
-00018580: 6574 7279 203d 207b 7265 6d61 702e 6861  etry = {remap.ha
-00018590: 7368 5f67 656f 6d65 7472 7928 2921 727d  sh_geometry()!r}
-000185a0: 220a 0a0a 6465 6620 7465 7374 5f72 656d  "...def test_rem
-000185b0: 6f76 655f 6c61 6265 6c73 2829 202d 3e20  ove_labels() -> 
-000185c0: 4e6f 6e65 3a0a 2020 2020 696d 706f 7274  None:.    import
-000185d0: 2067 6473 6661 6374 6f72 7920 6173 2067   gdsfactory as g
-000185e0: 660a 0a20 2020 2063 203d 2067 662e 632e  f..    c = gf.c.
-000185f0: 7374 7261 6967 6874 2829 0a20 2020 2063  straight().    c
-00018600: 2e72 656d 6f76 655f 6c61 6265 6c73 2829  .remove_labels()
-00018610: 0a0a 2020 2020 6173 7365 7274 206c 656e  ..    assert len
-00018620: 2863 2e6c 6162 656c 7329 203d 3d20 300a  (c.labels) == 0.
-00018630: 0a0a 6465 6620 7465 7374 5f69 6d70 6f72  ..def test_impor
-00018640: 745f 6764 735f 7365 7474 696e 6773 2829  t_gds_settings()
-00018650: 202d 3e20 4e6f 6e65 3a0a 2020 2020 696d   -> None:.    im
-00018660: 706f 7274 2067 6473 6661 6374 6f72 7920  port gdsfactory 
-00018670: 6173 2067 660a 0a20 2020 2063 203d 2067  as gf..    c = g
-00018680: 662e 636f 6d70 6f6e 656e 7473 2e6d 7a69  f.components.mzi
-00018690: 2829 0a20 2020 2067 6473 7061 7468 203d  ().    gdspath =
-000186a0: 2063 2e77 7269 7465 5f67 6473 5f77 6974   c.write_gds_wit
-000186b0: 685f 6d65 7461 6461 7461 2829 0a20 2020  h_metadata().   
-000186c0: 2063 3220 3d20 6766 2e69 6d70 6f72 745f   c2 = gf.import_
-000186d0: 6764 7328 6764 7370 6174 682c 206e 616d  gds(gdspath, nam
-000186e0: 653d 226d 7a69 5f73 616d 706c 6522 2c20  e="mzi_sample", 
-000186f0: 7265 6164 5f6d 6574 6164 6174 613d 5472  read_metadata=Tr
-00018700: 7565 290a 2020 2020 6333 203d 2067 662e  ue).    c3 = gf.
-00018710: 726f 7574 696e 672e 6164 645f 6669 6265  routing.add_fibe
-00018720: 725f 7369 6e67 6c65 2863 3229 0a20 2020  r_single(c2).   
-00018730: 2061 7373 6572 7420 6333 0a0a 0a64 6566   assert c3...def
-00018740: 2074 6573 745f 666c 6174 7465 6e5f 696e   test_flatten_in
-00018750: 7661 6c69 645f 7265 6673 5f72 6563 7572  valid_refs_recur
-00018760: 7369 7665 2829 202d 3e20 4e6f 6e65 3a0a  sive() -> None:.
-00018770: 2020 2020 696d 706f 7274 2067 6473 6661      import gdsfa
-00018780: 6374 6f72 7920 6173 2067 660a 2020 2020  ctory as gf.    
-00018790: 6672 6f6d 2067 6473 6661 6374 6f72 792e  from gdsfactory.
-000187a0: 6469 6666 7465 7374 2069 6d70 6f72 7420  difftest import 
-000187b0: 7275 6e5f 786f 720a 2020 2020 6672 6f6d  run_xor.    from
-000187c0: 2067 6473 6661 6374 6f72 792e 726f 7574   gdsfactory.rout
-000187d0: 696e 672e 616c 6c5f 616e 676c 6520 696d  ing.all_angle im
-000187e0: 706f 7274 2067 6574 5f62 756e 646c 655f  port get_bundle_
-000187f0: 616c 6c5f 616e 676c 650a 0a20 2020 2040  all_angle..    @
-00018800: 6766 2e63 656c 6c0a 2020 2020 6465 6620  gf.cell.    def 
-00018810: 666c 6174 2829 3a0a 2020 2020 2020 2020  flat():.        
-00018820: 6320 3d20 6766 2e43 6f6d 706f 6e65 6e74  c = gf.Component
-00018830: 2829 0a20 2020 2020 2020 206d 6d69 3120  ().        mmi1 
-00018840: 3d20 2863 203c 3c20 6766 2e63 6f6d 706f  = (c << gf.compo
-00018850: 6e65 6e74 732e 6d6d 6931 7832 2829 292e  nents.mmi1x2()).
-00018860: 6d6f 7665 2828 302c 202d 312e 3030 3035  move((0, -1.0005
-00018870: 2929 0a20 2020 2020 2020 206d 6d69 3220  )).        mmi2 
-00018880: 3d20 2863 203c 3c20 6766 2e63 6f6d 706f  = (c << gf.compo
-00018890: 6e65 6e74 732e 6d6d 6931 7832 2829 292e  nents.mmi1x2()).
-000188a0: 726f 7461 7465 2838 3029 0a20 2020 2020  rotate(80).     
-000188b0: 2020 206d 6d69 322e 6d6f 7665 2828 3430     mmi2.move((40
-000188c0: 2c20 3230 2929 0a20 2020 2020 2020 2062  , 20)).        b
-000188d0: 756e 646c 6520 3d20 6765 745f 6275 6e64  undle = get_bund
-000188e0: 6c65 5f61 6c6c 5f61 6e67 6c65 285b 6d6d  le_all_angle([mm
-000188f0: 6931 2e70 6f72 7473 5b22 6f32 225d 5d2c  i1.ports["o2"]],
-00018900: 205b 6d6d 6932 2e70 6f72 7473 5b22 6f31   [mmi2.ports["o1
-00018910: 225d 5d29 0a20 2020 2020 2020 2066 6f72  "]]).        for
-00018920: 2072 6f75 7465 2069 6e20 6275 6e64 6c65   route in bundle
-00018930: 3a0a 2020 2020 2020 2020 2020 2020 632e  :.            c.
-00018940: 6164 6428 726f 7574 652e 7265 6665 7265  add(route.refere
-00018950: 6e63 6573 290a 2020 2020 2020 2020 7265  nces).        re
-00018960: 7475 726e 2063 0a0a 2020 2020 4067 662e  turn c..    @gf.
-00018970: 6365 6c6c 0a20 2020 2064 6566 2068 6965  cell.    def hie
-00018980: 7261 7263 6879 2829 3a0a 2020 2020 2020  rarchy():.      
-00018990: 2020 6320 3d20 6766 2e43 6f6d 706f 6e65    c = gf.Compone
-000189a0: 6e74 2829 0a20 2020 2020 2020 2028 6320  nt().        (c 
-000189b0: 3c3c 2066 6c61 7428 2929 2e72 6f74 6174  << flat()).rotat
-000189c0: 6528 3333 290a 2020 2020 2020 2020 2863  e(33).        (c
-000189d0: 203c 3c20 666c 6174 2829 292e 726f 7461   << flat()).rota
-000189e0: 7465 2833 3329 2e6d 6f76 6528 2830 2c20  te(33).move((0, 
-000189f0: 3130 3029 290a 2020 2020 2020 2020 2863  100)).        (c
-00018a00: 203c 3c20 666c 6174 2829 292e 6d6f 7665   << flat()).move
-00018a10: 2828 3130 302c 2030 2929 0a20 2020 2020  ((100, 0)).     
-00018a20: 2020 2072 6574 7572 6e20 630a 0a20 2020     return c..   
-00018a30: 2063 5f6f 7269 6720 3d20 6869 6572 6172   c_orig = hierar
-00018a40: 6368 7928 290a 2020 2020 635f 6e65 7720  chy().    c_new 
-00018a50: 3d20 666c 6174 7465 6e5f 696e 7661 6c69  = flatten_invali
-00018a60: 645f 7265 6673 5f72 6563 7572 7369 7665  d_refs_recursive
-00018a70: 2863 5f6f 7269 6729 0a20 2020 2061 7373  (c_orig).    ass
-00018a80: 6572 7420 635f 6e65 7720 6973 206e 6f74  ert c_new is not
-00018a90: 2063 5f6f 7269 670a 2020 2020 696e 7661   c_orig.    inva
-00018aa0: 6c69 645f 7265 6673 5f66 696c 656e 616d  lid_refs_filenam
-00018ab0: 6520 3d20 2269 6e76 616c 6964 5f72 6566  e = "invalid_ref
-00018ac0: 732e 6764 7322 0a20 2020 2069 6e76 616c  s.gds".    inval
-00018ad0: 6964 5f72 6566 735f 6669 7865 645f 6669  id_refs_fixed_fi
-00018ae0: 6c65 6e61 6d65 203d 2022 696e 7661 6c69  lename = "invali
-00018af0: 645f 7265 6673 5f66 6978 6564 2e67 6473  d_refs_fixed.gds
-00018b00: 220a 2020 2020 2320 6764 7320 6669 6c65  ".    # gds file
-00018b10: 7320 7368 6f75 6c64 2073 7469 6c6c 2062  s should still b
-00018b20: 6520 7361 6d65 2074 6f20 316e 6d20 746f  e same to 1nm to
-00018b30: 6c65 7261 6e63 650a 2020 2020 635f 6f72  lerance.    c_or
-00018b40: 6967 2e77 7269 7465 5f67 6473 2869 6e76  ig.write_gds(inv
-00018b50: 616c 6964 5f72 6566 735f 6669 6c65 6e61  alid_refs_filena
-00018b60: 6d65 290a 2020 2020 635f 6e65 772e 7772  me).    c_new.wr
-00018b70: 6974 655f 6764 7328 696e 7661 6c69 645f  ite_gds(invalid_
-00018b80: 7265 6673 5f66 6978 6564 5f66 696c 656e  refs_fixed_filen
-00018b90: 616d 6529 0a20 2020 2072 756e 5f78 6f72  ame).    run_xor
-00018ba0: 2869 6e76 616c 6964 5f72 6566 735f 6669  (invalid_refs_fi
-00018bb0: 6c65 6e61 6d65 2c20 696e 7661 6c69 645f  lename, invalid_
-00018bc0: 7265 6673 5f66 6978 6564 5f66 696c 656e  refs_fixed_filen
-00018bd0: 616d 6529 0a0a 0a69 6620 5f5f 6e61 6d65  ame)...if __name
-00018be0: 5f5f 203d 3d20 225f 5f6d 6169 6e5f 5f22  __ == "__main__"
-00018bf0: 3a0a 2020 2020 2320 696d 706f 7274 2067  :.    # import g
-00018c00: 6473 6661 6374 6f72 7920 6173 2067 660a  dsfactory as gf.
-00018c10: 0a20 2020 2074 6573 745f 7265 6d61 705f  .    test_remap_
-00018c20: 6c61 7965 7273 2829 0a20 2020 2023 2063  layers().    # c
-00018c30: 203d 2067 662e 436f 6d70 6f6e 656e 7428   = gf.Component(
-00018c40: 290a 2020 2020 2320 7020 3d20 632e 6164  ).    # p = c.ad
-00018c50: 645f 706f 6c79 676f 6e28 0a20 2020 2023  d_polygon(.    #
-00018c60: 2020 2020 205b 282d 382c 2036 2c20 372c       [(-8, 6, 7,
-00018c70: 2039 292c 2028 2d36 2c20 382c 2031 372c   9), (-6, 8, 17,
-00018c80: 2035 295d 2c20 6c61 7965 723d 2831 2c20   5)], layer=(1, 
-00018c90: 3029 0a20 2020 2023 2029 2020 2320 4744  0).    # )  # GD
-00018ca0: 5320 6c61 7965 7273 2061 7265 2074 7570  S layers are tup
-00018cb0: 6c65 7320 6f66 2069 6e74 7320 2862 7574  les of ints (but
-00018cc0: 2069 6620 7765 2075 7365 206f 6e6c 7920   if we use only 
-00018cd0: 6f6e 6520 6e75 6d62 6572 2069 7420 6173  one number it as
-00018ce0: 7375 6d65 7320 7468 6520 6f74 6865 7220  sumes the other 
-00018cf0: 6e75 6d62 6572 2069 7320 3029 0a0a 2020  number is 0)..  
-00018d00: 2020 2320 6332 203d 2067 662e 436f 6d70    # c2 = gf.Comp
-00018d10: 6f6e 656e 7428 290a 2020 2020 2320 6320  onent().    # c 
-00018d20: 3d20 6766 2e63 6f6d 706f 6e65 6e74 732e  = gf.components.
-00018d30: 6d7a 6928 290a 2020 2020 2320 7072 696e  mzi().    # prin
-00018d40: 7428 632e 6765 745f 6c61 7965 725f 6e61  t(c.get_layer_na
-00018d50: 6d65 7328 2929 0a20 2020 2023 2063 203d  mes()).    # c =
-00018d60: 2067 662e 636f 6d70 6f6e 656e 7473 2e6d   gf.components.m
-00018d70: 7a69 2829 0a20 2020 2023 2070 7269 6e74  zi().    # print
-00018d80: 2863 2e67 6574 5f6c 6179 6572 5f6e 616d  (c.get_layer_nam
-00018d90: 6573 2829 290a 2020 2020 2320 7220 3d20  es()).    # r = 
-00018da0: 632e 7265 6628 290a 2020 2020 2320 6332  c.ref().    # c2
-00018db0: 2e63 6f70 795f 6368 696c 645f 696e 666f  .copy_child_info
-00018dc0: 2863 2e6e 616d 6564 5f72 6566 6572 656e  (c.named_referen
-00018dd0: 6365 735b 2273 7874 225d 290a 2020 2020  ces["sxt"]).    
-00018de0: 2320 7465 7374 5f72 656d 6170 5f6c 6179  # test_remap_lay
-00018df0: 6572 7328 290a 2020 2020 2320 6320 3d20  ers().    # c = 
-00018e00: 7465 7374 5f67 6574 5f6c 6179 6572 7328  test_get_layers(
-00018e10: 290a 2020 2020 2320 632e 706c 6f74 5f71  ).    # c.plot_q
-00018e20: 7428 290a 2020 2020 2320 632e 706c 6f74  t().    # c.plot
-00018e30: 6828 290a 2020 2020 2320 6320 3d20 7465  h().    # c = te
-00018e40: 7374 5f65 7874 7261 6374 2829 0a20 2020  st_extract().   
-00018e50: 2023 2067 6473 7061 7468 203d 2063 2e77   # gdspath = c.w
-00018e60: 7269 7465 5f67 6473 2829 0a20 2020 2023  rite_gds().    #
-00018e70: 2067 662e 7368 6f77 2867 6473 7061 7468   gf.show(gdspath
-00018e80: 290a 2020 2020 2320 632e 7368 6f77 2873  ).    # c.show(s
-00018e90: 686f 775f 706f 7274 733d 5472 7565 290a  how_ports=True).
-00018ea0: 2020 2020 2320 632e 7368 6f77 2829 0a        # c.show().
+00015b30: 0a0a 0a64 6566 2063 6f70 7928 0a20 2020  ...def copy(.   
+00015b40: 2044 3a20 436f 6d70 6f6e 656e 742c 0a20   D: Component,. 
+00015b50: 2020 2072 6566 6572 656e 6365 733d 4e6f     references=No
+00015b60: 6e65 2c0a 2020 2020 706f 7274 733d 4e6f  ne,.    ports=No
+00015b70: 6e65 2c0a 2020 2020 706f 6c79 676f 6e73  ne,.    polygons
+00015b80: 3d4e 6f6e 652c 0a20 2020 2070 6174 6873  =None,.    paths
+00015b90: 3d4e 6f6e 652c 0a20 2020 206e 616d 653d  =None,.    name=
+00015ba0: 4e6f 6e65 2c0a 2020 2020 6c61 6265 6c73  None,.    labels
+00015bb0: 3d4e 6f6e 652c 0a29 202d 3e20 436f 6d70  =None,.) -> Comp
+00015bc0: 6f6e 656e 743a 0a20 2020 2022 2222 5265  onent:.    """Re
+00015bd0: 7475 726e 7320 6120 436f 6d70 6f6e 656e  turns a Componen
+00015be0: 7420 636f 7079 2e0a 0a20 2020 2041 7267  t copy...    Arg
+00015bf0: 733a 0a20 2020 2020 2020 2044 3a20 636f  s:.        D: co
+00015c00: 6d70 6f6e 656e 7420 746f 2063 6f70 792e  mponent to copy.
+00015c10: 0a20 2020 2022 2222 0a20 2020 2044 5f63  .    """.    D_c
+00015c20: 6f70 7920 3d20 436f 6d70 6f6e 656e 7428  opy = Component(
+00015c30: 290a 2020 2020 445f 636f 7079 2e69 6e66  ).    D_copy.inf
+00015c40: 6f20 3d20 442e 696e 666f 0a20 2020 2023  o = D.info.    #
+00015c50: 2044 5f63 6f70 792e 5f63 656c 6c20 3d20   D_copy._cell = 
+00015c60: 442e 5f63 656c 6c2e 636f 7079 286e 616d  D._cell.copy(nam
+00015c70: 653d 445f 636f 7079 2e6e 616d 6529 0a0a  e=D_copy.name)..
+00015c80: 2020 2020 666f 7220 7265 6620 696e 2072      for ref in r
+00015c90: 6566 6572 656e 6365 7320 6966 2072 6566  eferences if ref
+00015ca0: 6572 656e 6365 7320 6973 206e 6f74 204e  erences is not N
+00015cb0: 6f6e 6520 656c 7365 2044 2e72 6566 6572  one else D.refer
+00015cc0: 656e 6365 733a 0a20 2020 2020 2020 2044  ences:.        D
+00015cd0: 5f63 6f70 792e 6164 6428 636f 7079 5f72  _copy.add(copy_r
+00015ce0: 6566 6572 656e 6365 2872 6566 2929 0a20  eference(ref)). 
+00015cf0: 2020 2066 6f72 2070 6f72 7420 696e 2028     for port in (
+00015d00: 706f 7274 7320 6966 2070 6f72 7473 2069  ports if ports i
+00015d10: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
+00015d20: 442e 706f 7274 7329 2e76 616c 7565 7328  D.ports).values(
+00015d30: 293a 0a20 2020 2020 2020 2044 5f63 6f70  ):.        D_cop
+00015d40: 792e 6164 645f 706f 7274 2870 6f72 743d  y.add_port(port=
+00015d50: 706f 7274 290a 2020 2020 666f 7220 706f  port).    for po
+00015d60: 6c79 2069 6e20 706f 6c79 676f 6e73 2069  ly in polygons i
+00015d70: 6620 706f 6c79 676f 6e73 2069 7320 6e6f  f polygons is no
+00015d80: 7420 4e6f 6e65 2065 6c73 6520 442e 706f  t None else D.po
+00015d90: 6c79 676f 6e73 3a0a 2020 2020 2020 2020  lygons:.        
+00015da0: 445f 636f 7079 2e61 6464 5f70 6f6c 7967  D_copy.add_polyg
+00015db0: 6f6e 2870 6f6c 7929 0a20 2020 2066 6f72  on(poly).    for
+00015dc0: 2070 6174 6820 696e 2070 6174 6873 2069   path in paths i
+00015dd0: 6620 7061 7468 7320 6973 206e 6f74 204e  f paths is not N
+00015de0: 6f6e 6520 656c 7365 2044 2e70 6174 6873  one else D.paths
+00015df0: 3a0a 2020 2020 2020 2020 445f 636f 7079  :.        D_copy
+00015e00: 2e61 6464 2870 6174 6829 0a20 2020 2066  .add(path).    f
+00015e10: 6f72 206c 6162 656c 2069 6e20 6c61 6265  or label in labe
+00015e20: 6c73 2069 6620 6c61 6265 6c73 2069 7320  ls if labels is 
+00015e30: 6e6f 7420 4e6f 6e65 2065 6c73 6520 442e  not None else D.
+00015e40: 6c61 6265 6c73 3a0a 2020 2020 2020 2020  labels:.        
+00015e50: 445f 636f 7079 2e61 6464 5f6c 6162 656c  D_copy.add_label
+00015e60: 280a 2020 2020 2020 2020 2020 2020 7465  (.            te
+00015e70: 7874 3d6c 6162 656c 2e74 6578 742c 0a20  xt=label.text,. 
+00015e80: 2020 2020 2020 2020 2020 2070 6f73 6974             posit
+00015e90: 696f 6e3d 6c61 6265 6c2e 6f72 6967 696e  ion=label.origin
+00015ea0: 2c0a 2020 2020 2020 2020 2020 2020 6c61  ,.            la
+00015eb0: 7965 723d 286c 6162 656c 2e6c 6179 6572  yer=(label.layer
+00015ec0: 2c20 6c61 6265 6c2e 7465 7874 7479 7065  , label.texttype
+00015ed0: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
+00015ee0: 2020 6966 206e 616d 6520 6973 206e 6f74    if name is not
+00015ef0: 204e 6f6e 653a 0a20 2020 2020 2020 2044   None:.        D
+00015f00: 5f63 6f70 792e 6e61 6d65 203d 206e 616d  _copy.name = nam
+00015f10: 650a 0a20 2020 2072 6574 7572 6e20 445f  e..    return D_
+00015f20: 636f 7079 0a0a 0a64 6566 2063 6f70 795f  copy...def copy_
+00015f30: 7265 6665 7265 6e63 6528 0a20 2020 2072  reference(.    r
+00015f40: 6566 2c0a 2020 2020 7061 7265 6e74 3d4e  ef,.    parent=N
+00015f50: 6f6e 652c 0a20 2020 2063 6f6c 756d 6e73  one,.    columns
+00015f60: 3d4e 6f6e 652c 0a20 2020 2072 6f77 733d  =None,.    rows=
+00015f70: 4e6f 6e65 2c0a 2020 2020 7370 6163 696e  None,.    spacin
+00015f80: 673d 4e6f 6e65 2c0a 2020 2020 6f72 6967  g=None,.    orig
+00015f90: 696e 3d4e 6f6e 652c 0a20 2020 2072 6f74  in=None,.    rot
+00015fa0: 6174 696f 6e3d 4e6f 6e65 2c0a 2020 2020  ation=None,.    
+00015fb0: 6d61 676e 6966 6963 6174 696f 6e3d 4e6f  magnification=No
+00015fc0: 6e65 2c0a 2020 2020 785f 7265 666c 6563  ne,.    x_reflec
+00015fd0: 7469 6f6e 3d4e 6f6e 652c 0a20 2020 206e  tion=None,.    n
+00015fe0: 616d 653d 4e6f 6e65 2c0a 2020 2020 7631  ame=None,.    v1
+00015ff0: 3d4e 6f6e 652c 0a20 2020 2076 323d 4e6f  =None,.    v2=No
+00016000: 6e65 2c0a 2920 2d3e 2043 6f6d 706f 6e65  ne,.) -> Compone
+00016010: 6e74 5265 6665 7265 6e63 653a 0a20 2020  ntReference:.   
+00016020: 2072 6574 7572 6e20 436f 6d70 6f6e 656e   return Componen
+00016030: 7452 6566 6572 656e 6365 280a 2020 2020  tReference(.    
+00016040: 2020 2020 636f 6d70 6f6e 656e 743d 7061      component=pa
+00016050: 7265 6e74 206f 7220 7265 662e 7061 7265  rent or ref.pare
+00016060: 6e74 2c0a 2020 2020 2020 2020 636f 6c75  nt,.        colu
+00016070: 6d6e 733d 636f 6c75 6d6e 7320 6f72 2072  mns=columns or r
+00016080: 6566 2e63 6f6c 756d 6e73 2c0a 2020 2020  ef.columns,.    
+00016090: 2020 2020 726f 7773 3d72 6f77 7320 6f72      rows=rows or
+000160a0: 2072 6566 2e72 6f77 732c 0a20 2020 2020   ref.rows,.     
+000160b0: 2020 2073 7061 6369 6e67 3d73 7061 6369     spacing=spaci
+000160c0: 6e67 206f 7220 7265 662e 7370 6163 696e  ng or ref.spacin
+000160d0: 672c 0a20 2020 2020 2020 206f 7269 6769  g,.        origi
+000160e0: 6e3d 6f72 6967 696e 206f 7220 7265 662e  n=origin or ref.
+000160f0: 6f72 6967 696e 2c0a 2020 2020 2020 2020  origin,.        
+00016100: 726f 7461 7469 6f6e 3d72 6f74 6174 696f  rotation=rotatio
+00016110: 6e20 6f72 2072 6566 2e72 6f74 6174 696f  n or ref.rotatio
+00016120: 6e2c 0a20 2020 2020 2020 206d 6167 6e69  n,.        magni
+00016130: 6669 6361 7469 6f6e 3d6d 6167 6e69 6669  fication=magnifi
+00016140: 6361 7469 6f6e 206f 7220 7265 662e 6d61  cation or ref.ma
+00016150: 676e 6966 6963 6174 696f 6e2c 0a20 2020  gnification,.   
+00016160: 2020 2020 2078 5f72 6566 6c65 6374 696f       x_reflectio
+00016170: 6e3d 785f 7265 666c 6563 7469 6f6e 206f  n=x_reflection o
+00016180: 7220 7265 662e 785f 7265 666c 6563 7469  r ref.x_reflecti
+00016190: 6f6e 2c0a 2020 2020 2020 2020 6e61 6d65  on,.        name
+000161a0: 3d6e 616d 6520 6f72 2072 6566 2e6e 616d  =name or ref.nam
+000161b0: 652c 0a20 2020 2020 2020 2076 313d 7631  e,.        v1=v1
+000161c0: 206f 7220 7265 662e 7631 2c0a 2020 2020   or ref.v1,.    
+000161d0: 2020 2020 7632 3d76 3220 6f72 2072 6566      v2=v2 or ref
+000161e0: 2e76 322c 0a20 2020 2029 0a0a 0a64 6566  .v2,.    )...def
+000161f0: 2074 6573 745f 6765 745f 6c61 7965 7273   test_get_layers
+00016200: 2829 202d 3e20 436f 6d70 6f6e 656e 743a  () -> Component:
+00016210: 0a20 2020 2069 6d70 6f72 7420 6764 7366  .    import gdsf
+00016220: 6163 746f 7279 2061 7320 6766 0a0a 2020  actory as gf..  
+00016230: 2020 6331 203d 2067 662e 636f 6d70 6f6e    c1 = gf.compon
+00016240: 656e 7473 2e73 7472 6169 6768 7428 0a20  ents.straight(. 
+00016250: 2020 2020 2020 206c 656e 6774 683d 3130         length=10
+00016260: 2c0a 2020 2020 2020 2020 7769 6474 683d  ,.        width=
+00016270: 302e 352c 0a20 2020 2020 2020 206c 6179  0.5,.        lay
+00016280: 6572 3d28 322c 2030 292c 0a20 2020 2020  er=(2, 0),.     
+00016290: 2020 2062 626f 785f 6c61 7965 7273 3d5b     bbox_layers=[
+000162a0: 2831 3131 2c20 3029 5d2c 0a20 2020 2020  (111, 0)],.     
+000162b0: 2020 2062 626f 785f 6f66 6673 6574 733d     bbox_offsets=
+000162c0: 5b33 5d2c 0a20 2020 2020 2020 2077 6974  [3],.        wit
+000162d0: 685f 6262 6f78 3d54 7275 652c 0a20 2020  h_bbox=True,.   
+000162e0: 2020 2020 2063 6c61 6464 696e 675f 6c61       cladding_la
+000162f0: 7965 7273 3d4e 6f6e 652c 0a20 2020 2020  yers=None,.     
+00016300: 2020 2061 6464 5f70 696e 733d 4e6f 6e65     add_pins=None
+00016310: 2c0a 2020 2020 2020 2020 6164 645f 6262  ,.        add_bb
+00016320: 6f78 3d4e 6f6e 652c 0a20 2020 2029 0a20  ox=None,.    ). 
+00016330: 2020 2061 7373 6572 7420 6331 2e67 6574     assert c1.get
+00016340: 5f6c 6179 6572 7328 2920 3d3d 207b 2832  _layers() == {(2
+00016350: 2c20 3029 2c20 2831 3131 2c20 3029 7d2c  , 0), (111, 0)},
+00016360: 2063 312e 6765 745f 6c61 7965 7273 2829   c1.get_layers()
+00016370: 0a20 2020 2023 2072 6574 7572 6e20 6331  .    # return c1
+00016380: 0a20 2020 2063 3220 3d20 6331 2e72 656d  .    c2 = c1.rem
+00016390: 6f76 655f 6c61 7965 7273 285b 2831 3131  ove_layers([(111
+000163a0: 2c20 3029 5d29 0a20 2020 2061 7373 6572  , 0)]).    asser
+000163b0: 7420 6332 2e67 6574 5f6c 6179 6572 7328  t c2.get_layers(
+000163c0: 2920 3d3d 207b 2832 2c20 3029 7d2c 2063  ) == {(2, 0)}, c
+000163d0: 322e 6765 745f 6c61 7965 7273 2829 0a20  2.get_layers(). 
+000163e0: 2020 2072 6574 7572 6e20 6332 0a0a 0a64     return c2...d
+000163f0: 6566 205f 6669 6c74 6572 5f70 6f6c 7973  ef _filter_polys
+00016400: 2870 6f6c 7967 6f6e 732c 206c 6179 6572  (polygons, layer
+00016410: 735f 6578 636c 293a 0a20 2020 2072 6574  s_excl):.    ret
+00016420: 7572 6e20 5b0a 2020 2020 2020 2020 706f  urn [.        po
+00016430: 6c79 676f 6e0a 2020 2020 2020 2020 666f  lygon.        fo
+00016440: 7220 706f 6c79 676f 6e2c 206c 6179 6572  r polygon, layer
+00016450: 2c20 6461 7461 7479 7065 2069 6e20 7a69  , datatype in zi
+00016460: 7028 0a20 2020 2020 2020 2020 2020 2070  p(.            p
+00016470: 6f6c 7967 6f6e 732e 706f 6c79 676f 6e73  olygons.polygons
+00016480: 2c20 706f 6c79 676f 6e73 2e6c 6179 6572  , polygons.layer
+00016490: 732c 2070 6f6c 7967 6f6e 732e 6461 7461  s, polygons.data
+000164a0: 7479 7065 730a 2020 2020 2020 2020 290a  types.        ).
+000164b0: 2020 2020 2020 2020 6966 2028 6c61 7965          if (laye
+000164c0: 722c 2064 6174 6174 7970 6529 206e 6f74  r, datatype) not
+000164d0: 2069 6e20 6c61 7965 7273 5f65 7863 6c0a   in layers_excl.
+000164e0: 2020 2020 5d0a 0a0a 6465 6620 7265 6375      ]...def recu
+000164f0: 7273 655f 7374 7275 6374 7572 6573 280a  rse_structures(.
+00016500: 2020 2020 636f 6d70 6f6e 656e 743a 2043      component: C
+00016510: 6f6d 706f 6e65 6e74 2c0a 2020 2020 6967  omponent,.    ig
+00016520: 6e6f 7265 5f63 6f6d 706f 6e65 6e74 735f  nore_components_
+00016530: 7072 6566 6978 3a20 4f70 7469 6f6e 616c  prefix: Optional
+00016540: 5b4c 6973 745b 7374 725d 5d20 3d20 4e6f  [List[str]] = No
+00016550: 6e65 2c0a 2020 2020 6967 6e6f 7265 5f66  ne,.    ignore_f
+00016560: 756e 6374 696f 6e73 5f70 7265 6669 783a  unctions_prefix:
+00016570: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
+00016580: 7472 5d5d 203d 204e 6f6e 652c 0a29 202d  tr]] = None,.) -
+00016590: 3e20 4469 6374 5b73 7472 2c20 416e 795d  > Dict[str, Any]
+000165a0: 3a0a 2020 2020 2222 2252 6563 7572 7365  :.    """Recurse
+000165b0: 2063 6f6d 706f 6e65 6e74 2061 6e64 2063   component and c
+000165c0: 6f6d 706f 6e65 6e74 7320 7265 6665 7265  omponents refere
+000165d0: 6e63 6573 2072 6563 7572 7369 7665 6c79  nces recursively
+000165e0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+000165f0: 2020 2020 2063 6f6d 706f 6e65 6e74 3a20       component: 
+00016600: 636f 6d70 6f6e 656e 7420 746f 2072 6563  component to rec
+00016610: 7572 7365 2e0a 2020 2020 2020 2020 6967  urse..        ig
+00016620: 6e6f 7265 5f63 6f6d 706f 6e65 6e74 735f  nore_components_
+00016630: 7072 6566 6978 3a20 6c69 7374 206f 6620  prefix: list of 
+00016640: 7072 6566 6978 2074 6f20 6967 6e6f 7265  prefix to ignore
+00016650: 2e0a 2020 2020 2020 2020 6967 6e6f 7265  ..        ignore
+00016660: 5f66 756e 6374 696f 6e73 5f70 7265 6669  _functions_prefi
+00016670: 783a 206c 6973 7420 6f66 2070 7265 6669  x: list of prefi
+00016680: 7820 746f 2069 676e 6f72 652e 0a20 2020  x to ignore..   
+00016690: 2022 2222 0a20 2020 2069 676e 6f72 655f   """.    ignore_
+000166a0: 6675 6e63 7469 6f6e 735f 7072 6566 6978  functions_prefix
+000166b0: 203d 2069 676e 6f72 655f 6675 6e63 7469   = ignore_functi
+000166c0: 6f6e 735f 7072 6566 6978 206f 7220 5b5d  ons_prefix or []
+000166d0: 0a20 2020 2069 676e 6f72 655f 636f 6d70  .    ignore_comp
+000166e0: 6f6e 656e 7473 5f70 7265 6669 7820 3d20  onents_prefix = 
+000166f0: 6967 6e6f 7265 5f63 6f6d 706f 6e65 6e74  ignore_component
+00016700: 735f 7072 6566 6978 206f 7220 5b5d 0a0a  s_prefix or []..
+00016710: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+00016720: 2068 6173 6174 7472 2863 6f6d 706f 6e65   hasattr(compone
+00016730: 6e74 2c20 2266 756e 6374 696f 6e5f 6e61  nt, "function_na
+00016740: 6d65 2229 0a20 2020 2020 2020 2061 6e64  me").        and
+00016750: 2063 6f6d 706f 6e65 6e74 2e66 756e 6374   component.funct
+00016760: 696f 6e5f 6e61 6d65 2069 6e20 6967 6e6f  ion_name in igno
+00016770: 7265 5f66 756e 6374 696f 6e73 5f70 7265  re_functions_pre
+00016780: 6669 780a 2020 2020 293a 0a20 2020 2020  fix.    ):.     
+00016790: 2020 2072 6574 7572 6e20 7b7d 0a0a 2020     return {}..  
+000167a0: 2020 6966 2068 6173 6174 7472 2863 6f6d    if hasattr(com
+000167b0: 706f 6e65 6e74 2c20 226e 616d 6522 2920  ponent, "name") 
+000167c0: 616e 6420 616e 7928 0a20 2020 2020 2020  and any(.       
+000167d0: 2063 6f6d 706f 6e65 6e74 2e6e 616d 652e   component.name.
+000167e0: 7374 6172 7473 7769 7468 2869 2920 666f  startswith(i) fo
+000167f0: 7220 6920 696e 2069 676e 6f72 655f 636f  r i in ignore_co
+00016800: 6d70 6f6e 656e 7473 5f70 7265 6669 780a  mponents_prefix.
+00016810: 2020 2020 293a 0a20 2020 2020 2020 2072      ):.        r
+00016820: 6574 7572 6e20 7b7d 0a0a 2020 2020 6f75  eturn {}..    ou
+00016830: 7470 7574 203d 207b 636f 6d70 6f6e 656e  tput = {componen
+00016840: 742e 6e61 6d65 3a20 6469 6374 2863 6f6d  t.name: dict(com
+00016850: 706f 6e65 6e74 2e73 6574 7469 6e67 7329  ponent.settings)
+00016860: 7d0a 2020 2020 666f 7220 7265 6665 7265  }.    for refere
+00016870: 6e63 6520 696e 2063 6f6d 706f 6e65 6e74  nce in component
+00016880: 2e72 6566 6572 656e 6365 733a 0a20 2020  .references:.   
+00016890: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+000168a0: 2020 2020 2020 6973 696e 7374 616e 6365        isinstance
+000168b0: 2872 6566 6572 656e 6365 2c20 436f 6d70  (reference, Comp
+000168c0: 6f6e 656e 7452 6566 6572 656e 6365 290a  onentReference).
+000168d0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+000168e0: 7265 6665 7265 6e63 652e 7265 665f 6365  reference.ref_ce
+000168f0: 6c6c 2e6e 616d 6520 6e6f 7420 696e 206f  ll.name not in o
+00016900: 7574 7075 740a 2020 2020 2020 2020 293a  utput.        ):
+00016910: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+00016920: 7075 742e 7570 6461 7465 2872 6563 7572  put.update(recur
+00016930: 7365 5f73 7472 7563 7475 7265 7328 7265  se_structures(re
+00016940: 6665 7265 6e63 652e 7265 665f 6365 6c6c  ference.ref_cell
+00016950: 2929 0a0a 2020 2020 7265 7475 726e 206f  ))..    return o
+00016960: 7574 7075 740a 0a0a 6465 6620 666c 6174  utput...def flat
+00016970: 7465 6e5f 696e 7661 6c69 645f 7265 6673  ten_invalid_refs
+00016980: 5f72 6563 7572 7369 7665 280a 2020 2020  _recursive(.    
+00016990: 636f 6d70 6f6e 656e 743a 2043 6f6d 706f  component: Compo
+000169a0: 6e65 6e74 2c0a 2020 2020 6772 6964 5f73  nent,.    grid_s
+000169b0: 697a 653a 204f 7074 696f 6e61 6c5b 666c  ize: Optional[fl
+000169c0: 6f61 745d 203d 204e 6f6e 652c 0a20 2020  oat] = None,.   
+000169d0: 2075 7064 6174 6564 5f63 6f6d 706f 6e65   updated_compone
+000169e0: 6e74 733d 4e6f 6e65 2c0a 2020 2020 7472  nts=None,.    tr
+000169f0: 6176 6572 7365 645f 636f 6d70 6f6e 656e  aversed_componen
+00016a00: 7473 3d4e 6f6e 652c 0a29 3a0a 2020 2020  ts=None,.):.    
+00016a10: 2222 2252 6563 7572 7369 7665 6c79 2066  """Recursively f
+00016a20: 6c61 7474 656e 7320 636f 6d70 6f6e 656e  lattens componen
+00016a30: 7420 7265 6665 7265 6e63 6573 2077 6869  t references whi
+00016a40: 6368 2068 6176 6520 696e 7661 6c69 6420  ch have invalid 
+00016a50: 7472 616e 7366 6f72 6d61 7469 6f6e 7320  transformations 
+00016a60: 2869 2e65 2e20 6e6f 6e2d 3930 2064 6567  (i.e. non-90 deg
+00016a70: 2072 6f74 6174 696f 6e73 206f 7220 7375   rotations or su
+00016a80: 622d 6772 6964 2074 7261 6e73 6c61 7469  b-grid translati
+00016a90: 6f6e 7329 2061 6e64 2072 6574 7572 6e73  ons) and returns
+00016aa0: 2061 2063 6f70 7920 6966 2061 6e79 2073   a copy if any s
+00016ab0: 7562 6365 6c6c 7320 6861 7665 2062 6565  ubcells have bee
+00016ac0: 6e20 6d6f 6469 6669 6564 2e0a 0a20 2020  n modified...   
+00016ad0: 2057 4152 4e49 4e47 3a20 7468 6973 2066   WARNING: this f
+00016ae0: 756e 6374 696f 6e20 7769 6c6c 2070 726f  unction will pro
+00016af0: 6475 6365 2073 616d 652d 6e61 6d65 2063  duce same-name c
+00016b00: 6f70 6965 7320 6f66 2063 656c 6c73 2e20  opies of cells. 
+00016b10: 4974 2069 7320 7374 7269 6374 6c79 206d  It is strictly m
+00016b20: 6561 6e74 2074 6f20 6265 2075 7365 6420  eant to be used 
+00016b30: 6f6e 2077 7269 7465 206f 6620 7468 6520  on write of the 
+00016b40: 4744 5320 6669 6c65 2061 6e64 0a20 2020  GDS file and.   
+00016b50: 2073 686f 756c 6420 6e6f 7420 6265 206d   should not be m
+00016b60: 6978 6564 2077 6974 6820 6f74 6865 7220  ixed with other 
+00016b70: 6365 6c6c 732c 206f 7220 796f 7520 7769  cells, or you wi
+00016b80: 6c6c 206c 696b 656c 7920 6578 7065 7269  ll likely experi
+00016b90: 656e 6365 2069 7373 7565 7320 7769 7468  ence issues with
+00016ba0: 2064 7570 6c69 6361 7465 2063 656c 6c73   duplicate cells
+00016bb0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00016bc0: 2020 2020 636f 6d70 6f6e 656e 743a 2074      component: t
+00016bd0: 6865 2063 6f6d 706f 6e65 6e74 2074 6f20  he component to 
+00016be0: 6669 7820 2869 6e20 706c 6163 6529 2e0a  fix (in place)..
+00016bf0: 2020 2020 2020 2020 6772 6964 5f73 697a          grid_siz
+00016c00: 653a 2074 6865 2047 4453 2067 7269 6420  e: the GDS grid 
+00016c10: 7369 7a65 2c20 696e 2075 6d2c 2064 6566  size, in um, def
+00016c20: 6175 6c74 7320 746f 2061 6374 6976 6520  aults to active 
+00016c30: 5044 4b2e 6765 745f 6772 6964 5f73 697a  PDK.get_grid_siz
+00016c40: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00016c50: 616e 7920 7472 616e 736c 6174 696f 6e73  any translations
+00016c60: 2077 6974 6820 6869 6768 6572 2072 6573   with higher res
+00016c70: 6f6c 7574 696f 6e20 7468 616e 2074 6869  olution than thi
+00016c80: 7320 6172 6520 636f 6e73 6964 6572 6564  s are considered
+00016c90: 2069 6e76 616c 6964 2e0a 2020 2020 2020   invalid..      
+00016ca0: 2020 7570 6461 7465 645f 636f 6d70 6f6e    updated_compon
+00016cb0: 656e 7473 3a20 7468 6520 7275 6e6e 696e  ents: the runnin
+00016cc0: 6720 6469 6374 696f 6e61 7279 206f 6620  g dictionary of 
+00016cd0: 636f 6d70 6f6e 656e 7473 2077 6869 6368  components which
+00016ce0: 2068 6176 6520 6265 656e 206d 6f64 6966   have been modif
+00016cf0: 6965 6420 6279 2074 6869 7320 7472 616e  ied by this tran
+00016d00: 7366 6f72 6d61 7469 6f6e 2e20 5368 6f75  sformation. Shou
+00016d10: 6c64 2061 6c77 6179 7320 6265 204e 6f6e  ld always be Non
+00016d20: 652c 2065 7863 6570 7420 666f 7220 7265  e, except for re
+00016d30: 6375 7273 6976 6520 696e 766f 6361 7469  cursive invocati
+00016d40: 6f6e 732e 0a20 2020 2020 2020 2074 7261  ons..        tra
+00016d50: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
+00016d60: 733a 2074 6865 2073 6574 206f 6620 636f  s: the set of co
+00016d70: 6d70 6f6e 656e 7420 6e61 6d65 7320 7768  mponent names wh
+00016d80: 6963 6820 6861 7665 2062 6565 6e20 7472  ich have been tr
+00016d90: 6176 6572 7365 642e 2053 686f 756c 6420  aversed. Should 
+00016da0: 616c 7761 7973 2062 6520 4e6f 6e65 2c20  always be None, 
+00016db0: 6578 6365 7074 2066 6f72 2072 6563 7572  except for recur
+00016dc0: 7369 7665 2069 6e76 6f63 6174 696f 6e73  sive invocations
+00016dd0: 2e0a 2020 2020 2222 220a 2020 2020 6672  ..    """.    fr
+00016de0: 6f6d 2067 6473 6661 6374 6f72 792e 6465  om gdsfactory.de
+00016df0: 636f 7261 746f 7273 2069 6d70 6f72 7420  corators import 
+00016e00: 6973 5f69 6e76 616c 6964 5f72 6566 0a0a  is_invalid_ref..
+00016e10: 2020 2020 696e 7661 6c69 645f 7265 6673      invalid_refs
+00016e20: 203d 205b 5d0a 2020 2020 7265 6673 203d   = [].    refs =
+00016e30: 2063 6f6d 706f 6e65 6e74 2e72 6566 6572   component.refer
+00016e40: 656e 6365 730a 2020 2020 7375 6263 656c  ences.    subcel
+00016e50: 6c5f 6d6f 6469 6669 6564 203d 2046 616c  l_modified = Fal
+00016e60: 7365 0a20 2020 2069 6620 7570 6461 7465  se.    if update
+00016e70: 645f 636f 6d70 6f6e 656e 7473 2069 7320  d_components is 
+00016e80: 4e6f 6e65 3a0a 2020 2020 2020 2020 7570  None:.        up
+00016e90: 6461 7465 645f 636f 6d70 6f6e 656e 7473  dated_components
+00016ea0: 203d 207b 7d0a 2020 2020 6966 2074 7261   = {}.    if tra
+00016eb0: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
+00016ec0: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
+00016ed0: 2020 2074 7261 7665 7273 6564 5f63 6f6d     traversed_com
+00016ee0: 706f 6e65 6e74 7320 3d20 7365 7428 290a  ponents = set().
+00016ef0: 2020 2020 666f 7220 7265 6620 696e 2072      for ref in r
+00016f00: 6566 733a 0a20 2020 2020 2020 2023 206d  efs:.        # m
+00016f10: 6172 6b20 616e 7920 696e 7661 6c69 6420  ark any invalid 
+00016f20: 7265 6673 2066 6f72 2066 6c61 7474 656e  refs for flatten
+00016f30: 696e 670a 2020 2020 2020 2020 2320 6f74  ing.        # ot
+00016f40: 6865 7277 6973 652c 2063 6865 636b 2069  herwise, check i
+00016f50: 6620 7468 6572 6520 6172 6520 616e 7920  f there are any 
+00016f60: 6d6f 6469 6669 6564 2063 656c 6c73 2062  modified cells b
+00016f70: 656e 6561 7468 2028 7765 206e 6565 6420  eneath (we need 
+00016f80: 6e6f 7420 646f 2074 6869 7320 6966 2074  not do this if t
+00016f90: 6865 2072 6566 2077 696c 6c20 6265 2066  he ref will be f
+00016fa0: 6c61 7474 656e 6564 2061 6e79 7761 7973  lattened anyways
+00016fb0: 290a 2020 2020 2020 2020 6966 2069 735f  ).        if is_
+00016fc0: 696e 7661 6c69 645f 7265 6628 7265 662c  invalid_ref(ref,
+00016fd0: 2067 7269 645f 7369 7a65 293a 0a20 2020   grid_size):.   
+00016fe0: 2020 2020 2020 2020 2069 6e76 616c 6964           invalid
+00016ff0: 5f72 6566 732e 6170 7065 6e64 2872 6566  _refs.append(ref
+00017000: 2e6e 616d 6529 0a20 2020 2020 2020 2065  .name).        e
+00017010: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00017020: 2023 206f 7468 6572 7769 7365 2c20 7265   # otherwise, re
+00017030: 6375 7273 6976 656c 7920 666c 6174 7465  cursively flatte
+00017040: 6e20 7265 6673 2069 6620 7468 6520 7375  n refs if the su
+00017050: 6263 656c 6c20 6861 7320 6e6f 7420 616c  bcell has not al
+00017060: 7265 6164 7920 6265 656e 2074 7261 7665  ready been trave
+00017070: 7273 6564 0a20 2020 2020 2020 2020 2020  rsed.           
+00017080: 2069 6620 7265 662e 7061 7265 6e74 2e6e   if ref.parent.n
+00017090: 616d 6520 6e6f 7420 696e 2074 7261 7665  ame not in trave
+000170a0: 7273 6564 5f63 6f6d 706f 6e65 6e74 733a  rsed_components:
+000170b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000170c0: 2066 6c61 7474 656e 5f69 6e76 616c 6964   flatten_invalid
+000170d0: 5f72 6566 735f 7265 6375 7273 6976 6528  _refs_recursive(
+000170e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000170f0: 2020 2020 2072 6566 2e70 6172 656e 742c       ref.parent,
+00017100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017110: 2020 2020 2067 7269 645f 7369 7a65 3d67       grid_size=g
+00017120: 7269 645f 7369 7a65 2c0a 2020 2020 2020  rid_size,.      
+00017130: 2020 2020 2020 2020 2020 2020 2020 7570                up
+00017140: 6461 7465 645f 636f 6d70 6f6e 656e 7473  dated_components
+00017150: 3d75 7064 6174 6564 5f63 6f6d 706f 6e65  =updated_compone
+00017160: 6e74 732c 0a20 2020 2020 2020 2020 2020  nts,.           
+00017170: 2020 2020 2020 2020 2074 7261 7665 7273           travers
+00017180: 6564 5f63 6f6d 706f 6e65 6e74 733d 7472  ed_components=tr
+00017190: 6176 6572 7365 645f 636f 6d70 6f6e 656e  aversed_componen
+000171a0: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
+000171b0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+000171c0: 2020 2320 6e6f 772c 2069 6620 7468 6520    # now, if the 
+000171d0: 7265 6627 7320 6365 6c6c 2062 6565 6e20  ref's cell been 
+000171e0: 6d6f 6469 6669 6564 2c20 6d61 726b 2069  modified, mark i
+000171f0: 7420 6173 2073 7563 680a 2020 2020 2020  t as such.      
+00017200: 2020 2020 2020 6966 2072 6566 2e70 6172        if ref.par
+00017210: 656e 742e 6e61 6d65 2069 6e20 7570 6461  ent.name in upda
+00017220: 7465 645f 636f 6d70 6f6e 656e 7473 3a0a  ted_components:.
+00017230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017240: 7375 6263 656c 6c5f 6d6f 6469 6669 6564  subcell_modified
+00017250: 203d 2054 7275 650a 2020 2020 6966 2069   = True.    if i
+00017260: 6e76 616c 6964 5f72 6566 7320 6f72 2073  nvalid_refs or s
+00017270: 7562 6365 6c6c 5f6d 6f64 6966 6965 643a  ubcell_modified:
+00017280: 0a20 2020 2020 2020 206e 6577 5f63 6f6d  .        new_com
+00017290: 706f 6e65 6e74 203d 2063 6f6d 706f 6e65  ponent = compone
+000172a0: 6e74 2e63 6f70 7928 290a 2020 2020 2020  nt.copy().      
+000172b0: 2020 6e65 775f 636f 6d70 6f6e 656e 742e    new_component.
+000172c0: 6e61 6d65 203d 2063 6f6d 706f 6e65 6e74  name = component
+000172d0: 2e6e 616d 650a 2020 2020 2020 2020 2320  .name.        # 
+000172e0: 6d61 6b65 2073 7572 6520 616c 6c20 6d6f  make sure all mo
+000172f0: 6469 6669 6564 2063 656c 6c73 2068 6176  dified cells hav
+00017300: 6520 7468 6569 7220 7265 6665 7265 6e63  e their referenc
+00017310: 6573 2075 7064 6174 6564 0a20 2020 2020  es updated.     
+00017320: 2020 206e 6577 5f72 6566 7320 3d20 6e65     new_refs = ne
+00017330: 775f 636f 6d70 6f6e 656e 742e 7265 6665  w_component.refe
+00017340: 7265 6e63 6573 2e63 6f70 7928 290a 2020  rences.copy().  
+00017350: 2020 2020 2020 666f 7220 7265 6620 696e        for ref in
+00017360: 206e 6577 5f72 6566 733a 0a20 2020 2020   new_refs:.     
+00017370: 2020 2020 2020 2069 6620 7265 662e 6e61         if ref.na
+00017380: 6d65 2069 6e20 696e 7661 6c69 645f 7265  me in invalid_re
+00017390: 6673 3a0a 2020 2020 2020 2020 2020 2020  fs:.            
+000173a0: 2020 2020 6e65 775f 636f 6d70 6f6e 656e      new_componen
+000173b0: 742e 666c 6174 7465 6e5f 7265 6665 7265  t.flatten_refere
+000173c0: 6e63 6528 7265 6629 0a20 2020 2020 2020  nce(ref).       
+000173d0: 2020 2020 2065 6c69 6620 280a 2020 2020       elif (.    
+000173e0: 2020 2020 2020 2020 2020 2020 7265 662e              ref.
+000173f0: 7061 7265 6e74 2e6e 616d 6520 696e 2075  parent.name in u
+00017400: 7064 6174 6564 5f63 6f6d 706f 6e65 6e74  pdated_component
+00017410: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00017420: 2020 616e 6420 7265 662e 7061 7265 6e74    and ref.parent
+00017430: 2069 7320 6e6f 7420 7570 6461 7465 645f   is not updated_
+00017440: 636f 6d70 6f6e 656e 7473 5b72 6566 2e70  components[ref.p
+00017450: 6172 656e 742e 6e61 6d65 5d0a 2020 2020  arent.name].    
+00017460: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+00017470: 2020 2020 2020 2020 2020 2072 6566 2e70             ref.p
+00017480: 6172 656e 7420 3d20 7570 6461 7465 645f  arent = updated_
+00017490: 636f 6d70 6f6e 656e 7473 5b72 6566 2e70  components[ref.p
+000174a0: 6172 656e 742e 6e61 6d65 5d0a 2020 2020  arent.name].    
+000174b0: 2020 2020 636f 6d70 6f6e 656e 7420 3d20      component = 
+000174c0: 6e65 775f 636f 6d70 6f6e 656e 740a 2020  new_component.  
+000174d0: 2020 2020 2020 7570 6461 7465 645f 636f        updated_co
+000174e0: 6d70 6f6e 656e 7473 5b63 6f6d 706f 6e65  mponents[compone
+000174f0: 6e74 2e6e 616d 655d 203d 206e 6577 5f63  nt.name] = new_c
+00017500: 6f6d 706f 6e65 6e74 0a20 2020 2074 7261  omponent.    tra
+00017510: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
+00017520: 732e 6164 6428 636f 6d70 6f6e 656e 742e  s.add(component.
+00017530: 6e61 6d65 290a 2020 2020 7265 7475 726e  name).    return
+00017540: 2063 6f6d 706f 6e65 6e74 0a0a 0a64 6566   component...def
+00017550: 205f 6368 6563 6b5f 756e 6361 6368 6564   _check_uncached
+00017560: 5f63 6f6d 706f 6e65 6e74 7328 636f 6d70  _components(comp
+00017570: 6f6e 656e 742c 206d 6f64 6529 3a0a 2020  onent, mode):.  
+00017580: 2020 7661 6c69 645f 6d6f 6465 7320 3d20    valid_modes = 
+00017590: 5b22 7761 726e 222c 2022 6572 726f 7222  ["warn", "error"
+000175a0: 2c20 2269 676e 6f72 6522 5d0a 0a20 2020  , "ignore"]..   
+000175b0: 2069 6620 6d6f 6465 203d 3d20 2269 676e   if mode == "ign
+000175c0: 6f72 6522 3a0a 2020 2020 2020 2020 7265  ore":.        re
+000175d0: 7475 726e 0a20 2020 2065 6c69 6620 6d6f  turn.    elif mo
+000175e0: 6465 206e 6f74 2069 6e20 7661 6c69 645f  de not in valid_
+000175f0: 6d6f 6465 733a 0a20 2020 2020 2020 2072  modes:.        r
+00017600: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00017610: 0a20 2020 2020 2020 2020 2020 2066 227b  .            f"{
+00017620: 6d6f 6465 7d20 6973 206e 6f74 2061 2076  mode} is not a v
+00017630: 616c 6964 2076 616c 7565 2066 6f72 206f  alid value for o
+00017640: 6e5f 756e 6361 6368 6564 5f63 6f6d 706f  n_uncached_compo
+00017650: 6e65 6e74 2e20 5472 7920 6f6e 6520 6f66  nent. Try one of
+00017660: 2074 6865 7365 3a20 7b76 616c 6964 5f6d   these: {valid_m
+00017670: 6f64 6573 7d2e 220a 2020 2020 2020 2020  odes}.".        
+00017680: 290a 0a20 2020 2066 6f72 2073 7562 5f63  )..    for sub_c
+00017690: 6f6d 706f 6e65 6e74 2069 6e20 636f 6d70  omponent in comp
+000176a0: 6f6e 656e 742e 6765 745f 6465 7065 6e64  onent.get_depend
+000176b0: 656e 6369 6573 2872 6563 7572 7369 7665  encies(recursive
+000176c0: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
+000176d0: 6966 206e 6f74 2073 7562 5f63 6f6d 706f  if not sub_compo
+000176e0: 6e65 6e74 2e5f 6c6f 636b 6564 3a0a 2020  nent._locked:.  
+000176f0: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+00017700: 6520 3d20 280a 2020 2020 2020 2020 2020  e = (.          
+00017710: 2020 2020 2020 6622 436f 6d70 6f6e 656e        f"Componen
+00017720: 7420 7b73 7562 5f63 6f6d 706f 6e65 6e74  t {sub_component
+00017730: 2e6e 616d 6521 727d 2077 6173 204e 4f54  .name!r} was NOT
+00017740: 2070 726f 7065 726c 7920 6c6f 636b 6564   properly locked
+00017750: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
+00017760: 2020 2020 2259 6f75 206e 6565 6420 746f      "You need to
+00017770: 2077 7269 7465 2069 7420 696e 746f 2061   write it into a
+00017780: 2066 756e 6374 696f 6e20 7468 6174 2068   function that h
+00017790: 6173 2074 6865 2040 6365 6c6c 2064 6563  as the @cell dec
+000177a0: 6f72 6174 6f72 2e22 0a20 2020 2020 2020  orator.".       
+000177b0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000177c0: 2020 2069 6620 6d6f 6465 203d 3d20 2277     if mode == "w
+000177d0: 6172 6e22 3a0a 2020 2020 2020 2020 2020  arn":.          
+000177e0: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
+000177f0: 6172 6e28 6d65 7373 6167 652c 2055 6e63  arn(message, Unc
+00017800: 6163 6865 6443 6f6d 706f 6e65 6e74 5761  achedComponentWa
+00017810: 726e 696e 672c 2073 7461 636b 6c65 7665  rning, stackleve
+00017820: 6c3d 3329 0a0a 2020 2020 2020 2020 2020  l=3)..          
+00017830: 2020 656c 6966 206d 6f64 6520 3d3d 2022    elif mode == "
+00017840: 6572 726f 7222 3a0a 2020 2020 2020 2020  error":.        
+00017850: 2020 2020 2020 2020 7261 6973 6520 556e          raise Un
+00017860: 6361 6368 6564 436f 6d70 6f6e 656e 7445  cachedComponentE
+00017870: 7272 6f72 286d 6573 7361 6765 290a 0a0a  rror(message)...
+00017880: 6465 6620 7465 7374 5f73 616d 655f 7569  def test_same_ui
+00017890: 6428 2920 2d3e 204e 6f6e 653a 0a20 2020  d() -> None:.   
+000178a0: 2069 6d70 6f72 7420 6764 7366 6163 746f   import gdsfacto
+000178b0: 7279 2061 7320 6766 0a0a 2020 2020 6320  ry as gf..    c 
+000178c0: 3d20 436f 6d70 6f6e 656e 7428 290a 2020  = Component().  
+000178d0: 2020 6320 3c3c 2067 662e 636f 6d70 6f6e    c << gf.compon
+000178e0: 656e 7473 2e72 6563 7461 6e67 6c65 2829  ents.rectangle()
+000178f0: 0a20 2020 2063 203c 3c20 6766 2e63 6f6d  .    c << gf.com
+00017900: 706f 6e65 6e74 732e 7265 6374 616e 676c  ponents.rectangl
+00017910: 6528 290a 0a20 2020 2072 3120 3d20 632e  e()..    r1 = c.
+00017920: 7265 6665 7265 6e63 6573 5b30 5d2e 7061  references[0].pa
+00017930: 7265 6e74 0a20 2020 2072 3220 3d20 632e  rent.    r2 = c.
+00017940: 7265 6665 7265 6e63 6573 5b31 5d2e 7061  references[1].pa
+00017950: 7265 6e74 0a0a 2020 2020 6173 7365 7274  rent..    assert
+00017960: 2072 312e 7569 6420 3d3d 2072 322e 7569   r1.uid == r2.ui
+00017970: 642c 2066 227b 7231 2e75 6964 7d20 6d75  d, f"{r1.uid} mu
+00017980: 7374 2065 7175 616c 207b 7232 2e75 6964  st equal {r2.uid
+00017990: 7d22 0a0a 0a64 6566 2074 6573 745f 6e65  }"...def test_ne
+000179a0: 746c 6973 745f 7369 6d70 6c65 2829 202d  tlist_simple() -
+000179b0: 3e20 4e6f 6e65 3a0a 2020 2020 696d 706f  > None:.    impo
+000179c0: 7274 2067 6473 6661 6374 6f72 7920 6173  rt gdsfactory as
+000179d0: 2067 660a 0a20 2020 2063 203d 2067 662e   gf..    c = gf.
+000179e0: 436f 6d70 6f6e 656e 7428 290a 2020 2020  Component().    
+000179f0: 6331 203d 2063 203c 3c20 6766 2e63 6f6d  c1 = c << gf.com
+00017a00: 706f 6e65 6e74 732e 7374 7261 6967 6874  ponents.straight
+00017a10: 286c 656e 6774 683d 312c 2077 6964 7468  (length=1, width
+00017a20: 3d32 290a 2020 2020 6332 203d 2063 203c  =2).    c2 = c <
+00017a30: 3c20 6766 2e63 6f6d 706f 6e65 6e74 732e  < gf.components.
+00017a40: 7374 7261 6967 6874 286c 656e 6774 683d  straight(length=
+00017a50: 322c 2077 6964 7468 3d32 290a 2020 2020  2, width=2).    
+00017a60: 6332 2e63 6f6e 6e65 6374 2870 6f72 743d  c2.connect(port=
+00017a70: 226f 3122 2c20 6465 7374 696e 6174 696f  "o1", destinatio
+00017a80: 6e3d 6331 2e70 6f72 7473 5b22 6f32 225d  n=c1.ports["o2"]
+00017a90: 290a 2020 2020 632e 6164 645f 706f 7274  ).    c.add_port
+00017aa0: 2822 6f31 222c 2070 6f72 743d 6331 2e70  ("o1", port=c1.p
+00017ab0: 6f72 7473 5b22 6f31 225d 290a 2020 2020  orts["o1"]).    
+00017ac0: 632e 6164 645f 706f 7274 2822 6f32 222c  c.add_port("o2",
+00017ad0: 2070 6f72 743d 6332 2e70 6f72 7473 5b22   port=c2.ports["
+00017ae0: 6f32 225d 290a 2020 2020 6e65 746c 6973  o2"]).    netlis
+00017af0: 7420 3d20 632e 6765 745f 6e65 746c 6973  t = c.get_netlis
+00017b00: 7428 290a 2020 2020 2320 7072 696e 7428  t().    # print(
+00017b10: 6e65 746c 6973 742e 7072 6574 7479 2829  netlist.pretty()
+00017b20: 290a 2020 2020 6173 7365 7274 206c 656e  ).    assert len
+00017b30: 286e 6574 6c69 7374 5b22 696e 7374 616e  (netlist["instan
+00017b40: 6365 7322 5d29 203d 3d20 320a 0a0a 6465  ces"]) == 2...de
+00017b50: 6620 7465 7374 5f6e 6574 6c69 7374 5f73  f test_netlist_s
+00017b60: 696d 706c 655f 7769 6474 685f 6d69 736d  imple_width_mism
+00017b70: 6174 6368 5f74 6872 6f77 735f 6572 726f  atch_throws_erro
+00017b80: 7228 2920 2d3e 204e 6f6e 653a 0a20 2020  r() -> None:.   
+00017b90: 2069 6d70 6f72 7420 7079 7465 7374 0a0a   import pytest..
+00017ba0: 2020 2020 696d 706f 7274 2067 6473 6661      import gdsfa
+00017bb0: 6374 6f72 7920 6173 2067 660a 0a20 2020  ctory as gf..   
+00017bc0: 2063 203d 2067 662e 436f 6d70 6f6e 656e   c = gf.Componen
+00017bd0: 7428 290a 2020 2020 6331 203d 2063 203c  t().    c1 = c <
+00017be0: 3c20 6766 2e63 6f6d 706f 6e65 6e74 732e  < gf.components.
+00017bf0: 7374 7261 6967 6874 286c 656e 6774 683d  straight(length=
+00017c00: 312c 2077 6964 7468 3d31 290a 2020 2020  1, width=1).    
+00017c10: 6332 203d 2063 203c 3c20 6766 2e63 6f6d  c2 = c << gf.com
+00017c20: 706f 6e65 6e74 732e 7374 7261 6967 6874  ponents.straight
+00017c30: 286c 656e 6774 683d 322c 2077 6964 7468  (length=2, width
+00017c40: 3d32 290a 2020 2020 6332 2e63 6f6e 6e65  =2).    c2.conne
+00017c50: 6374 2870 6f72 743d 226f 3122 2c20 6465  ct(port="o1", de
+00017c60: 7374 696e 6174 696f 6e3d 6331 2e70 6f72  stination=c1.por
+00017c70: 7473 5b22 6f32 225d 290a 2020 2020 632e  ts["o2"]).    c.
+00017c80: 6164 645f 706f 7274 2822 6f31 222c 2070  add_port("o1", p
+00017c90: 6f72 743d 6331 2e70 6f72 7473 5b22 6f31  ort=c1.ports["o1
+00017ca0: 225d 290a 2020 2020 632e 6164 645f 706f  "]).    c.add_po
+00017cb0: 7274 2822 6f32 222c 2070 6f72 743d 6332  rt("o2", port=c2
+00017cc0: 2e70 6f72 7473 5b22 6f32 225d 290a 2020  .ports["o2"]).  
+00017cd0: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
+00017ce0: 6973 6573 2856 616c 7565 4572 726f 7229  ises(ValueError)
+00017cf0: 3a0a 2020 2020 2020 2020 632e 6765 745f  :.        c.get_
+00017d00: 6e65 746c 6973 7428 290a 0a0a 6465 6620  netlist()...def 
+00017d10: 7465 7374 5f6e 6574 6c69 7374 5f63 6f6d  test_netlist_com
+00017d20: 706c 6578 2829 202d 3e20 4e6f 6e65 3a0a  plex() -> None:.
+00017d30: 2020 2020 696d 706f 7274 2067 6473 6661      import gdsfa
+00017d40: 6374 6f72 7920 6173 2067 660a 0a20 2020  ctory as gf..   
+00017d50: 2063 203d 2067 662e 636f 6d70 6f6e 656e   c = gf.componen
+00017d60: 7473 2e6d 7a69 5f61 726d 7328 290a 2020  ts.mzi_arms().  
+00017d70: 2020 6e65 746c 6973 7420 3d20 632e 6765    netlist = c.ge
+00017d80: 745f 6e65 746c 6973 7428 290a 2020 2020  t_netlist().    
+00017d90: 2320 7072 696e 7428 6e65 746c 6973 742e  # print(netlist.
+00017da0: 7072 6574 7479 2829 290a 2020 2020 6173  pretty()).    as
+00017db0: 7365 7274 206c 656e 286e 6574 6c69 7374  sert len(netlist
+00017dc0: 5b22 696e 7374 616e 6365 7322 5d29 203d  ["instances"]) =
+00017dd0: 3d20 342c 206c 656e 286e 6574 6c69 7374  = 4, len(netlist
+00017de0: 5b22 696e 7374 616e 6365 7322 5d29 0a0a  ["instances"])..
+00017df0: 0a64 6566 2074 6573 745f 6578 7472 6163  .def test_extrac
+00017e00: 7428 2920 2d3e 2043 6f6d 706f 6e65 6e74  t() -> Component
+00017e10: 3a0a 2020 2020 696d 706f 7274 2067 6473  :.    import gds
+00017e20: 6661 6374 6f72 7920 6173 2067 660a 0a20  factory as gf.. 
+00017e30: 2020 2063 203d 2067 662e 636f 6d70 6f6e     c = gf.compon
+00017e40: 656e 7473 2e73 7472 6169 6768 7428 0a20  ents.straight(. 
+00017e50: 2020 2020 2020 206c 656e 6774 683d 3130         length=10
+00017e60: 2c0a 2020 2020 2020 2020 7769 6474 683d  ,.        width=
+00017e70: 302e 352c 0a20 2020 2020 2020 2062 626f  0.5,.        bbo
+00017e80: 785f 6c61 7965 7273 3d5b 6766 2e4c 4159  x_layers=[gf.LAY
+00017e90: 4552 2e57 4743 4c41 445d 2c0a 2020 2020  ER.WGCLAD],.    
+00017ea0: 2020 2020 6262 6f78 5f6f 6666 7365 7473      bbox_offsets
+00017eb0: 3d5b 335d 2c0a 2020 2020 2020 2020 7769  =[3],.        wi
+00017ec0: 7468 5f62 626f 783d 5472 7565 2c0a 2020  th_bbox=True,.  
+00017ed0: 2020 2020 2020 636c 6164 6469 6e67 5f6c        cladding_l
+00017ee0: 6179 6572 733d 4e6f 6e65 2c0a 2020 2020  ayers=None,.    
+00017ef0: 2020 2020 6164 645f 7069 6e73 3d4e 6f6e      add_pins=Non
+00017f00: 652c 0a20 2020 2020 2020 2061 6464 5f62  e,.        add_b
+00017f10: 626f 783d 4e6f 6e65 2c0a 2020 2020 290a  box=None,.    ).
+00017f20: 2020 2020 6332 203d 2063 2e65 7874 7261      c2 = c.extra
+00017f30: 6374 286c 6179 6572 733d 5b67 662e 4c41  ct(layers=[gf.LA
+00017f40: 5945 522e 5747 434c 4144 5d29 0a0a 2020  YER.WGCLAD])..  
+00017f50: 2020 6173 7365 7274 206c 656e 2863 2e70    assert len(c.p
+00017f60: 6f6c 7967 6f6e 7329 203d 3d20 322c 206c  olygons) == 2, l
+00017f70: 656e 2863 2e70 6f6c 7967 6f6e 7329 0a20  en(c.polygons). 
+00017f80: 2020 2061 7373 6572 7420 6c65 6e28 6332     assert len(c2
+00017f90: 2e70 6f6c 7967 6f6e 7329 203d 3d20 312c  .polygons) == 1,
+00017fa0: 206c 656e 2863 322e 706f 6c79 676f 6e73   len(c2.polygons
+00017fb0: 290a 2020 2020 6173 7365 7274 2067 662e  ).    assert gf.
+00017fc0: 4c41 5945 522e 5747 434c 4144 2069 6e20  LAYER.WGCLAD in 
+00017fd0: 6332 2e6c 6179 6572 730a 2020 2020 7265  c2.layers.    re
+00017fe0: 7475 726e 2063 320a 0a0a 6465 6620 6861  turn c2...def ha
+00017ff0: 7368 5f66 696c 6528 6669 6c65 7061 7468  sh_file(filepath
+00018000: 293a 0a20 2020 206d 6435 203d 2068 6173  ):.    md5 = has
+00018010: 686c 6962 2e6d 6435 2829 0a20 2020 206d  hlib.md5().    m
+00018020: 6435 2e75 7064 6174 6528 6669 6c65 7061  d5.update(filepa
+00018030: 7468 2e72 6561 645f 6279 7465 7328 2929  th.read_bytes())
+00018040: 0a20 2020 2072 6574 7572 6e20 6d64 352e  .    return md5.
+00018050: 6865 7864 6967 6573 7428 290a 0a0a 6465  hexdigest()...de
+00018060: 6620 7465 7374 5f62 626f 785f 7265 6665  f test_bbox_refe
+00018070: 7265 6e63 6528 2920 2d3e 2043 6f6d 706f  rence() -> Compo
+00018080: 6e65 6e74 3a0a 2020 2020 696d 706f 7274  nent:.    import
+00018090: 2067 6473 6661 6374 6f72 7920 6173 2067   gdsfactory as g
+000180a0: 660a 0a20 2020 2063 203d 2067 662e 436f  f..    c = gf.Co
+000180b0: 6d70 6f6e 656e 7428 2263 6f6d 706f 6e65  mponent("compone
+000180c0: 6e74 5f77 6974 685f 6f66 6667 7269 645f  nt_with_offgrid_
+000180d0: 706f 6c79 676f 6e73 2229 0a20 2020 2063  polygons").    c
+000180e0: 3120 3d20 6320 3c3c 2067 662e 636f 6d70  1 = c << gf.comp
+000180f0: 6f6e 656e 7473 2e72 6563 7461 6e67 6c65  onents.rectangle
+00018100: 2873 697a 653d 2831 2e35 652d 332c 2031  (size=(1.5e-3, 1
+00018110: 2e35 652d 3329 2c20 706f 7274 5f74 7970  .5e-3), port_typ
+00018120: 653d 4e6f 6e65 290a 2020 2020 6332 203d  e=None).    c2 =
+00018130: 2063 203c 3c20 6766 2e63 6f6d 706f 6e65   c << gf.compone
+00018140: 6e74 732e 7265 6374 616e 676c 6528 7369  nts.rectangle(si
+00018150: 7a65 3d28 312e 3565 2d33 2c20 312e 3565  ze=(1.5e-3, 1.5e
+00018160: 2d33 292c 2070 6f72 745f 7479 7065 3d4e  -3), port_type=N
+00018170: 6f6e 6529 0a20 2020 2063 322e 786d 696e  one).    c2.xmin
+00018180: 203d 2063 312e 786d 6178 0a0a 2020 2020   = c1.xmax..    
+00018190: 6173 7365 7274 2063 322e 7873 697a 6520  assert c2.xsize 
+000181a0: 3d3d 2032 652d 330a 2020 2020 7265 7475  == 2e-3.    retu
+000181b0: 726e 2063 320a 0a0a 6465 6620 7465 7374  rn c2...def test
+000181c0: 5f62 626f 785f 636f 6d70 6f6e 656e 7428  _bbox_component(
+000181d0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2069  ) -> None:.    i
+000181e0: 6d70 6f72 7420 6764 7366 6163 746f 7279  mport gdsfactory
+000181f0: 2061 7320 6766 0a0a 2020 2020 6320 3d20   as gf..    c = 
+00018200: 6766 2e63 6f6d 706f 6e65 6e74 732e 7265  gf.components.re
+00018210: 6374 616e 676c 6528 7369 7a65 3d28 312e  ctangle(size=(1.
+00018220: 3565 2d33 2c20 312e 3565 2d33 292c 2070  5e-3, 1.5e-3), p
+00018230: 6f72 745f 7479 7065 3d4e 6f6e 6529 0a20  ort_type=None). 
+00018240: 2020 2061 7373 6572 7420 632e 7873 697a     assert c.xsiz
+00018250: 6520 3d3d 2032 652d 330a 0a0a 6465 6620  e == 2e-3...def 
+00018260: 7465 7374 5f72 656d 6170 5f6c 6179 6572  test_remap_layer
+00018270: 7328 2920 2d3e 204e 6f6e 653a 0a20 2020  s() -> None:.   
+00018280: 2069 6d70 6f72 7420 6764 7366 6163 746f   import gdsfacto
+00018290: 7279 2061 7320 6766 0a0a 2020 2020 6320  ry as gf..    c 
+000182a0: 3d20 6766 2e63 6f6d 706f 6e65 6e74 732e  = gf.components.
+000182b0: 7374 7261 6967 6874 286c 6179 6572 3d28  straight(layer=(
+000182c0: 322c 2030 2929 0a20 2020 2072 656d 6170  2, 0)).    remap
+000182d0: 203d 2063 2e72 656d 6170 5f6c 6179 6572   = c.remap_layer
+000182e0: 7328 6c61 7965 726d 6170 3d7b 2832 2c20  s(layermap={(2, 
+000182f0: 3029 3a20 6766 2e4c 4159 4552 2e57 474e  0): gf.LAYER.WGN
+00018300: 7d29 0a20 2020 2068 6173 685f 6765 6f6d  }).    hash_geom
+00018310: 6574 7279 203d 2022 3332 6364 3134 6561  etry = "32cd14ea
+00018320: 3763 6531 3363 6631 6634 3330 3237 3762  7ce13cf1f430277b
+00018330: 3435 3035 3461 3061 3739 3039 6133 6334  45054a0a7909a3c4
+00018340: 220a 0a20 2020 2061 7373 6572 7420 280a  "..    assert (.
+00018350: 2020 2020 2020 2020 7265 6d61 702e 6861          remap.ha
+00018360: 7368 5f67 656f 6d65 7472 7928 2920 3d3d  sh_geometry() ==
+00018370: 2068 6173 685f 6765 6f6d 6574 7279 0a20   hash_geometry. 
+00018380: 2020 2029 2c20 6622 6861 7368 5f67 656f     ), f"hash_geo
+00018390: 6d65 7472 7920 3d20 7b72 656d 6170 2e68  metry = {remap.h
+000183a0: 6173 685f 6765 6f6d 6574 7279 2829 2172  ash_geometry()!r
+000183b0: 7d22 0a0a 0a64 6566 2074 6573 745f 7265  }"...def test_re
+000183c0: 6d6f 7665 5f6c 6162 656c 7328 2920 2d3e  move_labels() ->
+000183d0: 204e 6f6e 653a 0a20 2020 2069 6d70 6f72   None:.    impor
+000183e0: 7420 6764 7366 6163 746f 7279 2061 7320  t gdsfactory as 
+000183f0: 6766 0a0a 2020 2020 6320 3d20 6766 2e63  gf..    c = gf.c
+00018400: 2e73 7472 6169 6768 7428 290a 2020 2020  .straight().    
+00018410: 632e 7265 6d6f 7665 5f6c 6162 656c 7328  c.remove_labels(
+00018420: 290a 0a20 2020 2061 7373 6572 7420 6c65  )..    assert le
+00018430: 6e28 632e 6c61 6265 6c73 2920 3d3d 2030  n(c.labels) == 0
+00018440: 0a0a 0a64 6566 2074 6573 745f 696d 706f  ...def test_impo
+00018450: 7274 5f67 6473 5f73 6574 7469 6e67 7328  rt_gds_settings(
+00018460: 2920 2d3e 204e 6f6e 653a 0a20 2020 2069  ) -> None:.    i
+00018470: 6d70 6f72 7420 6764 7366 6163 746f 7279  mport gdsfactory
+00018480: 2061 7320 6766 0a0a 2020 2020 6320 3d20   as gf..    c = 
+00018490: 6766 2e63 6f6d 706f 6e65 6e74 732e 6d7a  gf.components.mz
+000184a0: 6928 290a 2020 2020 6764 7370 6174 6820  i().    gdspath 
+000184b0: 3d20 632e 7772 6974 655f 6764 735f 7769  = c.write_gds_wi
+000184c0: 7468 5f6d 6574 6164 6174 6128 290a 2020  th_metadata().  
+000184d0: 2020 6332 203d 2067 662e 696d 706f 7274    c2 = gf.import
+000184e0: 5f67 6473 2867 6473 7061 7468 2c20 6e61  _gds(gdspath, na
+000184f0: 6d65 3d22 6d7a 695f 7361 6d70 6c65 222c  me="mzi_sample",
+00018500: 2072 6561 645f 6d65 7461 6461 7461 3d54   read_metadata=T
+00018510: 7275 6529 0a20 2020 2063 3320 3d20 6766  rue).    c3 = gf
+00018520: 2e72 6f75 7469 6e67 2e61 6464 5f66 6962  .routing.add_fib
+00018530: 6572 5f73 696e 676c 6528 6332 290a 2020  er_single(c2).  
+00018540: 2020 6173 7365 7274 2063 330a 0a0a 6465    assert c3...de
+00018550: 6620 7465 7374 5f66 6c61 7474 656e 5f69  f test_flatten_i
+00018560: 6e76 616c 6964 5f72 6566 735f 7265 6375  nvalid_refs_recu
+00018570: 7273 6976 6528 2920 2d3e 204e 6f6e 653a  rsive() -> None:
+00018580: 0a20 2020 2069 6d70 6f72 7420 6764 7366  .    import gdsf
+00018590: 6163 746f 7279 2061 7320 6766 0a20 2020  actory as gf.   
+000185a0: 2066 726f 6d20 6764 7366 6163 746f 7279   from gdsfactory
+000185b0: 2e64 6966 6674 6573 7420 696d 706f 7274  .difftest import
+000185c0: 2072 756e 5f78 6f72 0a20 2020 2066 726f   run_xor.    fro
+000185d0: 6d20 6764 7366 6163 746f 7279 2e72 6f75  m gdsfactory.rou
+000185e0: 7469 6e67 2e61 6c6c 5f61 6e67 6c65 2069  ting.all_angle i
+000185f0: 6d70 6f72 7420 6765 745f 6275 6e64 6c65  mport get_bundle
+00018600: 5f61 6c6c 5f61 6e67 6c65 0a0a 2020 2020  _all_angle..    
+00018610: 4067 662e 6365 6c6c 0a20 2020 2064 6566  @gf.cell.    def
+00018620: 2066 6c61 7428 293a 0a20 2020 2020 2020   flat():.       
+00018630: 2063 203d 2067 662e 436f 6d70 6f6e 656e   c = gf.Componen
+00018640: 7428 290a 2020 2020 2020 2020 6d6d 6931  t().        mmi1
+00018650: 203d 2028 6320 3c3c 2067 662e 636f 6d70   = (c << gf.comp
+00018660: 6f6e 656e 7473 2e6d 6d69 3178 3228 2929  onents.mmi1x2())
+00018670: 2e6d 6f76 6528 2830 2c20 2d31 2e30 3030  .move((0, -1.000
+00018680: 3529 290a 2020 2020 2020 2020 6d6d 6932  5)).        mmi2
+00018690: 203d 2028 6320 3c3c 2067 662e 636f 6d70   = (c << gf.comp
+000186a0: 6f6e 656e 7473 2e6d 6d69 3178 3228 2929  onents.mmi1x2())
+000186b0: 2e72 6f74 6174 6528 3830 290a 2020 2020  .rotate(80).    
+000186c0: 2020 2020 6d6d 6932 2e6d 6f76 6528 2834      mmi2.move((4
+000186d0: 302c 2032 3029 290a 2020 2020 2020 2020  0, 20)).        
+000186e0: 6275 6e64 6c65 203d 2067 6574 5f62 756e  bundle = get_bun
+000186f0: 646c 655f 616c 6c5f 616e 676c 6528 5b6d  dle_all_angle([m
+00018700: 6d69 312e 706f 7274 735b 226f 3222 5d5d  mi1.ports["o2"]]
+00018710: 2c20 5b6d 6d69 322e 706f 7274 735b 226f  , [mmi2.ports["o
+00018720: 3122 5d5d 290a 2020 2020 2020 2020 666f  1"]]).        fo
+00018730: 7220 726f 7574 6520 696e 2062 756e 646c  r route in bundl
+00018740: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
+00018750: 2e61 6464 2872 6f75 7465 2e72 6566 6572  .add(route.refer
+00018760: 656e 6365 7329 0a20 2020 2020 2020 2072  ences).        r
+00018770: 6574 7572 6e20 630a 0a20 2020 2040 6766  eturn c..    @gf
+00018780: 2e63 656c 6c0a 2020 2020 6465 6620 6869  .cell.    def hi
+00018790: 6572 6172 6368 7928 293a 0a20 2020 2020  erarchy():.     
+000187a0: 2020 2063 203d 2067 662e 436f 6d70 6f6e     c = gf.Compon
+000187b0: 656e 7428 290a 2020 2020 2020 2020 2863  ent().        (c
+000187c0: 203c 3c20 666c 6174 2829 292e 726f 7461   << flat()).rota
+000187d0: 7465 2833 3329 0a20 2020 2020 2020 2028  te(33).        (
+000187e0: 6320 3c3c 2066 6c61 7428 2929 2e72 6f74  c << flat()).rot
+000187f0: 6174 6528 3333 292e 6d6f 7665 2828 302c  ate(33).move((0,
+00018800: 2031 3030 2929 0a20 2020 2020 2020 2028   100)).        (
+00018810: 6320 3c3c 2066 6c61 7428 2929 2e6d 6f76  c << flat()).mov
+00018820: 6528 2831 3030 2c20 3029 290a 2020 2020  e((100, 0)).    
+00018830: 2020 2020 7265 7475 726e 2063 0a0a 2020      return c..  
+00018840: 2020 635f 6f72 6967 203d 2068 6965 7261    c_orig = hiera
+00018850: 7263 6879 2829 0a20 2020 2063 5f6e 6577  rchy().    c_new
+00018860: 203d 2066 6c61 7474 656e 5f69 6e76 616c   = flatten_inval
+00018870: 6964 5f72 6566 735f 7265 6375 7273 6976  id_refs_recursiv
+00018880: 6528 635f 6f72 6967 290a 2020 2020 6173  e(c_orig).    as
+00018890: 7365 7274 2063 5f6e 6577 2069 7320 6e6f  sert c_new is no
+000188a0: 7420 635f 6f72 6967 0a20 2020 2069 6e76  t c_orig.    inv
+000188b0: 616c 6964 5f72 6566 735f 6669 6c65 6e61  alid_refs_filena
+000188c0: 6d65 203d 2022 696e 7661 6c69 645f 7265  me = "invalid_re
+000188d0: 6673 2e67 6473 220a 2020 2020 696e 7661  fs.gds".    inva
+000188e0: 6c69 645f 7265 6673 5f66 6978 6564 5f66  lid_refs_fixed_f
+000188f0: 696c 656e 616d 6520 3d20 2269 6e76 616c  ilename = "inval
+00018900: 6964 5f72 6566 735f 6669 7865 642e 6764  id_refs_fixed.gd
+00018910: 7322 0a20 2020 2023 2067 6473 2066 696c  s".    # gds fil
+00018920: 6573 2073 686f 756c 6420 7374 696c 6c20  es should still 
+00018930: 6265 2073 616d 6520 746f 2031 6e6d 2074  be same to 1nm t
+00018940: 6f6c 6572 616e 6365 0a20 2020 2063 5f6f  olerance.    c_o
+00018950: 7269 672e 7772 6974 655f 6764 7328 696e  rig.write_gds(in
+00018960: 7661 6c69 645f 7265 6673 5f66 696c 656e  valid_refs_filen
+00018970: 616d 6529 0a20 2020 2063 5f6e 6577 2e77  ame).    c_new.w
+00018980: 7269 7465 5f67 6473 2869 6e76 616c 6964  rite_gds(invalid
+00018990: 5f72 6566 735f 6669 7865 645f 6669 6c65  _refs_fixed_file
+000189a0: 6e61 6d65 290a 2020 2020 7275 6e5f 786f  name).    run_xo
+000189b0: 7228 696e 7661 6c69 645f 7265 6673 5f66  r(invalid_refs_f
+000189c0: 696c 656e 616d 652c 2069 6e76 616c 6964  ilename, invalid
+000189d0: 5f72 6566 735f 6669 7865 645f 6669 6c65  _refs_fixed_file
+000189e0: 6e61 6d65 290a 0a0a 6966 205f 5f6e 616d  name)...if __nam
+000189f0: 655f 5f20 3d3d 2022 5f5f 6d61 696e 5f5f  e__ == "__main__
+00018a00: 223a 0a20 2020 2023 2069 6d70 6f72 7420  ":.    # import 
+00018a10: 6764 7366 6163 746f 7279 2061 7320 6766  gdsfactory as gf
+00018a20: 0a0a 2020 2020 7465 7374 5f72 656d 6170  ..    test_remap
+00018a30: 5f6c 6179 6572 7328 290a 2020 2020 2320  _layers().    # 
+00018a40: 6320 3d20 6766 2e43 6f6d 706f 6e65 6e74  c = gf.Component
+00018a50: 2829 0a20 2020 2023 2070 203d 2063 2e61  ().    # p = c.a
+00018a60: 6464 5f70 6f6c 7967 6f6e 280a 2020 2020  dd_polygon(.    
+00018a70: 2320 2020 2020 5b28 2d38 2c20 362c 2037  #     [(-8, 6, 7
+00018a80: 2c20 3929 2c20 282d 362c 2038 2c20 3137  , 9), (-6, 8, 17
+00018a90: 2c20 3529 5d2c 206c 6179 6572 3d28 312c  , 5)], layer=(1,
+00018aa0: 2030 290a 2020 2020 2320 2920 2023 2047   0).    # )  # G
+00018ab0: 4453 206c 6179 6572 7320 6172 6520 7475  DS layers are tu
+00018ac0: 706c 6573 206f 6620 696e 7473 2028 6275  ples of ints (bu
+00018ad0: 7420 6966 2077 6520 7573 6520 6f6e 6c79  t if we use only
+00018ae0: 206f 6e65 206e 756d 6265 7220 6974 2061   one number it a
+00018af0: 7373 756d 6573 2074 6865 206f 7468 6572  ssumes the other
+00018b00: 206e 756d 6265 7220 6973 2030 290a 0a20   number is 0).. 
+00018b10: 2020 2023 2063 3220 3d20 6766 2e43 6f6d     # c2 = gf.Com
+00018b20: 706f 6e65 6e74 2829 0a20 2020 2023 2063  ponent().    # c
+00018b30: 203d 2067 662e 636f 6d70 6f6e 656e 7473   = gf.components
+00018b40: 2e6d 7a69 2829 0a20 2020 2023 2070 7269  .mzi().    # pri
+00018b50: 6e74 2863 2e67 6574 5f6c 6179 6572 5f6e  nt(c.get_layer_n
+00018b60: 616d 6573 2829 290a 2020 2020 2320 6320  ames()).    # c 
+00018b70: 3d20 6766 2e63 6f6d 706f 6e65 6e74 732e  = gf.components.
+00018b80: 6d7a 6928 290a 2020 2020 2320 7072 696e  mzi().    # prin
+00018b90: 7428 632e 6765 745f 6c61 7965 725f 6e61  t(c.get_layer_na
+00018ba0: 6d65 7328 2929 0a20 2020 2023 2072 203d  mes()).    # r =
+00018bb0: 2063 2e72 6566 2829 0a20 2020 2023 2063   c.ref().    # c
+00018bc0: 322e 636f 7079 5f63 6869 6c64 5f69 6e66  2.copy_child_inf
+00018bd0: 6f28 632e 6e61 6d65 645f 7265 6665 7265  o(c.named_refere
+00018be0: 6e63 6573 5b22 7378 7422 5d29 0a20 2020  nces["sxt"]).   
+00018bf0: 2023 2074 6573 745f 7265 6d61 705f 6c61   # test_remap_la
+00018c00: 7965 7273 2829 0a20 2020 2023 2063 203d  yers().    # c =
+00018c10: 2074 6573 745f 6765 745f 6c61 7965 7273   test_get_layers
+00018c20: 2829 0a20 2020 2023 2063 2e70 6c6f 745f  ().    # c.plot_
+00018c30: 7174 2829 0a20 2020 2023 2063 2e70 6c6f  qt().    # c.plo
+00018c40: 7468 2829 0a20 2020 2023 2063 203d 2074  th().    # c = t
+00018c50: 6573 745f 6578 7472 6163 7428 290a 2020  est_extract().  
+00018c60: 2020 2320 6764 7370 6174 6820 3d20 632e    # gdspath = c.
+00018c70: 7772 6974 655f 6764 7328 290a 2020 2020  write_gds().    
+00018c80: 2320 6766 2e73 686f 7728 6764 7370 6174  # gf.show(gdspat
+00018c90: 6829 0a20 2020 2023 2063 2e73 686f 7728  h).    # c.show(
+00018ca0: 7368 6f77 5f70 6f72 7473 3d54 7275 6529  show_ports=True)
+00018cb0: 0a20 2020 2023 2063 2e73 686f 7728 290a  .    # c.show().
```

### Comparing `gdsfactory-6.96.0/gdsfactory/component_layout.py` & `gdsfactory-6.97.0/gdsfactory/component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/component_reference.py` & `gdsfactory-6.97.0/gdsfactory/component_reference.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/C.py` & `gdsfactory-6.97.0/gdsfactory/components/C.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/L.py` & `gdsfactory-6.97.0/gdsfactory/components/L.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/__init__.py` & `gdsfactory-6.97.0/gdsfactory/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/add_fiducials.py` & `gdsfactory-6.97.0/gdsfactory/components/add_fiducials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/add_grating_couplers.py` & `gdsfactory-6.97.0/gdsfactory/components/add_grating_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/add_trenches.py` & `gdsfactory-6.97.0/gdsfactory/components/add_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/align.py` & `gdsfactory-6.97.0/gdsfactory/components/align.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/array_component.py` & `gdsfactory-6.97.0/gdsfactory/components/array_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/array_with_fanout.py` & `gdsfactory-6.97.0/gdsfactory/components/array_with_fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/array_with_via.py` & `gdsfactory-6.97.0/gdsfactory/components/array_with_via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/awg.py` & `gdsfactory-6.97.0/gdsfactory/components/awg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/bbox.py` & `gdsfactory-6.97.0/gdsfactory/components/bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/bend_circular.py` & `gdsfactory-6.97.0/gdsfactory/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/bend_circular_heater.py` & `gdsfactory-6.97.0/gdsfactory/components/bend_circular_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/bend_euler.py` & `gdsfactory-6.97.0/gdsfactory/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/bend_port.py` & `gdsfactory-6.97.0/gdsfactory/components/bend_port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/bend_s.py` & `gdsfactory-6.97.0/gdsfactory/components/bend_s.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/bezier.py` & `gdsfactory-6.97.0/gdsfactory/components/bezier.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/cavity.py` & `gdsfactory-6.97.0/gdsfactory/components/cavity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/cdc.py` & `gdsfactory-6.97.0/gdsfactory/components/cdc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/cdsem_all.py` & `gdsfactory-6.97.0/gdsfactory/components/cdsem_all.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/cdsem_bend180.py` & `gdsfactory-6.97.0/gdsfactory/components/cdsem_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/cdsem_coupler.py` & `gdsfactory-6.97.0/gdsfactory/components/cdsem_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/cdsem_straight.py` & `gdsfactory-6.97.0/gdsfactory/components/cdsem_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/cdsem_straight_density.py` & `gdsfactory-6.97.0/gdsfactory/components/cdsem_straight_density.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/circle.py` & `gdsfactory-6.97.0/gdsfactory/components/circle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/coh_rx_dual_pol.py` & `gdsfactory-6.97.0/gdsfactory/components/coh_rx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/coh_rx_single_pol.py` & `gdsfactory-6.97.0/gdsfactory/components/coh_rx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/coh_tx_dual_pol.py` & `gdsfactory-6.97.0/gdsfactory/components/coh_tx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/coh_tx_single_pol.py` & `gdsfactory-6.97.0/gdsfactory/components/coh_tx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/compass.py` & `gdsfactory-6.97.0/gdsfactory/components/compass.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/component_lattice.py` & `gdsfactory-6.97.0/gdsfactory/components/component_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/component_sequence.py` & `gdsfactory-6.97.0/gdsfactory/components/component_sequence.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/copy_layers.py` & `gdsfactory-6.97.0/gdsfactory/components/copy_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/coupler.py` & `gdsfactory-6.97.0/gdsfactory/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/coupler90.py` & `gdsfactory-6.97.0/gdsfactory/components/coupler90.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/coupler90bend.py` & `gdsfactory-6.97.0/gdsfactory/components/coupler90bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/coupler_adiabatic.py` & `gdsfactory-6.97.0/gdsfactory/components/coupler_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/coupler_asymmetric.py` & `gdsfactory-6.97.0/gdsfactory/components/coupler_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/coupler_full.py` & `gdsfactory-6.97.0/gdsfactory/components/coupler_full.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/coupler_ring.py` & `gdsfactory-6.97.0/gdsfactory/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/coupler_straight.py` & `gdsfactory-6.97.0/gdsfactory/components/coupler_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/coupler_straight_asymmetric.py` & `gdsfactory-6.97.0/gdsfactory/components/coupler_straight_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/coupler_symmetric.py` & `gdsfactory-6.97.0/gdsfactory/components/coupler_symmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/cross.py` & `gdsfactory-6.97.0/gdsfactory/components/cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/crossing_waveguide.py` & `gdsfactory-6.97.0/gdsfactory/components/crossing_waveguide.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv` & `gdsfactory-6.97.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv` & `gdsfactory-6.97.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv` & `gdsfactory-6.97.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv` & `gdsfactory-6.97.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv` & `gdsfactory-6.97.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv` & `gdsfactory-6.97.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv` & `gdsfactory-6.97.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/cutback_2x2.py` & `gdsfactory-6.97.0/gdsfactory/components/cutback_2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/cutback_bend.py` & `gdsfactory-6.97.0/gdsfactory/components/cutback_bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/cutback_component.py` & `gdsfactory-6.97.0/gdsfactory/components/cutback_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/cutback_splitter.py` & `gdsfactory-6.97.0/gdsfactory/components/cutback_splitter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/dbr.py` & `gdsfactory-6.97.0/gdsfactory/components/dbr.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/dbr_tapered.py` & `gdsfactory-6.97.0/gdsfactory/components/dbr_tapered.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/delay_snake.py` & `gdsfactory-6.97.0/gdsfactory/components/delay_snake.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/delay_snake2.py` & `gdsfactory-6.97.0/gdsfactory/components/delay_snake2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/delay_snake3.py` & `gdsfactory-6.97.0/gdsfactory/components/delay_snake3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/delay_snake_sbend.py` & `gdsfactory-6.97.0/gdsfactory/components/delay_snake_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/dicing_lane.py` & `gdsfactory-6.97.0/gdsfactory/components/dicing_lane.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/die.py` & `gdsfactory-6.97.0/gdsfactory/components/die.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/die_bbox.py` & `gdsfactory-6.97.0/gdsfactory/components/die_bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/die_bbox_frame.py` & `gdsfactory-6.97.0/gdsfactory/components/die_bbox_frame.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/disk.py` & `gdsfactory-6.97.0/gdsfactory/components/disk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/edge_coupler_array.py` & `gdsfactory-6.97.0/gdsfactory/components/edge_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ellipse.py` & `gdsfactory-6.97.0/gdsfactory/components/ellipse.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/extend_ports_list.py` & `gdsfactory-6.97.0/gdsfactory/components/extend_ports_list.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/extension.py` & `gdsfactory-6.97.0/gdsfactory/components/extension.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/fiber.py` & `gdsfactory-6.97.0/gdsfactory/components/fiber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/fiber_array.py` & `gdsfactory-6.97.0/gdsfactory/components/fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/fiducial_squares.py` & `gdsfactory-6.97.0/gdsfactory/components/fiducial_squares.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ge_detector_straight_si_contacts.py` & `gdsfactory-6.97.0/gdsfactory/components/ge_detector_straight_si_contacts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_array.py` & `gdsfactory-6.97.0/gdsfactory/components/grating_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_dual_pol.py` & `gdsfactory-6.97.0/gdsfactory/components/grating_coupler_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical.py` & `gdsfactory-6.97.0/gdsfactory/components/grating_coupler_elliptical.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -200,24 +200,14 @@
         x = x1 / a1 * a
 
         pts = grating_tooth_points(a, b, x, w, taper_angle, spiked=False)
         c.add_polygon(pts, layer)
 
     x = np.round(taper_length + x_output, 3)
 
-    name = f"opt_{polarization.lower()}_{int(wavelength*1e3)}_{int(fiber_angle)}"
-    c.add_port(
-        name=name,
-        center=(x, 0),
-        width=10,
-        orientation=0,
-        layer=layer,
-        port_type=name,
-    )
-
     c.add_port(
         name="o1", center=(x_output, 0), width=wg_width, orientation=180, layer=layer
     )
 
     if layer_slab:
         slab_xmin += x_output + taper_length
         slab_length = total_length + slab_offset
@@ -232,14 +222,24 @@
             layer_slab,
         )
 
     if xs.add_bbox:
         c = xs.add_bbox(c)
     if xs.add_pins:
         c = xs.add_pins(c)
+
+    name = f"opt_{polarization.lower()}_{int(wavelength*1e3)}_{int(fiber_angle)}"
+    c.add_port(
+        name=name,
+        center=(x, 0),
+        width=10,
+        orientation=0,
+        layer=layer,
+        port_type=name,
+    )
     return c
 
 
 grating_coupler_elliptical_tm = gf.partial(
     grating_coupler_elliptical,
     grating_line_width=0.707,
     polarization="tm",
```

### Comparing `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py` & `gdsfactory-6.97.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,24 +127,14 @@
             x_output,
             x_taper + np.sum(widths) + np.sum(gaps) + 1,
             taper_angle,
             wg_width=wg_width,
         )
         c.add_polygon(pts, layer=layer_wg)
 
-    x = (taper_length + xis[-1]) / 2
-    name = f"opt_{polarization.lower()}_{int(wavelength*1e3)}_{int(fiber_angle)}"
-    c.add_port(
-        name=name,
-        center=(x, 0),
-        width=10,
-        orientation=0,
-        layer=xs.layer,
-        port_type=name,
-    )
     c.add_port(
         name="o1",
         center=(x_output, 0),
         width=wg_width,
         orientation=180,
         layer=layer_wg,
         cross_section=xs,
@@ -166,14 +156,24 @@
         )
 
     if xs.add_bbox:
         c = xs.add_bbox(c)
     if xs.add_pins:
         c = xs.add_pins(c)
 
+    x = (taper_length + xis[-1]) / 2
+    name = f"opt_{polarization.lower()}_{int(wavelength*1e3)}_{int(fiber_angle)}"
+    c.add_port(
+        name=name,
+        center=(x, 0),
+        width=10,
+        orientation=0,
+        layer=xs.layer,
+        port_type=name,
+    )
     return c
 
 
 @gf.cell
 def grating_coupler_elliptical_uniform(
     n_periods: int = 20,
     period: float = 0.75,
@@ -222,8 +222,8 @@
     gaps = [period * (1 - fill_factor)] * n_periods
     return grating_coupler_elliptical_arbitrary(gaps=gaps, widths=widths, **kwargs)
 
 
 if __name__ == "__main__":
     c = grating_coupler_elliptical_arbitrary(layer_grating=(3, 0))
     # c = grating_coupler_elliptical_arbitrary()
-    c.show(show_ports=True)
+    c.show(show_ports=False)
```

### Comparing `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py` & `gdsfactory-6.97.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,8 +167,8 @@
     c1.xmin = 0.7
     return c
 
 
 if __name__ == "__main__":
     # c = _compare()
     c = grating_coupler_elliptical_lumerical_etch70()
-    c.show(show_ports=True)
+    c.show(show_ports=False)
```

### Comparing `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical_trenches.py` & `gdsfactory-6.97.0/gdsfactory/components/grating_coupler_elliptical_trenches.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -105,25 +105,14 @@
         (xmax, y),
         (xmax + end_straight_length, y),
         (xmax + end_straight_length, -y),
         (xmax, -y),
     ]
     c.add_polygon(pts, layer)
 
-    x = np.round(taper_length + period * n_periods / 2, 3)
-    name = f"opt_{polarization.lower()}_{int(wavelength*1e3)}_{int(fiber_angle)}"
-    c.add_port(
-        name=name,
-        center=(x, 0),
-        width=10,
-        orientation=0,
-        layer=layer,
-        port_type=name,
-    )
-
     c.add_port(
         name="o1",
         center=(x_output, 0),
         width=wg_width,
         orientation=180,
         layer=layer,
         cross_section=xs,
@@ -131,14 +120,25 @@
     c.info["period"] = period
     c.info["polarization"] = polarization
     c.info["wavelength"] = wavelength
     if xs.add_bbox:
         c = xs.add_bbox(c)
     if xs.add_pins:
         c = xs.add_pins(c)
+
+    x = np.round(taper_length + period * n_periods / 2, 3)
+    name = f"opt_{polarization.lower()}_{int(wavelength*1e3)}_{int(fiber_angle)}"
+    c.add_port(
+        name=name,
+        center=(x, 0),
+        width=10,
+        orientation=0,
+        layer=layer,
+        port_type=name,
+    )
     return c
 
 
 grating_coupler_te = gf.partial(
     grating_coupler_elliptical_trenches, polarization="te", taper_angle=35
 )
```

### Comparing `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_functions.py` & `gdsfactory-6.97.0/gdsfactory/components/grating_coupler_functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_loss.py` & `gdsfactory-6.97.0/gdsfactory/components/grating_coupler_loss.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_loss_fiber_single.py` & `gdsfactory-6.97.0/gdsfactory/components/grating_coupler_loss_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_rectangular.py` & `gdsfactory-6.97.0/gdsfactory/components/grating_coupler_rectangular.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -97,25 +97,14 @@
         xsize = gf.snap.snap_to_grid(period * fill_factor)
         cgrating = c.add_ref(
             rectangle(size=(xsize, width_grating), layer=layer, port_type=None)
         )
         cgrating.xmin = gf.snap.snap_to_grid(x0 + i * period)
         cgrating.y = 0
 
-    xport = np.round((x0 + cgrating.x) / 2, 3)
-
-    name = f"opt_{polarization.lower()}_{int(wavelength*1e3)}_{int(fiber_angle)}"
-    c.add_port(
-        name=name,
-        port_type=name,
-        center=(xport, 0),
-        orientation=0,
-        width=width_grating,
-        layer=layer,
-    )
     c.info["polarization"] = polarization
     c.info["wavelength"] = wavelength
     gf.asserts.grating_coupler(c)
 
     if layer_slab:
         slab_xmin += length_taper
         slab_xsize = cgrating.xmax + slab_offset
@@ -130,14 +119,25 @@
             ],
             layer_slab,
         )
     if xs.add_bbox:
         c = xs.add_bbox(c)
     if xs.add_pins:
         c = xs.add_pins(c)
+
+    xport = np.round((x0 + cgrating.x) / 2, 3)
+    name = f"opt_{polarization.lower()}_{int(wavelength*1e3)}_{int(fiber_angle)}"
+    c.add_port(
+        name=name,
+        port_type=name,
+        center=(xport, 0),
+        orientation=0,
+        width=width_grating,
+        layer=layer,
+    )
     return c
 
 
 if __name__ == "__main__":
     # c = grating_coupler_rectangular(name='gcu', partial_etch=True)
     # c = grating_coupler_rectangular()
     c = gf.routing.add_fiber_array(grating_coupler=grating_coupler_rectangular)
```

### Comparing `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py` & `gdsfactory-6.97.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py` & `gdsfactory-6.97.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_tree.py` & `gdsfactory-6.97.0/gdsfactory/components/grating_coupler_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,8 +53,8 @@
         **kwargs,
     )
 
 
 if __name__ == "__main__":
     c = grating_coupler_tree()
     # print(c.settings)
-    c.show(show_ports=True)
+    c.show(show_ports=False)
```

### Comparing `gdsfactory-6.96.0/gdsfactory/components/greek_cross.py` & `gdsfactory-6.97.0/gdsfactory/components/greek_cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/hline.py` & `gdsfactory-6.97.0/gdsfactory/components/hline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/interdigital_capacitor.py` & `gdsfactory-6.97.0/gdsfactory/components/interdigital_capacitor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/litho_calipers.py` & `gdsfactory-6.97.0/gdsfactory/components/litho_calipers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/litho_ruler.py` & `gdsfactory-6.97.0/gdsfactory/components/litho_ruler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/litho_steps.py` & `gdsfactory-6.97.0/gdsfactory/components/litho_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/logo.py` & `gdsfactory-6.97.0/gdsfactory/components/logo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/loop_mirror.py` & `gdsfactory-6.97.0/gdsfactory/components/loop_mirror.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mmi1x2.py` & `gdsfactory-6.97.0/gdsfactory/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mmi1x2_with_sbend.py` & `gdsfactory-6.97.0/gdsfactory/components/mmi1x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mmi2x2.py` & `gdsfactory-6.97.0/gdsfactory/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mmi2x2_with_sbend.py` & `gdsfactory-6.97.0/gdsfactory/components/mmi2x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mmi_90degree_hybrid.py` & `gdsfactory-6.97.0/gdsfactory/components/mmi_90degree_hybrid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mode_converter.py` & `gdsfactory-6.97.0/gdsfactory/components/mode_converter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mzi.py` & `gdsfactory-6.97.0/gdsfactory/components/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mzi_arm.py` & `gdsfactory-6.97.0/gdsfactory/components/mzi_arm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mzi_arms.py` & `gdsfactory-6.97.0/gdsfactory/components/mzi_arms.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mzi_lattice.py` & `gdsfactory-6.97.0/gdsfactory/components/mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mzi_pads_center.py` & `gdsfactory-6.97.0/gdsfactory/components/mzi_pads_center.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mzi_phase_shifter.py` & `gdsfactory-6.97.0/gdsfactory/components/mzi_phase_shifter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mzit.py` & `gdsfactory-6.97.0/gdsfactory/components/mzit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mzit_lattice.py` & `gdsfactory-6.97.0/gdsfactory/components/mzit_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/mzm.py` & `gdsfactory-6.97.0/gdsfactory/components/mzm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/nxn.py` & `gdsfactory-6.97.0/gdsfactory/components/nxn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/optimal_90deg.py` & `gdsfactory-6.97.0/gdsfactory/components/optimal_90deg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/optimal_hairpin.py` & `gdsfactory-6.97.0/gdsfactory/components/optimal_hairpin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/optimal_step.py` & `gdsfactory-6.97.0/gdsfactory/components/optimal_step.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/pack_doe.py` & `gdsfactory-6.97.0/gdsfactory/components/pack_doe.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/pad.py` & `gdsfactory-6.97.0/gdsfactory/components/pad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/pad_gsg.py` & `gdsfactory-6.97.0/gdsfactory/components/pad_gsg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/pads_shorted.py` & `gdsfactory-6.97.0/gdsfactory/components/pads_shorted.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/polarization_splitter_rotator.py` & `gdsfactory-6.97.0/gdsfactory/components/polarization_splitter_rotator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ramp.py` & `gdsfactory-6.97.0/gdsfactory/components/ramp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/rectangle.py` & `gdsfactory-6.97.0/gdsfactory/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/rectangle_with_slits.py` & `gdsfactory-6.97.0/gdsfactory/components/rectangle_with_slits.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/regular_polygon.py` & `gdsfactory-6.97.0/gdsfactory/components/regular_polygon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/resistance_meander.py` & `gdsfactory-6.97.0/gdsfactory/components/resistance_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/resistance_sheet.py` & `gdsfactory-6.97.0/gdsfactory/components/resistance_sheet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ring.py` & `gdsfactory-6.97.0/gdsfactory/components/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ring_crow.py` & `gdsfactory-6.97.0/gdsfactory/components/ring_crow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ring_crow_couplers.py` & `gdsfactory-6.97.0/gdsfactory/components/ring_crow_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ring_double.py` & `gdsfactory-6.97.0/gdsfactory/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ring_double_bend_coupler.py` & `gdsfactory-6.97.0/gdsfactory/components/ring_double_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ring_double_heater.py` & `gdsfactory-6.97.0/gdsfactory/components/ring_double_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ring_double_pn.py` & `gdsfactory-6.97.0/gdsfactory/components/ring_double_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ring_section_based.py` & `gdsfactory-6.97.0/gdsfactory/components/ring_section_based.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ring_single.py` & `gdsfactory-6.97.0/gdsfactory/components/ring_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ring_single_array.py` & `gdsfactory-6.97.0/gdsfactory/components/ring_single_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ring_single_bend_coupler.py` & `gdsfactory-6.97.0/gdsfactory/components/ring_single_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ring_single_dut.py` & `gdsfactory-6.97.0/gdsfactory/components/ring_single_dut.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ring_single_heater.py` & `gdsfactory-6.97.0/gdsfactory/components/ring_single_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/ring_single_pn.py` & `gdsfactory-6.97.0/gdsfactory/components/ring_single_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/seal_ring.py` & `gdsfactory-6.97.0/gdsfactory/components/seal_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/snspd.py` & `gdsfactory-6.97.0/gdsfactory/components/snspd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/spiral_double.py` & `gdsfactory-6.97.0/gdsfactory/components/spiral_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/spiral_external_io.py` & `gdsfactory-6.97.0/gdsfactory/components/spiral_external_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/spiral_heater.py` & `gdsfactory-6.97.0/gdsfactory/components/spiral_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/spiral_inner_io.py` & `gdsfactory-6.97.0/gdsfactory/components/spiral_inner_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/splitter_chain.py` & `gdsfactory-6.97.0/gdsfactory/components/splitter_chain.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/splitter_tree.py` & `gdsfactory-6.97.0/gdsfactory/components/splitter_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/straight.py` & `gdsfactory-6.97.0/gdsfactory/components/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/straight_array.py` & `gdsfactory-6.97.0/gdsfactory/components/straight_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/straight_heater_doped_rib.py` & `gdsfactory-6.97.0/gdsfactory/components/straight_heater_doped_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/straight_heater_doped_strip.py` & `gdsfactory-6.97.0/gdsfactory/components/straight_heater_doped_strip.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/straight_heater_meander.py` & `gdsfactory-6.97.0/gdsfactory/components/straight_heater_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/straight_heater_meander_doped.py` & `gdsfactory-6.97.0/gdsfactory/components/straight_heater_meander_doped.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/straight_heater_metal.py` & `gdsfactory-6.97.0/gdsfactory/components/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/straight_pin.py` & `gdsfactory-6.97.0/gdsfactory/components/straight_pin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/straight_pin_slot.py` & `gdsfactory-6.97.0/gdsfactory/components/straight_pin_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/straight_rib.py` & `gdsfactory-6.97.0/gdsfactory/components/straight_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/switch_tree.py` & `gdsfactory-6.97.0/gdsfactory/components/switch_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/taper.py` & `gdsfactory-6.97.0/gdsfactory/components/taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/taper_adiabatic.py` & `gdsfactory-6.97.0/gdsfactory/components/taper_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/taper_cross_section.py` & `gdsfactory-6.97.0/gdsfactory/components/taper_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/taper_from_csv.py` & `gdsfactory-6.97.0/gdsfactory/components/taper_from_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/taper_parabolic.py` & `gdsfactory-6.97.0/gdsfactory/components/taper_parabolic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/terminator.py` & `gdsfactory-6.97.0/gdsfactory/components/terminator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/text.py` & `gdsfactory-6.97.0/gdsfactory/components/text.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/text_freetype.py` & `gdsfactory-6.97.0/gdsfactory/components/text_freetype.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/text_rectangular.py` & `gdsfactory-6.97.0/gdsfactory/components/text_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/text_rectangular_font.py` & `gdsfactory-6.97.0/gdsfactory/components/text_rectangular_font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/triangles.py` & `gdsfactory-6.97.0/gdsfactory/components/triangles.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/verniers.py` & `gdsfactory-6.97.0/gdsfactory/components/verniers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/version_stamp.py` & `gdsfactory-6.97.0/gdsfactory/components/version_stamp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/via.py` & `gdsfactory-6.97.0/gdsfactory/components/via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/via_corner.py` & `gdsfactory-6.97.0/gdsfactory/components/via_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/via_cutback.py` & `gdsfactory-6.97.0/gdsfactory/components/via_cutback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/via_stack.py` & `gdsfactory-6.97.0/gdsfactory/components/via_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/via_stack_slot.py` & `gdsfactory-6.97.0/gdsfactory/components/via_stack_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/via_stack_with_offset.py` & `gdsfactory-6.97.0/gdsfactory/components/via_stack_with_offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/wafer.py` & `gdsfactory-6.97.0/gdsfactory/components/wafer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/wire.py` & `gdsfactory-6.97.0/gdsfactory/components/wire.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/components/wire_sbend.py` & `gdsfactory-6.97.0/gdsfactory/components/wire_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/config.py` & `gdsfactory-6.97.0/gdsfactory/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from loguru import logger
 import omegaconf
 from omegaconf import OmegaConf
 
 from rich.console import Console
 from rich.table import Table
 
-__version__ = "6.96.0"
+__version__ = "6.97.0"
 PathType = Union[str, pathlib.Path]
 
 home = pathlib.Path.home()
 cwd = pathlib.Path.cwd()
 module_path = pathlib.Path(__file__).parent.absolute()
 repo_path = module_path.parent
 home_path = pathlib.Path.home() / ".gdsfactory"
```

### Comparing `gdsfactory-6.96.0/gdsfactory/constants.py` & `gdsfactory-6.97.0/gdsfactory/constants.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/containers.py` & `gdsfactory-6.97.0/gdsfactory/containers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/cross_section.py` & `gdsfactory-6.97.0/gdsfactory/cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/decorators.py` & `gdsfactory-6.97.0/gdsfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/difftest.py` & `gdsfactory-6.97.0/gdsfactory/difftest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/events.py` & `gdsfactory-6.97.0/gdsfactory/events.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/export/to_3d.py` & `gdsfactory-6.97.0/gdsfactory/export/to_3d.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/export/to_np.py` & `gdsfactory-6.97.0/gdsfactory/export/to_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/export/to_stl.py` & `gdsfactory-6.97.0/gdsfactory/export/to_stl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/export/write_gerbers.py` & `gdsfactory-6.97.0/gdsfactory/export/write_gerbers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/filestorage.py` & `gdsfactory-6.97.0/gdsfactory/filestorage.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/fill.py` & `gdsfactory-6.97.0/gdsfactory/fill.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/font.py` & `gdsfactory-6.97.0/gdsfactory/font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/functions.py` & `gdsfactory-6.97.0/gdsfactory/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/gdsdiff/gds_diff_git.py` & `gdsfactory-6.97.0/gdsfactory/gdsdiff/gds_diff_git.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/gdsdiff/gdsdiff.py` & `gdsfactory-6.97.0/gdsfactory/gdsdiff/gdsdiff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/gdsdiff/install.py` & `gdsfactory-6.97.0/gdsfactory/gdsdiff/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/gdsdiff/test_xor.py` & `gdsfactory-6.97.0/gdsfactory/gdsdiff/test_xor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/README.md` & `gdsfactory-6.97.0/gdsfactory/generic_tech/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/__init__.py` & `gdsfactory-6.97.0/gdsfactory/generic_tech/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/get_klayout_pyxs.py` & `gdsfactory-6.97.0/gdsfactory/generic_tech/get_klayout_pyxs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/drc/errors.py` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/drc/errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/grain.xml`

 * *Files 1% similar despite different names*

#### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/grain.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <salt-grain>
   <name>gdsfactory</name>
   <token/>
   <hidden>false</hidden>
-  <version>6.96.0</version>
+  <version>6.97.0</version>
   <api-version/>
   <title>gdsfactory</title>
   <doc>EDA tool to layout integrated circuits</doc>
   <doc-url>https://gdsfactory.github.io/gdsfactory/</doc-url>
   <url>https://github.com/gdsfactory/gdsfactory</url>
   <license>MIT</license>
   <author>Joaquin Matres</author>
```

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/icon_128x128.png` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/icon_64x64.png` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/README.md` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

 * *Files 1% similar despite different names*

#### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

```diff
@@ -12,15 +12,15 @@
   <show-in-menu>false</show-in-menu>
   <group-name/>
   <menu-path>gdsfactory.begin</menu-path>
   <interpreter>python</interpreter>
   <dsl-interpreter-name/>
   <text>import pya
 
-__version__ = &quot;6.96.0&quot;
+__version__ = &quot;6.97.0&quot;
 
 
 def set_menu():
     menu = pya.Application.instance().main_window().menu()
 
     s0 = &quot;gdsfactory&quot;
     if not (menu.is_menu(s0)):
```

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/layers.lyp` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/layers.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/tech.lyt` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/tech.lyt`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs` & `gdsfactory-6.97.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/layer_map.py` & `gdsfactory-6.97.0/gdsfactory/generic_tech/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/layer_stack.py` & `gdsfactory-6.97.0/gdsfactory/generic_tech/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/generic_tech/layer_views.yaml` & `gdsfactory-6.97.0/gdsfactory/generic_tech/layer_views.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/__init__.py` & `gdsfactory-6.97.0/gdsfactory/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/boolean.py` & `gdsfactory-6.97.0/gdsfactory/geometry/boolean.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/boolean_klayout.py` & `gdsfactory-6.97.0/gdsfactory/geometry/boolean_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/boolean_polygons.py` & `gdsfactory-6.97.0/gdsfactory/geometry/boolean_polygons.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/check_duplicated_cells.py` & `gdsfactory-6.97.0/gdsfactory/geometry/check_duplicated_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/check_exclusion.py` & `gdsfactory-6.97.0/gdsfactory/geometry/check_exclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/check_inclusion.py` & `gdsfactory-6.97.0/gdsfactory/geometry/check_inclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/check_space.py` & `gdsfactory-6.97.0/gdsfactory/geometry/check_space.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/check_width.py` & `gdsfactory-6.97.0/gdsfactory/geometry/check_width.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/fill_klayout.py` & `gdsfactory-6.97.0/gdsfactory/geometry/fill_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/fill_tiled.py` & `gdsfactory-6.97.0/gdsfactory/geometry/fill_tiled.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/fillet.py` & `gdsfactory-6.97.0/gdsfactory/geometry/fillet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/functions.py` & `gdsfactory-6.97.0/gdsfactory/geometry/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/invert.py` & `gdsfactory-6.97.0/gdsfactory/geometry/invert.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/layer_priority.py` & `gdsfactory-6.97.0/gdsfactory/geometry/layer_priority.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/manhattanize.py` & `gdsfactory-6.97.0/gdsfactory/geometry/manhattanize.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/maskprep.py` & `gdsfactory-6.97.0/gdsfactory/geometry/maskprep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/maskprep_flat.py` & `gdsfactory-6.97.0/gdsfactory/geometry/maskprep_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/offset.py` & `gdsfactory-6.97.0/gdsfactory/geometry/offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/outline.py` & `gdsfactory-6.97.0/gdsfactory/geometry/outline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/trim.py` & `gdsfactory-6.97.0/gdsfactory/geometry/trim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/union.py` & `gdsfactory-6.97.0/gdsfactory/geometry/union.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/write_connectivity.py` & `gdsfactory-6.97.0/gdsfactory/geometry/write_connectivity.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,25 +7,55 @@
 
 import gdsfactory as gf
 from gdsfactory.typings import CrossSectionSpec, Dict, Layer
 from gdsfactory.geometry.write_drc import write_drc_deck_macro
 
 layer_name_to_min_width: Dict[str, float]
 
+nm = 1e-3
+
 
 class ConnectivyCheck(BaseModel):
     cross_section: CrossSectionSpec
     pin_length: float
     pin_layer: Layer
 
 
 def write_connectivity_checks(
+    pin_widths: List[float], pin_layer: Layer, pin_length: float = 1 * nm
+):
+    """Return script for port connectivity check.
+    Assumes the port pins are inside the Component.
+
+    Args:
+        pin_widths: list of pin widths allowed.
+        pin_layer: for the pin markers.
+        pin_length: in um.
+    """
+
+    script = f"""pin = input{pin_layer}
+pin = pin.merged\n
+pin2 = pin.rectangles.without_area({pin_widths[0]} * {2 * pin_length})"""
+
+    for w in pin_widths[1:]:
+        script += f" - pin.rectangles.with_area({w} * {2 * pin_length})"
+
+    script += """\npin2.output(\"port alignment error\")\n
+pin2 = pin.sized(0.0).merged\n
+pin2.non_rectangles.output(\"port width check\")\n\n"""
+
+    return script
+
+
+def write_connectivity_checks_per_section(
     connectivity_checks: List[ConnectivyCheck],
 ) -> str:
-    """Return script for photonic port connectivity check. Assumes the photonic port pins are inside the Component.
+    """Return script for port connectivity check.
+    Assumes the port pins are inside the Component and each cross_section has pins on a different layer.
+    This is not the recommended way as it only supports two widths per cross_section (cross_section.width and cross_section.width_wide)
 
     Args:
         connectivity_checks: list of connectivity objects to check for.
     """
     script = ""
 
     for cc in connectivity_checks:
@@ -43,19 +73,26 @@
 {xs.name}_pin2 = {xs.name}_pin.sized(0.0).merged\n
 {xs.name}_pin2.non_rectangles.output(\"port width check\")\n\n"""
 
     return script
 
 
 if __name__ == "__main__":
+    from gdsfactory.generic_tech import LAYER
+
     nm = 1e-3
 
     connectivity_checks = [
         # ConnectivyCheck(cross_section="strip", pin_length=1 * nm, pin_layer=(1, 10))
         ConnectivyCheck(
             cross_section="strip_auto_widen", pin_length=1 * nm, pin_layer=(1, 10)
         )
     ]
-    rules = [write_connectivity_checks(connectivity_checks=connectivity_checks)]
+    rules = [
+        write_connectivity_checks_per_section(connectivity_checks=connectivity_checks)
+    ]
 
+    rules = [
+        write_connectivity_checks(pin_widths=[0.5, 0.9, 0.45], pin_layer=LAYER.PORT)
+    ]
     script = write_drc_deck_macro(rules=rules, layers=None)
     print(script)
```

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/write_drc.py` & `gdsfactory-6.97.0/gdsfactory/geometry/write_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/geometry/xor_diff.py` & `gdsfactory-6.97.0/gdsfactory/geometry/xor_diff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/get_factories.py` & `gdsfactory-6.97.0/gdsfactory/get_factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/get_netlist.py` & `gdsfactory-6.97.0/gdsfactory/get_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/get_netlist_flat.py` & `gdsfactory-6.97.0/gdsfactory/get_netlist_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/get_netlist_klayout.py` & `gdsfactory-6.97.0/gdsfactory/get_netlist_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/grid.py` & `gdsfactory-6.97.0/gdsfactory/grid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/install.py` & `gdsfactory-6.97.0/gdsfactory/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/klive.py` & `gdsfactory-6.97.0/gdsfactory/klive.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/labels/__init__.py` & `gdsfactory-6.97.0/gdsfactory/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/labels/add_label_yaml.py` & `gdsfactory-6.97.0/gdsfactory/labels/add_label_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/labels/ehva.py` & `gdsfactory-6.97.0/gdsfactory/labels/ehva.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/labels/merge_test_metadata.py` & `gdsfactory-6.97.0/gdsfactory/labels/merge_test_metadata.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/labels/siepic.py` & `gdsfactory-6.97.0/gdsfactory/labels/siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/labels/write_labels.py` & `gdsfactory-6.97.0/gdsfactory/labels/write_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/materials.py` & `gdsfactory-6.97.0/gdsfactory/materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/name.py` & `gdsfactory-6.97.0/gdsfactory/name.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/pack.py` & `gdsfactory-6.97.0/gdsfactory/pack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/path.py` & `gdsfactory-6.97.0/gdsfactory/path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/pdk.py` & `gdsfactory-6.97.0/gdsfactory/pdk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/picmodel.py` & `gdsfactory-6.97.0/gdsfactory/picmodel.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/pixelate.py` & `gdsfactory-6.97.0/gdsfactory/pixelate.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/plugins/dagster/workflow.py` & `gdsfactory-6.97.0/gdsfactory/plugins/dagster/workflow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/plugins/database/README.md` & `gdsfactory-6.97.0/gdsfactory/plugins/database/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/plugins/database/db_upload.py` & `gdsfactory-6.97.0/gdsfactory/plugins/database/db_upload.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/plugins/database/models.py` & `gdsfactory-6.97.0/gdsfactory/plugins/database/models.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/plugins/web/main.py` & `gdsfactory-6.97.0/gdsfactory/plugins/web/main.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/plugins/web/server.py` & `gdsfactory-6.97.0/gdsfactory/plugins/web/server.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/plugins/web/server_jupyter.py` & `gdsfactory-6.97.0/gdsfactory/plugins/web/server_jupyter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/plugins/web/static/client.css` & `gdsfactory-6.97.0/gdsfactory/plugins/web/static/client.css`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/port.py` & `gdsfactory-6.97.0/gdsfactory/port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/quickplotter.py` & `gdsfactory-6.97.0/gdsfactory/quickplotter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/read/__init__.py` & `gdsfactory-6.97.0/gdsfactory/read/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/read/from_dphox.py` & `gdsfactory-6.97.0/gdsfactory/read/from_dphox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/read/from_gdspaths.py` & `gdsfactory-6.97.0/gdsfactory/read/from_gdspaths.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/read/from_np.py` & `gdsfactory-6.97.0/gdsfactory/read/from_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/read/from_phidl.py` & `gdsfactory-6.97.0/gdsfactory/read/from_phidl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/read/from_yaml.py` & `gdsfactory-6.97.0/gdsfactory/read/from_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/read/from_yaml_template.py` & `gdsfactory-6.97.0/gdsfactory/read/from_yaml_template.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/read/import_gds.py` & `gdsfactory-6.97.0/gdsfactory/read/import_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/read/labels.py` & `gdsfactory-6.97.0/gdsfactory/read/labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/__init__.py` & `gdsfactory-6.97.0/gdsfactory/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/add_electrical_pads_shortest.py` & `gdsfactory-6.97.0/gdsfactory/routing/add_electrical_pads_shortest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/add_electrical_pads_top.py` & `gdsfactory-6.97.0/gdsfactory/routing/add_electrical_pads_top.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/add_electrical_pads_top_dc.py` & `gdsfactory-6.97.0/gdsfactory/routing/add_electrical_pads_top_dc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/add_fiber_array.py` & `gdsfactory-6.97.0/gdsfactory/routing/add_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/add_fiber_single.py` & `gdsfactory-6.97.0/gdsfactory/routing/add_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/add_pads.py` & `gdsfactory-6.97.0/gdsfactory/routing/add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/all_angle.py` & `gdsfactory-6.97.0/gdsfactory/routing/all_angle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/auto_taper.py` & `gdsfactory-6.97.0/gdsfactory/routing/auto_taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/factories.py` & `gdsfactory-6.97.0/gdsfactory/routing/factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/fanout.py` & `gdsfactory-6.97.0/gdsfactory/routing/fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/fanout2x2.py` & `gdsfactory-6.97.0/gdsfactory/routing/fanout2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/get_bundle.py` & `gdsfactory-6.97.0/gdsfactory/routing/get_bundle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/get_bundle_corner.py` & `gdsfactory-6.97.0/gdsfactory/routing/get_bundle_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/get_bundle_from_steps.py` & `gdsfactory-6.97.0/gdsfactory/routing/get_bundle_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/get_bundle_from_waypoints.py` & `gdsfactory-6.97.0/gdsfactory/routing/get_bundle_from_waypoints.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/get_bundle_path_length_match.py` & `gdsfactory-6.97.0/gdsfactory/routing/get_bundle_path_length_match.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/get_bundle_sbend.py` & `gdsfactory-6.97.0/gdsfactory/routing/get_bundle_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/get_bundle_u.py` & `gdsfactory-6.97.0/gdsfactory/routing/get_bundle_u.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/get_input_labels.py` & `gdsfactory-6.97.0/gdsfactory/routing/get_input_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/get_route.py` & `gdsfactory-6.97.0/gdsfactory/routing/get_route.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/get_route_astar.py` & `gdsfactory-6.97.0/gdsfactory/routing/get_route_astar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/get_route_from_steps.py` & `gdsfactory-6.97.0/gdsfactory/routing/get_route_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/get_route_sbend.py` & `gdsfactory-6.97.0/gdsfactory/routing/get_route_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/get_routes_bend180.py` & `gdsfactory-6.97.0/gdsfactory/routing/get_routes_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/get_routes_straight.py` & `gdsfactory-6.97.0/gdsfactory/routing/get_routes_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/manhattan.py` & `gdsfactory-6.97.0/gdsfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/path_length_matching.py` & `gdsfactory-6.97.0/gdsfactory/routing/path_length_matching.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/route_fiber_array.py` & `gdsfactory-6.97.0/gdsfactory/routing/route_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/route_fiber_single.py` & `gdsfactory-6.97.0/gdsfactory/routing/route_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/route_ports_to_side.py` & `gdsfactory-6.97.0/gdsfactory/routing/route_ports_to_side.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/route_quad.py` & `gdsfactory-6.97.0/gdsfactory/routing/route_quad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/route_sharp.py` & `gdsfactory-6.97.0/gdsfactory/routing/route_sharp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/route_south.py` & `gdsfactory-6.97.0/gdsfactory/routing/route_south.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/sort_ports.py` & `gdsfactory-6.97.0/gdsfactory/routing/sort_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/routing/utils.py` & `gdsfactory-6.97.0/gdsfactory/routing/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell.py` & `gdsfactory-6.97.0/gdsfactory/samples/01_component_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml` & `gdsfactory-6.97.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell_with_pins.py` & `gdsfactory-6.97.0/gdsfactory/samples/01_component_pcell_with_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml` & `gdsfactory-6.97.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/03_move.py` & `gdsfactory-6.97.0/gdsfactory/samples/03_move.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/04_connect.py` & `gdsfactory-6.97.0/gdsfactory/samples/04_connect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/05_remove_layers.py` & `gdsfactory-6.97.0/gdsfactory/samples/05_remove_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/06_remapping_layers.py` & `gdsfactory-6.97.0/gdsfactory/samples/06_remapping_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/07_flattening_device.py` & `gdsfactory-6.97.0/gdsfactory/samples/07_flattening_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/11_component_layout.py` & `gdsfactory-6.97.0/gdsfactory/samples/11_component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/12_component_refs.py` & `gdsfactory-6.97.0/gdsfactory/samples/12_component_refs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/13_component_netlist.py` & `gdsfactory-6.97.0/gdsfactory/samples/13_component_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/14_component_connectivity.py` & `gdsfactory-6.97.0/gdsfactory/samples/14_component_connectivity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/15_component_sequence1.py` & `gdsfactory-6.97.0/gdsfactory/samples/15_component_sequence1.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/16_component_sequence2.py` & `gdsfactory-6.97.0/gdsfactory/samples/16_component_sequence2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/17_ports.py` & `gdsfactory-6.97.0/gdsfactory/samples/17_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/20_components.py` & `gdsfactory-6.97.0/gdsfactory/samples/20_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/22_add_pads.py` & `gdsfactory-6.97.0/gdsfactory/samples/22_add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/23_reticle.py` & `gdsfactory-6.97.0/gdsfactory/samples/23_reticle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/23_reticle_passives.py` & `gdsfactory-6.97.0/gdsfactory/samples/23_reticle_passives.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/24_doe_2.py` & `gdsfactory-6.97.0/gdsfactory/samples/24_doe_2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/24_doe_3.py` & `gdsfactory-6.97.0/gdsfactory/samples/24_doe_3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/30_lidar.py` & `gdsfactory-6.97.0/gdsfactory/samples/30_lidar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/30_lidar_pcell.py` & `gdsfactory-6.97.0/gdsfactory/samples/30_lidar_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/30_lidar_with_pads.py` & `gdsfactory-6.97.0/gdsfactory/samples/30_lidar_with_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing.py` & `gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml` & `gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml` & `gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml` & `gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml` & `gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml` & `gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml` & `gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml` & `gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml` & `gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml` & `gdsfactory-6.97.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/big_device.py` & `gdsfactory-6.97.0/gdsfactory/samples/big_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/demo/benchmark/fill_demo.py` & `gdsfactory-6.97.0/gdsfactory/samples/demo/benchmark/fill_demo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/mask.pic.yml` & `gdsfactory-6.97.0/gdsfactory/samples/demo/circuits/mask.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml` & `gdsfactory-6.97.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml` & `gdsfactory-6.97.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/demo/drc_errors.py` & `gdsfactory-6.97.0/gdsfactory/samples/demo/drc_errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/demo/drc_write.py` & `gdsfactory-6.97.0/gdsfactory/samples/demo/drc_write.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/demo/layers.py` & `gdsfactory-6.97.0/gdsfactory/samples/demo/layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/demo/lvs.py` & `gdsfactory-6.97.0/gdsfactory/samples/demo/lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/demo/pcell.py` & `gdsfactory-6.97.0/gdsfactory/samples/demo/pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/netlists/mzi.yml` & `gdsfactory-6.97.0/gdsfactory/samples/netlists/mzi.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/netlists/mzi_full.yml` & `gdsfactory-6.97.0/gdsfactory/samples/netlists/mzi_full.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/fab_c.py` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c.py` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml` & `gdsfactory-6.97.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/schematic_editor.py` & `gdsfactory-6.97.0/gdsfactory/schematic_editor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/serialization.py` & `gdsfactory-6.97.0/gdsfactory/serialization.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/show.py` & `gdsfactory-6.97.0/gdsfactory/show.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/__init__.py` & `gdsfactory-6.97.0/gdsfactory/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/add_simulation_markers.py` & `gdsfactory-6.97.0/gdsfactory/simulation/add_simulation_markers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/convert_sparameters.py` & `gdsfactory-6.97.0/gdsfactory/simulation/convert_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/devsim/__init__.py` & `gdsfactory-6.97.0/gdsfactory/simulation/devsim/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/devsim/doping.py` & `gdsfactory-6.97.0/gdsfactory/simulation/devsim/doping.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/devsim/get_simulation.py` & `gdsfactory-6.97.0/gdsfactory/simulation/devsim/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/devsim/get_simulation_xsection.py` & `gdsfactory-6.97.0/gdsfactory/simulation/devsim/get_simulation_xsection.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/devsim/get_solver.py` & `gdsfactory-6.97.0/gdsfactory/simulation/devsim/get_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/devsim/test_devsim.py` & `gdsfactory-6.97.0/gdsfactory/simulation/devsim/test_devsim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/eme/meow_eme.py` & `gdsfactory-6.97.0/gdsfactory/simulation/eme/meow_eme.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/eme/test_meow_simulation.py` & `gdsfactory-6.97.0/gdsfactory/simulation/eme/test_meow_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/fem/mode_solver.py` & `gdsfactory-6.97.0/gdsfactory/simulation/fem/mode_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/fem/test_mode_solver.py` & `gdsfactory-6.97.0/gdsfactory/simulation/fem/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/get_effective_indices.py` & `gdsfactory-6.97.0/gdsfactory/simulation/get_effective_indices.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/get_modes_path.py` & `gdsfactory-6.97.0/gdsfactory/simulation/get_modes_path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/get_sparameters_path.py` & `gdsfactory-6.97.0/gdsfactory/simulation/get_sparameters_path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/__init__.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_material.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/get_material.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_meep_geometry.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/get_meep_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_simulation.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_eigenmode.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_materials.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/__init__.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmsh/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/break_geometry.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmsh/break_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/mesh.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmsh/mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/meshtracker.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmsh/meshtracker.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/parse_component.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmsh/parse_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/parse_gds.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmsh/parse_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/parse_layerstack.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmsh/parse_layerstack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/refine.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmsh/refine.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/tests/test_meshing.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmsh/tests/test_meshing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/xyz_mesh.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gmsh/xyz_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/__init__.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/get_results.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/get_results.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/get_simulation.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/materials.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/modes.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/sim_run.yaml` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/sim_run.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_results.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/utils.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/write_sparameters.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py` & `gdsfactory-6.97.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/lumerical/__init__.py` & `gdsfactory-6.97.0/gdsfactory/simulation/lumerical/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/lumerical/interconnect.py` & `gdsfactory-6.97.0/gdsfactory/simulation/lumerical/interconnect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/lumerical/read.py` & `gdsfactory-6.97.0/gdsfactory/simulation/lumerical/read.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/lumerical/settings.py` & `gdsfactory-6.97.0/gdsfactory/simulation/lumerical/settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/lumerical/test_read_sparameters.py` & `gdsfactory-6.97.0/gdsfactory/simulation/lumerical/test_read_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py` & `gdsfactory-6.97.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py` & `gdsfactory-6.97.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/__init__.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/coupler.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/find_mode_dispersion.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/find_mode_dispersion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/find_modes.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/find_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/find_modes_cross_section.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/find_modes_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/find_neff_vs_width.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/find_neff_vs_width.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/get_mode_solver_rib.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/get_mode_solver_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/neff_convergence_test.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/neff_convergence_test.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/overlap.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/overlap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_find_modes.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/tests/test_find_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/types.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/types.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/modes/waveguide.py` & `gdsfactory-6.97.0/gdsfactory/simulation/modes/waveguide.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/__init__.py` & `gdsfactory-6.97.0/gdsfactory/simulation/photonic_circuit_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/coupler.py` & `gdsfactory-6.97.0/gdsfactory/simulation/photonic_circuit_models/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/mzi.py` & `gdsfactory-6.97.0/gdsfactory/simulation/photonic_circuit_models/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/ring.py` & `gdsfactory-6.97.0/gdsfactory/simulation/photonic_circuit_models/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/plot.py` & `gdsfactory-6.97.0/gdsfactory/simulation/plot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/plot_csv.py` & `gdsfactory-6.97.0/gdsfactory/simulation/plot_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/port_symmetries.py` & `gdsfactory-6.97.0/gdsfactory/simulation/port_symmetries.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/process/diffusion.py` & `gdsfactory-6.97.0/gdsfactory/simulation/process/diffusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/process/implant_tables.py` & `gdsfactory-6.97.0/gdsfactory/simulation/process/implant_tables.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/process/pysrim.py` & `gdsfactory-6.97.0/gdsfactory/simulation/process/pysrim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/process/silicon.py` & `gdsfactory-6.97.0/gdsfactory/simulation/process/silicon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/process/skew/boron_si_skew.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/process/skew/boron_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv` & `gdsfactory-6.97.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sax/build_model.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sax/build_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sax/femwell_waveguide_model.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sax/femwell_waveguide_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sax/interpolators.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sax/interpolators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sax/meep_FDTD_model.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sax/meep_FDTD_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sax/meow_eme_model.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sax/meow_eme_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sax/mlp.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sax/mlp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sax/models.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sax/models.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sax/parameter.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sax/parameter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sax/plot_model.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sax/plot_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sax/read.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sax/read.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sax/tests/test_mzi.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sax/tests/test_mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sax/tests/test_parameters.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sax/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/__init__.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/add_gc.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/add_gc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/circuit.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/__init__.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/bend_circular.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/bend_euler.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_ring.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/gc.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/gc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mmi1x2.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mmi2x2.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mzi.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mzi_siepic.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/mzi_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_double.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_single.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/ring_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/straight.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/components/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/get_transmission.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/get_transmission.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/model_from_sparameters.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/model_from_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/plot_circuit.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/plot_circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/plot_model.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/plot_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_circuit.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components.py` & `gdsfactory-6.97.0/gdsfactory/simulation/simphony/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sipann/bend_circular.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sipann/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sipann/bend_euler.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sipann/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sipann/coupler.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sipann/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sipann/coupler_ring.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sipann/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/sipann/straight.py` & `gdsfactory-6.97.0/gdsfactory/simulation/sipann/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/simulation/thermal/heater.py` & `gdsfactory-6.97.0/gdsfactory/simulation/thermal/heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/snap.py` & `gdsfactory-6.97.0/gdsfactory/snap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/symbols.py` & `gdsfactory-6.97.0/gdsfactory/symbols.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/technology/__init__.py` & `gdsfactory-6.97.0/gdsfactory/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/technology/klayout_tech.py` & `gdsfactory-6.97.0/gdsfactory/technology/klayout_tech.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/technology/layer_map.py` & `gdsfactory-6.97.0/gdsfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/technology/layer_stack.py` & `gdsfactory-6.97.0/gdsfactory/technology/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/technology/layer_views.py` & `gdsfactory-6.97.0/gdsfactory/technology/layer_views.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/technology/simulation_settings.py` & `gdsfactory-6.97.0/gdsfactory/technology/simulation_settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/types.py` & `gdsfactory-6.97.0/gdsfactory/types.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/typings.py` & `gdsfactory-6.97.0/gdsfactory/typings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/utils/async_utils.py` & `gdsfactory-6.97.0/gdsfactory/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/utils/file_utils.py` & `gdsfactory-6.97.0/gdsfactory/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/utils/xml_utils.py` & `gdsfactory-6.97.0/gdsfactory/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/utils/yaml_utils.py` & `gdsfactory-6.97.0/gdsfactory/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/watch.py` & `gdsfactory-6.97.0/gdsfactory/watch.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/widgets/layout_viewer.py` & `gdsfactory-6.97.0/gdsfactory/widgets/layout_viewer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/gdsfactory/write_cells.py` & `gdsfactory-6.97.0/gdsfactory/write_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.96.0/pyproject.toml` & `gdsfactory-6.97.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: OS Independent",
 ]
-version = "6.96.0"
+version = "6.97.0"
 authors = [
 {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 keywords = ["eda", "photonics", "python"]
 license = {file = "LICENSE"}
 dependencies = [
   "click",
```

### Comparing `gdsfactory-6.96.0/PKG-INFO` & `gdsfactory-6.97.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdsfactory
-Version: 6.96.0
+Version: 6.97.0
 Summary: python library to generate GDS layouts
 Keywords: eda,photonics,python
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -114,15 +114,15 @@
 Provides-Extra: full
 Provides-Extra: gmsh
 Provides-Extra: meow
 Provides-Extra: ray
 Provides-Extra: sax
 Provides-Extra: tidy3d
 
-# gdsfactory 6.96.0
+# gdsfactory 6.97.0
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![issues](https://img.shields.io/github/issues/gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/issues)
```

