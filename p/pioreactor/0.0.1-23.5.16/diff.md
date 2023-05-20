# Comparing `tmp/pioreactor-0.0.1-py3.8.egg` & `tmp/pioreactor-23.5.16-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,89 @@
-Zip file size: 1023 bytes, number of entries: 6
--rw-r--r--  2.0 unx      191 b- defN 21-Apr-22 20:00 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      191 b- defN 21-Apr-22 20:00 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 21-Apr-22 20:00 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       62 b- defN 21-Apr-22 20:00 EGG-INFO/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 21-Apr-22 20:00 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 21-Apr-22 20:00 EGG-INFO/zip-safe
-6 files, 447 bytes uncompressed, 285 bytes compressed:  36.2%
+Zip file size: 187063 bytes, number of entries: 87
+-rw-r--r--  2.0 unx      117 b- defN 23-Apr-14 19:03 pioreactor/__init__.py
+-rw-r--r--  2.0 unx     6488 b- defN 23-May-20 00:10 pioreactor/config.py
+-rw-r--r--  2.0 unx      265 b- defN 23-May-16 18:44 pioreactor/error_codes.py
+-rw-r--r--  2.0 unx      443 b- defN 23-Mar-03 15:51 pioreactor/exc.py
+-rw-r--r--  2.0 unx     3105 b- defN 23-May-16 18:44 pioreactor/hardware.py
+-rw-r--r--  2.0 unx     6614 b- defN 23-Feb-25 16:12 pioreactor/logging.py
+-rw-r--r--  2.0 unx    14871 b- defN 23-Apr-04 14:54 pioreactor/mureq.py
+-rw-r--r--  2.0 unx    12957 b- defN 23-Apr-28 13:20 pioreactor/pubsub.py
+-rw-r--r--  2.0 unx     6400 b- defN 23-May-16 18:44 pioreactor/structs.py
+-rw-r--r--  2.0 unx     2724 b- defN 23-May-16 18:44 pioreactor/types.py
+-rw-r--r--  2.0 unx     2153 b- defN 23-May-16 18:44 pioreactor/version.py
+-rw-r--r--  2.0 unx     3654 b- defN 23-May-16 18:44 pioreactor/whoami.py
+-rw-r--r--  2.0 unx      548 b- defN 23-May-16 18:44 pioreactor/actions/__init__.py
+-rw-r--r--  2.0 unx     8895 b- defN 23-May-20 00:10 pioreactor/actions/led_intensity.py
+-rw-r--r--  2.0 unx     7755 b- defN 23-Apr-04 14:54 pioreactor/actions/od_blank.py
+-rw-r--r--  2.0 unx    20343 b- defN 23-May-16 18:44 pioreactor/actions/od_calibration.py
+-rw-r--r--  2.0 unx    16524 b- defN 23-Apr-28 13:20 pioreactor/actions/pump.py
+-rw-r--r--  2.0 unx    21362 b- defN 23-May-16 18:44 pioreactor/actions/pump_calibration.py
+-rw-r--r--  2.0 unx    16662 b- defN 23-Apr-28 13:20 pioreactor/actions/self_test.py
+-rw-r--r--  2.0 unx     5175 b- defN 23-Apr-14 19:03 pioreactor/actions/stirring_calibration.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Nov-16 00:22 pioreactor/actions/leader/__init__.py
+-rw-r--r--  2.0 unx     4744 b- defN 23-May-16 18:44 pioreactor/actions/leader/backup_database.py
+-rw-r--r--  2.0 unx     5593 b- defN 23-May-16 18:44 pioreactor/actions/leader/execute_experiment_profile.py
+-rw-r--r--  2.0 unx     6426 b- defN 23-Apr-28 13:20 pioreactor/actions/leader/export_experiment_data.py
+-rw-r--r--  2.0 unx      445 b- defN 23-Mar-01 19:03 pioreactor/automations/__init__.py
+-rw-r--r--  2.0 unx      496 b- defN 23-Mar-01 19:03 pioreactor/automations/dosing/__init__.py
+-rw-r--r--  2.0 unx    28029 b- defN 23-May-16 18:44 pioreactor/automations/dosing/base.py
+-rw-r--r--  2.0 unx     1404 b- defN 23-Feb-06 16:41 pioreactor/automations/dosing/chemostat.py
+-rw-r--r--  2.0 unx     2472 b- defN 22-Apr-19 23:22 pioreactor/automations/dosing/continuous_cycle.py
+-rw-r--r--  2.0 unx     1194 b- defN 23-Mar-21 18:37 pioreactor/automations/dosing/fed_batch.py
+-rw-r--r--  2.0 unx     2724 b- defN 23-Jan-05 15:58 pioreactor/automations/dosing/morbidostat.py
+-rw-r--r--  2.0 unx     4379 b- defN 23-Mar-01 19:03 pioreactor/automations/dosing/pid_morbidostat.py
+-rw-r--r--  2.0 unx      468 b- defN 23-Jan-13 16:17 pioreactor/automations/dosing/silent.py
+-rw-r--r--  2.0 unx     2252 b- defN 23-Feb-06 16:41 pioreactor/automations/dosing/turbidostat.py
+-rw-r--r--  2.0 unx      510 b- defN 22-Apr-19 23:22 pioreactor/automations/events/__init__.py
+-rw-r--r--  2.0 unx      473 b- defN 23-Apr-14 19:03 pioreactor/automations/led/__init__.py
+-rw-r--r--  2.0 unx    11851 b- defN 23-Mar-09 15:25 pioreactor/automations/led/base.py
+-rw-r--r--  2.0 unx     3136 b- defN 23-Mar-01 19:03 pioreactor/automations/led/light_dark_cycle.py
+-rw-r--r--  2.0 unx      205 b- defN 23-Mar-01 19:03 pioreactor/automations/temperature/__init__.py
+-rw-r--r--  2.0 unx     9368 b- defN 23-Mar-09 15:25 pioreactor/automations/temperature/base.py
+-rw-r--r--  2.0 unx      674 b- defN 23-Apr-14 19:03 pioreactor/automations/temperature/constant_duty_cycle.py
+-rw-r--r--  2.0 unx      540 b- defN 22-Sep-07 19:29 pioreactor/automations/temperature/only_record_ambient_temperature.py
+-rw-r--r--  2.0 unx      517 b- defN 23-Apr-14 19:03 pioreactor/automations/temperature/only_record_temperature.py
+-rw-r--r--  2.0 unx      471 b- defN 22-Apr-19 23:22 pioreactor/automations/temperature/silent.py
+-rw-r--r--  2.0 unx     3005 b- defN 22-Jul-29 15:20 pioreactor/automations/temperature/stable.py
+-rw-r--r--  2.0 unx     4139 b- defN 23-Mar-01 19:03 pioreactor/automations/temperature/thermostat.py
+-rw-r--r--  2.0 unx      715 b- defN 23-Mar-01 19:03 pioreactor/background_jobs/__init__.py
+-rw-r--r--  2.0 unx    42800 b- defN 23-May-12 02:11 pioreactor/background_jobs/base.py
+-rw-r--r--  2.0 unx     6854 b- defN 23-Mar-09 15:25 pioreactor/background_jobs/dosing_control.py
+-rw-r--r--  2.0 unx    20167 b- defN 23-Apr-04 14:54 pioreactor/background_jobs/growth_rate_calculating.py
+-rw-r--r--  2.0 unx     5488 b- defN 23-Mar-09 15:25 pioreactor/background_jobs/led_control.py
+-rw-r--r--  2.0 unx    24261 b- defN 23-May-16 18:44 pioreactor/background_jobs/monitor.py
+-rw-r--r--  2.0 unx    46776 b- defN 23-May-20 00:10 pioreactor/background_jobs/od_reading.py
+-rw-r--r--  2.0 unx    17440 b- defN 23-Apr-28 13:20 pioreactor/background_jobs/stirring.py
+-rw-r--r--  2.0 unx    24607 b- defN 23-May-20 00:10 pioreactor/background_jobs/temperature_control.py
+-rw-r--r--  2.0 unx      605 b- defN 23-Apr-14 19:03 pioreactor/background_jobs/leader/__init__.py
+-rw-r--r--  2.0 unx    16280 b- defN 23-May-16 18:44 pioreactor/background_jobs/leader/mqtt_to_db_streaming.py
+-rw-r--r--  2.0 unx     3829 b- defN 23-Apr-14 19:03 pioreactor/background_jobs/leader/watchdog.py
+-rw-r--r--  2.0 unx      609 b- defN 22-Nov-10 16:45 pioreactor/background_jobs/subjobs/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Jan-26 16:52 pioreactor/cli/__init__.py
+-rw-r--r--  2.0 unx    29658 b- defN 23-May-16 18:44 pioreactor/cli/pio.py
+-rw-r--r--  2.0 unx    21532 b- defN 23-Apr-28 13:20 pioreactor/cli/pios.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-16 18:44 pioreactor/experiment_profiles/__init__.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-16 18:44 pioreactor/experiment_profiles/profile_struct.py
+-rw-r--r--  2.0 unx     3517 b- defN 23-Apr-14 19:03 pioreactor/plugin_management/__init__.py
+-rw-r--r--  2.0 unx     1316 b- defN 23-Jan-24 17:34 pioreactor/plugin_management/install_plugin.py
+-rw-r--r--  2.0 unx     1086 b- defN 22-Nov-02 15:50 pioreactor/plugin_management/list_plugins.py
+-rw-r--r--  2.0 unx     1605 b- defN 23-Mar-21 18:37 pioreactor/plugin_management/uninstall_plugin.py
+-rw-r--r--  2.0 unx      792 b- defN 23-Mar-21 18:37 pioreactor/plugin_management/utils.py
+-rw-r--r--  2.0 unx    10951 b- defN 23-May-16 18:44 pioreactor/utils/__init__.py
+-rw-r--r--  2.0 unx     4096 b- defN 23-May-16 15:26 pioreactor/utils/adcs.py
+-rw-r--r--  2.0 unx     1930 b- defN 23-May-16 18:44 pioreactor/utils/dacs.py
+-rw-r--r--  2.0 unx      976 b- defN 23-Mar-01 19:03 pioreactor/utils/gpio_helpers.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Apr-14 19:03 pioreactor/utils/math_helpers.py
+-rw-r--r--  2.0 unx     4122 b- defN 23-Apr-14 19:03 pioreactor/utils/mock.py
+-rw-r--r--  2.0 unx     3692 b- defN 23-Apr-28 13:20 pioreactor/utils/networking.py
+-rw-r--r--  2.0 unx     7559 b- defN 23-Apr-14 19:03 pioreactor/utils/pwm.py
+-rw-r--r--  2.0 unx     3393 b- defN 23-Apr-28 13:20 pioreactor/utils/rpi_bad_power.py
+-rw-r--r--  2.0 unx     7749 b- defN 23-May-16 18:44 pioreactor/utils/sqlite_worker.py
+-rw-r--r--  2.0 unx    15186 b- defN 23-Apr-14 19:03 pioreactor/utils/streaming_calculations.py
+-rw-r--r--  2.0 unx     5614 b- defN 23-Apr-28 13:20 pioreactor/utils/timing.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-May-20 00:10 pioreactor-23.5.16.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3436 b- defN 23-May-20 00:10 pioreactor-23.5.16.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-20 00:10 pioreactor-23.5.16.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 23-May-20 00:10 pioreactor-23.5.16.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-May-20 00:10 pioreactor-23.5.16.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8103 b- defN 23-May-20 00:10 pioreactor-23.5.16.dist-info/RECORD
+87 files, 604438 bytes uncompressed, 174003 bytes compressed:  71.2%
```

## zipnote «TEMP»/diffoscope_4wh01xq1_/tmp8um_dg9b_.zip

```diff
@@ -1,19 +1,262 @@
-Filename: EGG-INFO/PKG-INFO
+Filename: pioreactor/__init__.py
 Comment: 
 
