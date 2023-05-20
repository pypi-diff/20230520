# Comparing `tmp/pioreactor_relay_plugin-0.3.0-py3-none-any.whl.zip` & `tmp/pioreactor_relay_plugin-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,12 @@
-Zip file size: 5664 bytes, number of entries: 11
+Zip file size: 5163 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       53 b- defN 22-Aug-26 19:03 pioreactor_relay_plugin/__init__.py
--rw-r--r--  2.0 unx      104 b- defN 22-Dec-23 20:09 pioreactor_relay_plugin/additional_config.ini
--rw-r--r--  2.0 unx     2699 b- defN 22-Dec-23 20:09 pioreactor_relay_plugin/relay.py
--rw-r--r--  2.0 unx      495 b- defN 22-Nov-02 15:07 pioreactor_relay_plugin/ui/contrib/jobs/13_relay.yaml
--rw-r--r--  2.0 unx      528 b- defN 22-Dec-23 19:41 pioreactor_relay_plugin/ui/contrib/jobs/relay.yaml
--rw-r--r--  2.0 unx     1061 b- defN 22-Dec-23 20:10 pioreactor_relay_plugin-0.3.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1642 b- defN 22-Dec-23 20:10 pioreactor_relay_plugin-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-23 20:10 pioreactor_relay_plugin-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 22-Dec-23 20:10 pioreactor_relay_plugin-0.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       24 b- defN 22-Dec-23 20:10 pioreactor_relay_plugin-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1076 b- defN 22-Dec-23 20:10 pioreactor_relay_plugin-0.3.0.dist-info/RECORD
-11 files, 7845 bytes uncompressed, 3778 bytes compressed:  51.8%
+-rw-r--r--  2.0 unx      104 b- defN 23-Jan-19 01:10 pioreactor_relay_plugin/additional_config.ini
+-rw-r--r--  2.0 unx     2866 b- defN 23-May-20 01:50 pioreactor_relay_plugin/relay.py
+-rw-r--r--  2.0 unx      406 b- defN 23-Jan-26 21:04 pioreactor_relay_plugin/ui/contrib/jobs/relay.yaml
+-rw-r--r--  2.0 unx     1061 b- defN 23-May-20 01:54 pioreactor_relay_plugin-0.3.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1642 b- defN 23-May-20 01:54 pioreactor_relay_plugin-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-20 01:54 pioreactor_relay_plugin-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 23-May-20 01:54 pioreactor_relay_plugin-0.3.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 23-May-20 01:54 pioreactor_relay_plugin-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      967 b- defN 23-May-20 01:54 pioreactor_relay_plugin-0.3.1.dist-info/RECORD
+10 files, 7286 bytes uncompressed, 3459 bytes compressed:  52.5%
```

## zipnote {}

```diff
@@ -3,32 +3,29 @@
 
 Filename: pioreactor_relay_plugin/additional_config.ini
 Comment: 
 
 Filename: pioreactor_relay_plugin/relay.py
 Comment: 
 
-Filename: pioreactor_relay_plugin/ui/contrib/jobs/13_relay.yaml
-Comment: 
-
 Filename: pioreactor_relay_plugin/ui/contrib/jobs/relay.yaml
 Comment: 
 
-Filename: pioreactor_relay_plugin-0.3.0.dist-info/LICENSE.txt
+Filename: pioreactor_relay_plugin-0.3.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pioreactor_relay_plugin-0.3.0.dist-info/METADATA
+Filename: pioreactor_relay_plugin-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: pioreactor_relay_plugin-0.3.0.dist-info/WHEEL
+Filename: pioreactor_relay_plugin-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: pioreactor_relay_plugin-0.3.0.dist-info/entry_points.txt
+Filename: pioreactor_relay_plugin-0.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pioreactor_relay_plugin-0.3.0.dist-info/top_level.txt
+Filename: pioreactor_relay_plugin-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pioreactor_relay_plugin-0.3.0.dist-info/RECORD
+Filename: pioreactor_relay_plugin-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pioreactor_relay_plugin/relay.py

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
+import click
 from pioreactor.background_jobs.base import BackgroundJobWithDodgingContrib
 from pioreactor.config import config
 from pioreactor.hardware import PWM_TO_PIN
 from pioreactor.utils.pwm import PWM
 from pioreactor.whoami import get_latest_experiment_name
 from pioreactor.whoami import get_unit_name
 
