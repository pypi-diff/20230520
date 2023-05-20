# Comparing `tmp/eptlsoot-0.0.8-cp39-cp39-win_amd64.whl.zip` & `tmp/eptlsoot-0.0.9-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 1713341 bytes, number of entries: 20
+Zip file size: 1723964 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat      513 b- defN 23-Apr-27 02:29 eptlsoot/__init__.py
 -rw-rw-rw-  2.0 fat  1465856 b- defN 23-Apr-05 21:26 eptlsoot/_eptlsoot.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat     6093 b- defN 23-Apr-05 21:43 eptlsoot/cpfr.py
 -rw-rw-rw-  2.0 fat      679 b- defN 23-Apr-05 21:38 eptlsoot/eptlsoot.py
 -rw-rw-rw-  2.0 fat      644 b- defN 23-Apr-05 21:43 eptlsoot/psr.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-05 04:38 eptlsoot/apps/__init__.py
 -rw-rw-rw-  2.0 fat      882 b- defN 23-Apr-25 22:15 eptlsoot/apps/flame.py
--rw-rw-rw-  2.0 fat     1843 b- defN 23-Apr-13 14:11 eptlsoot/apps/pahgrowth.py
--rw-rw-rw-  2.0 fat     9348 b- defN 23-May-17 02:00 eptlsoot/apps/reactors.py
+-rw-rw-rw-  2.0 fat     2059 b- defN 23-May-19 22:36 eptlsoot/apps/pahgrowth.py
+-rw-rw-rw-  2.0 fat     9340 b- defN 23-May-18 20:56 eptlsoot/apps/reactors.py
 -rw-rw-rw-  2.0 fat      265 b- defN 23-Apr-05 04:46 eptlsoot/apps/solutionarray.py
 -rw-rw-rw-  2.0 fat     3447 b- defN 23-May-17 00:40 eptlsoot/apps/sootgas.py
 -rw-rw-rw-  2.0 fat      950 b- defN 23-Apr-05 21:55 eptlsoot/apps/sootmodels.py
 -rw-rw-rw-  2.0 fat     5993 b- defN 23-Apr-08 23:53 eptlsoot/apps/sootwrappers.py
 -rw-rw-rw-  2.0 fat      239 b- defN 23-Apr-05 21:52 eptlsoot/apps/surfacereactions.py
--rw-rw-rw-  2.0 fat  1717248 b- defN 23-May-17 14:49 eptlsoot/lib/_eptlsoot.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  1755136 b- defN 23-May-19 22:46 eptlsoot/lib/_eptlsoot.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat  1468928 b- defN 23-Apr-05 21:11 eptlsoot2/_eptlsoot2.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      734 b- defN 23-May-17 14:49 eptlsoot-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-17 14:49 eptlsoot-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-17 14:49 eptlsoot-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1641 b- defN 23-May-17 14:49 eptlsoot-0.0.8.dist-info/RECORD
-20 files, 4685412 bytes uncompressed, 1710677 bytes compressed:  63.5%
+-rw-rw-rw-  2.0 fat      734 b- defN 23-May-19 22:46 eptlsoot-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-19 22:46 eptlsoot-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-19 22:46 eptlsoot-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1641 b- defN 23-May-19 22:46 eptlsoot-0.0.9.dist-info/RECORD
+20 files, 4723508 bytes uncompressed, 1721300 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: eptlsoot/lib/_eptlsoot.cp39-win_amd64.pyd
 Comment: 
 
 Filename: eptlsoot2/_eptlsoot2.cp39-win_amd64.pyd
 Comment: 
 
-Filename: eptlsoot-0.0.8.dist-info/METADATA
+Filename: eptlsoot-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: eptlsoot-0.0.8.dist-info/WHEEL
+Filename: eptlsoot-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: eptlsoot-0.0.8.dist-info/top_level.txt
+Filename: eptlsoot-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: eptlsoot-0.0.8.dist-info/RECORD
+Filename: eptlsoot-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## eptlsoot/apps/pahgrowth.py