-Filename: EGG-INFO/SOURCES.txt
+Filename: pioreactor/config.py
 Comment: 
 
-Filename: EGG-INFO/dependency_links.txt
+Filename: pioreactor/error_codes.py
 Comment: 
 
-Filename: EGG-INFO/entry_points.txt
+Filename: pioreactor/exc.py
 Comment: 
 
-Filename: EGG-INFO/top_level.txt
+Filename: pioreactor/hardware.py
 Comment: 
 
-Filename: EGG-INFO/zip-safe
+Filename: pioreactor/logging.py
+Comment: 
+
+Filename: pioreactor/mureq.py
+Comment: 
+
+Filename: pioreactor/pubsub.py
+Comment: 
+
+Filename: pioreactor/structs.py
+Comment: 
+
+Filename: pioreactor/types.py
+Comment: 
+
+Filename: pioreactor/version.py
+Comment: 
+
+Filename: pioreactor/whoami.py
+Comment: 
+
+Filename: pioreactor/actions/__init__.py
+Comment: 
+
+Filename: pioreactor/actions/led_intensity.py
+Comment: 
+
+Filename: pioreactor/actions/od_blank.py
+Comment: 
+
+Filename: pioreactor/actions/od_calibration.py
+Comment: 
+
+Filename: pioreactor/actions/pump.py
+Comment: 
+
+Filename: pioreactor/actions/pump_calibration.py
+Comment: 
+
+Filename: pioreactor/actions/self_test.py
+Comment: 
+
+Filename: pioreactor/actions/stirring_calibration.py
+Comment: 
+
+Filename: pioreactor/actions/leader/__init__.py
+Comment: 
+
+Filename: pioreactor/actions/leader/backup_database.py
+Comment: 
+
+Filename: pioreactor/actions/leader/execute_experiment_profile.py
+Comment: 
+
+Filename: pioreactor/actions/leader/export_experiment_data.py
+Comment: 
+
+Filename: pioreactor/automations/__init__.py
+Comment: 
+
+Filename: pioreactor/automations/dosing/__init__.py
+Comment: 
+
+Filename: pioreactor/automations/dosing/base.py
+Comment: 
+
+Filename: pioreactor/automations/dosing/chemostat.py
+Comment: 
+
+Filename: pioreactor/automations/dosing/continuous_cycle.py
+Comment: 
+
+Filename: pioreactor/automations/dosing/fed_batch.py
+Comment: 
+
+Filename: pioreactor/automations/dosing/morbidostat.py
+Comment: 
+
+Filename: pioreactor/automations/dosing/pid_morbidostat.py
+Comment: 
+
+Filename: pioreactor/automations/dosing/silent.py
+Comment: 
+
+Filename: pioreactor/automations/dosing/turbidostat.py
+Comment: 
+
+Filename: pioreactor/automations/events/__init__.py
+Comment: 
+
+Filename: pioreactor/automations/led/__init__.py
+Comment: 
+
+Filename: pioreactor/automations/led/base.py
+Comment: 
+
+Filename: pioreactor/automations/led/light_dark_cycle.py
+Comment: 
+
+Filename: pioreactor/automations/temperature/__init__.py
+Comment: 
+
+Filename: pioreactor/automations/temperature/base.py
+Comment: 
+
+Filename: pioreactor/automations/temperature/constant_duty_cycle.py
+Comment: 
+
+Filename: pioreactor/automations/temperature/only_record_ambient_temperature.py
+Comment: 
+
+Filename: pioreactor/automations/temperature/only_record_temperature.py
+Comment: 
+
+Filename: pioreactor/automations/temperature/silent.py
+Comment: 
+
+Filename: pioreactor/automations/temperature/stable.py
+Comment: 
+
+Filename: pioreactor/automations/temperature/thermostat.py
+Comment: 
+
+Filename: pioreactor/background_jobs/__init__.py
+Comment: 
+
+Filename: pioreactor/background_jobs/base.py
+Comment: 
+
+Filename: pioreactor/background_jobs/dosing_control.py
+Comment: 
+
+Filename: pioreactor/background_jobs/growth_rate_calculating.py
+Comment: 
+
+Filename: pioreactor/background_jobs/led_control.py
+Comment: 
+
+Filename: pioreactor/background_jobs/monitor.py
+Comment: 
+
+Filename: pioreactor/background_jobs/od_reading.py
+Comment: 
+
+Filename: pioreactor/background_jobs/stirring.py
+Comment: 
+
+Filename: pioreactor/background_jobs/temperature_control.py
+Comment: 
+
+Filename: pioreactor/background_jobs/leader/__init__.py
+Comment: 
+
+Filename: pioreactor/background_jobs/leader/mqtt_to_db_streaming.py
+Comment: 
+
+Filename: pioreactor/background_jobs/leader/watchdog.py
+Comment: 
+
+Filename: pioreactor/background_jobs/subjobs/__init__.py
+Comment: 
+
+Filename: pioreactor/cli/__init__.py
+Comment: 
+
+Filename: pioreactor/cli/pio.py
+Comment: 
+
+Filename: pioreactor/cli/pios.py
+Comment: 
+
+Filename: pioreactor/experiment_profiles/__init__.py
+Comment: 
+
+Filename: pioreactor/experiment_profiles/profile_struct.py
+Comment: 
+
+Filename: pioreactor/plugin_management/__init__.py
+Comment: 
+
+Filename: pioreactor/plugin_management/install_plugin.py
+Comment: 
+
+Filename: pioreactor/plugin_management/list_plugins.py
+Comment: 
+
+Filename: pioreactor/plugin_management/uninstall_plugin.py
+Comment: 
+
+Filename: pioreactor/plugin_management/utils.py
+Comment: 
+
+Filename: pioreactor/utils/__init__.py
+Comment: 
+
+Filename: pioreactor/utils/adcs.py
+Comment: 
+
+Filename: pioreactor/utils/dacs.py
+Comment: 
+
+Filename: pioreactor/utils/gpio_helpers.py
+Comment: 
+
+Filename: pioreactor/utils/math_helpers.py
+Comment: 
+
+Filename: pioreactor/utils/mock.py
+Comment: 
+
+Filename: pioreactor/utils/networking.py
+Comment: 
+
+Filename: pioreactor/utils/pwm.py
+Comment: 
+
+Filename: pioreactor/utils/rpi_bad_power.py
+Comment: 
+
+Filename: pioreactor/utils/sqlite_worker.py
+Comment: 
+
+Filename: pioreactor/utils/streaming_calculations.py
+Comment: 
+
+Filename: pioreactor/utils/timing.py
+Comment: 
+
+Filename: pioreactor-23.5.16.dist-info/LICENSE
+Comment: 
+
+Filename: pioreactor-23.5.16.dist-info/METADATA
+Comment: 
+
+Filename: pioreactor-23.5.16.dist-info/WHEEL
+Comment: 
+
+Filename: pioreactor-23.5.16.dist-info/entry_points.txt
+Comment: 
+
+Filename: pioreactor-23.5.16.dist-info/top_level.txt
+Comment: 
+
+Filename: pioreactor-23.5.16.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