@@ -17,69 +18,71 @@
 
     job_name = "relay"
 
     def __init__(self, unit, experiment, start_on=True):
         super().__init__(unit=unit, experiment=experiment, plugin_name="relay")
         if start_on:
             self.duty_cycle = 100
-            self.relay_on = True
+            self.is_relay_on = True
         else:
             self.duty_cycle = 0
-            self.relay_on = False
+            self.is_relay_on = False
 
         self.pwm_pin = PWM_TO_PIN[config.get("PWM_reverse", "relay")]
         # looks at config.ini/configuration on UI to match
         # changed PWM channel 2 to "relay" on leader
         # whatevers connected to channel 2 will turn on/off
 
         self.pwm = PWM(
             self.pwm_pin, hz=10, unit=unit, experiment=experiment
         )  # since we also go 100% high or 0% low, we don't need hz.
         self.pwm.lock()
 
+    def on_init_to_ready(self):
+        super().on_init_to_ready()
+        self.logger.debug(f"Starting relay {'ON' if self.is_relay_on else 'OFF'}.")
+        self.pwm.start(self.duty_cycle)
+
     def set_relay_on(self, value: bool):
-        if value == self.relay_on:
+        if value == self.is_relay_on:
             return
+
         if value:
-            self.set_duty_cycle(100)
-            self.relay_on = True
+            self._set_duty_cycle(100)
+            self.is_relay_on = True
         else:
-            self.set_duty_cycle(0)
-            self.relay_on = False
+            self._set_duty_cycle(0)
+            self.is_relay_on = False
 
-    def set_duty_cycle(self, new_duty_cycle: float):
+    def _set_duty_cycle(self, new_duty_cycle: float):
         self.duty_cycle = new_duty_cycle
 
         if hasattr(self, "pwm"):
             self.pwm.change_duty_cycle(self.duty_cycle)
 
-    def on_init_to_ready(self):
-        self.logger.debug(f"Starting relay {'ON' if self.relay_on else 'OFF'}.")
-        self.pwm.start(self.duty_cycle)
-
     def on_ready_to_sleeping(self):
+        super().on_ready_to_sleeping()
         self.set_relay_on(False)
 
     def on_sleeping_to_ready(self):
+        super().on_sleeping_to_ready()
         self.set_relay_on(True)
 
     def on_disconnected(self):
+        super().on_disconnected()
         self.set_relay_on(False)
         self.pwm.cleanup()
 
     def action_to_do_before_od_reading(self):
         self.set_relay_on(False)
 
     def action_to_do_after_od_reading(self):
         self.set_relay_on(True)
 
 
-import click
-
-
 @click.command(name="relay")
 @click.option(
     "-s",
     "--start-on",
     default=config.getint("relay.config", "start_on", fallback=1),
     type=click.BOOL,
 )
```

## pioreactor_relay_plugin/ui/contrib/jobs/relay.yaml

```diff
@@ -1,14 +1,14 @@
 ---
-display_name: Relay # human readable name
+display_name: Relay # human readable name, can be overwritten
 job_name: relay
-display: true  # true to display on the /Pioreactors card
+display: true
 source: pioreactor_relay_plugin
 description: Turn your hardware add-on (switch, pump, valve) on or off.
 published_settings:
-  - key: relay_on   # as defined in Python
+  - key: relay_on
     unit:
-    label: Relay # human readable name
+    label: Relay on # human readable name
     description: Switch the power supply to the relay on/off.
-    type: boolean  # one of numeric, boolean, text
+    type: boolean
     default: null