```diff
@@ -1,8 +1,8 @@
-from ..lib._eptlsoot import CReactDim, CDimerCoal, CDimerCoalMod, CCrossLink, CCrossLinkMod
+from ..lib._eptlsoot import CReactDim, CDimerCoal, CDimerCoalMod, CCrossLink, CCrossLinkMod, CCrossLinkMerge
 
 class PAHGrowthAbstract:
     def __init__(self, soot_wrapper):
         super().__init__(soot_wrapper);
 
 
     def set_precursor_names(self, precursor_list):
@@ -43,8 +43,14 @@
         super().__init__(soot_wrapper);
 
 class CrossLinkMod(PAHGrowthAbstract, CCrossLinkMod):
     serialized_name = "CrossLinkingModified"
     def __init__(self, soot_wrapper):
         super().__init__(soot_wrapper);
 
-PAH_GROWTH_MODELS = [ReactDim, DimerCoal, CrossLink, DimerCoalMod, CrossLinkMod]
+
+class CrossLinkMerge(PAHGrowthAbstract, CCrossLinkMerge):
+    serialized_name = "CrossLinkMerge"
+    def __init__(self, soot_wrapper):
+        super().__init__(soot_wrapper);
+
+PAH_GROWTH_MODELS = [ReactDim, DimerCoal, CrossLink, DimerCoalMod, CrossLinkMod, CrossLinkMerge]
```

## eptlsoot/apps/reactors.py

```diff
@@ -64,29 +64,29 @@
     
     @property
     def gas_carbon_flux(self) -> float:
         return self.soot_gas.elemental_mass_fraction('C') * self.mdot;
 
     @property
     def soot_carbon_flux(self) -> float:
-        return self.soot_wrapper.soot_model.elemental_mass_fraction('C') * self.mdot;
+        return self.soot_wrapper.soot_gas.elemental_mass_fraction('C') * self.mdot;
 
 
     @property
     def total_hydrogen_flux(self) -> float:
         hydrogen_mass = self.soot_gas.elemental_mass_fraction('H') + self.soot_wrapper.soot_model.hydrogen_mass();
         return hydrogen_mass * self.mdot;
     
     @property
     def gas_hydrogen_flux(self) -> float:
         return self.soot_gas.elemental_mass_fraction('H') * self.mdot;
 
     @property
     def soot_hydrogen_flux(self) -> float:
-        return self.soot_wrapper.soot_model.elemental_mass_fraction('H') * self.mdot;
+        return self.soot_wrapper.soot_gas.elemental_mass_fraction('H') * self.mdot;
 
     @property
     def gas_elemental_flux(self, element_name) -> float:
         return self.soot_gas.elemental_mass_fraction(element_name) * self.mdot;
 
 
 class Inlet:
@@ -233,29 +233,29 @@
     
     @property
     def gas_carbon_flux(self) -> float:
         return self.soot_gas.elemental_mass_fraction('C') * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
 
     @property
     def soot_carbon_flux(self) -> float:
-        return self.soot_wrapper.soot_model.elemental_mass_fraction('C') * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
+        return self.soot_wrapper.soot_gas.elemental_mass_fraction('C') * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
 
 
     @property
     def total_hydrogen_flux(self) -> float:
         hydrogen_mass = self.soot_gas.elemental_mass_fraction('H') + self.soot_wrapper.soot_model.hydrogen_mass();
         return hydrogen_mass * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
     
     @property
     def gas_hydrogen_flux(self) -> float:
         return self.soot_gas.elemental_mass_fraction('H') * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
 
     @property
     def soot_hydrogen_flux(self) -> float:
-        return self.soot_wrapper.soot_model.elemental_mass_fraction('H') * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
+        return self.soot_wrapper.soot_gas.elemental_mass_fraction('H') * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
 
     @property
     def gas_elemental_flux(self, element_name) -> float:
         return self.soot_gas.elemental_mass_fraction(element_name) * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
 
 
     @property
```

## Comparing `eptlsoot-0.0.8.dist-info/METADATA` & `eptlsoot-0.0.9.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eptlsoot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Soot model from EPTL group
 Author-email: Mo Adib <moademic@gmail.com>
 Project-URL: Homepage, https://carleton.ca/eptl/people/336/
 Keywords: computational,soot
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

