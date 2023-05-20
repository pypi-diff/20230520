# Comparing `tmp/easyFermi-1.1.0.tar.gz` & `tmp/easyFermi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyFermi-1.1.0.tar", last modified: Wed Mar  8 11:40:12 2023, max compression
+gzip compressed data, was "easyFermi-1.1.1.tar", last modified: Sat May 20 14:12:54 2023, max compression
```

## Comparing `easyFermi-1.1.0.tar` & `easyFermi-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-03-08 11:40:12.060002 easyFermi-1.1.0/
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1522 2022-01-31 12:02:33.000000 easyFermi-1.1.0/LICENSE.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)     1702 2023-03-08 11:40:12.060002 easyFermi-1.1.0/PKG-INFO
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1172 2022-08-22 09:22:30.000000 easyFermi-1.1.0/README.md
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-03-08 11:40:12.056002 easyFermi-1.1.0/easyFermi/
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)       63 2022-02-01 13:52:31.000000 easyFermi-1.1.0/easyFermi/__init__.py
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)    91750 2023-03-08 11:14:57.000000 easyFermi-1.1.0/easyFermi/easyFermi.py
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-03-08 11:40:12.060002 easyFermi-1.1.0/easyFermi/images/
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)    40332 2022-01-15 16:04:30.000000 easyFermi-1.1.0/easyFermi/images/easyFermiIcon.png
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)   120340 2022-03-07 14:06:40.000000 easyFermi-1.1.0/easyFermi/images/easyFermiWindow.png
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)   121691 2021-11-23 14:18:26.000000 easyFermi-1.1.0/easyFermi/images/fermi.png
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-03-08 11:40:12.060002 easyFermi-1.1.0/easyFermi.egg-info/
--rw-rw-r--   0 raniere   (1000) raniere   (1000)     1702 2023-03-08 11:40:12.000000 easyFermi-1.1.0/easyFermi.egg-info/PKG-INFO
--rw-rw-r--   0 raniere   (1000) raniere   (1000)      338 2023-03-08 11:40:12.000000 easyFermi-1.1.0/easyFermi.egg-info/SOURCES.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)        1 2023-03-08 11:40:12.000000 easyFermi-1.1.0/easyFermi.egg-info/dependency_links.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)       14 2023-03-08 11:40:12.000000 easyFermi-1.1.0/easyFermi.egg-info/requires.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)       10 2023-03-08 11:40:12.000000 easyFermi-1.1.0/easyFermi.egg-info/top_level.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)       38 2023-03-08 11:40:12.060002 easyFermi-1.1.0/setup.cfg
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1181 2023-03-08 11:38:58.000000 easyFermi-1.1.0/setup.py
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-05-20 14:12:54.372224 easyFermi-1.1.1/
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1522 2022-01-31 12:02:33.000000 easyFermi-1.1.1/LICENSE.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)     1702 2023-05-20 14:12:54.372224 easyFermi-1.1.1/PKG-INFO
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1172 2022-08-22 09:22:30.000000 easyFermi-1.1.1/README.md
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-05-20 14:12:54.372224 easyFermi-1.1.1/easyFermi/
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)       63 2022-02-01 13:52:31.000000 easyFermi-1.1.1/easyFermi/__init__.py
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)    92545 2023-05-20 14:10:42.000000 easyFermi-1.1.1/easyFermi/easyFermi.py
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-05-20 14:12:54.372224 easyFermi-1.1.1/easyFermi/images/
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)    40332 2022-01-15 16:04:30.000000 easyFermi-1.1.1/easyFermi/images/easyFermiIcon.png
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)   120905 2023-03-08 11:57:13.000000 easyFermi-1.1.1/easyFermi/images/easyFermiWindow.png
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)   121691 2021-11-23 14:18:26.000000 easyFermi-1.1.1/easyFermi/images/fermi.png
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-05-20 14:12:54.372224 easyFermi-1.1.1/easyFermi.egg-info/
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)     1702 2023-05-20 14:12:54.000000 easyFermi-1.1.1/easyFermi.egg-info/PKG-INFO
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)      338 2023-05-20 14:12:54.000000 easyFermi-1.1.1/easyFermi.egg-info/SOURCES.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)        1 2023-05-20 14:12:54.000000 easyFermi-1.1.1/easyFermi.egg-info/dependency_links.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)       14 2023-05-20 14:12:54.000000 easyFermi-1.1.1/easyFermi.egg-info/requires.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)       10 2023-05-20 14:12:54.000000 easyFermi-1.1.1/easyFermi.egg-info/top_level.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)       38 2023-05-20 14:12:54.372224 easyFermi-1.1.1/setup.cfg
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1181 2023-05-20 14:11:32.000000 easyFermi-1.1.1/setup.py
```

### Comparing `easyFermi-1.1.0/LICENSE.txt` & `easyFermi-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyFermi-1.1.0/PKG-INFO` & `easyFermi-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyFermi
-Version: 1.1.0
+Version: 1.1.1
 Summary: The easiest way to analyze Fermi-LAT data
 Author: Raniere de Menezes
 Author-email: <easyfermi@gmail.com>
 Keywords: python,fermi,GUI,graphical interface,easyFermi,gamma-rays
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyFermi-1.1.0/README.md` & `easyFermi-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `easyFermi-1.1.0/easyFermi/easyFermi.py` & `easyFermi-1.1.1/easyFermi/easyFermi.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,18 +72,20 @@
 import matplotlib
 matplotlib.interactive(True)
 import numpy as np
 import astropy.io.fits as pyfits
 from astropy.time import Time
 from fermipy.gtanalysis import GTAnalysis
 from fermipy.plotting import ROIPlotter
+import platform
 
 import pathlib
 libpath = str(pathlib.Path(__file__).parent.resolve())+"/images/"
 
+OS_name = platform.system()
 
 class Worker(QtCore.QObject):
     starting = QtCore.pyqtSignal()
     finished = QtCore.pyqtSignal()
     progress = QtCore.pyqtSignal(int)
     
     
@@ -628,14 +630,17 @@
         self.checkBox_13.setToolTip("Check if you wish that only the normalizations can vary")
         self.checkBox_14.setToolTip("Freeze the Galactic diffuse model")
         self.checkBox_15.setToolTip("Freeze the isotropic diffuse model")
         self.checkBox_16.setToolTip("If checked, you will freeze the spectral shape of the target")
         self.checkBox_8.setToolTip("Check to look for extra sources in the ROI, i.e. sources not listed in the adopted catalog")
         self.checkBox_6.setToolTip("If checked, the target will be removed from the model. If unchecked, easyFermi computes the residuals TS map")
         self.label_11.setToolTip("The photon index of the test source")
+        self.spinBox_2.setToolTip("Multiprocessing is available only for Linux OS")
+        self.checkBox_4.setToolTip("Check this to find the optimal R.A. and Dec. of the target's gamma-ray emission")
+        self.lineEdit_12.setToolTip("Only the sources within this radius will have free parameters during the fit")
 
     def retranslateUi(self, mainWindow):
         _translate = QtCore.QCoreApplication.translate
         mainWindow.setWindowIcon(QtGui.QIcon(libpath+'easyFermiIcon.png'))
         mainWindow.setWindowTitle(_translate("mainWindow", "easyFermi"))
         self.pushButton.setText(_translate("mainWindow", "Go!"))
         self.label_2.setText(_translate("mainWindow", "Log:"))
@@ -1407,17 +1412,19 @@
             self.toolButton_6.setChecked(False)
         
        
     def activate(self):
         """ This function activates/deactivates the entries in the main window"""
         if self.checkBox.isChecked():
             self.spinBox.setEnabled(True)
-            self.spinBox_2.setEnabled(True)
+            if OS_name != "Darwin":
+                self.spinBox_2.setEnabled(True)
+                self.label_9.setEnabled(True)
             self.label_4.setEnabled(True)
-            self.label_9.setEnabled(True)
+            
         else:
             self.spinBox.setEnabled(False)
             self.spinBox_2.setEnabled(False)
             self.label_4.setEnabled(False)
             self.label_9.setEnabled(False)
             
         if self.checkBox_2.isChecked():
@@ -1774,15 +1781,20 @@
             plt.tight_layout()
             plt.savefig(self.OutputDir+'Quickplot_extension.'+output_format,bbox_inches='tight')
             
             
             
         #LC:    
         if self.checkBox.isChecked():
-            lc = self.gta.lightcurve(self.sourcename, nbins=self.spinBox.value(), free_radius=self.roiwidth/2,use_local_ltcube=True, use_scaled_srcmap=True, free_params=['norm'], shape_ts_threshold=9, multithread=True, nthread=self.spinBox_2.value())
+            #Running the LC in parallel cores is possible only in Linux systems:
+            if OS_name != "Darwin":
+                lc = self.gta.lightcurve(self.sourcename, nbins=self.spinBox.value(), free_radius=self.roiwidth/2,use_local_ltcube=True, use_scaled_srcmap=True, free_params=['norm'], shape_ts_threshold=9, multithread=True, nthread=self.spinBox_2.value())
+            else:
+                lc = self.gta.lightcurve(self.sourcename, nbins=self.spinBox.value(), free_radius=self.roiwidth/2,use_local_ltcube=True, use_scaled_srcmap=True, free_params=['norm'], shape_ts_threshold=9, multithread=False)
+            
             TSmin = 9
             
             f = plt.figure(figsize=(9,4),dpi=250)
             ax = f.add_subplot(1,1,1)
             ax.xaxis.set_minor_locator(AutoMinorLocator(2))
             ax.yaxis.set_minor_locator(AutoMinorLocator(2))
             ax.tick_params(which='major', length=5, direction='in')
```

### Comparing `easyFermi-1.1.0/easyFermi/images/easyFermiIcon.png` & `easyFermi-1.1.1/easyFermi/images/easyFermiIcon.png`

 * *Files identical despite different names*

### Comparing `easyFermi-1.1.0/easyFermi/images/fermi.png` & `easyFermi-1.1.1/easyFermi/images/fermi.png`

 * *Files identical despite different names*

### Comparing `easyFermi-1.1.0/easyFermi.egg-info/PKG-INFO` & `easyFermi-1.1.1/easyFermi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyFermi
-Version: 1.1.0
+Version: 1.1.1
 Summary: The easiest way to analyze Fermi-LAT data
 Author: Raniere de Menezes
 Author-email: <easyfermi@gmail.com>
 Keywords: python,fermi,GUI,graphical interface,easyFermi,gamma-rays
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyFermi-1.1.0/setup.py` & `easyFermi-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.0'
+VERSION = '1.1.1'
 DESCRIPTION = 'The easiest way to analyze Fermi-LAT data'
 LONG_DESCRIPTION = 'A GUI that allows to do measure the flux, create light curves, SEDs, and TS maps for Fermi-LAT data.'
 
 # Setting up
 setup(
     name="easyFermi",
     version=VERSION,
```