-    display: true # true to display on the /Pioreactors card
+    display: true
```

## Comparing `pioreactor_relay_plugin-0.3.0.dist-info/LICENSE.txt` & `pioreactor_relay_plugin-0.3.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pioreactor_relay_plugin-0.3.0.dist-info/METADATA` & `pioreactor_relay_plugin-0.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pioreactor-relay-plugin
-Version: 0.3.0
+Version: 0.3.1
 Summary: Turn the PWM channels into a simple on/off relay for additional hardware.
 Home-page: https://github.com/CamDavidsonPilon/pioreactor-relay-plugin
 Author: Kelly Tran, Cam Davidson-Pilon
 Author-email: cam@pioreactor.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

## Comparing `pioreactor_relay_plugin-0.3.0.dist-info/RECORD` & `pioreactor_relay_plugin-0.3.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 pioreactor_relay_plugin/__init__.py,sha256=nzaA-lKGw3qkVWG-sUeDh3T3kL9Qn6uk055B38nfLKI,53
 pioreactor_relay_plugin/additional_config.ini,sha256=2NDiRYnY_lF3_dB0ZwD7ExMO23toseu-cKrNjguRFWg,104
-pioreactor_relay_plugin/relay.py,sha256=V0XXxjxDcFDWkTq79aW5nwVeg5BYKA_tKWdaKSZsyRA,2699
-pioreactor_relay_plugin/ui/contrib/jobs/13_relay.yaml,sha256=RkBoz5TV83RKd8R-GJhAhLB9c9C5KJuKx2lkyr41Bao,495
-pioreactor_relay_plugin/ui/contrib/jobs/relay.yaml,sha256=5KnDw-0_m7ZzXBYDuHnTOy0UoCShJw-iwmiaEqp6oLU,528
-pioreactor_relay_plugin-0.3.0.dist-info/LICENSE.txt,sha256=Ln7xVAOPmdFrbD7I-uwGZgbLrRdLxzhv4hPqZwVLzOM,1061
-pioreactor_relay_plugin-0.3.0.dist-info/METADATA,sha256=RFQrpdh1vTD3orvTFKhDt4O9f-n9LTsXJ2OQE9xumn8,1642
-pioreactor_relay_plugin-0.3.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pioreactor_relay_plugin-0.3.0.dist-info/entry_points.txt,sha256=eoInJCHltj2GDoz1keQngjmowbJ8e1OHV6b8si2G5x4,71
-pioreactor_relay_plugin-0.3.0.dist-info/top_level.txt,sha256=ycPmfjvugfCgM68hl_LSwxvU5fKcmHeDoY0ZKS1HKNM,24
-pioreactor_relay_plugin-0.3.0.dist-info/RECORD,,
+pioreactor_relay_plugin/relay.py,sha256=8QS0XyXdSOYFCXtqp6jyO2Sjmug7CxniyH3TQG2ACWc,2866
+pioreactor_relay_plugin/ui/contrib/jobs/relay.yaml,sha256=tZOi1ODlPtBMYBLBFdXUfcARi1qq9xdrLVcZfGYx6Bg,406
+pioreactor_relay_plugin-0.3.1.dist-info/LICENSE.txt,sha256=Ln7xVAOPmdFrbD7I-uwGZgbLrRdLxzhv4hPqZwVLzOM,1061
+pioreactor_relay_plugin-0.3.1.dist-info/METADATA,sha256=GXHwTSzv_6nIajMfIYYIfvhtfYhndPnpy0YzlSbb4xU,1642
+pioreactor_relay_plugin-0.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pioreactor_relay_plugin-0.3.1.dist-info/entry_points.txt,sha256=eoInJCHltj2GDoz1keQngjmowbJ8e1OHV6b8si2G5x4,71
+pioreactor_relay_plugin-0.3.1.dist-info/top_level.txt,sha256=ycPmfjvugfCgM68hl_LSwxvU5fKcmHeDoY0ZKS1HKNM,24
+pioreactor_relay_plugin-0.3.1.dist-info/RECORD,,
```

