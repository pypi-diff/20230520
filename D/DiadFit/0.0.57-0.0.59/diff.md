# Comparing `tmp/DiadFit-0.0.57.tar.gz` & `tmp/DiadFit-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DiadFit-0.0.57.tar", last modified: Fri Mar 31 16:01:21 2023, max compression
+gzip compressed data, was "DiadFit-0.0.59.tar", last modified: Fri May 19 22:41:59 2023, max compression
```

## Comparing `DiadFit-0.0.57.tar` & `DiadFit-0.0.59.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:01:21.784028 DiadFit-0.0.57/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-31 16:01:21.784028 DiadFit-0.0.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-31 16:01:08.000000 DiadFit-0.0.57/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 16:01:21.784028 DiadFit-0.0.57/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-03-31 16:01:10.000000 DiadFit-0.0.57/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:01:21.776028 DiadFit-0.0.57/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:01:21.780028 DiadFit-0.0.57/src/DiadFit/
--rw-r--r--   0 runner    (1001) docker     (123)    26343 2023-03-31 16:01:10.000000 DiadFit-0.0.57/src/DiadFit/CO2_EOS.py
--rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-03-31 16:01:10.000000 DiadFit-0.0.57/src/DiadFit/H2O_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-03-31 16:01:10.000000 DiadFit-0.0.57/src/DiadFit/Psensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-31 16:01:10.000000 DiadFit-0.0.57/src/DiadFit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-31 16:01:10.000000 DiadFit-0.0.57/src/DiadFit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    22411 2023-03-31 16:01:10.000000 DiadFit-0.0.57/src/DiadFit/cosmicray_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-03-31 16:01:10.000000 DiadFit-0.0.57/src/DiadFit/densimeters.py
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-03-31 16:01:10.000000 DiadFit-0.0.57/src/DiadFit/density_depth_crustal_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)   153634 2023-03-31 16:01:10.000000 DiadFit-0.0.57/src/DiadFit/diads.py
--rw-r--r--   0 runner    (1001) docker     (123)    32657 2023-03-31 16:01:10.000000 DiadFit-0.0.57/src/DiadFit/error_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)    34802 2023-03-31 16:01:10.000000 DiadFit-0.0.57/src/DiadFit/importing_data_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    55322 2023-03-31 16:01:10.000000 DiadFit-0.0.57/src/DiadFit/ne_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:01:21.784028 DiadFit-0.0.57/src/DiadFit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-31 16:01:21.000000 DiadFit-0.0.57/src/DiadFit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-31 16:01:21.000000 DiadFit-0.0.57/src/DiadFit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 16:01:21.000000 DiadFit-0.0.57/src/DiadFit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 16:01:21.000000 DiadFit-0.0.57/src/DiadFit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-31 16:01:21.000000 DiadFit-0.0.57/src/DiadFit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:41:59.802765 DiadFit-0.0.59/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-19 22:41:59.802765 DiadFit-0.0.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 22:41:45.000000 DiadFit-0.0.59/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:41:59.802765 DiadFit-0.0.59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-19 22:41:48.000000 DiadFit-0.0.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:41:59.798765 DiadFit-0.0.59/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:41:59.802765 DiadFit-0.0.59/src/DiadFit/
+-rw-r--r--   0 runner    (1001) docker     (123)    26927 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/CO2_EOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43406 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/H2O_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/Psensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/argon_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/cosmicray_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/densimeters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/density_depth_crustal_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)   162634 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/diads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32657 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/error_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35199 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/importing_data_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63568 2023-05-19 22:41:48.000000 DiadFit-0.0.59/src/DiadFit/ne_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:41:59.802765 DiadFit-0.0.59/src/DiadFit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-19 22:41:59.000000 DiadFit-0.0.59/src/DiadFit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-19 22:41:59.000000 DiadFit-0.0.59/src/DiadFit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:41:59.000000 DiadFit-0.0.59/src/DiadFit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 22:41:59.000000 DiadFit-0.0.59/src/DiadFit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 22:41:59.000000 DiadFit-0.0.59/src/DiadFit.egg-info/top_level.txt
```

### Comparing `DiadFit-0.0.57/PKG-INFO` & `DiadFit-0.0.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiadFit
-Version: 0.0.57
+Version: 0.0.59
 Summary: DiadFit
 Home-page: https://github.com/PennyWieser/DiadFit
 Author: Penny Wieser
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/DiadFit)](https://pypi.org/project/DiadFit/)
         [![Build Status](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml)
```

### Comparing `DiadFit-0.0.57/README.md` & `DiadFit-0.0.59/README.md`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.57/setup.py` & `DiadFit-0.0.59/setup.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.57/src/DiadFit/CO2_EOS.py` & `DiadFit-0.0.59/src/DiadFit/CO2_EOS.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,28 @@
 
     Returns
     -------------
     pd.DataFrame:
         colums for Liq_gcm3 and gas_gcm3, bulk density if homog_to specified
 
     """
+    if isinstance(homog_to, str):
+        if homog_to=='L' or homog_to=='V':
+            a=1
+        else:
+            raise TypeError('unsupported input for homog_to, has to be L or V')
+
+    if isinstance(T_h_C, float) or isinstance(T_h_C, int):
+        if T_h_C>=30.9782: # 29.878:
+        #print('Sorry, algorithm cant converge for Ts above 29.878')
+            raise TypeError('Sorry, algorithm cant converge for Ts above 30.9782')
+    if isinstance(T_h_C, pd.Series) or isinstance(T_h_C, np.ndarray):
+        if any(T_h_C)>=30.9782:
+            raise TypeError('Sorry, algorithm cant converge for Ts above 30.9782')
+
     if EOS!='SW96':
         raise TypeError('At the moment, only Span and Wanger (SW96) EOS can be used to convert T_h_C into density')
 
     T_K_hom=T_h_C+273.15
     TempTerm=1-T_K_hom/304.1282
     # This is equation 3.14 from Span and Wanger (1996)
     Liq_density=(np.exp(1.9245108*TempTerm**0.34-0.62385555*TempTerm**0.5-0.32731127*TempTerm**1.6666667+0.39245142*TempTerm**1.8333333)*0.4676)
@@ -105,18 +119,19 @@
             if homog_to=='V':
                 df=pd.DataFrame(data={'Bulk_gcm3': gas_density,
         'Liq_gcm3': Liq_density,
         'Gas_gcm3': gas_density,
         'T_h_C': T_h_C,
         'homog_to': homog_to})
 
+
+
         # If its a panda series
         else:
 
-
             df=pd.DataFrame(data={'Bulk_gcm3': np.nan,
         'Liq_gcm3': Liq_density,
         'Gas_gcm3': gas_density,
         'T_h_C': T_h_C,
         'homog_to': homog_to})
 
 
@@ -305,15 +320,15 @@
     if EOS=='SW96':
         CO2_dens_gcm3=calculate_rho_for_P_T_SW96(P_kbar, T_K)
 
 
     if EOS=='SP94':
 
         CO2_dens_gcm3=calculate_rho_for_P_T_SP94(T_K=T_K, P_kbar=P_kbar)
-    
+
     if Sample_ID is not None:
         df['Sample_ID']=Sample_ID
 
     return pd.Series(CO2_dens_gcm3)
 
 
 
@@ -407,15 +422,15 @@
 
     if EOS=='SW96':
         df=calculate_P_for_rho_T_SW96(CO2_dens_gcm3=CO2_dens_gcm3, T_K=T_K)
     elif EOS=='SP94':
         df=calculate_P_for_rho_T_SP94(CO2_dens_gcm3=CO2_dens_gcm3, T_K=T_K)
     else:
         raise TypeError('Please choose either SP94 or SW96 as an EOS')
-    
+
     if Sample_ID is not None:
         df['Sample_ID']=Sample_ID
 
     return df
 
 # Calculating P for a given density and Temperature using Coolprop
 
@@ -512,26 +527,26 @@
     P_MPa=(0.1*83.14472*(T-T0)*(MolConc+a1*MolConc**2-MolConc**2*((a3
     +2*a4*MolConc+3*a5*MolConc**2+4*a6*MolConc**3)/(a2+
     a3*MolConc+a4*MolConc**2+a5*MolConc**3+a6*MolConc**4)**2)
     +a7*MolConc**2*np.exp(-a8*MolConc)
     +a9*MolConc**2*np.exp(-a10*MolConc)))
     if scalar_return is True:
         return P_MPa
-    
+
     elif isinstance(P_MPa, pd.Series) or isinstance(P_MPa, np.ndarray):
-    
+
 
         df=pd.DataFrame(data={'P_kbar': P_MPa/100,
                             'P_MPa': P_MPa,
                             'T_K': T_K,
                             'CO2_dens_gcm3': CO2_dens_gcm3
 
                             })
-        
-        
+
+
     else:
         df=pd.DataFrame(data={'P_kbar': P_MPa/100,
                             'P_MPa': P_MPa,
                             'T_K': T_K,
                             'CO2_dens_gcm3': CO2_dens_gcm3
 
                             }, index=[0])
@@ -568,15 +583,15 @@
 
     if EOS=='SW96':
         df=calculate_T_for_rho_P_SW96(CO2_dens_gcm3=CO2_dens_gcm3, P_kbar=P_kbar)
     elif EOS=='SP94':
         df=calculate_T_for_rho_P_SP94(CO2_dens_gcm3=CO2_dens_gcm3, P_kbar=P_kbar)
     else:
         raise TypeError('Please choose either SP94 or SW96 as an EOS')
-    
+
     if Sample_ID is not None:
         df['Sample_ID']=Sample_ID
 
     return df
 
 def calculate_T_for_rho_P_SW96(CO2_dens_gcm3, P_kbar):
     """ This function calculates Temperature for a known CO2 density in g/cm3  and a known Pressure (in kbar)
@@ -606,15 +621,15 @@
 
     try:
         import CoolProp.CoolProp as cp
     except ImportError:
         raise RuntimeError('You havent installed CoolProp, which is required to convert FI densities to pressures. If you have python through conda, run conda install -c conda-forge coolprop in your command line')
 
     Temp=cp.PropsSI('T', 'D', CO2_dens_gcm3*1000, 'P', P_Pa, 'CO2')
-  
+
 
     return pd.Series(Temp)
 
 def calculate_T_for_rho_P_SP94(P_kbar, CO2_dens_gcm3):
     """ This function calculates Temp for a known Pressure (in kbar) and a known CO2 density in g/cm3
     using the Sterner and Pitzer EOS.
     it references the objective functions to solve for density.
@@ -626,15 +641,15 @@
 
    CO2_dens_gcm3: int, float, pd.Series, np.array
         CO2 density in g/cm3
 
     Returns
     --------------------
     pd.Series
-        Temp in K 
+        Temp in K
 
     """
     target_pressure_MPa=P_kbar*100
     Temp=calculate_SP1994_Temp(CO2_dens_gcm3=CO2_dens_gcm3, target_pressure_MPa=target_pressure_MPa)
     return  pd.Series(Temp)
```

### Comparing `DiadFit-0.0.57/src/DiadFit/H2O_fitting.py` & `DiadFit-0.0.59/src/DiadFit/H2O_fitting.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,20 @@
         df_out (pandas DataFrame): A dataframe with columns "filename", "crystal_name", and "MI_name", containing the input filenames, the extracted crystal sample names, and the extracted MI sample names, respectively.
 
     """
 
     file_simple=pf.extracting_filenames_generic(names=files,
     prefix=prefix, str_prefix=str_prefix,
    file_type=file_type)
+    
+
+
     xstal=np.empty(len(file_simple), dtype=object)
     MI=np.empty(len(file_simple), dtype=object)
+
     for i in range(0, len(file_simple)):
         name=file_simple[i]
         xstal[i]=name.split(char_xstal)[pos_xstal]
         MI[i]=name.split(char_MI)[pos_MI]
     df_out=pd.DataFrame(data={'filename': files,
                          'crystal_name': xstal,
                          'MI_name': MI})
@@ -101,15 +105,15 @@
 
     trough_y=np.min(trim_y_cub_Ol)
     trough_x=trim_x[trim_y_cub_Ol==trough_y]
 
 
     return peak_pos_Ol, peak_height_Ol, trough_y, trough_x
 
-def smooth_and_trim_around_olivine(filename, x_range=[800,900], x_max=900, Ol_spectra=None,
+def smooth_and_trim_around_olivine(filename=None, x_range=[800,900], x_max=900, Ol_spectra=None,
                                    MI_spectra=None, plot_figure=True):
     """
     Takes melt inclusion and olivine spectra, and trims into the region around the olivine peaks,
     and fits a cubic spline (used for unmixing spectra)
 
     Parameters
     -----------
@@ -118,14 +122,17 @@
 
     Ol_spectra: nd.array
         numpy array of olivine spectra (x is wavenumber, y is intensity)
 
     MI_spectra: nd.array
         numpy array of melt inclusion spectra (x is wavenumber, y is intensity)
 
+    filename:str
+        name of file for saving figure
+
 
 
     Returns:
     -----------
     x_new: x coordinates of smoothed curves
     y_cub_MI: smoothed y coordinates using a cubic spline for MI
     y_cub_Ol: smoothed y coordinates using a cubic spline for Ol
@@ -168,15 +175,16 @@
     # Plot peaks and troughs on this to check they are right
     peak_pos_Ol, peak_height_Ol, trough_y, trough_x=find_olivine_peak_trough_pos(
         smoothed_ol_y=y_cub_Ol, x_new=x_new, height=1)
 
 
     if plot_figure is True:
         fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(8,3.5))
-        fig.suptitle('file='+filename)
+        if filename is not None:
+            fig.suptitle('file='+filename)
         ax1.plot(Ol_spectra[:, 0], Ol_spectra[:, 1], '-g', label='Ol Spectra')
         ax1.plot(MI_spectra[:, 0], MI_spectra[:, 1], '-',
                 color='salmon', label='MI Spectra')
 
         ax2.plot(Filt_MI[:, 0], Filt_MI[:, 1], '+', color='salmon')
         ax2.plot(Filt_Ol[:, 0], Filt_Ol[:, 1], '+g')
         ax2.plot(x_new, y_cub_MI, '-', color='salmon', label='MI Spectra')
@@ -329,14 +337,17 @@
 
     x_max:  float or int
         Maximum mixing proportion allowed
 
     N_steps: int
         Number of mixing steps to use between X_Max and X_Max. E.g. Precisoin of mixed value.
 
+    av_width: int
+        averages +- 1 width either side of the peak and troughs when doing assesment and regression
+
 
 
     Returns:
     -----------
     MI_Mix_Best: np.array
         Spectra of best-fit unmixed spectra (e.g. where olivine peak and trough the smallest)
     ideal_mix: float
@@ -552,14 +563,15 @@
             if os.path.exists(path3):
                 out='path exists'
             else:
                 os.makedirs(path+'/'+ 'H2O_Silicate_images', exist_ok=False)
 
 
             file=filename
+            fig.tight_layout()
             fig.savefig(path3+'/'+'Check_if_negative_{}.png'.format(filename), dpi=dpi)
 
     return Spectra
 
 
 
 
@@ -1002,14 +1014,21 @@
         File path
     filename : str
         File name
     Spectra : numpy.ndarray, optional
         2D array representing the spectrum data
     config1 : object
         Configuration object for water peak and background positions. Default parameters stored in water_bck_pos, user can tweak.
+        Parameters that need tweaking:
+
+        fit_water: str 'poly', 
+        N_poly_water: str, degree of polynomial to fit to background
+        lower_bck_water: [float, float], background position to left of water peak
+        upper_bck_water: [float, float], background position to right of water peak
+
     exclude_range1_water : list of float, optional
         List of two numbers representing the start and end of a range of wavenumbers to be excluded from the spectrum
     exclude_range2_water : list of float, optional
         List of two numbers representing the start and end of a second range of wavenumbers to be excluded from the spectrum
     plot_figure : bool, optional
         Indicates whether or not to plot the fit (default is True)
     dpi : int, optional
```

### Comparing `DiadFit-0.0.57/src/DiadFit/Psensor.py` & `DiadFit-0.0.59/src/DiadFit/Psensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 import os
 
 try:
     import docx
 except ImportError:
     ImportError('Not installed')
 
-#from docx import Document
 import datetime
 import warnings
 
 encode="ISO-8859-1"
 
 ## Function for getting file names
 
-def get_files(*,path=None,filetype=None):
+def get_files(*,path,filetype):
     """
     Returns a list of files with specific file type(s) in the specified directory
     Parameters
     --------------
     path: str
         Path of the directory where the files are located.
     filetype: str or list of str
@@ -34,15 +33,15 @@
     file_ls=[]
     for file in os.listdir(path):
         if file.endswith(tuple(filetype)):
             file_ls.append(file)
     return file_ls
 
 ## Function for extracting information from the docx reports
-def report_info (*,path=None,report=None):
+def report_info (*,path,report):
     """
     Reads a word document report (exported from ESI-TEC software), extracts and returns the start date and time of the pressure recording and the serial number of the sensor.
     Parameters
     --------------
     path: str
         Path of the directory where the word document is located
     report: str
@@ -53,15 +52,15 @@
     start_time: datetime object
         Start time of the analysis in the report
     sn_str: str
         Serial number of the sensor
     """
 
     # Open the Word document
-    document = Document(path+'/'+report)
+    document = docx.Document(path+'/'+report)
 
     # Iterate over all paragraphs in the document
     for para in document.paragraphs:
         # Check if the paragraph contains the text "Test Date:"
         if "Test Date:" in para.text:
             # Extract the date and time from the paragraph text
             date_time_str = ":".join(para.text.split(":")[1:]).strip()
@@ -72,15 +71,15 @@
 
     print(start_time)
     print('Serial No. '+ sn_str)
     return start_time, sn_str
 
 ## Function for reading in data
 
-def read_pfiles(*,path=None,file=None,start_time=None,sn_name='0132212'): #UCB '0132212', cornell '0830903'
+def read_pfiles(*,path,file,start_time,sn_name='0132212'): #UCB '0132212', cornell '0830903'
     """
     Reads a csv or xlsx file of pressure data exported from ESI-TEC software and returns a dataframe with two extra columns "Date and Time" (datetime object) and "unix_timestamp" (timestamp expressed as UNIX time, or time in seconds since the epoch time Jan 1st, 1970 00:00:00 UTC) based on the start_time of the pressure recording and time since start in the file. It also renames the time column to Time_sincestart.
     Parameters
     --------------
     path: str
         Path of the directory where the file is located
     file: str
@@ -111,15 +110,15 @@
         data['unix_timestamp'] = data['Date and Time'].apply(lambda x: x.timestamp())
         data= data.rename(columns={'Time': 'Time_sincestart'})
 
     return data
 
 ## Function for calculating datetime and duration from metadata file
 
-def add_datetime_and_duration_cols(*,df=None,raman_cpu_offset='none',offset_hms=[0,0,0]):
+def add_datetime_and_duration_cols(*,df,raman_cpu_offset='none',offset_hms=[0,0,0]):
     """
     Takes a DataFrame and adds columns for "Date and Time", "unix_timestamp" and "duration_s". The input frame should be either the complete DataFrame with spectra metadata and fits output by DiadFit or just the spectral metadata. "Date and Time" contains datetime objects; 'unix_timestamp' contains the numeric (float) timestamp for the date and time in standard UNIX time or seconds since epoch time (Jan 1st 1970 00:00:00 UTC), this is plottable; and "duration_s" is the duration of the analysis in seconds.
 
     Parameters
     --------------
     df: pd.DataFrame
         The input DataFrame
@@ -169,15 +168,15 @@
         return
     dur_days = df['duration'].apply(duration_to_timedelta)
     df['duration_s']=dur_days.dt.total_seconds()
     return df
 
 ## Function for calculating the pressure median for each analysis
 
-def get_p_medians(*,pdata=None,sdata=None,export_all=False):
+def get_p_medians(*,pdata,sdata,export_all=False):
     """
     Takes two DataFrames and returns a new DataFrame containing the median and median absolute deviation of the pressure values for each Raman analysis. It finds the closest matching rows in the two DataFrames based on timestamp and filters the pressure data between the matched timestamps. It then calculates the median and mean absolute deviation of the filtered pressure data. If export_all==True, it also includes the start time, end time, duration, and filename in the output DataFrame.
 
     Parameters
     --------------
     pdata: pd.DataFrame
         The pressure DataFrame (output by read_pfiles)
@@ -212,15 +211,18 @@
         start_time_S = df2.loc[idx_df2,'unix_timestamp']
         duration = df2.loc[idx_df2, 'duration_s']
         end_time_P = start_time_P + pd.Timedelta(seconds=float(duration))
         # filter pressure data between start_time_P and end_time
         pressure_data = df1[(df1['unix_timestamp'] >= start_time_P) & (df1['unix_timestamp'] <= end_time_P)]
         median_pressure = pressure_data['Pressure / MPa'].median()
         mad_pressure = (pressure_data['Pressure / MPa'] - pressure_data['Pressure / MPa'].mean()).abs().mean()
+        median_temp = pressure_data['Temperature / °C'].median()
+        mad_temp = (pressure_data['Temperature / °C'] - pressure_data['Temperature / °C'].mean()).abs().mean()
+
         # Append a new row to the new dataframe
         if export_all==True:
-            new_row = pd.DataFrame({'filename_x': filename, 'start_time_S':start_time_S,'start_time_P': start_time_P, 'duration': duration,'end_time_P':end_time_P, 'median_pressure': median_pressure, 'mad_pressure': mad_pressure},index=[0])
+            new_row = pd.DataFrame({'filename_x': filename, 'start_time_S':start_time_S,'start_time_P': start_time_P, 'duration': duration,'end_time_P':end_time_P, 'median_pressure': median_pressure, 'mad_pressure': mad_pressure,'median_temp': median_temp, 'mad_temp': mad_temp},index=[0])
             new_data=pd.concat([new_data,new_row],ignore_index=True)
         else:
-            new_row = pd.DataFrame({'filename_x': filename, 'start_time_P': start_time_P, 'end_time_P':end_time_P, 'median_pressure': median_pressure, 'mad_pressure': mad_pressure},index=[0])
+            new_row = pd.DataFrame({'filename_x': filename, 'start_time_P': start_time_P, 'end_time_P':end_time_P, 'median_pressure': median_pressure, 'mad_pressure': mad_pressure,'median_temp': median_temp, 'mad_temp': mad_temp},index=[0])
             new_data=pd.concat([new_data,new_row],ignore_index=True)
     return new_data
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `DiadFit-0.0.57/src/DiadFit/__init__.py` & `DiadFit-0.0.59/src/DiadFit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from DiadFit.Psensor import *
 
 # This reads different data formats, imports files, and does the string stripping for WITEC
 from DiadFit.importing_data_files import *
 
 # This does the work associated with fitting Ne lines
 from DiadFit.ne_lines import *
-
+from DiadFit.argon_lines import *
 
 # This does the work associated with fitting Diads
 from DiadFit.diads import *
 
 
 # This has densimeters from different instruments
 from DiadFit.densimeters import *
```

### Comparing `DiadFit-0.0.57/src/DiadFit/cosmicray_filter.py` & `DiadFit-0.0.59/src/DiadFit/cosmicray_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # from tqdm.autonotebook import tqdm - Gave error
 
 from tqdm import tqdm
 import DiadFit as pf
 
 encode="ISO-8859-1"
 
-def check_pars(plot_rays, save_fig,export_cleanspec,exclude_ranges):
+def check_pars(plot_rays, save_fig,export_cleanspec,exclude_ranges,Diad_files,diad_peaks):
     """ Checks if input parameters plot_rays, save_fig, export_cleanspec and exclude_ranges are valid. If any of them is not valid, it raises a ValueError indicating which parameter is incorrect and what the allowed values are.
 
     Parameters
     --------------
     plot_rays: str ('all' or 'rays_only')
         Plot all spectra or just those for which cosmic rays were found
     save_fig: str ('all' or 'rays_only')
@@ -33,14 +33,18 @@
         raise ValueError("plot_rays can only be 'all' or 'rays_only', please correct")
     if not isinstance(save_fig, str) or save_fig not in ['all', 'rays_only']:
         raise ValueError("save_fig can only be 'all' or 'rays_only', please correct")
     if not isinstance(export_cleanspec, bool):
         raise ValueError("export_cleanspec can only be True or False, please correct")
     if not isinstance(exclude_ranges,(list,type(None))):
         raise ValueError("exclude_ranges can only be a list of tuples (i.e., [(1145,1155),(1080,1090)]), an empty list or None, please correct")
+    if not isinstance(Diad_files,pd.core.series.Series):
+        raise ValueError("Diad_files can only be a pandas Series, please correct")
+    if not isinstance(diad_peaks,(pd.core.frame.DataFrame,type(None))):
+        raise ValueError("diad_peaks can only be a pandas DataFrame or None, please correct")
 ## This function is the main filter, runs on one spectrum
 
 def filter_singleray(*,path=None,Diad_files=None,i=None,diad_peaks=None, exclude_ranges=[], filetype='headless_txt',n=1,dynfact=0.01,dynfact_2=0.003,
                         export_cleanspec=True,plot_rays='all',save_fig='rays_only',figsize=(20,5), xlims=None):
     """ This function is used to filter out cosmic rays in single Raman spectra of CO2.
     It requires the input of pre-identified peaks to avoid excluding peaks of interest.
     The filter compares the intensity of each pixel in the spectrum to n surrounding pixels and calculates an intensity factor.
@@ -84,19 +88,22 @@
     record: pd.DataFrame
         Dataframe containing the filename and whether cosmic rays were found
     clean_spec_df: pd.DataFrame
         DataFrame containing the cleaned spectrum (Wavenumber and Intensity columns)
 
     """
     try:
-        check_pars(plot_rays, save_fig,export_cleanspec,exclude_ranges)
+        check_pars(plot_rays, save_fig,export_cleanspec,exclude_ranges,Diad_files,diad_peaks)
     except ValueError as e:
         print(str(e))
         raise e
 
+    if type(diad_peaks)==type(None):
+        diad_peaks=pd.DataFrame()
+
     file=Diad_files.iloc[i]
     #open the spectrum in form of array
     Diad_array=pf.get_data(path=path, filename=file, filetype=filetype)
 
     # Get the intensity of the next and previous pixels
     intensity_prev = np.roll(Diad_array[:,1], -n)
     intensity_next = np.roll(Diad_array[:,1], n)
@@ -109,42 +116,49 @@
     # Create a new DataFrame with the calculated factors
     pxdf = pd.DataFrame({'Wavenumber': Diad_array[:,0],
                         'Intensity': Diad_array[:,1],
                         'minpx_fact': minpx_fact,
                         'maxpx_fact': maxpx_fact,
                         'maxpx_fact*minpx_fact':combo_fact})
 
-    # this creates a three pixel range for the peaks around the identify peak spot, "signal region"
-    res=np.round(max(np.diff(Diad_array[:,0])),1) # resolution of the spectrum - max distance between two pixels, rounded up.
-    snr_diad1=[diad_peaks['Diad1_pos']-res,diad_peaks['Diad1_pos']+res]
-    snr_diad2=[diad_peaks['Diad2_pos']-res,diad_peaks['Diad2_pos']+res]
-    snr_hb1=[diad_peaks['HB1_pos']-res,diad_peaks['HB1_pos']+res]
-    snr_hb2=[diad_peaks['HB2_pos']-res,diad_peaks['HB2_pos']+res]
-    snr_c13=[diad_peaks['C13_pos']-res,diad_peaks['C13_pos']+res]
-
-
-
-    # These identifies regions that aren't the peak regions
-    not_diad1=~pxdf.Wavenumber.between(snr_diad1[0][i],snr_diad1[1][i])
-    not_diad2=~pxdf.Wavenumber.between(snr_diad2[0][i],snr_diad2[1][i])
-
-    not_hb1=~pxdf.Wavenumber.between(snr_hb1[0][i],snr_hb1[1][i])
-    not_hb2=~pxdf.Wavenumber.between(snr_hb2[0][i],snr_hb2[1][i])
-    not_c13=~pxdf.Wavenumber.between(snr_c13[0][i],snr_c13[1][i])
-
     #This is for the extra ranges defined by the user
     if exclude_ranges==None:
         exclude_ranges=[]
 
     exclude_mask = pd.Series(False, index=pxdf.index)
     for r in exclude_ranges:
         exclude_mask |= (pxdf.Wavenumber >= r[0]) & (pxdf.Wavenumber <= r[1])
     not_exclude_mask=~exclude_mask
-    #This filters wavenumbers, intensities and intensity factors based on the query criteria.
-    query_str='maxpx_fact*minpx_fact > @dynfact & @not_diad1 & @not_diad2 & @not_hb1 & @not_hb2 & @not_c13 & @not_exclude_mask'
+
+    # this creates a three pixel range for the peaks around the identify peak spot, "signal region"
+    res=np.round(max(np.diff(Diad_array[:,0])),1) # resolution of the spectrum - max distance between two pixels, rounded up.
+
+    if diad_peaks.empty==True:
+        query_str='maxpx_fact*minpx_fact > @dynfact & @not_exclude_mask'
+    else:
+        snr_diad1=[diad_peaks['Diad1_pos']-res,diad_peaks['Diad1_pos']+res]
+        snr_diad2=[diad_peaks['Diad2_pos']-res,diad_peaks['Diad2_pos']+res]
+        snr_hb1=[diad_peaks['HB1_pos']-res,diad_peaks['HB1_pos']+res]
+        snr_hb2=[diad_peaks['HB2_pos']-res,diad_peaks['HB2_pos']+res]
+        snr_c13=[diad_peaks['C13_pos']-res,diad_peaks['C13_pos']+res]
+
+
+
+        # These identifies regions that aren't the peak regions
+        not_diad1=~pxdf.Wavenumber.between(snr_diad1[0][i],snr_diad1[1][i])
+        not_diad2=~pxdf.Wavenumber.between(snr_diad2[0][i],snr_diad2[1][i])
+
+        not_hb1=~pxdf.Wavenumber.between(snr_hb1[0][i],snr_hb1[1][i])
+        not_hb2=~pxdf.Wavenumber.between(snr_hb2[0][i],snr_hb2[1][i])
+        not_c13=~pxdf.Wavenumber.between(snr_c13[0][i],snr_c13[1][i])
+
+
+        #This filters wavenumbers, intensities and intensity factors based on the query criteria.
+        query_str='maxpx_fact*minpx_fact > @dynfact & @not_diad1 & @not_diad2 & @not_hb1 & @not_hb2 & @not_c13 & @not_exclude_mask'
+
     rays_wavenumber=pxdf.query(query_str)['Wavenumber']
     rays_intensity=pxdf.query(query_str)['Intensity']
     rays_fact=pxdf.query(query_str)['maxpx_fact*minpx_fact']
 
     # Removal of cosmic rays from the main dataframe, the distinction is important for the filter.
     # Second pass will not be efficient with nan values in the spectrum
 
@@ -174,31 +188,36 @@
 
         # Create a new DataFrame with the calculated factors
         pxdf_pass2 = pd.DataFrame({'Wavenumber': derayed_spectrum[:,0],
                             'Intensity': derayed_spectrum[:,1],
                             'minpx_fact_pass2': minpx_fact_pass2,
                             'maxpx_fact_pass2': maxpx_fact_pass2,
                             'maxpx_fact_pass2*minpx_fact_pass2':combo_fact_pass2})
-
-        not_diad1=~pxdf_pass2.Wavenumber.between(snr_diad1[0][i],snr_diad1[1][i])
-        not_diad2=~pxdf_pass2.Wavenumber.between(snr_diad2[0][i],snr_diad2[1][i])
-
-        not_hb1=~pxdf_pass2.Wavenumber.between(snr_hb1[0][i],snr_hb1[1][i])
-        not_hb2=~pxdf_pass2.Wavenumber.between(snr_hb2[0][i],snr_hb2[1][i])
-        not_c13=~pxdf_pass2.Wavenumber.between(snr_c13[0][i],snr_c13[1][i])
         #This is for the extra ranges defined by the user
         if exclude_ranges==None:
             exclude_ranges=[]
 
         exclude_mask2 = pd.Series(False, index=pxdf_pass2.index)
         for r in exclude_ranges:
             exclude_mask2 |= (pxdf_pass2.Wavenumber >= r[0]) & (pxdf_pass2.Wavenumber <= r[1])
         not_exclude_mask2=~exclude_mask2
-        #This filters the dataframe
-        query_str2='maxpx_fact_pass2*minpx_fact_pass2 > @dynfact_2 & @not_diad1 & @not_diad2 & @not_hb1 & @not_hb2 and @not_c13 & @not_exclude_mask2'
+
+        #
+        if diad_peaks.empty==True:
+            query_str2='maxpx_fact_pass2*minpx_fact_pass2 > @dynfact_2 & @not_exclude_mask2'
+        else:
+            not_diad1=~pxdf_pass2.Wavenumber.between(snr_diad1[0][i],snr_diad1[1][i])
+            not_diad2=~pxdf_pass2.Wavenumber.between(snr_diad2[0][i],snr_diad2[1][i])
+
+            not_hb1=~pxdf_pass2.Wavenumber.between(snr_hb1[0][i],snr_hb1[1][i])
+            not_hb2=~pxdf_pass2.Wavenumber.between(snr_hb2[0][i],snr_hb2[1][i])
+            not_c13=~pxdf_pass2.Wavenumber.between(snr_c13[0][i],snr_c13[1][i])
+
+            #This filters the dataframe
+            query_str2='maxpx_fact_pass2*minpx_fact_pass2 > @dynfact_2 & @not_diad1 & @not_diad2 & @not_hb1 & @not_hb2 and @not_c13 & @not_exclude_mask2'
 
         rays_wavenumber_pass2=pxdf_pass2.query(query_str2)['Wavenumber']
         rays_intensity_pass2=pxdf_pass2.query(query_str2)['Intensity']
         rays_fact_pass2=pxdf_pass2.query(query_str2)['maxpx_fact_pass2*minpx_fact_pass2']
 
         # Removal of cosmic rays from the main dataframe (replaces intensity with NaN - only for plotting!)
         all_rayswave=pd.concat([rays_wavenumber, rays_wavenumber_pass2])
@@ -388,16 +407,16 @@
     if second_pass==False:
         clean_spec_df=pxdf[['Wavenumber','Intensity']]
 
     return record ,clean_spec_df
 
 ## Filter rays in a loop
 
-def filter_raysinloop(*,spectra_path=None,Diad_files=None, diad_peaks=None,fit_params=None,exclude_ranges=[],filetype='headless_txt',
-n=1,dynfact=0.01, dynfact_2=0.0005, export_cleanspec=True,plot_rays='all', save_fig='all', xlims=None):
+def filter_raysinloop(*,spectra_path=None,Diad_files=None, diad_peaks=None,exclude_ranges=[],filetype='headless_txt',
+n=1,dynfact=0.01, dynfact_2=0.0005, export_cleanspec=True,plot_rays='all', save_fig='all', xlims=None,fit_params=None, filename_col='filename'):
     """ This function is used to filter out cosmic rays in multiple Raman spectra of CO2 in a loop.
 
     Parameters
     --------------
     spectra_path: str
         The folder path of the spectrum files
     Diad_files: pd.Series
@@ -405,15 +424,17 @@
     filetype: str
         Identifies type of file
         choose from 'Witec_ASCII', 'headless_txt', 'headless_csv', 'head_csv', 'Witec_ASCII',
         'HORIBA_txt', 'Renishaw_txt'
     diad_peaks: pd.DataFrame
         Dataframe containing the peaks of interest for each file subset from fit_params variable output by pf.loop_approx_diad_fits(columns Diad1_pos,	Diad2_pos,HB1_pos,HB2_pos,C13_pos)
     fit_params: pd.DataFrame
-        Dataframe output as fit_params from pf.loop_approx_diad_fits
+        Dataframe containing peak fits and filenames. Used to be called fit_params, still works.
+    filename_col: str
+        Column name that contains the filenames in fit_params, this is used to merge the new CRR filenames
     exclude_ranges: tuple list
         List of tuples containing ranges for user-defined peaks of interest to exclude from ray-filtering.
     filetype: str ('headless_txt')
         Sets the filetype of the spectrum file
     n: int
         Neighbor pixels to consider, 1 is typically enough.
     dynfact: float or int
@@ -433,36 +454,40 @@
     -------------
     data_y_all_CRR_DiadFit: np.array
         Array containing all cleaned spectra for plotting
     fit_params_CRR_DiadFit: pd.DataFrame
         fit_params DataFrame output from pf.loop_approx_diad_fits with updated filenames when cosmic rays were found and a new column indicating if cosmic rays were found
 
     """
+
     try:
-        check_pars(plot_rays, save_fig,export_cleanspec,exclude_ranges)
+        check_pars(plot_rays, save_fig,export_cleanspec,exclude_ranges,Diad_files,diad_peaks)
     except ValueError as e:
         print(str(e))
         raise e
 
     ray_list=pd.DataFrame([])
     spectra_df=pd.DataFrame([])
 
     for i in tqdm(Diad_files.index.tolist()):
 
 
         filename_select=Diad_files.iloc[i]
 
-        rays_found,spectrum=filter_singleray(path=spectra_path,Diad_files=Diad_files,i=i,diad_peaks=diad_peaks,exclude_ranges=exclude_ranges,plot_rays=plot_rays,
-                                 export_cleanspec=export_cleanspec,save_fig=save_fig,dynfact=dynfact,dynfact_2=dynfact_2,n=n,xlims=xlims,filetype=filetype)
+        rays_found,spectrum=pf.filter_singleray(path=spectra_path,Diad_files=Diad_files,i=i,diad_peaks=diad_peaks,exclude_ranges=exclude_ranges,plot_rays=plot_rays,
+                                export_cleanspec=export_cleanspec,save_fig=save_fig,dynfact=dynfact,dynfact_2=dynfact_2,n=n,xlims=xlims,filetype=filetype)
+
         ray_list=pd.concat([ray_list,rays_found])
         spectra_df=pd.concat([spectra_df,spectrum['Intensity']],axis=1)
 
     ray_list=ray_list.reset_index(drop=True)
 
     # this is the new data_y_all array, contains all intensities for the spectra, with rays removed.
     data_y_all_CRR_DiadFit=spectra_df.to_numpy()
 
-    # This merges the results of the CRR filtering loop back in with the fit_parameters (filenames for which CRR detected are replaced by filename_CRR_DiadFit
-    fit_params_CRR_DiadFit=pd.merge(ray_list, fit_params, on='filename', how='outer')
-    fit_params_CRR_DiadFit.loc[fit_params_CRR_DiadFit['rays_present']==True, 'filename']=fit_params_CRR_DiadFit['filename'].str.replace('.txt', '',regex=True)+'_CRR_DiadFit.txt'
+
+    # # This merges the results of the CRR filtering loop back in with the fit_parameters (filenames for which CRR detected are replaced by filename_CRR_DiadFit
+    fit_params_CRR_DiadFit=pd.merge(left=ray_list, right=fit_params, left_on='filename',right_on=filename_col, how='outer')
+    fit_params_CRR_DiadFit.loc[fit_params_CRR_DiadFit['rays_present']==True, filename_col]=fit_params_CRR_DiadFit[filename_col].str.replace('.txt', '',regex=True)+'_CRR_DiadFit.txt'
     display(fit_params_CRR_DiadFit.head())
+
     return data_y_all_CRR_DiadFit,fit_params_CRR_DiadFit
```

### Comparing `DiadFit-0.0.57/src/DiadFit/densimeters.py` & `DiadFit-0.0.59/src/DiadFit/densimeters.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import re
 from os import listdir
 from os.path import isfile, join
 
 encode="ISO-8859-1"
 
 
-def calculate_density_cornell(temp='SupCrit', Split=None):
+def calculate_density_cornell(*, temp='SupCrit', Split, split_err=None):
     """ This function converts Diad Splitting into CO$_2$ density using the densimeters of DeVitre et al. (2021)
     This should only be used for the Cornell Raman, not other Ramans at present
 
     Parameters
     -------------
     temp: str
         'SupCrit' if measurements done at 37C
@@ -166,8 +166,43 @@
     df.loc[roomT&Upper_Cal_RT, 'Notes']='Above upper Cali Limit'
     df.loc[roomT&Upper_Cal_RT, 'in range']='N'
 
     df.loc[SupCrit&Upper_Cal_SC, 'Preferred D'] = HighD_SC
     df.loc[SupCrit&Upper_Cal_SC, 'Notes']='Above upper Cali Limit'
     df.loc[SupCrit&Upper_Cal_SC, 'in range']='N'
 
-    return df
+    if split_err is not None:
+        df2=calculate_dens_error(temp, Split, split_err)
+
+        df.insert(1, 'dens+1σ', df2['max_dens'])
+        df.insert(1, 'dens-1σ', df2['min_dens'])
+        df.insert(3, '1σ', (df2['max_dens']-df2['min_dens'])/2 )
+
+    return df
+
+def calculate_dens_error(temp, Split, split_err):
+
+    max_dens=calculate_density_cornell(temp=temp, Split=Split+split_err)
+    min_dens=calculate_density_cornell(temp=temp, Split=Split-split_err)
+    df=pd.DataFrame(data={
+                        'max_dens': max_dens['Preferred D'],
+                        'min_dens': min_dens['Preferred D']})
+
+    return df
+
+
+def propagate_errors_for_splitting(Ne_corr, df_sorted):
+    """ This function propagates errors in your Ne correection model and peak fits by quadrature
+
+    """
+    Ne_err=(Ne_corr['upper_values']-Ne_corr['lower_values'])/2
+    Diad1_err=df_sorted['Diad1_cent_err'].fillna(0)
+    Diad2_err=df_sorted['Diad2_cent_err'].fillna(0)
+    split_err=(Diad1_err**2 + Diad2_err**2)**0.5
+    Combo_err= (((df_sorted['Splitting']* (Ne_err))**2) +  (Ne_corr['preferred_values'] *split_err  )**2 )**0.5
+
+    return Combo_err
+
+
+
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `DiadFit-0.0.57/src/DiadFit/density_depth_crustal_profiles.py` & `DiadFit-0.0.59/src/DiadFit/density_depth_crustal_profiles.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.57/src/DiadFit/diads.py` & `DiadFit-0.0.59/src/DiadFit/diads.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 from os.path import isfile, join
 from DiadFit.importing_data_files import *
 from typing import Tuple, Optional
 from dataclasses import dataclass
 import matplotlib.patches as patches
 import warnings as w
 from tqdm import tqdm
+from numpy import trapz
+from scipy.integrate import simps
+from scipy.interpolate import interp1d
 
 # For debuggin
 
 #import warnings
 #warnings.simplefilter('error')
 
 encode="ISO-8859-1"
@@ -863,14 +866,15 @@
             ax0.set_yticks([])
 
             # av_prom_Group1=np.abs(np.nanmedian(Group1_df[x_param])/intc)
             # ax0.plot(x_cord, Group1_np_y[:, i]+av_prom_Group1*i, '-r')
 
         if sum(~grp1)>0:
 
+
             if sum(~grp1)==1:
                 j=0
                 av_prom_disc=np.abs(np.nanmedian(Groupnot1_df['Diad1_abs_prom'])/intc)
                 Diff=np.nanmax(Groupnot1_np_y[:, j])-np.nanmin(Groupnot1_np_y[:, j])
                 ax1.plot(x_cord-j*5,
                 (Groupnot1_np_y[:, j]-np.nanmin(Groupnot1_np_y[:, j]))/Diff+j/3, '-k', lw=0.5)
 
@@ -1411,14 +1415,15 @@
     ydat_inrange: np.array of data within 'span'
     xdat_inrange:np.array of data within 'span'
 
 
 
     """
 
+
     # Calculate the amplitude from the sigma and the prominence
     calc_diad_amplitude=((config1.diad_sigma)*(config1.diad_prom))/0.3939
     calc_HB_amplitude=((config1.diad_sigma)*(config1.HB_prom))/0.3939
     if diad2 is True and fit_peaks==3:
         calc_C13_amplitude=(0.5*(config1.diad_sigma)*(config1.C13_prom))/0.3939
     # Gets overridden if you have triggered any of the warnings
     refit=False
@@ -1475,14 +1480,15 @@
             pars1 = model_F.make_params()
             pars1['lz1_'+ 'amplitude'].set(calc_diad_amplitude, min=0, max=calc_diad_amplitude*10)
             pars1['lz1_'+ 'center'].set(Center_ini, min=Center_ini-5*spec_res, max=Center_ini+5*spec_res)
             pars1['lz1_'+ 'sigma'].set(config1.diad_sigma, min=config1.diad_sigma*config1.diad_sigma_min_allowance,
                          max=config1.diad_sigma*config1.diad_sigma_max_allowance)
             params=pars1
 
+
         # If there is more than one peak
         else:
             # Set up Lz1 the same for all situations
             if config1.model_name=='VoigtModel':
                 model1 = VoigtModel(prefix='lz1_')# + ConstantModel(prefix='c1')
             if config1.model_name=='PseudoVoigtModel':
                 model1 = PseudoVoigtModel(prefix='lz1_') #+ ConstantModel(prefix='c1')
@@ -1493,14 +1499,16 @@
             pars1['lz1_'+ 'center'].set(Center_ini, min=Center_ini-3*spec_res, max=Center_ini+3*spec_res)
 
             pars1['lz1_'+ 'sigma'].set(config1.diad_sigma, min=config1.diad_sigma*config1.diad_sigma_min_allowance,
                         max=config1.diad_sigma*config1.diad_sigma_max_allowance)
 
 
 
+
+
             if fit_peaks>1:
                 model_F=model1
                 params=pars1
 
             if fit_peaks==2:
 
                 # Second wee peak
@@ -1516,17 +1524,36 @@
                     min=HB_initial_guess-2*spec_res, max=HB_initial_guess+2)
 
                 pars[prefix + 'amplitude'].set(calc_HB_amplitude, min=Amplitude_ini*config1.HB_amp_min_allowance, max=Amplitude_ini*config1.HB_amp_max_allowance)
                 pars[prefix+ 'sigma'].set(sigma_ini, min=sigma_ini*config1.HB_sigma_min_allowance, max=sigma_ini*config1.HB_sigma_max_allowance)
 
 
                 model_F=model1+peak
+
+                # updating pars 1 with values in pars
                 pars1.update(pars)
                 params=pars1
 
+
+                # Attempt at stabilizing peak fit
+                result = model_F.fit(ydat, pars1, x=xdat)
+                result.params['lz2_center'].vary = False
+                result.params['lz2_amplitude'].vary = False
+                result.params['lz2_sigma'].vary = False
+                final_result = model_F.fit(ydat, result.params, x=xdat)
+                params.update(final_result.params)
+                params.update(final_result.params)
+                result=final_result
+
+
+
+
+
+
+
             if fit_peaks==3:
                 if block_print is False:
                     print('Trying to iteratively fit 3 peaks')
 
                 peak_pos_left=np.array([HB_initial_guess, C13_initial_guess])
 
                 for i, cen in enumerate(peak_pos_left):
@@ -1551,18 +1578,36 @@
                         amplitude=calc_C13_amplitude,
                         min_amplitude=calc_C13_amplitude*(0.5*config1.HB_amp_min_allowance),
                         max_amplitude=calc_C13_amplitude*2*(config1.HB_amp_max_allowance),
                         model_name=config1.model_name)
                         model = peak+model
                         params.update(pars)
 
+
+
+
                 model_F=model
 
 
 
+                # Attempt at stabilizing peak fit
+                result = model_F.fit(ydat, pars1, x=xdat)
+                result.params['lz2_center'].vary = False
+                result.params['lz2_amplitude'].vary = False
+                result.params['lz2_sigma'].vary = False
+                result.params['lz3_center'].vary = False
+                result.params['lz3_amplitude'].vary = False
+                result.params['lz3_sigma'].vary = False
+                final_result = model_F.fit(ydat, result.params, x=xdat)
+                params.update(final_result.params)
+                params.update(final_result.params)
+                result=final_result
+
+
+
 
     # Same, but also with a Gaussian Background
     if config1.fit_gauss is not False:
 
 
         # making the gaussian model
         model1 = GaussianModel(prefix='bkg_')
@@ -1599,14 +1644,35 @@
                         min_amplitude=Amplitude_ini*config1.HB_amp_min_allowance,
                         max_amplitude=Amplitude_ini*config1.HB_amp_max_allowance,
                         model_name=config1.model_name)
                     model2 = peak+model
                     params.update(pars)
 
 
+            # Attempt at stabilizing peak fit
+# updating pars 1 with values in pars
+
+            result = model2.fit(ydat, params, x=xdat)
+
+
+            # Set the parameters of 'lz1' to be fixed
+            result.params['lz2_center'].vary = False
+            result.params['lz2_amplitude'].vary = False
+            result.params['lz2_sigma'].vary = False
+            result.params['bkg_center'].vary = False
+            result.params['bkg_amplitude'].vary = False
+            result.params['bkg_sigma'].vary = False
+
+            # Perform fitting using the entire model (model2) with the stabilized 'lz1' parameters
+            final_result = model2.fit(ydat, result.params, x=xdat)
+            center_error = final_result.params['lz1_center'].stderr
+            params.update(final_result.params)
+
+
+            result=final_result
             model_F=model2
 
 
         if fit_peaks==3:
             peak_pos_voigt=np.array([initial_guess, HB_initial_guess, C13_initial_guess])
 
             for i, cen in enumerate(peak_pos_voigt):
@@ -1641,69 +1707,101 @@
                         sigma=sigma_ini/5,
                         min_sigma=sigma_ini/20,
                         max_sigma=sigma_ini/2,
                         amplitude=calc_C13_amplitude,
                         min_amplitude=calc_C13_amplitude*(0.5*config1.HB_amp_min_allowance),
                         max_amplitude=calc_C13_amplitude*2*(config1.HB_amp_max_allowance),
                         model_name=config1.model_name)
+                    model3 = peak+model2
+                    params.update(pars)
 
+            result = model3.fit(ydat, params, x=xdat)
 
 
+            # Set the parameters of 'lz1' to be fixed
+            result.params['lz2_center'].vary = False
+            result.params['lz2_amplitude'].vary = False
+            result.params['lz2_sigma'].vary = False
+            result.params['lz3_center'].vary = False
+            result.params['lz3_amplitude'].vary = False
+            result.params['lz3_sigma'].vary = False
+            result.params['bkg_center'].vary = False
+            result.params['bkg_amplitude'].vary = False
+            result.params['bkg_sigma'].vary = False
+
+            # Perform fitting using the entire model (model2) with the stabilized 'lz1' parameters
+            final_result = model3.fit(ydat, result.params, x=xdat)
+            center_error = final_result.params['lz1_center'].stderr
 
-
-                    model3 = peak+model2
-                    params.update(pars)
+            result=final_result
             model_F=model3
 
+            params.update(final_result.params)
+
+
 
 
 
 
 
 
 
     # Regardless of fit, evaluate model
     init = model_F.eval(params, x=xdat)
     result = model_F.fit(ydat, params, x=xdat)
     comps = result.eval_components()
 
+    #print(result.ci_report())
+
+    #print(result.conf_interval(method='bootstrap'))
+
     #print(result.fit_report(min_correl=0.5))
     # Check if function gives error bars
-    Error_bars=result.errorbars
-    if Error_bars is False:
-        if block_print is False:
-            print('Error bars not determined by function')
 
+
+    #print(result.best_values)
     # Get first peak center
     Peak1_Cent=result.best_values.get('lz1_center')
     Peak1_Int=result.best_values.get('lz1_amplitude')
     Peak1_Sigma=result.best_values.get('lz1_sigma')
     Peak1_gamma=result.best_values.get('lz1_gamma')
     Peak1_Prop_Lor=result.best_values.get('lz1_fraction')
     Peak1_fwhm=result.params['lz1_fwhm'].value
 
+    Center_pk2_error=result.params.get('lz1_center')
+
+    error_pk2 = result.params['lz1_center'].stderr
+
+
+
     x_lin=np.linspace(span[0], span[1], 2000)
     y_best_fit=result.eval(x=x_lin)
     components=result.eval_components(x=x_lin)
 
-    # Checking whether you need any flags.
+    #Checking whether you need any flags.
+    if error_pk2 is None:
+        refit=True
+        refit_param=str(refit_param)+' No Error'
+
 
     if Peak1_Int>=(calc_diad_amplitude*10-0.1):
         refit=True
         refit_param=str(refit_param)+' V_LowAmp'
     if Peak1_Sigma>=(calc_diad_amplitude*10-0.1):
         refit=True
         refit_param=str(refit_param)+' V_HighAmp'
     if Peak1_Sigma>=(config1.diad_sigma*config1.diad_sigma_max_allowance-0.001):
         refit=True
         refit_param=str(refit_param)+' V_input_TooLowSigma'
     if Peak1_Sigma<=(config1.diad_sigma*config1.diad_sigma_min_allowance+0.001):
         refit=True
         refit_param=str(refit_param)+' V_input_TooHighSigma'
 
+    #if findme
+
 
     if config1.fit_gauss is not False:
         Gauss_cent=result.best_values.get('bkg_center')
         Gauss_amp=result.best_values.get('bkg_amplitude')
         Gauss_sigma=result.best_values.get('bkg_sigma')
 
         max_Gauss=np.max(components.get('bkg_'))
@@ -1771,14 +1869,15 @@
             Peak3_Sigma=result.best_values.get('lz3_sigma')
 
             ax1_xlim=[Center_ini-30, Center_ini+30]
             ax2_xlim=[Center_ini-30, Center_ini+30]
 
         if Peak2_Cent is None:
             df_out=pd.DataFrame(data={'Diad2_Voigt_Cent': Peak1_Cent,
+                                    'Diad2_cent_err': error_pk2,
                                     'Diad2_Voigt_Area': Peak1_Int,
                                 'Diad2_Voigt_Sigma': Peak1_Sigma,
                                 'Diad2_Voigt_Gamma': Peak1_gamma,
 
 
             }, index=[0])
 
@@ -1840,14 +1939,15 @@
                     C13_Int=Peak1_Int
                     C13_Sigma=Peak1_Sigma
                 if C13_Cent==Peak3_Cent:
                     C13_Int=Peak3_Int
                     C13_Sigma=Peak3_Sigma
 
             df_out=pd.DataFrame(data={'Diad2_Voigt_Cent': Diad2_Cent,
+            'Diad2_cent_err': error_pk2,
                                     'Diad2_Voigt_Area': Diad2_Int,
                                     'Diad2_Voigt_Sigma': Peak1_Sigma,
                                     'Diad2_Voigt_Gamma': Peak1_gamma,
             }, index=[0])
 
             df_out['HB2_Cent']=HB2_Cent
             df_out['HB2_Area']=HB2_Int
@@ -1972,27 +2072,29 @@
             ax1_xlim=[Center_ini-30, Center_ini+15]
             ax2_xlim=[Center_ini-30, Center_ini+15]
 
 
 
         if Peak2_Cent is None:
             df_out=pd.DataFrame(data={'Diad1_Voigt_Cent': Peak1_Cent,
+            'Diad1_cent_err': error_pk2,
                                     'Diad1_Voigt_Area': Peak1_Int,
                                 'Diad1_Voigt_Sigma': Peak1_Sigma,
                                 'Diad1_Voigt_Gamma': Peak1_gamma,
 
 
             }, index=[0])
         if Peak2_Cent is not None:
 
 
 
 
 
             df_out=pd.DataFrame(data={'Diad1_Voigt_Cent': Peak1_Cent,
+            'Diad1_cent_err': error_pk2,
                                     'Diad1_Voigt_Area': Peak1_Int,
                                     'Diad1_Voigt_Sigma': Peak1_Sigma,
                                     'Diad1_Voigt_Gamma': Peak1_gamma,
             }, index=[0])
 
             df_out['HB1_Cent']=Peak2_Cent
             df_out['HB1_Area']=Peak2_Int
@@ -2089,15 +2191,15 @@
         best_fit=result.best_fit
 
         df_out['Diad1_refit']=refit_param
 
         # Final check - that Gaussian isnt anywhere near the height of the diad
 
 
-
+    df_out=df_out.fillna(0)
 
     return result, df_out, y_best_fit, x_lin, components, xdat, ydat, ax1_xlim, ax2_xlim, residual_diad_coords, ydat_inrange,  xdat_inrange
 
 
 
 def fit_diad_2_w_bck(*, config1: diad2_fit_config=diad2_fit_config(), config2: diad_id_config=diad_id_config(),
     path=None, filename=None, peak_pos_voigt=None,filetype=None,
@@ -2260,18 +2362,25 @@
 
 
 
 
     # Try Refitting once
     if str(df_out['Diad2_refit'].iloc[0])!='Flagged Warnings:':
         print('refit attempt 1')
-        print(str(df_out['Diad2_refit'].iloc[0]))
-        config_tweaked=config1
         factor=2
 
+        import copy
+        config_tweaked=config1
+        config_tweaked=copy.copy(config1)
+
+        if any(df_out['Diad2_refit'].str.contains(' No Error')):
+            if config1.fit_peaks>1:
+                config_tweaked.fit_peaks=config1.fit_peaks-1
+                fit_peaks=config_tweaked.fit_peaks
+
 
 
         # if any(df_out['Diad2_refit'].str.contains('V_HighAmp')):
         #     config_tweaked.diad_amplitude=calc_diad_amplitude/10
         if any(df_out['Diad2_refit'].str.contains('V_input_TooLowSigma')):
             config_tweaked.diad_sigma=config1.diad_sigma*factor
         if any(df_out['Diad2_refit'].str.contains('V_input_TooHighSigma')):
@@ -2293,22 +2402,23 @@
         #     config_tweaked.HB_amplitude=calc_HB_amplitude/2
         # if any(df_out['Diad2_refit'].str.contains('HB2_HighAmp')):
         #     config_tweaked.HB_amplitude=calc_HB_amplitude*2
 
 
         result, df_out, y_best_fit, x_lin, components, xdat, ydat, ax1_xlim, ax2_xlim,residual_diad_coords, ydat_inrange,  xdat_inrange=fit_gaussian_voigt_generic_diad(config_tweaked, diad2=True, path=path, filename=filename,
          xdat=x_diad2, ydat=y_corr_diad2,
-    span=span_diad2, plot_figure=False, Diad_pos=Diad_pos, HB_pos=HB_pos, C13_pos=C13_pos, fit_peaks=fit_peaks)
+    span=span_diad2, plot_figure=False, Diad_pos=Diad_pos, HB_pos=HB_pos, C13_pos=C13_pos, fit_peaks=config_tweaked.fit_peaks)
         i=2
         while str(df_out['Diad2_refit'].iloc[0])!='Flagged Warnings:':
 
             print('refit attempt  ='+str(i) + ', '+str(df_out['Diad2_refit'].iloc[0]))
             print(df_out['Diad2_refit'].iloc[0])
 
-            config_tweaked2=config_tweaked
+
+            config_tweaked2=copy.copy(config_tweaked)
             factor2=factor*2
 
             #
             # if any(df_out['Diad2_refit'].str.contains('V_LowAmp')):
             #     config_tweaked2.diad_amplitude=config_tweaked.diad_amplitude*10
             # if any(df_out['Diad2_refit'].str.contains('V_HighAmp')):
             #     config_tweaked2.diad_amplitude=config_tweaked.diad_amplitude/10
@@ -2332,15 +2442,15 @@
         #     if any(df_out['Diad2_refit'].str.contains('HB2_LowAmp')):
         #         config_tweaked2.HB_amplitude=config_tweaked.HB_amplitude/2
         #     if any(df_out['Diad2_refit'].str.contains('HB2_HighAmp')):
         #         config_tweaked2.HB_amplitude=config_tweaked.HB_amplitude*2
 
 
             result, df_out, y_best_fit, x_lin, components, xdat, ydat, ax1_xlim, ax2_xlim,residual_diad_coords, ydat_inrange,  xdat_inrange=fit_gaussian_voigt_generic_diad(config_tweaked2, diad2=True, path=path, filename=filename,
-        xdat=x_diad2, ydat=y_corr_diad2, span=span_diad2, plot_figure=False, Diad_pos=Diad_pos, HB_pos=HB_pos, C13_pos=C13_pos, fit_peaks=fit_peaks)
+        xdat=x_diad2, ydat=y_corr_diad2, span=span_diad2, plot_figure=False, Diad_pos=Diad_pos, HB_pos=HB_pos, C13_pos=C13_pos, fit_peaks=config_tweaked.fit_peaks)
             i=i+1
             if i>5:
                 print('Got to 5 iteratoins and still couldnt adjust the fit parameters')
                 break
 
 
     # get a best fit to the baseline using a linspace from the peak fitting
@@ -2349,205 +2459,206 @@
     # We extract the full spectra to plot at the end, and convert to a dataframe
     Spectra_df=get_data(path=path, filename=filename, filetype=filetype)
     Spectra=np.array(Spectra_df)
 
 
 
     # Make nice figure
+    if plot_figure is True:
 
-    figure_mosaic="""
-    XY
-    AB
-    CD
-    EE
-    """
+        figure_mosaic="""
+        XY
+        AB
+        CD
+        EE
+        """
 
-    fig,axes=plt.subplot_mosaic(mosaic=figure_mosaic, figsize=(12, 16))
-    if df_out['Diad2_refit'] is not False:
-        fig.suptitle('Diad 2, file= '+ str(filename) + ' \n' + str(df_out['Diad2_refit'].iloc[0]), fontsize=16, x=0.5, y=1.0)
-    else:
-        fig.suptitle('Diad 2, file= '+ str(filename), fontsize=16, x=0.5, y=1.0)
-    # Background plot for real
+        fig,axes=plt.subplot_mosaic(mosaic=figure_mosaic, figsize=(12, 16))
+        if df_out['Diad2_refit'] is not False:
+            fig.suptitle('Diad 2, file= '+ str(filename) + ' \n' + str(df_out['Diad2_refit'].iloc[0]), fontsize=16, x=0.5, y=1.0)
+        else:
+            fig.suptitle('Diad 2, file= '+ str(filename), fontsize=16, x=0.5, y=1.0)
+        # Background plot for real
 
-    # Plot best fit on the LHS, and individual fits on the RHS at the top
+        # Plot best fit on the LHS, and individual fits on the RHS at the top
 
-    axes['X'].set_title('a) Background fit')
-    axes['X'].plot(Diad[:, 0], Diad[:, 1], '-', color='grey')
-    axes['X'].plot(Diad_short_diad2[:, 0], Diad_short_diad2[:, 1], '-r', label='Spectra')
+        axes['X'].set_title('a) Background fit')
+        axes['X'].plot(Diad[:, 0], Diad[:, 1], '-', color='grey')
+        axes['X'].plot(Diad_short_diad2[:, 0], Diad_short_diad2[:, 1], '-r', label='Spectra')
 
-    #axes['X'].plot(Baseline[:, 0], Baseline[:, 1], '-b', label='Bck points')
-    axes['X'].plot(Baseline_diad2[:, 0], Baseline_diad2[:, 1], '.b', label='bel. Bck. pts')
-    axes['X'].plot(Diad_short_diad2[:, 0], Py_base_diad2, '-k', label='bck. poly fit')
+        #axes['X'].plot(Baseline[:, 0], Baseline[:, 1], '-b', label='Bck points')
+        axes['X'].plot(Baseline_diad2[:, 0], Baseline_diad2[:, 1], '.b', label='bel. Bck. pts')
+        axes['X'].plot(Diad_short_diad2[:, 0], Py_base_diad2, '-k', label='bck. poly fit')
 
 
 
-    ax1_ymin=np.min(Baseline_diad2[:, 1])-10*np.std(Baseline_diad2[:, 1])
-    ax1_ymax=np.max(Baseline_diad2[:, 1])+10*np.std(Baseline_diad2[:, 1])
-    ax1_xmin=config1.lower_bck_diad2[0]-30
-    ax1_xmax=config1.upper_bck_diad2[1]+30
-    # Adding patches
+        ax1_ymin=np.min(Baseline_diad2[:, 1])-10*np.std(Baseline_diad2[:, 1])
+        ax1_ymax=np.max(Baseline_diad2[:, 1])+10*np.std(Baseline_diad2[:, 1])
+        ax1_xmin=config1.lower_bck_diad2[0]-30
+        ax1_xmax=config1.upper_bck_diad2[1]+30
+        # Adding patches
 
 
-    rect_diad2_b1=patches.Rectangle((config1.lower_bck_diad2[0], ax1_ymin),config1.lower_bck_diad2[1]-config1.lower_bck_diad2[0],ax1_ymax-ax1_ymin,
-                            linewidth=1,edgecolor='none',facecolor='cyan', label='sel. bck. region', alpha=0.3, zorder=0)
-    axes['X'].add_patch(rect_diad2_b1)
-    rect_diad2_b2=patches.Rectangle((config1.upper_bck_diad2[0], ax1_ymin),config1.upper_bck_diad2[1]-config1.upper_bck_diad2[0],ax1_ymax-ax1_ymin,
-                            linewidth=1,edgecolor='none',facecolor='cyan', alpha=0.3, zorder=0)
-    axes['X'].add_patch(rect_diad2_b2)
-    axes['X'].set_xlim([ax1_xmin, ax1_xmax])
-    axes['X'].set_ylim([ax1_ymin, ax1_ymax])
+        rect_diad2_b1=patches.Rectangle((config1.lower_bck_diad2[0], ax1_ymin),config1.lower_bck_diad2[1]-config1.lower_bck_diad2[0],ax1_ymax-ax1_ymin,
+                                linewidth=1,edgecolor='none',facecolor='cyan', label='sel. bck. region', alpha=0.3, zorder=0)
+        axes['X'].add_patch(rect_diad2_b1)
+        rect_diad2_b2=patches.Rectangle((config1.upper_bck_diad2[0], ax1_ymin),config1.upper_bck_diad2[1]-config1.upper_bck_diad2[0],ax1_ymax-ax1_ymin,
+                                linewidth=1,edgecolor='none',facecolor='cyan', alpha=0.3, zorder=0)
+        axes['X'].add_patch(rect_diad2_b2)
+        axes['X'].set_xlim([ax1_xmin, ax1_xmax])
+        axes['X'].set_ylim([ax1_ymin, ax1_ymax])
 
-    axes['X'].set_ylabel('Intensity')
-    axes['Y'].set_ylabel('Intensity')
-    axes['Y'].set_xlabel('Wavenumber')
-    axes['X'].legend()
+        axes['X'].set_ylabel('Intensity')
+        axes['Y'].set_ylabel('Intensity')
+        axes['Y'].set_xlabel('Wavenumber')
+        axes['X'].legend()
 
 
 
-    axes['Y'].set_title('b) Background subtracted spectra')
-    axes['Y'].plot(x_diad2, y_corr_diad2, '-r')
-    height_p=np.max(Diad_short_diad2[:, 1])-np.min(Diad_short_diad2[:, 1])
-    axes['Y'].set_ylim([np.min(y_corr_diad2), 1.2*height_p ])
-    axes['X'].set_xlabel('Wavenumber')
+        axes['Y'].set_title('b) Background subtracted spectra')
+        axes['Y'].plot(x_diad2, y_corr_diad2, '-r')
+        height_p=np.max(Diad_short_diad2[:, 1])-np.min(Diad_short_diad2[:, 1])
+        axes['Y'].set_ylim([np.min(y_corr_diad2), 1.2*height_p ])
+        axes['X'].set_xlabel('Wavenumber')
 
 
 
-    axes['A'].plot(xdat, ydat,  '.k', label='bck. sub. data')
-    axes['A'].plot( x_lin ,y_best_fit, '-g', linewidth=1, label='best fit')
-    axes['A'].legend()
-    axes['A'].set_ylabel('Intensity')
-    axes['A'].set_xlabel('Wavenumber')
-    axes['A'].set_xlim(ax1_xlim)
-    axes['A'].set_title('c) Overall Best Fit')
+        axes['A'].plot(xdat, ydat,  '.k', label='bck. sub. data')
+        axes['A'].plot( x_lin ,y_best_fit, '-g', linewidth=1, label='best fit')
+        axes['A'].legend()
+        axes['A'].set_ylabel('Intensity')
+        axes['A'].set_xlabel('Wavenumber')
+        axes['A'].set_xlim(ax1_xlim)
+        axes['A'].set_title('c) Overall Best Fit')
 
-   # individual fits
-    axes['B'].plot(xdat, ydat, '.k')
+    # individual fits
+        axes['B'].plot(xdat, ydat, '.k')
 
-    # This is for if there is more than 1 peak, this is when we want to plot the best fit
+        # This is for if there is more than 1 peak, this is when we want to plot the best fit
 
-    if fit_peaks>1:
+        if fit_peaks>1:
 
 
-        axes['B'].plot(x_lin, components.get('lz2_'), '-r', linewidth=2, label='HB2')
+            axes['B'].plot(x_lin, components.get('lz2_'), '-r', linewidth=2, label='HB2')
 
-    axes['B'].plot(x_lin, components.get('lz1_'), '-b', linewidth=2, label='Diad2')
-    if config1.fit_gauss is not False:
-        axes['B'].plot(x_lin, components.get('bkg_'), '-m', label='Gaussian bck', linewidth=2)
-    #ax2.plot(xdat, result.best_fit, '-g', label='best fit')
-    axes['B'].legend()
+        axes['B'].plot(x_lin, components.get('lz1_'), '-b', linewidth=2, label='Diad2')
+        if config1.fit_gauss is not False:
+            axes['B'].plot(x_lin, components.get('bkg_'), '-m', label='Gaussian bck', linewidth=2)
+        #ax2.plot(xdat, result.best_fit, '-g', label='best fit')
+        axes['B'].legend()
 
-    fitspan=max(y_best_fit)-min(y_best_fit)
-    axes['B'].set_ylim([min(y_best_fit)-fitspan/5, max(y_best_fit)+fitspan/5])
+        fitspan=max(y_best_fit)-min(y_best_fit)
+        axes['B'].set_ylim([min(y_best_fit)-fitspan/5, max(y_best_fit)+fitspan/5])
 
-    axes['B'].set_ylabel('Intensity')
-    axes['B'].set_xlabel('Wavenumber')
+        axes['B'].set_ylabel('Intensity')
+        axes['B'].set_xlabel('Wavenumber')
 
 
-    axes['B'].set_xlim(ax2_xlim)
+        axes['B'].set_xlim(ax2_xlim)
 
-    # Dashed lines so matches part D
+        # Dashed lines so matches part D
 
-    axes['B'].plot([df_out['Diad2_Voigt_Cent'], df_out['Diad2_Voigt_Cent']], [np.min(ydat), np.max(ydat)], ':b')
+        axes['B'].plot([df_out['Diad2_Voigt_Cent'], df_out['Diad2_Voigt_Cent']], [np.min(ydat), np.max(ydat)], ':b')
 
 
-    if fit_peaks>=2:
-            axes['B'].plot([df_out['HB2_Cent'], df_out['HB2_Cent']], [np.min(ydat), np.max(ydat)], ':r')
+        if fit_peaks>=2:
+                axes['B'].plot([df_out['HB2_Cent'], df_out['HB2_Cent']], [np.min(ydat), np.max(ydat)], ':r')
 
-    axes['B'].set_title('c) Fit Components')
+        axes['B'].set_title('c) Fit Components')
 
-    # Background fit
+        # Background fit
 
-    # First, set up x and y limits on axis
+        # First, set up x and y limits on axis
 
-    if config1.x_range_baseline is not None:
-        axc_xmin=df_out['Diad2_Voigt_Cent'][0]-config1.x_range_baseline
-        axc_xmax=df_out['Diad2_Voigt_Cent'][0]+config1.x_range_baseline
-    else:
-        axc_xmin=config1.lower_bck_diad2[0]
-        axc_xmax=config1.upper_bck_diad2[1]
-    axc_ymin=np.min(Baseline_diad2[:, 1])-config1.y_range_baseline/3
-    axc_ymax=np.max(Baseline_diad2[:, 1])+config1.y_range_baseline
+        if config1.x_range_baseline is not None:
+            axc_xmin=df_out['Diad2_Voigt_Cent'][0]-config1.x_range_baseline
+            axc_xmax=df_out['Diad2_Voigt_Cent'][0]+config1.x_range_baseline
+        else:
+            axc_xmin=config1.lower_bck_diad2[0]
+            axc_xmax=config1.upper_bck_diad2[1]
+        axc_ymin=np.min(Baseline_diad2[:, 1])-config1.y_range_baseline/3
+        axc_ymax=np.max(Baseline_diad2[:, 1])+config1.y_range_baseline
 
-    rect_diad2_b1=patches.Rectangle((config1.lower_bck_diad2[0],axc_ymin),config1.lower_bck_diad2[1]-config1.lower_bck_diad2[0],axc_ymax-axc_ymin,
-                              linewidth=1,edgecolor='none',facecolor='cyan', label='bck', alpha=0.3, zorder=0)
+        rect_diad2_b1=patches.Rectangle((config1.lower_bck_diad2[0],axc_ymin),config1.lower_bck_diad2[1]-config1.lower_bck_diad2[0],axc_ymax-axc_ymin,
+                                linewidth=1,edgecolor='none',facecolor='cyan', label='bck', alpha=0.3, zorder=0)
 
 
 
-    axes['C'].set_title('d) Peaks overlain on data before subtraction')
-    axes['C'].plot(Diad_short_diad2[:, 0], Diad_short_diad2[:, 1], '.r', label='data')
-    axes['C'].plot(Baseline_diad2[:, 0], Baseline_diad2[:, 1], '.b', label='bck')
-    axes['C'].plot(Diad_short_diad2[:, 0], Py_base_diad2, '-k', label='Poly bck fit')
+        axes['C'].set_title('d) Peaks overlain on data before subtraction')
+        axes['C'].plot(Diad_short_diad2[:, 0], Diad_short_diad2[:, 1], '.r', label='data')
+        axes['C'].plot(Baseline_diad2[:, 0], Baseline_diad2[:, 1], '.b', label='bck')
+        axes['C'].plot(Diad_short_diad2[:, 0], Py_base_diad2, '-k', label='Poly bck fit')
 
 
-    axes['C'].set_ylabel('Intensity')
-    axes['C'].set_xlabel('Wavenumber')
+        axes['C'].set_ylabel('Intensity')
+        axes['C'].set_xlabel('Wavenumber')
 
 
-    if config1.fit_gauss is not False:
+        if config1.fit_gauss is not False:
 
-        axes['C'].plot(x_lin, components.get('bkg_')+ybase_xlin, '-m', label='Gaussian bck', linewidth=2)
+            axes['C'].plot(x_lin, components.get('bkg_')+ybase_xlin, '-m', label='Gaussian bck', linewidth=2)
 
-    axes['C'].plot( x_lin ,y_best_fit+ybase_xlin, '-g', linewidth=2, label='Best Fit')
-    axes['C'].plot(x_lin, components.get('lz1_')+ybase_xlin, '-b', label='Diad2', linewidth=1)
-    if fit_peaks>1:
-        axes['C'].plot(x_lin, components.get('lz2_')+ybase_xlin, '-r', label='HB2', linewidth=1)
-    if fit_peaks>2:
-        axes['C'].plot(x_lin, components.get('lz3_')+ybase_xlin, '-c', label='C13', linewidth=1)
+        axes['C'].plot( x_lin ,y_best_fit+ybase_xlin, '-g', linewidth=2, label='Best Fit')
+        axes['C'].plot(x_lin, components.get('lz1_')+ybase_xlin, '-b', label='Diad2', linewidth=1)
+        if fit_peaks>1:
+            axes['C'].plot(x_lin, components.get('lz2_')+ybase_xlin, '-r', label='HB2', linewidth=1)
+        if fit_peaks>2:
+            axes['C'].plot(x_lin, components.get('lz3_')+ybase_xlin, '-c', label='C13', linewidth=1)
 
-    axes['C'].legend(ncol=3, loc='lower center')
+        axes['C'].legend(ncol=3, loc='lower center')
 
 
 
-    axes['C'].set_xlim([axc_xmin, axc_xmax])
-    axes['C'].set_ylim([axc_ymin, axc_ymax])
-    #axes['C'].plot(Diad_short[:, 0], Diad_short[:, 1], '"r', label='Data')
+        axes['C'].set_xlim([axc_xmin, axc_xmax])
+        axes['C'].set_ylim([axc_ymin, axc_ymax])
+        #axes['C'].plot(Diad_short[:, 0], Diad_short[:, 1], '"r', label='Data')
 
 
-    # Residual on plot D
-    axes['D'].set_title('f) Residuals')
-    axes['D'].plot([df_out['Diad2_Voigt_Cent'], df_out['Diad2_Voigt_Cent']], [np.min(residual_diad_coords), np.max(residual_diad_coords)], ':b')
-    if fit_peaks>1:
-            axes['D'].plot([df_out['HB2_Cent'], df_out['HB2_Cent']], [np.min(residual_diad_coords), np.max(residual_diad_coords)], ':r')
+        # Residual on plot D
+        axes['D'].set_title('f) Residuals')
+        axes['D'].plot([df_out['Diad2_Voigt_Cent'], df_out['Diad2_Voigt_Cent']], [np.min(residual_diad_coords), np.max(residual_diad_coords)], ':b')
+        if fit_peaks>1:
+                axes['D'].plot([df_out['HB2_Cent'], df_out['HB2_Cent']], [np.min(residual_diad_coords), np.max(residual_diad_coords)], ':r')
 
-    axes['D'].plot(xdat_inrange, residual_diad_coords, 'ok', mfc='c' )
-    axes['D'].plot(xdat_inrange, residual_diad_coords, '-c' )
-    axes['D'].set_ylabel('Residual')
-    axes['D'].set_xlabel('Wavenumber')
-    # axes['D'].set_xlim(ax1_xlim)
-    # axes['D'].set_xlim(ax2_xlim)
-    Local_Residual_diad2=residual_diad_coords[((xdat_inrange>(df_out['Diad2_Voigt_Cent'][0]-config1.x_range_residual))
-                                            &(xdat_inrange<df_out['Diad2_Voigt_Cent'][0]+config1.x_range_residual))]
-    axes['D'].set_xlim([df_out['Diad2_Voigt_Cent'][0]-config1.x_range_residual,
-                df_out['Diad2_Voigt_Cent'][0]+config1.x_range_residual])
-    #ax5.plot([cent_1117, cent_1117 ], [np.min(Local_Residual_1117)-10, np.max(Local_Residual_1117)+10], ':k')
-    axes['D'].set_ylim([np.min(Local_Residual_diad2)-10, np.max(Local_Residual_diad2)+10])
+        axes['D'].plot(xdat_inrange, residual_diad_coords, 'ok', mfc='c' )
+        axes['D'].plot(xdat_inrange, residual_diad_coords, '-c' )
+        axes['D'].set_ylabel('Residual')
+        axes['D'].set_xlabel('Wavenumber')
+        # axes['D'].set_xlim(ax1_xlim)
+        # axes['D'].set_xlim(ax2_xlim)
+        Local_Residual_diad2=residual_diad_coords[((xdat_inrange>(df_out['Diad2_Voigt_Cent'][0]-config1.x_range_residual))
+                                                &(xdat_inrange<df_out['Diad2_Voigt_Cent'][0]+config1.x_range_residual))]
+        axes['D'].set_xlim([df_out['Diad2_Voigt_Cent'][0]-config1.x_range_residual,
+                    df_out['Diad2_Voigt_Cent'][0]+config1.x_range_residual])
+        #ax5.plot([cent_1117, cent_1117 ], [np.min(Local_Residual_1117)-10, np.max(Local_Residual_1117)+10], ':k')
+        axes['D'].set_ylim([np.min(Local_Residual_diad2)-10, np.max(Local_Residual_diad2)+10])
 
 
 
 
 
-    # Overal spectra
-    axes['E'].set_title('g) Summary plot of raw spectra for file = ' + filename)
-    axes['E'].plot(Spectra[:, 0], Spectra[:, 1], '-r')
-    axes['E'].set_ylabel('Intensity')
-    axes['E'].set_xlabel('Wavenumber')
+        # Overal spectra
+        axes['E'].set_title('g) Summary plot of raw spectra for file = ' + filename)
+        axes['E'].plot(Spectra[:, 0], Spectra[:, 1], '-r')
+        axes['E'].set_ylabel('Intensity')
+        axes['E'].set_xlabel('Wavenumber')
 
 
 
 
-    path3=path+'/'+'diad_fit_images'
-    if os.path.exists(path3):
-        out='path exists'
-    else:
-        os.makedirs(path+'/'+ 'diad_fit_images', exist_ok=False)
+        path3=path+'/'+'diad_fit_images'
+        if os.path.exists(path3):
+            out='path exists'
+        else:
+            os.makedirs(path+'/'+ 'diad_fit_images', exist_ok=False)
 
-    fig.tight_layout()
+        fig.tight_layout()
 
-    file=filename.rsplit('.txt', 1)[0]
-    fig.savefig(path3+'/'+'diad2_Fit_{}.png'.format(file), dpi=config1.dpi)
+        file=filename.rsplit('.txt', 1)[0]
+        fig.savefig(path3+'/'+'diad2_Fit_{}.png'.format(file), dpi=config1.dpi)
 
 
     if close_figure is True:
         plt.close(fig)
 
 
 
@@ -2680,26 +2791,36 @@
     # Then, we feed this baseline-corrected data into the combined gaussian-voigt peak fitting function
 
     result, df_out, y_best_fit, x_lin, components, xdat, ydat, ax1_xlim, ax2_xlim,residual_diad_coords, ydat_inrange,  xdat_inrange=fit_gaussian_voigt_generic_diad(config1,diad1=True, path=path, filename=filename,
                     xdat=x_diad1, ydat=y_corr_diad1,
                     span=span_diad1, plot_figure=False,
                     Diad_pos=Diad_pos, HB_pos=HB_pos,fit_peaks=fit_peaks)
 
+
+
+    # if df_out['Diad1_cent_err'].iloc[0]==0:
+    #     if config1.fit_peaks>1:
+    #         config_tweaked.fit_peaks=config1.fit_peaks-1
+    #         print('reducing peaks by 1 to try to get an error')
+
+
     # Try Refitting once
     if str(df_out['Diad1_refit'].iloc[0])!='Flagged Warnings:':
         print('refit attempt 1')
-        print(str(df_out['Diad1_refit'].iloc[0]))
-        config_tweaked=config1
         factor=2
+        import copy
+        config_tweaked=config1
+        config_tweaked=copy.copy(config1)
+
+        if any(df_out['Diad1_refit'].str.contains(' No Error')):
+            if config1.fit_peaks>1:
+                config_tweaked.fit_peaks=config1.fit_peaks-1
+                fit_peaks=config_tweaked.fit_peaks
 
 
-        # if any(df_out['Diad1_refit'].str.contains('V_LowAmp')):
-        #     config_tweaked.diad_amplitude=calc_diad_amplitude*10
-        # if any(df_out['Diad1_refit'].str.contains('V_HighAmp')):
-        #     config_tweaked.diad_amplitude=calc_diad_amplitude/10
         if any(df_out['Diad1_refit'].str.contains('V_input_TooLowSigma')):
             config_tweaked.diad_sigma=config1.diad_sigma*factor
         if any(df_out['Diad1_refit'].str.contains('V_input_TooHighSigma')):
             config_tweaked.diad_sigma=config1.diad_sigma/factor
         # Gaussian fit bits
         if any(df_out['Diad1_refit'].str.contains('G_input_TooHighSigma')):
             config_tweaked.gauss_sigma=config1.gauss_sigma/factor
@@ -2714,24 +2835,25 @@
             config_tweaked.gauss_sigma=config1.gauss_sigma*factor
         # # Hot band fit bits
         # if any(df_out['Diad1_refit'].str.contains('HB1_LowAmp')):
         #     config_tweaked.HB_amplitude=calc_HB_amplitude/2
         # if any(df_out['Diad1_refit'].str.contains('HB1_HighAmp')):
         #     config_tweaked.HB_amplitude=calc_HB_amplitude*2
 
-        result, df_out, y_best_fit, x_lin, components, xdat, ydat, ax1_xlim, ax2_xlim,residual_diad_coords, ydat_inrange,  xdat_inrange=fit_gaussian_voigt_generic_diad(config_tweaked,diad1=True, path=path, filename=filename,
+        result, df_out, y_best_fit, x_lin, components, xdat, ydat, ax1_xlim, ax2_xlim,residual_diad_coords, ydat_inrange,  xdat_inrange=fit_gaussian_voigt_generic_diad(config_tweaked, diad1=True, path=path, filename=filename,
                     xdat=x_diad1, ydat=y_corr_diad1,
-                    span=span_diad1, plot_figure=False, Diad_pos=Diad_pos, HB_pos=HB_pos, fit_peaks=fit_peaks)
+                    span=span_diad1, plot_figure=False, Diad_pos=Diad_pos, HB_pos=HB_pos, fit_peaks=config_tweaked.fit_peaks)
         i=2
         while str(df_out['Diad1_refit'].iloc[0])!='Flagged Warnings:':
 
             print('refit attempt  ='+str(i) + ', '+str(df_out['Diad1_refit'].iloc[0]))
             print(df_out['Diad1_refit'].iloc[0])
 
-            config_tweaked2=config_tweaked
+            import copy
+            config_tweaked2=copy.copy(config_tweaked)
             factor2=factor*2
 
 
             # if any(df_out['Diad1_refit'].str.contains('V_LowAmp')):
             #     config_tweaked2.diad_amplitude=config_tweaked.diad_amplitude*10
             # if any(df_out['Diad1_refit'].str.contains('V_HighAmp')):
             #     config_tweaked2.diad_amplitude=config_tweaked.diad_amplitude/10
@@ -2756,15 +2878,15 @@
             #     config_tweaked2.HB_amplitude=config_tweaked.HB_amplitude/2
             # if any(df_out['Diad1_refit'].str.contains('HB1_HighAmp')):
             #     config_tweaked2.HB_amplitude=config_tweaked.HB_amplitude*2
 
 
             result, df_out, y_best_fit, x_lin, components, xdat, ydat, ax1_xlim, ax2_xlim,residual_diad_coords, ydat_inrange,  xdat_inrange=fit_gaussian_voigt_generic_diad(config_tweaked2,diad1=True, path=path, filename=filename,
                     xdat=x_diad1, ydat=y_corr_diad1,
-                    span=span_diad1, plot_figure=False, Diad_pos=Diad_pos, HB_pos=HB_pos, fit_peaks=fit_peaks)
+                    span=span_diad1, plot_figure=False, Diad_pos=Diad_pos, HB_pos=HB_pos, fit_peaks=config_tweaked.fit_peaks)
             i=i+1
             if i>5:
                 print('Got to 5 iteratoins and still couldnt adjust the fit parameters')
                 break
 
 
 
@@ -3031,15 +3153,17 @@
             combo['Diad1_Gauss_Sigma']=np.nan
         if 'Diad2_Gauss_Cent' not in combo.columns:
             combo['Diad2_Gauss_Cent']=np.nan
             combo['Diad2_Gauss_Area']=np.nan
             combo['Diad2_Gauss_Sigma']=np.nan
 
         combo['Splitting']=combo['Diad2_Voigt_Cent']-combo['Diad1_Voigt_Cent']
-        cols_to_move = ['Splitting', 'Diad1_Combofit_Cent', 'Diad1_Combofit_Height', 'Diad1_Voigt_Cent', 'Diad1_Voigt_Area', 'Diad1_Voigt_Sigma',  'Diad1_Residual', 'Diad1_Prop_Lor', 'Diad1_fwhm', 'Diad1_refit','Diad2_Combofit_Cent', 'Diad2_Combofit_Height', 'Diad2_Voigt_Cent', 'Diad2_Voigt_Area', 'Diad2_Voigt_Sigma', 'Diad2_Voigt_Gamma', 'Diad2_Residual', 'Diad2_Prop_Lor', 'Diad2_fwhm', 'Diad2_refit',
+        combo['Split_err_abs']=combo['Diad1_cent_err']+combo['Diad2_cent_err']
+        combo['Split_err_quadrature']=(combo['Diad1_cent_err']**2+combo['Diad2_cent_err']**2)**0.5
+        cols_to_move = ['Splitting', 'Split_err_abs', 'Split_err_quadrature', 'Diad1_Combofit_Cent', 'Diad1_cent_err', 'Diad1_Combofit_Height', 'Diad1_Voigt_Cent', 'Diad1_Voigt_Area', 'Diad1_Voigt_Sigma',  'Diad1_Residual', 'Diad1_Prop_Lor', 'Diad1_fwhm', 'Diad1_refit','Diad2_Combofit_Cent', 'Diad2_cent_err',  'Diad2_Combofit_Height', 'Diad2_Voigt_Cent', 'Diad2_Voigt_Area', 'Diad2_Voigt_Sigma', 'Diad2_Voigt_Gamma', 'Diad2_Residual', 'Diad2_Prop_Lor', 'Diad2_fwhm', 'Diad2_refit',
                     'HB1_Cent', 'HB1_Area', 'HB1_Sigma', 'HB2_Cent', 'HB2_Area', 'HB2_Sigma', 'C13_Cent', 'C13_Area', 'C13_Sigma',
                     'Diad2_Gauss_Cent', 'Diad2_Gauss_Area','Diad2_Gauss_Sigma', 'Diad1_Gauss_Cent', 'Diad1_Gauss_Area','Diad1_Gauss_Sigma',]
         combo_f = combo[cols_to_move + [
                 col for col in combo.columns if col not in cols_to_move]]
         combo_f=combo_f.iloc[:, 0:len(cols_to_move)]
         file=filename.rsplit('.txt', 1)[0]
         combo_f.insert(0, 'filename', file)
@@ -3093,14 +3217,15 @@
     # Name that gets stamped onto fits
     name: str= 'generic'
     # Selecting the two background positions
     lower_bck: Tuple[float, float]=(1060, 1065)
     upper_bck: Tuple[float, float]=(1120, 1130)
 
     #
+    model_name: str='PseudoVoigtModel'
     x_range_bck: float=10
 
     # Background degree of polynomial
     N_poly_carb_bck: float =1
     # Seletcting the amplitude
     amplitude: float =1000
 
@@ -3130,21 +3255,24 @@
 
 
 
 
 
 
 def fit_generic_peak(*, config: generic_peak_config=generic_peak_config(),
-path=None, filename=None, filetype=None, model_name='VoigtModel',
+path=None, filename=None, filetype=None,
  plot_figure=True, dpi=200):
 
     """ This function fits a generic peak with a gaussian, and returns a plot
 
     config: from dataclass generic_peak_config
 
+        model_name: str, 'GaussianModel', 'VoigtModel', 'PseudoVoigtModel', 'Spline', 'Poly',
+            Fits Gaussian, Voigt, or PseudoVoigt, or fits a spline or polynomail and gets area underneath
+
         name: str
             Name of feature you are fitting. Used to make column headings in output (e.g., if SO2, outputs are Peak_Cent_SO2, Peak_Area_SO2)
 
         lower_bkc: Tuple[float, float]
             Upper and lower x coordinate for background to left of peak
 
         upper_bkc: Tuple[float, float]
@@ -3218,21 +3346,23 @@
     lower_0baseline=config.lower_bck[0]
     upper_0baseline=config.lower_bck[1]
     lower_1baseline=config.upper_bck[0]
     upper_1baseline=config.upper_bck[1]
 
     # Filter out spectra outside these baselines
     Spectra_short=Spectra[ (Spectra[:,0]>lower_0baseline) & (Spectra[:,0]<upper_1baseline) ]
+    Spectra_fit=Spectra[ (Spectra[:,0]>upper_0baseline) & (Spectra[:,0]<lower_1baseline) ]
 
     # To make a nice plot, give 50 wavenumber units on either side as a buffer
     Spectra_plot=Spectra[ (Spectra[:,0]>lower_0baseline-50) & (Spectra[:,0]<upper_1baseline+50) ]
 
     # Find peaks using Scipy find peaks
-    y=Spectra_plot[:, 1]
-    x=Spectra_plot[:, 0]
+    y=Spectra_fit[:, 1]
+    x=Spectra_fit[:, 0]
+    spec_res=np.abs(x[0]-x[1])
 
 
     peaks = find_peaks(y,height = config.height, threshold = config.threshold,
     distance = config.distance, prominence=config.prominence, width=config.width)
 
     height = peaks[1]['peak_heights'] #list of the heights of the peaks
     peak_pos = x[peaks[0]] #list of the peaks positions
@@ -3277,86 +3407,223 @@
 
 
 
 
     # Fits a polynomial to the baseline of degree
     Pf_baseline = np.poly1d(np.polyfit(Baseline[:, 0], Baseline[:, 1], config.N_poly_carb_bck))
     Py_base =Pf_baseline(Spectra_short[:, 0])
+    Py_base_fit =Pf_baseline(Spectra_fit[:, 0])
+
+
 
     Baseline_ysub=Pf_baseline(Baseline[:, 0])
     Baseline_x=Baseline[:, 0]
     y_corr= Spectra_short[:, 1]-Py_base
-    x=Spectra_short[:, 0]
+    y_corr_fit=Spectra_fit[:, 1]-Py_base_fit
+    x_fit=Spectra_fit[:, 0]
+    x_corr=Spectra_short[:, 0]
+
+
+
+    if config.model_name not in ['GaussianModel', 'VoigtModel', 'PseudoVoigtModel', 'Spline', 'Poly']:
+        raise TypeError('model_name not a permitted input, Please select either GaussianModel, VoigtModel, PseudoVoigtModel, or Spline or Poly')
+
+
+    if config.model_name in ['GaussianModel', 'VoigtModel', 'PseudoVoigtModel']:
 
-    # NOw into the voigt fitting
-    if model_name=='VoigtModel':
-        model0 = VoigtModel()#+ ConstantModel()
-    if model_name == 'PseudoVoigtModel':
-        model0 = PseudoVoigtModel()
 
-    # create parameters with initial values
-    pars0 = model0.make_params()
-    pars0['center'].set(config.cent, min=config.cent-30, max=config.cent+30)
-    pars0['amplitude'].set(config.amplitude, min=0)
+        # NOw into the voigt fitting
+        if config.model_name=='VoigtModel':
+            model0 = VoigtModel()#+ ConstantModel()
+        if config.model_name == 'PseudoVoigtModel':
+            model0 = PseudoVoigtModel()
+        if config.model_name=='GaussianModel':
+            model0=GaussianModel()
 
+        # create parameters with initial values
+        pars0 = model0.make_params()
+        pars0['center'].set(config.cent, min=config.cent-30, max=config.cent+30)
+        pars0['amplitude'].set(config.amplitude, min=0)
 
-    init0 = model0.eval(pars0, x=x)
-    result0 = model0.fit(y_corr, pars0, x=x)
-    Center_p0=result0.best_values.get('center')
-    area_p0=result0.best_values.get('amplitude')
 
+        init0 = model0.eval(pars0, x=x)
+        result0 = model0.fit(y_corr_fit, pars0, x=x)
+        Center_p0=result0.best_values.get('center')
+        area_p0=result0.best_values.get('amplitude')
 
 
-    # Make a nice linspace for plotting with smooth curves.
-    xx_carb=np.linspace(min(x), max(x), 2000)
-    y_carb=result0.eval(x=xx_carb)
-    height=np.max(y_carb)
 
-    df=pd.DataFrame(data={'filename': filename,
+        # Make a nice linspace for plotting with smooth curves.
+        xx_carb=np.linspace(min(x), max(x), 2000)
+        y_carb=result0.eval(x=xx_carb)
+        height=np.max(y_carb)
+
+        # Moved this form down below, think it belongs here
+        if area_p0 is None:
+            area_p0=np.nan
+            if area_p0 is not None:
+                if area_p0<0:
+                    area_p0=np.nan
+
+
+        df=pd.DataFrame(data={'filename': filename,
     'Peak_Cent_{}'.format(name): Center_p0,
     'Peak_Area_{}'.format(name): area_p0,
-    'Peak_Height_{}'.format(name): height}, index=[0])
+    'Peak_Height_{}'.format(name): height,
+    'Model_name': config.model_name}, index=[0])
+
+    else:
+
+        if  config.model_name == 'Spline':
+            from scipy.interpolate import CubicSpline
+            # fit a spline first to find intensity cut off
+            mix_spline_sil = interp1d(x_fit, y_corr_fit,
+                                    kind='cubic')
+            x_new=np.linspace(np.min(x_fit), np.max(x_fit), 1000)
+            Baseline_ysub_sil=mix_spline_sil(x_new)
+
+            x_max = x_new[np.argmax(Baseline_ysub_sil)]
+            cent=x_max
+            Peak_Center=x_max
+
+            max_y=np.max(y_corr_fit)
+
+            # Lets trim x and y based on intensity values
+        # Find intensity cut off
+            int_cut_off=0.1
+            y_int_cut=max_y*int_cut_off
+
+            # Check peak isnt at edge of window, else wont work
+
+            if Peak_Center==np.max(x_fit) or Peak_Center==np.min(x_fit):
+                print('peak at edge of window, setting params to nans')
+
+
+
+                df=pd.DataFrame(data={'filename': filename,
+            'Peak_Cent_{}'.format(name): np.nan,
+            'Peak_Area_{}'.format(name): np.nan,
+            'Peak_Height_{}'.format(name): np.nan,
+            'Model_name': config.model_name}, index=[0])
+
+            else:
+
+
+
+            # Split the array into a LHS and a RHS
+
+                LHS_y=Baseline_ysub_sil[x_new<=Peak_Center]
+                RHS_y=Baseline_ysub_sil[x_new>Peak_Center]
+
+                LHS_x=x_new[x_new<=Peak_Center]
+                RHS_x=x_new[x_new>Peak_Center]
+
+                # Need to flip LHS to put into the find closest function
+                LHS_y_flip=np.flip(LHS_y)
+                LHS_x_flip=np.flip(LHS_x)
+
+
+                val=np.argmax(LHS_y_flip<y_int_cut)
+
+                val2=np.argmax(RHS_y<y_int_cut)
+
+                # Find nearest x unit to this value
+                y_nearest_LHS=LHS_y_flip[val]
+                x_nearest_LHS=LHS_x_flip[val]
+
+                y_nearest_RHS=RHS_y[val2]
+                x_nearest_RHS=RHS_x[val2]
+
+                diff_LHS=Peak_Center-x_nearest_LHS
+                diff_RHS=x_nearest_RHS-Peak_Center
+
+
+
+                n_res=3
+                x_new_skewness=np.linspace(x_nearest_LHS-spec_res*n_res, x_nearest_RHS+spec_res*n_res)
+
+                x_new=x_new_skewness
+
+
+                Baseline_ysub_sil=mix_spline_sil(x_new_skewness)
+
+
+
+
+
+
+                N_poly_sil='Spline'
+
+
+                xspace_sil=x_new[1]-x_new[0]
+                area_trap = trapz(Baseline_ysub_sil, dx=xspace_sil)
+                area_simps = simps(Baseline_ysub_sil, dx=xspace_sil)
+
+
+
+                area_p0=area_trap
+
+
+
+
+                df=pd.DataFrame(data={'filename': filename,
+            'Peak_Cent_{}'.format(name): x_max,
+            'Peak_Area_{}'.format(name): area_p0,
+            'Peak_Height_{}'.format(name): max_y,
+            'Model_name': config.model_name}, index=[0])
+
+
+
+
 
-    if area_p0 is None:
-        area_p0=np.nan
-        if area_p0 is not None:
-            if area_p0<0:
-                area_p0=np.nan
 
     # Plotting what its doing
+
     if plot_figure is True:
         fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(10,5))
         fig.suptitle('Secondary Phase, file= '+ str(filename), fontsize=12, x=0.5, y=1.0)
 
         # Plot the peak positions and heights
 
 
 
         ax1.set_title('Background fit')
 
         ax1.plot(Spectra_plot[:, 0], Spectra_plot[:, 1], '-r', label='Spectra')
-        ax1.plot(RH_baseline_filt[:, 0], RH_baseline_filt[:, 1], '-b',
-        lw=3,  label='bck points')
+        ax1.plot(RH_baseline_filt[:, 0], RH_baseline_filt[:, 1], '.b',
+        label='bck points')
         ax1.plot(LH_baseline_filt[:, 0], LH_baseline_filt[:, 1], '-b',
         lw=3, label='_bck points')
+
+        #ax2.plot(x, y_corr_fit, '-r', label='Bck-sub data', lw=0.5)
+        ax2.plot(x, y_corr_fit, '.r', label='Bck-sub data')
         ax1.plot(Spectra_short[:, 0], Py_base, '-k', label='Bck Poly')
 
 
+        if config.model_name != 'Spline' and config.model_name != 'Poly':
+            ax2.plot(xx_carb, y_carb, '-k', label='Peak fit')
+            cent=df['Peak_Cent_{}'.format(name)].iloc[0]
+            ax2.set_xlim([cent-config.x_range_bck, cent+config.x_range_bck])
+        else:
+            ax2.plot(x_new, Baseline_ysub_sil, '-k')
+            ax2.fill_between(x_new, Baseline_ysub_sil, color='yellow', label='fit', alpha=0.5)
+
+
         ax2.set_title('Bkg-subtracted, ' + name + ' peak fit')
 
-        ax2.plot(xx_carb, y_carb, '-k', label='Peak fit')
-        ax2.plot(x, y_corr, '.r', label='Bck-sub data')
 
 
 
-        cent=df['Peak_Cent_{}'.format(name)].iloc[0]
-        ax2.set_xlim([cent-config.x_range_bck, cent+config.x_range_bck])
-        # ax2.set_ylim([min(y_carb)-0.5*(max(y_carb)-min(y_carb)),
-        #             max(y_carb)+0.1*max(y_carb),
-        # ])
+
+
+
+
+    # ax2.set_ylim([min(y_carb)-0.5*(max(y_carb)-min(y_carb)),
+    #             max(y_carb)+0.1*max(y_carb),
+    # ])
 
 
 
         if find_peaks is True:
 
             ax1.plot(df_peak_sort_short['pos'], df_peak_sort_short['height'], '*k', mfc='yellow', label='SciPy Peaks')
             ax1.plot(Spectra_short[:, 0], Py_base, '-k')
@@ -3472,16 +3739,16 @@
     yplot=np.empty(len(Diad_Files), dtype=float)
     Diad_df=get_data(path=path, filename=Diad_Files[0], filetype=filetype)
     x_data=Diad_df[:, 0]
     y_data=np.empty([  len(x_data), len(Diad_Files)], float)
 
 
     for file in Diad_Files:
-       
-        
+
+
 
 
         Diad_df=get_data(path=path, filename=file, filetype=filetype)
         Diad=np.array(Diad_df)
 
 
         # First lets use find peaks
@@ -3502,35 +3769,35 @@
 
         # IF using scipy find peaks
         if find_peaks_filter is True:
             # Find peaks for trimmed spectra (e.g. in region peaks have been asked for)
             peaks = find_peaks(y_trim,height = height, threshold = threshold,
             distance = distance, prominence=prominence, width=width)
 
-            
+
             height_PEAK = peaks[1]['peak_heights'] #list of the heights of the peaks
             peak_pos = x_trim[peaks[0]] #list of the peaks positions
 
             df_sort=pd.DataFrame(data={'pos': peak_pos,
                                 'height': height_PEAK})
 
             df_peak_sort=df_sort.sort_values('height', axis=0, ascending=False)
 
             # Trim number of peaks based on user-defined N peaks
-            
+
 
 
             #print(df_peak_sort_short)
             if len(df_peak_sort>=1):
-                
+
                 df_peak_sort_short=df_peak_sort[0:1]
                 peak_pos_saved[i]=df_peak_sort_short['pos'].values
                 peak_height_saved[i]=df_peak_sort_short['height'].values
             else:
-                
+
                 peak_pos_saved[i]=np.nan
                 peak_height_saved[i]=np.nan
 
             peak_bck[i]=np.quantile(y_plot, 0.2)
             av_y=np.quantile(y_plot, 0.5)
             Diff=np.max(y_plot)-np.min(y_plot)
             Y_sum=np.max(y_plot)/Diff
@@ -3627,14 +3894,17 @@
     ax1.plot([1094, 1094], [0, yplot[-1]+2], '-c', lw=1, label='MgCO$_3$')
     ax1.plot([1097, 1097], [0, yplot[-1]+2], '-b', lw=1, label='Dolomite')
     ax1.plot([1131, 1131], [0, yplot[-1]+2], '-', color='grey', lw=1, label='CaSO$_4$')
     ax1.plot([1136, 1136], [0, yplot[-1]+2], '--', color='rosybrown', lw=1, label='MgSO$_4$')
     ax1.plot([1151, 1151], [0, yplot[-1]+2], '-k', lw=1, label='SO$_2$')
 
 
+    ax1.fill_between(xlim_peaks, -0.5, yplot[-1]+3, color='blue', alpha=0.1)
+
+
     ax1.legend(ncol=7,loc='upper center', fontsize=10,  bbox_to_anchor=[0.5, 1.05])
     ax1.set_ylim([-0.5, yplot[-1]+3])
     ax1.set_xlim([xlim_plot[0], xlim_plot[1]+0.5])
 
     # df_peaks=pd.DataFrame(data={'filename': Diad_Files,
     #                         'pos': peak_pos_saved,
     #                             'prom': peak_height_saved-peak_bck})
```

### Comparing `DiadFit-0.0.57/src/DiadFit/error_propagation.py` & `DiadFit-0.0.59/src/DiadFit/error_propagation.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.57/src/DiadFit/importing_data_files.py` & `DiadFit-0.0.59/src/DiadFit/importing_data_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1009,15 +1009,15 @@
 
 
     return Time_Df_2
 
 ## Getting nice names from any file types
 
 def extracting_filenames_generic(*, names, prefix=False,
-    str_prefix=None, suffix=False,
+    str_prefix=None, suffix=False, CRR_filter=True,
     str_suffix=None,
    file_type=None):
     """
     Takes filenames from a panda series (e.g., a column of a dataframe of metadata), outputs a numpy array that is consistent with the same function for 
     spectra, to allow stitching of spectra and metadata. 
 
 
@@ -1042,18 +1042,33 @@
         The file extension, e.g., '.csv'
 
     Returns
     -----------------
     np.array of names, with prefix, suffix and filetype stripped away
 
     """
+    
+
     if isinstance(names, list):
         names_df=pd.DataFrame(data={'name': names})
         names=names_df['name']
 
+    if CRR_filter is True:
+        names = names.str.replace('_CRR_DiadFit', '')
+
+    # if prefix is True:
+    #     names=names.str.split(str_prefix).str[1]
+
+    # if suffix is True:
+    #     names=names.str.split(str_suffix).str[1]
+
+    # if file_type is not None:
+    #     names=names.str.replace(file_type, '')
+
+    file_m=list(names)
 
     file_m=np.empty(len(names), dtype=object)
     for i in range(0, len(names)):
         name=names.iloc[i]
         # If no prefix or suffix to remove, simple
         if prefix is False and suffix is False:
             file_m[i]=name
@@ -1076,17 +1091,18 @@
         if file_type in file_m[i]:
             file_m[i]=file_m[i].replace(file_type, '')
 
 
 
     if len(file_m)!=len(pd.Series(file_m).unique()):
         file_m_s=pd.Series(file_m)
-        print('duplicates')
-        print(file_m_s[file_m_s.duplicated()])
         print('OOPS. at least one of your file name is duplicated go back to your spectra, you named a file twice, this will confuse the stitching ')
+        print(file_m_s[file_m_s.duplicated()])
+    else:
+        print('good job, no duplicate file names')
         #raise Exception('Duplicate file')
 
     return file_m
 
 # These are largely redundant.  
 def extract_temp_Aranet(df):
     """ Extracts temperature data from the aranet
```

### Comparing `DiadFit-0.0.57/src/DiadFit/ne_lines.py` & `DiadFit-0.0.59/src/DiadFit/ne_lines.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,33 +11,35 @@
 from os.path import isfile, join
 from DiadFit.importing_data_files import *
 from typing import Tuple, Optional
 from dataclasses import dataclass
 import matplotlib.patches as patches
 from tqdm.notebook import tqdm
 import re
+import scipy.stats as stats
+import pickle
+
 
-## Test this
 
 
 encode="ISO-8859-1"
 
 ## Plotting Ne lines, returns peak position
 def find_closest(df, line1_shift):
     """ 
    This function finds the closest Raman shift value in the inputted dataframe to the inputted line position
 
    Parameters
    -------------
     df: pd.DataFrame
-        Dataframe of Ne line positions based on laser wavelength from the function calculate_Ne_line_positions
+        Dataframe of Ne line positions based on laser wavelength from the function calculate_Ne_line_positions, or calculate_Ar_line_positions
     
     line1_shift: int, float
         input line position
-
+error_pk2
    Returns
    -------------
    Closest theoretical line position
 
     """
     dist = (df['Raman_shift (cm-1)'] - line1_shift).abs()
     return df.loc[dist.idxmin()]
@@ -297,27 +299,29 @@
     # Apply Scipy Find peaks using the parameters in the config file.
     peaks = find_peaks(y,height = height, threshold = threshold, distance = distance, prominence=prominence, width=width)
 
     # This gets a list of peak heights
     height = peaks[1]['peak_heights']
     # This gets a list of peak positions
     peak_pos = x[peaks[0]]
+    
+   
 
     # Lets combine them in a dataframe
     df=pd.DataFrame(data={'pos': peak_pos,
                         'height': height})
 
 
     # Find bigest peaks, and take up to n peaks
     df_sort_Ne=df.sort_values('height', axis=0, ascending=False)
     df_sort_Ne_trim=df_sort_Ne[0:n_peaks]
 
     if print_df is True:
         print('Biggest N peaks:')
-        display(df_sort_Ne_trim)
+        print(df_sort_Ne_trim)
 
     # Get peak within +-5
     df_pk1=df_sort_Ne.loc[df['pos'].between(peak1_cent-10*spec_res, peak1_cent+10*spec_res)]
     df_pk2=df_sort_Ne.loc[df['pos'].between(peak2_cent-10*spec_res, peak2_cent+10*spec_res)]
 
     df_pk1_trim=df_pk1[0:1]
     df_pk2_trim=df_pk2[0:1]
@@ -428,14 +432,18 @@
 
         ax1.set_ylim([0, 1.5*df_fit_params['Peak1_height'].iloc[0]+100])
         ax2.set_ylim([0, 1.5*df_fit_params['Peak2_height'].iloc[0]+100])
         fig.tight_layout()
 
     df_fit_params['Peak1_prom']=df_fit_params['Peak1_height']-Baseline_Neon1
     df_fit_params['Peak2_prom']=df_fit_params['Peak2_height']-Baseline_Neon2
+    
+    df_fit_params=df_fit_params.reset_index(drop=True)
+    
+    
 
 
     return Ne, df_fit_params
 
 
 
 ## Ne baselines
@@ -687,14 +695,15 @@
         Center_p0_error=result0.params.get('p0_center')
         Amp_p0=result0.params.get('p0_amplitude')
         if block_print is False:
             print('first iteration, peak Amplitude='+str(np.round(Amp_p0, 4)))
         fwhm_p0=result0.params.get('p0_fwhm')
 
 
+
         pattern = r"\+/-\s*([\d.]+)"
         match = re.search(pattern, str(Center_p0_error))
         if match:
             Center_p0_errorval = float(match.group(1))
         else:
             Center_p0_errorval=np.nan
 
@@ -732,14 +741,29 @@
 
 
         pars[prefix + 'amplitude'].set(Amp_p0/5, min=0, max=Amp_p0/2)
         pars[prefix + 'sigma'].set(0.2, min=0)
 
         model_combo=model1+peak
         pars1.update(pars)
+        
+        # Attempt at stabilizing peak fit
+        result = model_combo.fit(ydat, pars1, x=xdat)
+        
+        result.params['p2_center'].vary = False
+        result.params['p2_amplitude'].vary = False
+        result.params['p2_sigma'].vary = False
+        
+        model1_only = model1
+        
+        pars1.update(result.params)
+        
+        result_pk1 = model1_only.fit(ydat, pars1, x=xdat)
+                
+
 
 
     if peaks_pk1==1:
 
         if model_name == 'PseudoVoigtModel':
             model_combo = PseudoVoigtModel(prefix='p1_')#+ ConstantModel(prefix='c0')
         if model_name=="VoigtModel":
@@ -760,71 +784,59 @@
 
     init = model_combo.eval(pars1, x=xdat)
     result = model_combo.fit(ydat, pars1, x=xdat)
     # Need to check errors output
     Error_bars=result.errorbars
 
 
+
     # Get center value
     Center_p1=result.best_values.get('p1_center')
-    Center_p1_error=result.params.get('p1_center')
+    
+    
+    
+    error_pk1 = result.params['p1_center'].stderr
+  
+    
 
     # Get mix of lorenz
     Peak1_Prop_Lor=result.best_values.get('p1_fraction')
 
 
-    if peaks_pk1==1:
-        Center_pk1=Center_p1
-        if Error_bars is False:
-            if block_print is False:
-                print('Error bars not determined by function')
-            error_pk1=np.nan
-        else:
-            error_pk1 = float(str(Center_p1_error).split()[4].replace(",", ""))
-
+   
 
     if peaks_pk1>1:
         Center_p2=result.best_values.get('p2_center')
         Center_p2_error=result.params.get('p2_center')
 
 
-        if Error_bars is False:
-            if block_print is False:
-                print('Error bars not determined by function')
-            Center_p1_errorval=np.nan
-            if peaks_pk1>1:
-                Center_p2_errorval=np.nan
-        else:
-            Center_p1_errorval=float(str(Center_p1_error).split()[4].replace(",", ""))
-            if peaks_pk1>1:
-                Center_p2_errorval=float(str(Center_p2_error).split()[4].replace(",", ""))
-
-        # Check if nonsense, e.g. if center 2 miles away, just use center 0
-        if Center_p2 is not None:
-            if Center_p2>Center_p0 or Center_p2<1112:
-                Center_pk1=Center_p0
-                error_pk1=Center_p0_errorval
-                if block_print is False:
-                    print('No  meaningful second peak found')
-
-            elif Center_p1 is None and Center_p2 is None:
-                if block_print is False:
-                    print('No peaks found')
-            elif Center_p1 is None and Center_p2>0:
-                Center_pk1=Center_p2
-                error_pk1=Center_p2_errorval
-            elif Center_p2 is None and Center_p1>0:
-                Center_pk1=Center_p1
-                error_pk1=Center_p1_errorval
-            elif Center_p1>Center_p2:
-                Center_pk1=Center_p1
-                error_pk1=Center_p1_errorval
-            elif Center_p1<Center_p2:
-                Center_pk1=Center_p2
-                error_pk1=Center_p2_errorval
+
+        # # Check if nonsense, e.g. if center 2 miles away, just use center 0
+        # if Center_p2 is not None:
+        #     if Center_p2>Center_p0 or Center_p2<1112:
+        #         Center_pk1=Center_p0
+        #         error_pk1=Center_p0_errorval
+        #         if block_print is False:
+        #             print('No  meaningful second peak found')
+        # 
+        #     elif Center_p1 is None and Center_p2 is None:
+        #         if block_print is False:
+        #             print('No peaks found')
+        #     elif Center_p1 is None and Center_p2>0:
+        #         Center_pk1=Center_p2
+        #         error_pk1=Center_p2_errorval
+        #     elif Center_p2 is None and Center_p1>0:
+        #         Center_pk1=Center_p1
+        #         error_pk1=Center_p1_errorval
+        #     elif Center_p1>Center_p2:
+        #         Center_pk1=Center_p1
+        #         
+        #     elif Center_p1<Center_p2:
+        #         Center_pk1=Center_p2
+                
 
     Area_pk1=result.best_values.get('p1_amplitude')
     sigma_pk1=result.best_values.get('p1_sigma')
     gamma_pk1=result.best_values.get('p1_gamma')
 
 
     # Evaluate the peak at 100 values for pretty plotting
@@ -832,14 +844,15 @@
 
     result_pk1=result.eval(x=xx_pk1)
     comps=result.eval_components(x=xx_pk1)
 
 
     result_pk1_origx=result.eval(x=Ne_pk1_reg_x)
 
+    Center_pk1=Center_p1
 
 
     return Center_pk1, Area_pk1, sigma_pk1, gamma_pk1, Ne_pk1_reg_x_plot, Ne_pk1_reg_y_plot, Ne_pk1_reg_x, Ne_pk1_reg_y, xx_pk1, result_pk1, error_pk1, result_pk1_origx, comps, Peak1_Prop_Lor
 
 
 def fit_pk2(x, y_corr, x_span=[-5, 5], Ne_center=1447.5, amplitude=1000, pk2_sigma=0.4,
 model_name='PseudoVoigtModel', print_report=False, const_params=True) :
@@ -911,26 +924,38 @@
     result = model.fit(Ne_pk2_reg_y.flatten(), params, x=Ne_pk2_reg_x.flatten())
 
     # Get center value
     Center_pk2=result.best_values.get('center')
     Center_pk2_error=result.params.get('center')
 
     Peak2_Prop_Lor=result.best_values.get('fraction')
+    
+
 
     #print(result.best_values)
 
     Area_pk2=result.best_values.get('amplitude')
     sigma_pk2=result.best_values.get('sigma')
     gamma_pk2=result.best_values.get('gamma')
     # Have to strip away the rest of the string, as center + error
     # print('debug:')
     # print(Center_pk2_error)
     # Center_pk2_errorval=float(str(Center_pk2_error).split()[4].replace(",", ""))
     # error_pk2=Center_pk2_errorval
-    error_pk2=1
+    
+    
+    error_pk2=np.nan
+    
+    try:
+        error_pk2_str = str(Center_pk2_error).split('+/-')[1].split(' bounds')[0].strip()
+        error_pk2 = float(error_pk2_str.replace(",", ""))
+    except IndexError:
+        pass
+    
+   
 
     # Evaluate the peak at 100 values for pretty plotting
     xx_pk2=np.linspace(lower_pk2, upper_pk2, 2000)
 
     result_pk2=result.eval(x=xx_pk2)
     result_pk2_origx=result.eval(x=Ne_pk2_reg_x)
 
@@ -1075,16 +1100,34 @@
         lower_bck_2, upper_bck2, upper_bck2: 3 lists of length 2:
             Positions used for background relative to peak.[-50, -20] takes a
             background -50 and -20 from the peak center
 
         x_span_pk2: list length 2. Default [-10, 8]
             Span either side of peak center used for fitting,
             e.g. by default, fits to 10 wavenumbers below peak, 8 above.
+            
     """
 
+    # check they havent messed up background
+    if config.lower_bck_pk1[0]>config.lower_bck_pk1[1]:
+        raise TypeError('Your left hand number needs to be a smaller number than the right, e.g. you can have [2, 5] but you cant have [5, 2]')
+    if config.upper_bck1_pk1[0]>config.upper_bck1_pk1[1]:
+        raise TypeError('Your left hand number needs to be a smaller number than the right, e.g. you can have [2, 5] but you cant have [5, 2]')
+    if config.upper_bck2_pk1[0]>config.upper_bck2_pk1[1]:
+        raise TypeError('Your left hand number needs to be a smaller number than the right, e.g. you can have [2, 5] but you cant have [5, 2]')
+
+    # check they havent messed up background
+    if config.lower_bck_pk2[0]>config.lower_bck_pk2[1]:
+        raise TypeError('Your left hand number needs to be a smaller number than the right, e.g. you can have [2, 5] but you cant have [5, 2]')
+    if config.upper_bck1_pk2[0]>config.upper_bck1_pk2[1]:
+        raise TypeError('Your left hand number needs to be a smaller number than the right, e.g. you can have [2, 5] but you cant have [5, 2]')
+    if config.upper_bck2_pk2[0]>config.upper_bck2_pk2[1]:
+        raise TypeError('Your left hand number needs to be a smaller number than the right, e.g. you can have [2, 5] but you cant have [5, 2]')
+   
+    
     x=Ne[:, 0]
     spec_res=np.abs(x[1]-x[0])
     # Getting things from config file
     peaks_1=config.peaks_1
     DeltaNe_ideal=config.DeltaNe_ideal
 
     # Estimate amplitude from prominence and sigma you entered
@@ -1126,17 +1169,23 @@
     # Fit the 1447 peak
     cent_pk2,Area_pk2, sigma_pk2, gamma_pk2, Ne_pk2_reg_x_plot, Ne_pk2_reg_y_plot, Ne_pk2_reg_x, Ne_pk2_reg_y, xx_pk2, result_pk2, error_pk2, result_pk2_origx, Peak2_Prop_Lor = fit_pk2( x_pk2, y_corr_pk2, x_span=x_span_pk2,  Ne_center=Ne_center_2, model_name=config.model_name, amplitude=Pk2_Amp, pk2_sigma=config.pk2_sigma, const_params=const_params)
 
 
     # Calculate difference between peak centers, and Delta Ne
     DeltaNe=cent_pk2-cent_pk1
 
+
     Ne_Corr=DeltaNe_ideal/DeltaNe
 
+
     # Calculate maximum splitting (+1 sigma)
+    error_pk1 = error_pk1 if error_pk1 is not None else 0
+    error_pk2 = error_pk2 if error_pk2 is not None else 0
+
+    
     DeltaNe_max=(cent_pk2+error_pk2)-(cent_pk1-error_pk1)
     DeltaNe_min=(cent_pk2-error_pk2)-(cent_pk1+error_pk1)
     Ne_Corr_max=DeltaNe_ideal/DeltaNe_min
     Ne_Corr_min=DeltaNe_ideal/DeltaNe_max
 
     # Calculating least square residual
     residual_pk1=np.sum(((Ne_pk1_reg_y-result_pk1_origx)**2)**0.5)/(len(Ne_pk1_reg_y))
@@ -1299,16 +1348,18 @@
         figure_str=path+'/'+ 'Ne_fit_images'+ '/'+ filename+str('_Ne_Line_Fit')+str('.png')
 
         fig.savefig(figure_str, dpi=200)
         if close_figure is True:
             plt.close(fig)
 
     if prefix is True:
-
         filename=filename.split(' ')[1:][0]
+        
+        
+        
     df=pd.DataFrame(data={'filename': filename,
                           'pk2_peak_cent':cent_pk2,
                           'pk2_amplitude': Area_pk2,
                           'pk2_sigma': sigma_pk2,
                           'pk2_gamma': gamma_pk2,
                           'error_pk2': error_pk2,
                           'Peak2_Prop_Lor': Peak2_Prop_Lor,
@@ -1323,14 +1374,34 @@
                          'Ne_Corr': Ne_Corr,
                          'Ne_Corr_min':Ne_Corr_min,
                          'Ne_Corr_max': Ne_Corr_max,
                          'residual_pk2':residual_pk2,
                          'residual_pk1': residual_pk1,
                          'residual_pk1+pk2':residual_pk1+residual_pk2,
                          }, index=[0])
+                         
+                         
+    df_combo=df
+    pk1_peak_cent_values = df_combo['pk1_peak_cent'].values
+    pk1_peak_cent_errors = df_combo['error_pk1'].fillna(0).values
+    pk2_peak_cent_values = df_combo['pk2_peak_cent'].values
+    pk2_peak_cent_errors = df_combo['error_pk2'].fillna(0).values
+    
+    constant=df_combo['deltaNe']
+    
+    # Calculate the error on Ne_Corr using error propagation (quadrature)
+    Ne_Corr_errors = np.sqrt((pk1_peak_cent_errors / constant) ** 2 + (pk2_peak_cent_errors / constant) ** 2)
+    
+    test_err=np.sqrt(pk1_peak_cent_errors ** 2 + pk2_peak_cent_errors ** 2)
+    
+    total_err=test_err/constant
+    
+    df.insert(1,'1σ_Ne_Corr', Ne_Corr_errors)
+    df.insert(1,'1σ_Ne_Corr_test', total_err)
+    
     if save_clipboard is True:
         df.to_clipboard(excel=True, header=False, index=False)
 
     if loop is False:
         return df, Ne_pk1_reg_x_plot, Ne_pk1_reg_y_plot
     if loop is True:
         return df
@@ -1341,20 +1412,28 @@
 def plot_Ne_corrections(df=None, x_axis=None, x_label='index', marker='o', mec='k',
                        mfc='r'):
     if x_axis is not None:
         x=x_axis
     else:
         x=df.index
     fig, ((ax5, ax6), (ax1, ax2), (ax3, ax4), ) = plt.subplots(3, 2, figsize=(10, 12))
-    ax1.plot(x, df['Ne_Corr'], marker,  mec='k', mfc='grey')
+
+    ax1.errorbar(x, df['Ne_Corr'], xerr=0, yerr=df['1σ_Ne_Corr'].fillna(0),
+             fmt='o', ecolor='k', elinewidth=0.8, mfc='grey', ms=5, mec='k',capsize=3)
+    
     ax1.set_ylabel('Ne Correction factor')
     ax1.set_xlabel(x_label)
 
-    ax5.plot(x, df['pk1_peak_cent'], marker,  mec='k', mfc='b')
+    
+    ax5.errorbar(x, df['pk1_peak_cent'], xerr=0, yerr=df['error_pk1'].fillna(0),
+             fmt='o', ecolor='k', elinewidth=0.8, mfc='b', ms=5, mec='k', capsize=3)
+             
     ax6.plot(x, df['pk2_peak_cent'], marker,  mec='k', mfc='r')
+    ax6.errorbar(x, df['pk2_peak_cent'], xerr=0, yerr=df['error_pk2'].fillna(0),
+             fmt='o', ecolor='k', elinewidth=0.8, mfc='r', ms=5, mec='k', capsize=3)
     ax5.set_xlabel(x_label)
     ax6.set_xlabel(x_label)
     ax5.set_ylabel('Peak 1 center')
     ax6.set_ylabel('Peak 2 center')
 
 
     ax2.plot( df['residual_pk2']+df['residual_pk1'], df['Ne_Corr'], marker,  mec='k', mfc='r')
@@ -1429,19 +1508,23 @@
 
 
 #print('working on ' + str(files[i]))
 
 
     df2=df.reset_index(drop=True)
 
+
     # Now lets reorder some columns
 
-    cols_to_move = ['filename', 'Ne_Corr', 'deltaNe', 'pk2_peak_cent', 'pk1_peak_cent', 'pk2_amplitude', 'pk1_amplitude', 'residual_pk2', 'residual_pk1']
+    cols_to_move = ['filename', 'Ne_Corr', '1σ_Ne_Corr', 'deltaNe', 'pk2_peak_cent', 'pk1_peak_cent', 'pk2_amplitude', 'pk1_amplitude', 'residual_pk2', 'residual_pk1']
     df2 = df2[cols_to_move + [
                 col for col in df2.columns if col not in cols_to_move]]
+                
+
+
 
 
     return df2
 
 ## Regressing Ne lines against time
 from scipy.interpolate import interp1d
 def reg_Ne_lines_time(df, fit='poly', N_poly=None, spline_fit=None):
@@ -1472,15 +1555,18 @@
     Px=np.linspace(np.min(df['sec since midnight']), np.max(df['sec since midnight']),
                          101)
     if fit=='poly':
         Pf = np.poly1d(np.polyfit(df['sec since midnight'], df['Ne_Corr'],
                               N_poly))
 
     if fit == 'spline':
-            Pf = interp1d(df['sec since midnight'], df['Ne_Corr'], kind=spline_fit)
+            if spline_fit is None:
+                raise TypeError('If you choose spline you also need to choose the type of spline fit. do help of this function to get the options')
+            else:
+                Pf = interp1d(df['sec since midnight'], df['Ne_Corr'], kind=spline_fit)
 
     Py=Pf(Px)
 
     fig, (ax1) = plt.subplots(1, 1, figsize=(6, 3))
     ax1.plot(df['sec since midnight'], df['Ne_Corr'], 'xk')
     ax1.plot(Px, Py, '-r')
     ax1.set_xlabel('Seconds since midnight')
@@ -1513,9 +1599,171 @@
     ds=pd.Series(Corr_factor_Filt)
 
 
 
     return ds
 
 
+## Lets make a plotting function for this notebook 
+
+def plot_and_save_Ne_line_pickle(*, time, Ne_corr, N_poly=3, CI=0.67, bootstrap=False, std_error=True, N_bootstrap=500):
+# Define the x and y values
+    x_all   = np.array([time])
+    y_all = np.array([Ne_corr['Ne_Corr']])
+    y_err=Ne_corr['1σ_Ne_Corr']
+    non_nan_indices = ~np.isnan(x_all) & ~np.isnan(y_all)
+
+    # Filter out NaN values
+    x = x_all[non_nan_indices]
+    y = y_all[non_nan_indices]
+    # Perform polynomial regression
+  
+    coefficients = np.polyfit(x, y, N_poly)
+    Pf = np.poly1d(coefficients)
+
+
+    # Save the model and the data to a pickle file
+    data = {'model': Pf, 'x': x, 'y': y}
+    with open('polyfit_data.pkl', 'wb') as f:
+        pickle.dump(data, f)
+        
+    if bootstrap is True:
+
+        new_x_plot=np.linspace(np.min(x), np.max(x), 100)
+        Ne_corr2=calculate_Ne_corr_bootstrap_values(pickle_str='polyfit_data.pkl',
+            new_x=pd.Series(new_x_plot), N_poly=N_poly, CI=CI, N_bootstrap=N_bootstrap)
+
+    if std_error is True:
+        new_x_plot=np.linspace(np.min(x), np.max(x), 100)
+        Ne_corr2=calculate_Ne_corr_std_err_values(pickle_str='polyfit_data.pkl',
+        new_x=pd.Series(new_x_plot), CI=CI)
+
+    
+
+    # Now lets plot the prediction interval
+    fig, (ax1) = plt.subplots(1, 1, figsize=(10,5))
+    ax1.errorbar(x, y, xerr=0, yerr=y_err,
+             fmt='o', ecolor='k', elinewidth=0.8, mfc='grey', ms=5, mec='k',capsize=3)
+    
+    ax1.plot(new_x_plot, Ne_corr2['preferred_values'], '-k', label='best fit')
+    ax1.plot(new_x_plot, Ne_corr2['lower_values'], ':k', label='lower vals')
+    ax1.plot(new_x_plot, Ne_corr2['upper_values'], ':k', label='upper vals')
+    ax1.set_xlabel('sec after midnight')
+    ax1.set_ylabel('Ne Corr factor')
+    ax1.set_title(str(100*CI) + ' % prediction interval')
+    ax1.legend()
+    ax1.plot(x, y, '+r', label='Ne lines')
+    ax1.ticklabel_format(useOffset=False)
+    
+
+    
+from scipy.stats import t
+import numpy as np
+
+def calculate_Ne_corr_std_err_values(*, pickle_str, new_x, CI=0.67):
+    # Load the model and the data from the pickle file
+    with open(pickle_str, 'rb') as f:
+        data = pickle.load(f)
+
+    model = data['model']
+    N_poly = model.order - 1
+    print(N_poly)
+    Pf = data['model']
+    x = data['x']
+    y = data['y']
+
+    # Calculate the residuals
+    residuals = y - Pf(x)
+
+    # Calculate the standard deviation of the residuals
+    residual_std = np.std(residuals)
+
+    # Calculate the standard errors for the new x values
+    mean_x = np.mean(x)
+    n = len(x)
+    standard_errors = residual_std * np.sqrt(1 + 1/n + (new_x - mean_x)**2 / np.sum((x - mean_x)**2))
+
+    # Calculate the degrees of freedom
+    df = len(x) - (N_poly + 1)
+
+    # Calculate the t value for the given confidence level
+    t_value = t.ppf((1 + CI) / 2, df)
+
+    # Calculate the prediction intervals
+    preferred_values = Pf(new_x)
+    lower_values = preferred_values - t_value * standard_errors
+    upper_values = preferred_values + t_value * standard_errors
+
+    df=pd.DataFrame(data={
+        'time': new_x,
+        'preferred_values': preferred_values,
+        'lower_values': lower_values,
+        'upper_values': upper_values
+    })
+
+    return df
+
+
+
+
+def calculate_Ne_corr_bootstrap_values(*, pickle_str, new_x, N_poly=3, CI=0.67, N_bootstrap=500):
+    # Load the model and the data from the pickle file
+    with open(pickle_str, 'rb') as f:
+        data = pickle.load(f)
+
+    Pf = data['model']
+    x = data['x']
+    y = data['y']
+
+    # Define the function
+
+    x_values=new_x
+    N_poly = N_poly  # degree of the polynomial
+    n_bootstrap = N_bootstrap  # number of bootstrap samples
+    confidence = CI  # confidence level
+
+    preferred_values = []
+    lower_values = []
+    upper_values = []
+
+    for new_x in x_values:
+        # Perform bootstrapping
+        bootstrap_predictions = []
+        for _ in range(n_bootstrap):
+            # Resample with replacement
+            bootstrap_indices = np.random.choice(len(x), size=len(x), replace=True)
+            bootstrap_x = x[bootstrap_indices]
+            bootstrap_y = y[bootstrap_indices]
+
+            # Perform polynomial regression on the bootstrap sample
+            bootstrap_coefficients = np.polyfit(bootstrap_x, bootstrap_y, N_poly)
+            bootstrap_Pf = np.poly1d(bootstrap_coefficients)
+
+            # Calculate predicted value for the new x
+            bootstrap_prediction = bootstrap_Pf(new_x)
+            bootstrap_predictions.append(bootstrap_prediction)
+
+        # Calculate prediction interval
+        lower_quantile = (1 - confidence) / 2
+        upper_quantile = 1 - lower_quantile
+        lower_index = int(lower_quantile * n_bootstrap)
+        upper_index = int(upper_quantile * n_bootstrap)
+        bootstrap_predictions_sorted = np.sort(bootstrap_predictions)
+        lower_value = bootstrap_predictions_sorted[lower_index]
+        upper_value = bootstrap_predictions_sorted[upper_index]
+
+        preferred_values.append(Pf(new_x))
+        lower_values.append(lower_value)
+        upper_values.append(upper_value)
+        
+    df=pd.DataFrame(data={'time': new_x,
+        'preferred_values': preferred_values,
+        'lower_values': lower_values,
+        'upper_values': upper_values}
+    )
+
+    return df
+    
+    
+
```

### Comparing `DiadFit-0.0.57/src/DiadFit.egg-info/PKG-INFO` & `DiadFit-0.0.59/src/DiadFit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiadFit
-Version: 0.0.57
+Version: 0.0.59
 Summary: DiadFit
 Home-page: https://github.com/PennyWieser/DiadFit
 Author: Penny Wieser
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/DiadFit)](https://pypi.org/project/DiadFit/)
         [![Build Status](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml)
```

### Comparing `DiadFit-0.0.57/src/DiadFit.egg-info/SOURCES.txt` & `DiadFit-0.0.59/src/DiadFit.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 setup.py
 src/DiadFit/CO2_EOS.py
 src/DiadFit/H2O_fitting.py
 src/DiadFit/Psensor.py
 src/DiadFit/__init__.py
 src/DiadFit/_version.py
+src/DiadFit/argon_lines.py
 src/DiadFit/cosmicray_filter.py
 src/DiadFit/densimeters.py
 src/DiadFit/density_depth_crustal_profiles.py
 src/DiadFit/diads.py
 src/DiadFit/error_propagation.py
 src/DiadFit/importing_data_files.py
 src/DiadFit/ne_lines.py
```

