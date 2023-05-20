# Comparing `tmp/findpeaks-2.4.6.tar.gz` & `tmp/findpeaks-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findpeaks-2.4.6.tar", last modified: Wed Mar 22 09:44:56 2023, max compression
+gzip compressed data, was "findpeaks-2.4.7.tar", last modified: Sat May 20 18:40:20 2023, max compression
```

## Comparing `findpeaks-2.4.6.tar` & `findpeaks-2.4.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 09:44:56.644795 findpeaks-2.4.6/
--rw-rw-rw-   0        0        0     1122 2021-01-28 13:20:53.000000 findpeaks-2.4.6/LICENSE
--rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0     8765 2023-03-22 09:44:56.643799 findpeaks-2.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     8149 2023-02-18 16:10:18.000000 findpeaks-2.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-03-22 09:44:56.502195 findpeaks-2.4.6/findpeaks/
--rw-rw-rw-   0        0        0     2199 2023-03-22 09:43:25.000000 findpeaks-2.4.6/findpeaks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 09:44:56.563118 findpeaks-2.4.6/findpeaks/data/
--rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.4.6/findpeaks/data/__init__.py
--rw-rw-rw-   0        0        0    18309 2023-02-25 10:27:27.000000 findpeaks-2.4.6/findpeaks/examples.py
-drwxrwxrwx   0        0        0        0 2023-03-22 09:44:56.628838 findpeaks-2.4.6/findpeaks/filters/
--rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.4.6/findpeaks/filters/__init__.py
--rw-rw-rw-   0        0        0     5665 2021-12-05 14:23:41.000000 findpeaks-2.4.6/findpeaks/filters/frost.py
--rw-rw-rw-   0        0        0     4133 2021-12-05 14:23:35.000000 findpeaks-2.4.6/findpeaks/filters/kuan.py
--rw-rw-rw-   0        0        0     6429 2021-12-05 14:24:04.000000 findpeaks-2.4.6/findpeaks/filters/lee.py
--rw-rw-rw-   0        0        0     5248 2021-12-05 14:25:22.000000 findpeaks-2.4.6/findpeaks/filters/lee_enhanced.py
--rw-rw-rw-   0        0        0     3921 2021-12-05 14:27:45.000000 findpeaks-2.4.6/findpeaks/filters/mean.py
--rw-rw-rw-   0        0        0     3180 2021-12-05 14:30:08.000000 findpeaks-2.4.6/findpeaks/filters/median.py
--rw-rw-rw-   0        0        0    50237 2023-02-24 22:45:37.000000 findpeaks-2.4.6/findpeaks/findpeaks.py
--rw-rw-rw-   0        0        0     5995 2021-12-05 12:54:20.000000 findpeaks-2.4.6/findpeaks/interpolate.py
--rw-rw-rw-   0        0        0    23022 2023-02-24 22:51:49.000000 findpeaks-2.4.6/findpeaks/stats.py
-drwxrwxrwx   0        0        0        0 2023-03-22 09:44:56.641841 findpeaks-2.4.6/findpeaks/tests/
--rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.4.6/findpeaks/tests/__init__.py
--rw-rw-rw-   0        0        0     9112 2021-12-05 15:01:16.000000 findpeaks-2.4.6/findpeaks/tests/test_findpeaks.py
--rw-rw-rw-   0        0        0     2469 2021-01-28 13:20:53.000000 findpeaks-2.4.6/findpeaks/union_find.py
-drwxrwxrwx   0        0        0        0 2023-03-22 09:44:56.549963 findpeaks-2.4.6/findpeaks.egg-info/
--rw-rw-rw-   0        0        0     8765 2023-03-22 09:44:55.000000 findpeaks-2.4.6/findpeaks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      622 2023-03-22 09:44:56.000000 findpeaks-2.4.6/findpeaks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 09:44:55.000000 findpeaks-2.4.6/findpeaks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-03-22 09:44:56.000000 findpeaks-2.4.6/findpeaks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-22 09:44:56.000000 findpeaks-2.4.6/findpeaks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-22 09:44:56.644795 findpeaks-2.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1469 2023-03-22 09:37:25.000000 findpeaks-2.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 18:40:20.099969 findpeaks-2.4.7/
+-rw-rw-rw-   0        0        0     1122 2021-01-28 13:20:53.000000 findpeaks-2.4.7/LICENSE
+-rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     8724 2023-05-20 18:40:20.082904 findpeaks-2.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8149 2023-02-18 16:10:18.000000 findpeaks-2.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 18:40:19.946205 findpeaks-2.4.7/findpeaks/
+-rw-rw-rw-   0        0        0     2199 2023-05-20 18:24:20.000000 findpeaks-2.4.7/findpeaks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 18:40:20.007900 findpeaks-2.4.7/findpeaks/data/
+-rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.4.7/findpeaks/data/__init__.py
+-rw-rw-rw-   0        0        0    18962 2023-05-20 18:02:04.000000 findpeaks-2.4.7/findpeaks/examples.py
+drwxrwxrwx   0        0        0        0 2023-05-20 18:40:20.062249 findpeaks-2.4.7/findpeaks/filters/
+-rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.4.7/findpeaks/filters/__init__.py
+-rw-rw-rw-   0        0        0     5665 2021-12-05 14:23:41.000000 findpeaks-2.4.7/findpeaks/filters/frost.py
+-rw-rw-rw-   0        0        0     4133 2021-12-05 14:23:35.000000 findpeaks-2.4.7/findpeaks/filters/kuan.py
+-rw-rw-rw-   0        0        0     6429 2021-12-05 14:24:04.000000 findpeaks-2.4.7/findpeaks/filters/lee.py
+-rw-rw-rw-   0        0        0     5248 2021-12-05 14:25:22.000000 findpeaks-2.4.7/findpeaks/filters/lee_enhanced.py
+-rw-rw-rw-   0        0        0     3921 2021-12-05 14:27:45.000000 findpeaks-2.4.7/findpeaks/filters/mean.py
+-rw-rw-rw-   0        0        0     3180 2021-12-05 14:30:08.000000 findpeaks-2.4.7/findpeaks/filters/median.py
+-rw-rw-rw-   0        0        0    52243 2023-05-20 18:08:01.000000 findpeaks-2.4.7/findpeaks/findpeaks.py
+-rw-rw-rw-   0        0        0     5995 2021-12-05 12:54:20.000000 findpeaks-2.4.7/findpeaks/interpolate.py
+-rw-rw-rw-   0        0        0    23022 2023-02-24 22:51:49.000000 findpeaks-2.4.7/findpeaks/stats.py
+drwxrwxrwx   0        0        0        0 2023-05-20 18:40:20.081913 findpeaks-2.4.7/findpeaks/tests/
+-rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.4.7/findpeaks/tests/__init__.py
+-rw-rw-rw-   0        0        0     9124 2023-05-20 18:26:50.000000 findpeaks-2.4.7/findpeaks/tests/test_findpeaks.py
+-rw-rw-rw-   0        0        0     2469 2021-01-28 13:20:53.000000 findpeaks-2.4.7/findpeaks/union_find.py
+drwxrwxrwx   0        0        0        0 2023-05-20 18:40:19.989403 findpeaks-2.4.7/findpeaks.egg-info/
+-rw-rw-rw-   0        0        0     8724 2023-05-20 18:40:19.000000 findpeaks-2.4.7/findpeaks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2023-05-20 18:40:19.000000 findpeaks-2.4.7/findpeaks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 18:40:19.000000 findpeaks-2.4.7/findpeaks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-05-20 18:40:19.000000 findpeaks-2.4.7/findpeaks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-20 18:40:19.000000 findpeaks-2.4.7/findpeaks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 18:40:20.100972 findpeaks-2.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1467 2023-05-20 18:39:58.000000 findpeaks-2.4.7/setup.py
```

### Comparing `findpeaks-2.4.6/LICENSE` & `findpeaks-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.6/PKG-INFO` & `findpeaks-2.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: findpeaks
-Version: 2.4.6
+Version: 2.4.7
 Summary: findpeaks is for the detection of peaks and valleys in a 1D vector and 2D array (image).
 Home-page: https://erdogant.github.io/findpeaks
-Download-URL: https://github.com/erdogant/findpeaks/archive/2.4.6.tar.gz
+Download-URL: https://github.com/erdogant/findpeaks/archive/2.4.7.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -185,9 +183,7 @@
 ### Citation
 Please cite ``findpeaks`` in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
-
-
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: findpeaks Version: 2.4.6 Summary: findpeaks is for
+Metadata-Version: 2.1 Name: findpeaks Version: 2.4.7 Summary: findpeaks is for
 the detection of peaks and valleys in a 1D vector and 2D array (image). Home-
 page: https://erdogant.github.io/findpeaks Download-URL: https://github.com/
-erdogant/findpeaks/archive/2.4.6.tar.gz Author: Erdogan Taskesen Author-email:
-erdogant@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # findpeaks [!
-[Python](https://img.shields.io/pypi/pyversions/findpeaks)](https://
-img.shields.io/pypi/pyversions/findpeaks) [![Pypi](https://img.shields.io/pypi/
-v/findpeaks)](https://pypi.org/project/findpeaks/) [![Docs](https://
-img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/findpeaks/
-) [![LOC](https://sloc.xyz/github/erdogant/findpeaks/?category=code)](https://
-github.com/erdogant/findpeaks/) [![Downloads](https://static.pepy.tech/
-personalized-badge/
+erdogant/findpeaks/archive/2.4.7.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE # findpeaks [![Python](https://img.shields.io/pypi/
+pyversions/findpeaks)](https://img.shields.io/pypi/pyversions/findpeaks) [!
+[Pypi](https://img.shields.io/pypi/v/findpeaks)](https://pypi.org/project/
+findpeaks/) [![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
+erdogant.github.io/findpeaks/) [![LOC](https://sloc.xyz/github/erdogant/
+findpeaks/?category=code)](https://github.com/erdogant/findpeaks/) [!
+[Downloads](https://static.pepy.tech/personalized-badge/
 findpeaks?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/
 month)](https://pepy.tech/project/findpeaks) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 findpeaks?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)]
 (https://pepy.tech/project/findpeaks) [![License](https://img.shields.io/badge/
 license-MIT-green.svg)](https://github.com/erdogant/findpeaks/blob/master/
 LICENSE) [![Forks](https://img.shields.io/github/forks/erdogant/findpeaks.svg)]
```

### Comparing `findpeaks-2.4.6/README.md` & `findpeaks-2.4.7/README.md`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.6/findpeaks/__init__.py` & `findpeaks-2.4.7/findpeaks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from findpeaks.filters.median import median_filter
 from findpeaks.filters.mean import mean_filter
 
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.4.6'
+__version__ = '2.4.7'
 
 # module level doc-string
 __doc__ = """
 findpeaks
 =====================================================================
 
 Description
```

### Comparing `findpeaks-2.4.6/findpeaks/examples.py` & `findpeaks-2.4.7/findpeaks/examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,30 @@
 # print(dir(findpeaks))
 # print(findpeaks.__version__)
 
 # pip install opencv-python
 # import matplotlib.pyplot as plt
 # from findpeaks import findpeaks
 
+# %% Issue 18:
+from findpeaks import findpeaks
+
+fp = findpeaks(method='topology', scale=False, denoise=None, togray=False, imsize=False, window=15)
+X = fp.import_example('2dpeaks')
+fp.fit(X)
+# fp.plot_mesh(wireframe=False, title='Test', cmap='RdBu', view=(70,5))
+fp.plot_mesh()
+fp.plot_mesh(xlim=[10, 30], ylim=[4, 10])
+fp.plot_mesh(xlim=[10, None], ylim=[4, 10])
+fp.plot_mesh(xlim=[10, None], ylim=[4, None])
+fp.plot_mesh(xlim=[10, 30], ylim=[4, 10], zlim=[0, 3])
+fp.plot_mesh(xlim=[10, 30], ylim=[4, 10], zlim=[0, None])
+fp.plot_mesh(xlim=[10, 30], ylim=[4, 10], zlim=[None, 6])
+fp.plot_mesh(xlim=[10, 30], ylim=[4, 10], zlim=[2, 6])
+
 # %%
 from findpeaks import findpeaks
 path = r'https://user-images.githubusercontent.com/44827483/221152897-133839bb-7364-492a-921b-c9077ab9930b.png'
 fp = findpeaks(method='topology', denoise='lee_enhanced', window=5, whitelist='peak')
 
 X = fp.imread(path)
 results = fp.fit(X)
```

### Comparing `findpeaks-2.4.6/findpeaks/filters/frost.py` & `findpeaks-2.4.7/findpeaks/filters/frost.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.6/findpeaks/filters/kuan.py` & `findpeaks-2.4.7/findpeaks/filters/kuan.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.6/findpeaks/filters/lee.py` & `findpeaks-2.4.7/findpeaks/filters/lee.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.6/findpeaks/filters/lee_enhanced.py` & `findpeaks-2.4.7/findpeaks/filters/lee_enhanced.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.6/findpeaks/filters/mean.py` & `findpeaks-2.4.7/findpeaks/filters/mean.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.6/findpeaks/filters/median.py` & `findpeaks-2.4.7/findpeaks/filters/median.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.6/findpeaks/findpeaks.py` & `findpeaks-2.4.7/findpeaks/findpeaks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Python library for the detection of peaks and valleys."""
 # ----------------------------------------------------
 # Name        : findpeaks.py
 # Author      : E.Taskesen
 # Contact     : erdogant@gmail.com
 # github      : https://github.com/erdogant/findpeaks
 # Licence     : See LICENSE
 # ----------------------------------------------------
@@ -27,15 +28,15 @@
 import findpeaks.stats as stats
 from findpeaks.stats import disable_tqdm
 import findpeaks.interpolate as interpolate
 
 
 # %%
 class findpeaks():
-    """For the detection of peaks in 1d and 2d data.
+    """Python library for the detection of peaks and valleys.
 
     findpeaks is for the detection and vizualization of peaks and valleys in a 1D-vector and 2D-array.
     In case of 2D-array, the image can be pre-processed by resizing, scaling, and denoising. For a 1D-vector,
     pre-processing by interpolation is possible. Peaks can be detected using various methods, and the results can be
     vizualized, such as the preprocessing steps, the persistence of peaks, the masking plot and a 3d-mesh plot.
 
     Examples
@@ -855,15 +856,27 @@
                 ax3.text(idx[1], idx[0], 'v' + self.results['Xranked'][idx].astype(str))
 
         # Show plot
         plt.show()
         # Return
         return (ax1, ax2, ax3)
 
-    def plot_mesh(self, wireframe=True, surface=True, rstride=2, cstride=2, cmap=plt.cm.hot_r, title='', figsize=None, view=None, savepath=None):
+    def plot_mesh(self,
+                  wireframe=True,
+                  surface=True,
+                  rstride=2,
+                  cstride=2,
+                  cmap=plt.cm.hot_r,
+                  view=None,
+                  xlim=None,
+                  ylim=None,
+                  zlim=None,
+                  title='',
+                  figsize=None,
+                  savepath=None):
         """Plot the 3d-mesh.
 
         Parameters
         ----------
         wireframe : bool, (default is True)
             Plot the wireframe
         surface : bool, (default is True)
@@ -878,14 +891,32 @@
             * Rotate the mesh plot.
             * (0, 0) : y vs z
             * (0, 90) : x vs z
             * (90, 0) : y vs x
             * (90, 90) : x vs y
         cmap : object
             Colormap. The default is plt.cm.hot_r.
+        xlim : tuple(int, int), (default: None)
+            x-limit in the axis.
+            None: No limit.
+            [1, 5]: Limit between the range 1 and 5.
+            [1, None]: Limit between range 1 and unlimited.
+            [None, 5]: Limit between range unlimited and 5.
+        ylim : tuple(int, int), (default: None)
+            y-limit in the axis.
+            None: No limit.
+            [1, 5]: Limit between the range 1 and 5.
+            [1, None]: Limit between range 1 and unlimited.
+            [None, 5]: Limit between range unlimited and 5.
+        zlim : tuple(int, int), (default: None)
+            z-limit in the axis.
+            None: No limit.
+            [1, 5]: Limit between the range 1 and 5.
+            [1, None]: Limit between range 1 and unlimited.
+            [None, 5]: Limit between range unlimited and 5.
         figsize : (int, int), (default: None)
             (width, height) in inches.
         savepath : bool (default : None)
             Path with filename to save the figure, eg: './tmp/my_image.png'
         verbose : int (default : 3)
             Print to screen. 0: None, 1: Error, 2: Warning, 3: Info, 4: Debug, 5: Trace.
 
@@ -902,51 +933,67 @@
             return None
 
         figsize = figsize if figsize is not None else self.args['figsize']
         if self.verbose>=3: print('[findpeaks] >Plotting 3d-mesh..')
         ax1, ax2 = None, None
         if savepath is not None:
             savepath = str.replace(savepath, ',', '_')
-            # savepath = str.replace(savepath, ':', '_')
             savepath = str.replace(savepath, '=', '_')
-            # savepath = str.replace(savepath, ' ', '_')
 
         # Compute meshgrid
-        xx, yy = np.mgrid[0:self.results['Xproc'].shape[0], 0:self.results['Xproc'].shape[1]]
+        Z = self.results['Xproc'].copy()
+        X, Y = np.mgrid[0:Z.shape[0], 0:Z.shape[1]]
+        # To limit on the X and Y axis, we need to create a trick by setting all values to nan in the Z-axis that should be limited.
+        if xlim is not None:
+            if xlim[0] is not None: Z[X<xlim[0]]=np.nan
+            if xlim[1] is not None: Z[X>xlim[1]]=np.nan
+        if ylim is not None:
+            if ylim[0] is not None: Z[Y<ylim[0]]=np.nan
+            if ylim[1] is not None: Z[Y>ylim[1]]=np.nan
+        if zlim is not None:
+            if zlim[0] is not None: Z[Z<zlim[0]]=np.nan
+            if zlim[1] is not None: Z[Z>zlim[1]]=np.nan
 
         # Plot the figure
         if wireframe:
             fig = plt.figure(figsize=figsize)
             ax1 = fig.add_subplot(projection='3d')
             ax1 = fig.gca()
-            ax1.plot_wireframe(xx, yy, self.results['Xproc'], rstride=rstride, cstride=cstride, linewidth=0.8)
+            ax1.plot_wireframe(X, Y, Z, rstride=rstride, cstride=cstride, linewidth=0.8)
             ax1.set_xlabel('x-axis')
             ax1.set_ylabel('y-axis')
             ax1.set_zlabel('z-axis')
             if view is not None:
                 ax1.view_init(view[0], view[1])
                 # ax1.view_init(50, -10) # x vs y
             ax1.set_title(title)
+            if xlim is not None: ax1.set_xlim3d(xlim[0], xlim[1])
+            if ylim is not None: ax1.set_ylim3d(ylim[0], ylim[1])
+            if zlim is not None: ax1.set_zlim3d(zlim[0], zlim[1])
+
             plt.show()
             if savepath is not None:
                 if self.verbose>=3: print('[findpeaks] >Saving wireframe to disk..')
                 fig.savefig(savepath)
 
         if surface:
             # Plot the figure
             fig = plt.figure(figsize=figsize)
             ax2 = fig.add_subplot(projection='3d')
             ax2 = fig.gca()
-            ax2.plot_surface(xx, yy, self.results['Xproc'], rstride=rstride, cstride=cstride, cmap=cmap, linewidth=0, shade=True, antialiased=False)
+            ax2.plot_surface(X, Y, Z, rstride=rstride, cstride=cstride, cmap=cmap, linewidth=0, shade=True, antialiased=False)
             if view is not None:
                 ax2.view_init(view[0], view[1])
             ax2.set_xlabel('x-axis')
             ax2.set_ylabel('y-axis')
             ax2.set_zlabel('z-axis')
             ax2.set_title(title)
+            if xlim is not None: ax2.set_xlim3d(xlim[0], xlim[1])
+            if ylim is not None: ax2.set_ylim3d(ylim[0], ylim[1])
+            if zlim is not None: ax2.set_zlim3d(zlim[0], zlim[1])
             plt.show()
             if savepath is not None:
                 if self.verbose>=3: print('[findpeaks] >Saving surface to disk..')
                 fig.savefig(savepath)
 
         # Plot with contours
         # fig = plt.figure(figsize=figsize)
```

### Comparing `findpeaks-2.4.6/findpeaks/interpolate.py` & `findpeaks-2.4.7/findpeaks/interpolate.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.6/findpeaks/stats.py` & `findpeaks-2.4.7/findpeaks/stats.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.6/findpeaks/tests/test_findpeaks.py` & `findpeaks-2.4.7/findpeaks/tests/test_findpeaks.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,14 +187,14 @@
         img = fp.import_example('2dpeaks')
     
         for getfilter in filters:
             for window in windows:
                 for cu in cus:
                     fp = findpeaks(method='topology', scale=True, denoise=getfilter, window=window, cu=cu, togray=True, imsize=None, verbose=3)
                     assert fp.fit(img)
-                    assert fp.plot_mesh(wireframe=False)
-                    plt.close('all')
-                    assert fp.plot_persistence()
-                    plt.close('all')
-                    assert fp.plot()
-                    plt.close('all')
+                    # assert fp.plot_mesh(wireframe=False)
+                    # plt.close('all')
+                    # assert fp.plot_persistence()
+                    # plt.close('all')
+                    # assert fp.plot()
+                    # plt.close('all')
                     # assert fp.plot_preprocessing()
```

### Comparing `findpeaks-2.4.6/findpeaks/union_find.py` & `findpeaks-2.4.7/findpeaks/union_find.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.6/findpeaks.egg-info/PKG-INFO` & `findpeaks-2.4.7/findpeaks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: findpeaks
-Version: 2.4.6
+Version: 2.4.7
 Summary: findpeaks is for the detection of peaks and valleys in a 1D vector and 2D array (image).
 Home-page: https://erdogant.github.io/findpeaks
-Download-URL: https://github.com/erdogant/findpeaks/archive/2.4.6.tar.gz
+Download-URL: https://github.com/erdogant/findpeaks/archive/2.4.7.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -185,9 +183,7 @@
 ### Citation
 Please cite ``findpeaks`` in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
-
-
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: findpeaks Version: 2.4.6 Summary: findpeaks is for
+Metadata-Version: 2.1 Name: findpeaks Version: 2.4.7 Summary: findpeaks is for
 the detection of peaks and valleys in a 1D vector and 2D array (image). Home-
 page: https://erdogant.github.io/findpeaks Download-URL: https://github.com/
-erdogant/findpeaks/archive/2.4.6.tar.gz Author: Erdogan Taskesen Author-email:
-erdogant@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # findpeaks [!
-[Python](https://img.shields.io/pypi/pyversions/findpeaks)](https://
-img.shields.io/pypi/pyversions/findpeaks) [![Pypi](https://img.shields.io/pypi/
-v/findpeaks)](https://pypi.org/project/findpeaks/) [![Docs](https://
-img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/findpeaks/
-) [![LOC](https://sloc.xyz/github/erdogant/findpeaks/?category=code)](https://
-github.com/erdogant/findpeaks/) [![Downloads](https://static.pepy.tech/
-personalized-badge/
+erdogant/findpeaks/archive/2.4.7.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE # findpeaks [![Python](https://img.shields.io/pypi/
+pyversions/findpeaks)](https://img.shields.io/pypi/pyversions/findpeaks) [!
+[Pypi](https://img.shields.io/pypi/v/findpeaks)](https://pypi.org/project/
+findpeaks/) [![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
+erdogant.github.io/findpeaks/) [![LOC](https://sloc.xyz/github/erdogant/
+findpeaks/?category=code)](https://github.com/erdogant/findpeaks/) [!
+[Downloads](https://static.pepy.tech/personalized-badge/
 findpeaks?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/
 month)](https://pepy.tech/project/findpeaks) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 findpeaks?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)]
 (https://pepy.tech/project/findpeaks) [![License](https://img.shields.io/badge/
 license-MIT-green.svg)](https://github.com/erdogant/findpeaks/blob/master/
 LICENSE) [![Forks](https://img.shields.io/github/forks/erdogant/findpeaks.svg)]
```

### Comparing `findpeaks-2.4.6/findpeaks.egg-info/SOURCES.txt` & `findpeaks-2.4.7/findpeaks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.6/setup.py` & `findpeaks-2.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Setup ------------
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
-     install_requires=['scipy','matplotlib','numpy','pandas','tqdm','peakdetect==1.1','requests','caerus>="0.1.9"'],
+     install_requires=['scipy','matplotlib','numpy','pandas','tqdm','peakdetect==1.1','requests','caerus>=0.1.9'],
      python_requires='>=3',
      name='findpeaks',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
      description="findpeaks is for the detection of peaks and valleys in a 1D vector and 2D array (image).",
      long_description=long_description,
```

