# Comparing `tmp/ssid-0.0.2.tar.gz` & `tmp/ssid-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssid-0.0.2.tar", last modified: Mon Aug 15 15:43:05 2022, max compression
+gzip compressed data, was "ssid-0.0.3.tar", last modified: Sat May 20 21:18:44 2023, max compression
```

## Comparing `ssid-0.0.2.tar` & `ssid-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,29 @@
-drwxr-xr-x   0 claudio   (1000) claudio   (1000)        0 2022-08-15 15:43:05.552796 ssid-0.0.2/
--rw-r--r--   0 claudio   (1000) claudio   (1000)      324 2022-08-15 15:43:05.552796 ssid-0.0.2/PKG-INFO
--rw-r--r--   0 claudio   (1000) claudio   (1000)      569 2022-08-15 15:42:57.000000 ssid-0.0.2/pyproject.toml
--rw-r--r--   0 claudio   (1000) claudio   (1000)       38 2022-08-15 15:43:05.552796 ssid-0.0.2/setup.cfg
--rwxr-xr-x   0 claudio   (1000) claudio   (1000)      718 2022-07-25 03:40:43.000000 ssid-0.0.2/setup.py
-drwxr-xr-x   0 claudio   (1000) claudio   (1000)        0 2022-08-15 15:43:05.552796 ssid-0.0.2/src/
-drwxr-xr-x   0 claudio   (1000) claudio   (1000)        0 2022-08-15 15:43:05.552796 ssid-0.0.2/src/ssid/
--rwxr-xr-x   0 claudio   (1000) claudio   (1000)     2682 2022-05-06 02:51:56.000000 ssid-0.0.2/src/ssid/ExtractModes.py
--rw-r--r--   0 claudio   (1000) claudio   (1000)      138 2022-05-06 02:51:56.000000 ssid-0.0.2/src/ssid/__init__.py
--rw-r--r--   0 claudio   (1000) claudio   (1000)     4215 2022-08-15 15:00:23.000000 ssid-0.0.2/src/ssid/__main__.py
-drwxr-xr-x   0 claudio   (1000) claudio   (1000)        0 2022-08-15 15:43:05.552796 ssid-0.0.2/src/ssid/brace2/
--rw-r--r--   0 claudio   (1000) claudio   (1000)     2925 2022-07-25 23:21:58.000000 ssid-0.0.2/src/ssid/brace2/__main__.py
--rw-r--r--   0 claudio   (1000) claudio   (1000)     5998 2022-07-25 06:41:04.000000 ssid-0.0.2/src/ssid/integrate.py
--rwxr-xr-x   0 claudio   (1000) claudio   (1000)    14449 2022-07-25 06:38:24.000000 ssid-0.0.2/src/ssid/okid.py
--rw-r--r--   0 claudio   (1000) claudio   (1000)      294 2022-05-06 02:51:56.000000 ssid-0.0.2/src/ssid/spec.py
--rw-r--r--   0 claudio   (1000) claudio   (1000)    21433 2022-08-15 15:06:41.000000 ssid-0.0.2/src/ssid/srim.py
-drwxr-xr-x   0 claudio   (1000) claudio   (1000)        0 2022-08-15 15:43:05.552796 ssid-0.0.2/src/ssid.egg-info/
--rw-r--r--   0 claudio   (1000) claudio   (1000)      324 2022-08-15 15:43:05.000000 ssid-0.0.2/src/ssid.egg-info/PKG-INFO
--rw-r--r--   0 claudio   (1000) claudio   (1000)      319 2022-08-15 15:43:05.000000 ssid-0.0.2/src/ssid.egg-info/SOURCES.txt
--rw-r--r--   0 claudio   (1000) claudio   (1000)        1 2022-08-15 15:43:05.000000 ssid-0.0.2/src/ssid.egg-info/dependency_links.txt
--rw-r--r--   0 claudio   (1000) claudio   (1000)        5 2022-08-15 15:43:05.000000 ssid-0.0.2/src/ssid.egg-info/top_level.txt
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-05-20 21:18:44.772606 ssid-0.0.3/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      341 2023-05-20 21:18:44.772606 ssid-0.0.3/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      685 2023-05-20 21:13:24.000000 ssid-0.0.3/pyproject.toml
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       38 2023-05-20 21:18:44.772606 ssid-0.0.3/setup.cfg
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)      718 2023-05-20 17:46:14.000000 ssid-0.0.3/setup.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-05-20 21:18:44.762606 ssid-0.0.3/src/
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-05-20 21:18:44.772606 ssid-0.0.3/src/ssid/
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)     4696 2023-05-20 17:46:20.000000 ssid-0.0.3/src/ssid/ExtractModes.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       27 2023-05-20 21:13:24.000000 ssid-0.0.3/src/ssid/__init__.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     4819 2023-05-20 21:13:24.000000 ssid-0.0.3/src/ssid/__main__.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-05-20 21:18:44.772606 ssid-0.0.3/src/ssid/brace2/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2925 2023-05-20 17:46:14.000000 ssid-0.0.3/src/ssid/brace2/__main__.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     5997 2023-05-20 17:46:14.000000 ssid-0.0.3/src/ssid/integrate.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1692 2023-05-20 17:46:20.000000 ssid-0.0.3/src/ssid/markov.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2036 2023-05-20 17:46:20.000000 ssid-0.0.3/src/ssid/modes.py
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)    21710 2023-05-20 17:46:20.000000 ssid-0.0.3/src/ssid/okid.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)    14802 2023-05-20 21:13:24.000000 ssid-0.0.3/src/ssid/realize.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      294 2023-05-20 17:46:14.000000 ssid-0.0.3/src/ssid/spec.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)    17469 2023-05-20 17:46:14.000000 ssid-0.0.3/src/ssid/srim.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      415 2023-05-20 17:46:20.000000 ssid-0.0.3/src/ssid/system.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1224 2023-05-20 17:46:14.000000 ssid-0.0.3/src/ssid/validation.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-05-20 21:18:44.772606 ssid-0.0.3/src/ssid.egg-info/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      341 2023-05-20 21:18:44.000000 ssid-0.0.3/src/ssid.egg-info/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      468 2023-05-20 21:18:44.000000 ssid-0.0.3/src/ssid.egg-info/SOURCES.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2023-05-20 21:18:44.000000 ssid-0.0.3/src/ssid.egg-info/dependency_links.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       44 2023-05-20 21:18:44.000000 ssid-0.0.3/src/ssid.egg-info/entry_points.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        5 2023-05-20 21:18:44.000000 ssid-0.0.3/src/ssid.egg-info/top_level.txt
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-05-20 21:18:44.772606 ssid-0.0.3/tests/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3468 2023-05-20 17:46:14.000000 ssid-0.0.3/tests/test1.py
```

### Comparing `ssid-0.0.2/setup.py` & `ssid-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `ssid-0.0.2/src/ssid/__main__.py` & `ssid-0.0.3/src/ssid/brace2/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,83 +25,46 @@
     freq   frequency
     cycl   cyclic frequency
     t      period
     m      modes
     c      condition-number
 """
 
-def parse_brace2(args, config):
-    pass
 
 def parse_args(args):
     outputs = []
     parsers = {
         "srim": parse_srim,
         "test": parse_srim,
-        "okid": parse_okid,
         "okid": parse_okid
     }
-    config = {
-            "method": None,
-            "operation": None,
-            "protocol": None
-    }
-    config["channels"] = channels = [[], []]
+    config = {}
     argi = iter(args[1:])
     for arg in argi:
         if arg == "-p":
             outputs.append(next(arg))
-        elif arg == "--setup":
+        if arg == "--setup":
             install_me()
             sys.exit()
         elif arg in ["--help", "-h"]:
             print(HELP)
             sys.exit()
-        elif arg == "--protocol":
-            config["protocol"] = next(arg)
-
-        # Positional args
-        elif config["method"] is None:
-            config["method"] = arg
-            break
-
-        elif config["protocol"] and config["operation"] is None:
-            config["operation"] = arg
-
-        elif arg == "--inputs":
-            inputs = next(argi)[1:-1].split(",")
-            if isinstance(inputs, str):
-                channels[0] = [int(inputs)]
-            else:
-                channels[0] = list(map(int, inputs))
-        elif arg == "--outputs":
-            outputs = next(argi)[1:-1].split(",")
-            if isinstance(outputs, str):
-                channels[1] = [int(outputs)]
-            else:
-                channels[1] = list(map(int, outputs))
-        elif arg == "--":
-            continue
-
         else:
-            break
-
-    return parsers[arg](argi, config), outputs
+            config["method"] = arg
+            return parsers[arg](argi, config), outputs
 
 if __name__ == "__main__":
     import sys
     import quakeio
     import numpy as np
     from pathlib import Path
+    channels = [[17, 3, 20], [9, 7, 4]]
     method = None
 
     config, out_ops = parse_args(sys.argv)
-    sys.exit()
-
-    channels = config.get("channels", [[17, 3, 20], [9, 7, 4]])
 
     if config["method"] == "test":
         data_dir = Path("RioDell_Petrolia_Processed_Data")
 
         first_input = quakeio.read(data_dir/f"CHAN{channels[0][0]:03d}.V2")
         npoints = len(first_input.accel.data)
         inputs, outputs = np.zeros((2,npoints,len(channels[0])))
@@ -116,34 +79,25 @@
             outputs[:,i] = quakeio.read(data_dir/f"CHAN{inp:03d}.V2").accel.data
 
         dt = first_input.accel["time_step"]
         config["dt"] = dt
 
     elif "event_file" in config:
         event = quakeio.read(config["event_file"])
-        try:
-            inputs = [
-                event.match("l", station_channel=f"{i}").accel.data for i in channels[0]
-            ]
-        except AttributeError:
-            print(f"{channels[0]}", "\n"*3, file=sys.stderr)
-            raise
-
-        try:
-            outputs = [
-                event.match("l", station_channel=f"{i}").accel.data for i in channels[1]
-            ]
-        except AttributeError:
-            print(f"{channels[1]}", "\n"*3, file=sys.stderr)
-            raise
-
-        #npoints = len(inputs[:,0])
-        dt = event.match("l", station_channel=f"{channels[0][0]}").accel["time_step"]
+        inputs = np.array([
+            event.at(file_name=f"CHAN{i:03d}.V2").accel.data for i in channels[0]
+        ]).T
+        outputs = np.array([
+            event.at(file_name=f"CHAN{i:03d}.V2").accel.data for i in channels[1]
+        ]).T
+        npoints = len(inputs[:,0])
+        dt = event.at(file_name=f"CHAN{channels[0][0]:03d}.V2").accel["time_step"]
         config["dt"] = dt
 
+    #print(config)
 
     A,B,C,D = srim(inputs, outputs, **config)
 
     freqdmpSRIM, modeshapeSRIM, *_ = ComposeModes(dt, A, B, C, D)
 
     if not out_ops:
         print(f"period: {np.real(1/freqdmpSRIM[:,0])}")
```

### Comparing `ssid-0.0.2/src/ssid/integrate.py` & `ssid-0.0.3/src/ssid/integrate.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,14 @@
             per=per,
             gamma=gamma,
             beta=beta,
             damping=damping,
             interp=interp
         )
 
-
     @_plot_func
     def plot(self, **kwds):
         #sa = spectrum(self._accel, **kwds)
         tsa = self.spect(self._accel, **kwds)
         if len(tsa) > 2:
             for sa in tsa[1:]:
                 self.ax.plot(tsa[0], sa)
```

### Comparing `ssid-0.0.2/src/ssid/okid.py` & `ssid-0.0.3/src/ssid/srim.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,224 @@
-import numpy as np
-from numpy import zeros, pi, size
-import scipy.linalg
+__doc__="""
+# ssid : Structural System Identification
+"""
+# Standard library
+import sys
+import json
+import multiprocessing
+from functools import partial
+# Dependencies
+try:
+    from tqdm import tqdm
+except:
+    tqdm = lambda x,*args,**kwds: x
 
-linsolve = scipy.linalg.solve
+import quakeio
+import numpy as np
+# from numpy import pi, log, sign
+from numpy.linalg import eig
+# import scipy.linalg as sl
+from ssid import ExtractModes
 
+linsolve = np.linalg.solve
 lsqminnorm = lambda *args: np.linalg.lstsq(*args, rcond=None)[0]
 
-def parse_okid(args, config):
-    """
-    p determines order of the observer Kalman ARX filter used in OKID-ERA-DC.
-    n determines size of the state-space model used for representing the system.
+class JSON_Encoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, np.ndarray):
+            return obj.tolist()
+        elif isinstance(obj, np.integer):
+            return int(obj)
+        elif isinstance(obj, np.floating):
+            return float(obj)
+        return json.JSONEncoder.default(self, obj)
+
+REQUIREMENTS = """
+numpy
+scipy
+tqdm
+quakeio
+"""
+
+"""
+ssid srim <event.zip> <options>
+
+Options
+-p
+-m
+"""
+
+class IdentifiedSystem:
+    def __init__(self, time_step, A, B, C, D, **kwds):
+        self.system = A, B, C, D
+        self.freqdmp, modeshapeSRIM, *_ = ExtractModes.ComposeModes(time_step, A, B, C, D)
+
+    def __repr__(self):
+        import textwrap
+        try:
+            nln = "\n                "
+            return textwrap.dedent(f"""
+            Spectral quantities:
+                   T      \N{Mathematical Italic Small F}       \N{Greek Small Letter Zeta}
+                {nln.join(f"{1/i: <6.4}  {i: <6.4}  {j: <6.4}" for i,j in np.real(self.freqdmp[:,:2]))}
+            """)
+        except Exception as e:
+            return f"Error extracting modes: {e}; got '{self.freqdmp = }'"
+
+def parse_args(args):
+    outputs = []
+    parsers = {
+        "srim": parse_srim,
+        "test": parse_srim,
+        "okid": parse_okid
+    }
+    config = {}
+    argi = iter(args[1:])
+    for arg in argi:
+        if arg == "-p":
+            outputs.append(next(arg))
+        if arg == "--setup":
+            install_me()
+            sys.exit()
+        elif arg in ["--help", "-h"]:
+            print(HELP)
+            sys.exit()
+        else:
+            config["method"] = arg
+            return parsers[arg](argi, config), outputs
+
+#
+# SRIM
+#
+def _blk_3(i, CA, U):
+    return i, np.einsum('kil,klj->ij', CA[:i,:,:], U[-i:,:,:])
+
+
+def parse_srim(argi, config):
+    help="""
+    SRIM -- System Identification with Information Matrix
+
+    Parameters
+    p           order of the observer Kalman ARX filter.
+    n           size of the state-space model used for 
+                representing the system.
     """
+    config.update({"p"  :  5, "orm":  4})
+    #argi = iter(args)
+    channels = [[17, 3, 20], [9, 7, 4]]
+    for arg in argi:
+        if arg == "-p":
+            config["p"] = int(next(argi))
+        elif arg == "--dt":
+            config["dt"] = float(next(argi))
+        elif arg == "-n":
+            config["orm"] = int(next(argi))
+        elif arg in ["--help", "-h"]:
+            print(help)
+            sys.exit()
+        elif arg == "--inputs":
+            inputs = next(argi)[1:-1].split(",")
+            if isinstance(inputs, str):
+                channels[0] = [int(inputs)]
+            else:
+                channels[0] = list(map(int, inputs))
+        elif arg == "--outputs":
+            outputs = next(argi)[1:-1].split(",")
+            if isinstance(outputs, str):
+                channels[1] = [int(outputs)]
+            else:
+                channels[1] = list(map(int, outputs))
+        elif arg == "--":
+            continue
+
+        else:
+            config["event_file"] = arg
+
+
+    event = quakeio.read(config["event_file"])
+    inputs = np.array([
+        event.match("l", station_channel=f"{i}").accel.data for i in channels[0]
+    ]).T
+    outputs = np.array([
+        event.match("l", station_channel=f"{i}").accel.data for i in channels[1]
+        #event.at(file_name=f"CHAN{i:03d}.V2").accel.data for i in channels[1]
+    ]).T
+    npoints = len(inputs[:,0])
+    dt = event.at(station_channel=f"{channels[0][0]}").accel["time_step"]
+    config["dt"] = dt
+
+    A,B,C,D = srim(inputs, outputs, **config)
+    freqdmpSRIM, modeshapeSRIM, *_ = ComposeModes(dt, A, B, C, D)
+    output = [
+            {"frequency": np.real(x[0]), "damping": np.real(x[1])} 
+            for x in freqdmpSRIM if all(x > 0.0)
+    ]
+    import json
+    print(json.dumps(output, cls=JSON_Encoder, indent=4))
     return config
 
-def okid(dati, dato, svd="gesvd", **config):
+def srim(
+    dati,
+    dato,
+    debug = False,
+    full     : bool = True,
+    verbose  : bool = False,
+    pool_size: int  = 6,
+    **config
+):
     """
-    PART 2: OKID-ERA-DC (Observer Kalman filter Identification -
-            Eigen Realization with Direct Correlations)
-    -----------------------------------------------------------------
-
-    # Inputs
-    Modelparameters
-        div = 1;     # A parameter used for decimating data. 1 uses entire data without downsampling.
-        mro = 10;    # Model reduction order
-        orm = 4;     # Order of the model. # of computed and plotted modes dep on orm.
-                     # For orm = 2, one mode is found, for orm = 4, two modes are found.
-    svd:
-        GESDD: a two-stage algorithm. It first reduces the input matrix to bidiagonal form via 
-        Householder reflection, then divides the bidiagonal matrix into smaller matrices to calculate 
-        singular values and the unitary matrices U and V. Finally, the singular values of the entire 
-        input matrix is simply the those of the smaller sub-matrices.
-        
-        GESVD: also a two-stage algorithm where the first step is identical to GESDD. The second step 
-        can be done using iterative QR decomposition to derive singular values. More mathematical details are available here.
+    mro $(p)$ determines order of the observer Kalman ARX filter used in OKID-ERA-DC.
+    orm $(n)$ determines size of the state-space model used for representing the system.
+
+    Returns
+    =======
+     freqdampSRIM:
+        variable is a matrix that includes the information of identified
+        frequencies, damping ratios & validation of the modes with MPC & EMAC criteria.
+        Each row of freqdamp corresponds to a mode. Columns are as follows:
+        1) frequency, 2) damping ratio, 3) order index, 4) condition number, 5) MPC.
+        If values in columns 5 is > 0.5, identified mode is valid.
+     modeshapeSRIM:
+         stores the mode shape information for identified modes.
+     RMSEpredSRIM:
+         root mean square error of the predicted output from
+         identified parameters with respect to the actual output
+
+    ## SRIM Methodology
+
+    More information on SRIM algorithm can be found in Sections 3.4.4 & 3.4.5 of
+    (Arici & Mosalam, 2006). Equations below refer to this report. SRIM is a MIMO
+    SI method that is based on state space identification using least squares and
+    consists of the following steps:
+
+
+    2a. Determine output (y) & input (u) vectors [Eqs. 3.58 & 3.60].
+    2b. Compute the correlation terms & the coefficient matrix (Eqs. 3.68 & 3.69).
+    2c. Obtain observability matrix using full or partial decomposition (Eqs. 3.72 & 3.74).
+    2d. Use the observability matrix to compute system matrices A, B & C, in which modal 
+        information is embedded.
+    2e. Obtain the modal information from matrices A, B & C.
+    2f. Spatial & temporal validation of the identified modes.
+    2g. Back calculate (estimate) the output accelerations with the state-space system &
+        check against the actual output accelerations.
 
+    For orm = 2, one mode is found, for orm = 4, two modes are found.
+    For case 1, one mode is transverse & the other is torsion.
+    For all other cases, the second mode is a higher mode.
     Sometimes higher orm still gives fewer modes, e.g. orm = 8 for case 1 gives
     three modes, but one of them is invalid according to the EMAC & MPC criteria.
-    kmax = 100;  #Number of computed Markov parameters, indicated as 1000 on page 43 of
-    (Arici & Mosalam, 2006). However, it was input as 100 in the code.
-    kmax = 100 runs much faster & both kmax = 100 & 1000 give the same results.
-
-    # Outputs
-    1. freqdamp variable is a matrix that includes the information of identified
-       frequencies, damping ratios & validation of the modes with MPC & EMAC criteria
-       Each row of freqdamp corresponds to a mode. Columns are as follows:
-       1) frequency, 2) damping ratio, 3) order index, 4) condition number, 5) input EMAC,
-       6) output EMAC, 7) MPC. If values in columns 5-7 are > 0.5, identified mode is valid.
-    2. modeshape stores the mode shape information for identified modes.
-    3. RMSEpred: root mean square error of the predicted output from
-       identified parameters with respect to the actual output.
-    4. Markovparamerror: root mean square error used to validate accurate
-       computation of Markov parameters
-
-    # Description of the Methodology
-    More information on OKID-ERA-DC method can be found in
-    Section 3.4.6 of (Arici & Mosalam, 2006). Equations below refer to this report.
-    OKID-ERA-DC is a Multiple Input - Multiple Output (MIMO) System Identification (SI) method
-    that consists of the following steps:
-    1. Data pre-processing (baseline correction, filtering & decimation)
-    2. Identify observer Kalman filters using Observer Kalman filter Identification (OKID)
-       methodology. This step basically consists of developing a simple observer model of
-       a system from a MIMO ARX structure, Eq. (3.76), which is broken into these 6 steps:
-   
-    3a. Determine Markov parameters (M) in a least squares sense, Eq. (3.76).
-
-    3b. Establish the Hankel matrix (H) from the Markov parameters, (Eq. 3.80).
-    3c. Use H to compute system matrices A, B & C, in which modal information is embedded.
-    // 3d. Obtain the modal information from matrices A, B & C.
-    3e. Spatial & temporal validation of the identified modes.
-    3f. Back calculate (estimate) the output accelerations with the state-space system &
-        check against the actual output accelerations.
-    """ 
+    same orm in OKID-ERA-DC is used. It can be changed if needed.
+
+    """
+    #
+    # Convenience argument handling
+    #
     dt = to = config.get("dt", None) or dati["time_step"]
-    p = config.get("p", config.get("mro")) # # steps used for the identification (ie, prediction horizon)
+    p = config.get("p", config.get("mro"))         # # steps used for the identification (ie, prediction horizon)
     n = n1 = config.get("n", config.get("orm", 4))  # Order of the model.
-    
-    if svd in ["gesvd", "gesdd"]:
-        import scipy.linalg
-        def _svd(*args):
-            U,S,V = scipy.linalg.svd(*args, lapack_driver=svd)
-            return U,S,V.T.conj()
-
-    elif svd in ["xla", "jax"]:
-        from jax.scipy.linalg import svd as _svd
 
     if isinstance(dati, list):
         dati = np.array([i.data for i in dati]).T
     elif issubclass(dati.__class__, dict):
         dati = dati.data
 
     if isinstance(dato, list):
@@ -94,285 +226,295 @@
     elif issubclass(dato.__class__, dict):
         dato = dato.data
 
     if len(dati.shape) < 2:
         dati = np.atleast_2d(dati).T
     if len(dato.shape) < 2:
         dato = np.atleast_2d(dato).T
-        
-    dati = dati[:-1,:]
-    dato = dato[:-1,:]
-
-    #verbose = True
-    #dn = config.get("dn", None) or dati.shape[0]
-    kmax    = config["kmax"]
-    n = config["orm"]   # assign order of model input to variable n, consistent with Eqs. 3.81-3.84
-    p = config["mro"]   # assign input model reduction order to variable p, consistent with Eq. 3.76
 
+    if verbose:
+        progress_bar = tqdm
+    else:
+        progress_bar = lambda arg, **kwds: (i for i in arg)
+
+    dn = config.get("dn", None) or dati.shape[0]
+
+    # 2a. Compute y (output) and u (input) vectors (Eqs. 3.58 & 3.60)
+
+    # Note that main Step 2 develops Eq. 3.57.
+    # Therefore, it is not part of the code.
+    # Accordingly, the code continues with Step 2a to compute the output & input vectors.
+
+    # Calculate the usable size of the data matrix
+    # dn = size(dat,1)/div;       # total # time steps after decimating
+    nsizS = dn-1-p+2
 
     l,m = dato.shape # m is the number of output channels
     _,r = dati.shape # r is the number of input channels
 
-    # ASSERT SIZE(DATO,1) == SIZE(DATI,1)
-
-    ## 2a. Obtain Observer Markov Parameters
-    # The Markov parameters are computed in two steps:
-    # i)  The Observer Markov matrices are computed from Eq. 3.76 using a linear regression approach
-    # ii) Compute the system Markov parameters from the Markov matrices using recursive relations
-
-    # Compute matrix U that represents ARX equation of current output on p time steps of past output
-    # & input values (Eq. 3.76)
-    U = np.zeros(((m+r)*p+r, l))
-    U[:r,:] = dati.T
-    for b in range(1,p+1):
-        U[(b-1)*(r+m)+r:(b-1)*(r+m)+r+r+m, b:] = [*dati[:-b,:r].T, *dato[:-b, :m].T]
-
-
-    # i) Compute the matrix of Observer Markov Parameter Matrix (M)
-    #    in Eq 3.76 using Linear Regression
-    uu,wr,v = _svd(U,0)
-    pg = (r+m)*p+r
-    for i in range((r+m)*p+r):
-        if wr[i] <= 0.001:
-            pg = i
-            break
-
-    s = np.diag(wr)
-
-    pss = v[:,:pg]@linsolve(s[:pg,:pg], uu[:,:pg].T)
-    M = dato.T@pss           # M: Observer Markov Parameter Matrix
-
-    # Fit for multiple regression
-    # RMSE between actual output & y on left hand side in Eq. 3.76. It should be 
-    # quite small (e.g., 10^-3) for accurately computed Markow parameters.
-    ypreo = M@U
-    markovParamError = 1/m*sum((
-        sum((dato[:,i] - ypreo[i,:].T)**2)/sum(dato[:,i]**2)
-        for i in range(m)
-    ))  
-
-
-    ## ii) Compute Markov parameters (Y) using recursive relations in Eqs. 3.78 & 3.79
-    #      (Equation 6.21 in Juang 1994)
-
-    # Matrix D is directly equal to the Observer Markov parameter matrix (Eq. 3.77)
-    M1 = D = M[:, :r]  # D: Direct Transmission term
-
-    Y = [D]
-    # First p steps (Eq. 3.78)
-    for i in range(p):
-        Y.append(
-            M[:, r+i*(r+m):r+i*(r+m)+r] + sum(
-                M[:, r+j*(r+m)+r:r+j*(r+m)+r+m]@Y[i-j]
-                for j in range(i+1)
-            )
-        )
-    # Remainder (Eq. 3.79)
-    for i in range(p, l+kmax):
-        sumt = zeros((m,r))
-        for j in range(p):
-            sumt += M[:,r+j*(r+m)+r:r+j*(r+m)+r+m]@Y[i-j]
 
-        Y.append(sumt)
+    assert p >= n/m + 1
 
-    # The Markow parameters Y have been computed.
+    ypS = np.zeros((m*p,nsizS))
+    upS = np.zeros((r*p,nsizS))
 
-
-    #
-    # ERA/DC
-    #
-    # Form Hankel matrix (H) from the Markov parameters (Y) (Eq. 3.80)
-
-    # Obtain Hankel Matrix of Zeroth Order & First Order
-    H0,H1 = np.zeros((2, kmax*m, l*r))
-    #H0 = hankel(Y,0)
-    for hj in range(kmax):
-        for jh in range(l):
-            H0[hj*m:hj*m+m, jh*r:jh*r+r] = Y[jh+hj+1]
-            H1[hj*m:hj*m+m, jh*r:jh*r+r] = Y[jh+hj+2]
-    
-    ## 2c. Use H matrix to compute system matrices A, B & C
-    R1,sis,S1 = _svd(H0) # singular value decomposition
-    Sis = np.diag(sis[:n])
-
-    Siv = np.diag(1/np.sqrt(sis[:n]))
-    # A: state transition matrix (Eqs. 3.32 & 3.82)
-    A  = Siv@R1[:,:n].T@H1@S1[:,:n]@Siv
-    # B: input influence matrix (Eqs. 3.32 & 3.83)
-    B = (np.sqrt(Sis)@S1[:,:n].T)[:,:r]
-    Pb = R1[:,:n]@np.sqrt(Sis)
-    # C: output influence matrix (Eqs. 3.34 & 3.84)
-    C  = Pb[:m,:]
-    return locals()
+    # Compute Y (output) & U (input) vectors (Eqs. 3.58 & 3.60 Arici 2006)
+    for b in range(p):
+        ypS[b*m:(b+1)*m,:nsizS+1] = dato[b:nsizS+b, :].T
+        upS[b*r:(b+1)*r,:nsizS+1] = dati[b:nsizS+b, :].T
+
+
+    # 2b. Compute the correlation terms and the coefficient matrix 
+    #     (Eqs. 3.68 & 3.69).
+
+    # Compute the correlation terms (Eq. 3.68)
+    Ryy = ypS@ypS.T/nsizS
+    Ruu = upS@upS.T/nsizS
+    Ruy = upS@ypS.T/nsizS
+
+    assert Ryy.shape[0] == Ryy.shape[1] == p*m
+    assert Ruy.shape[0] == p*r
+    assert Ruy.shape[1] == p*m
+
+    # Compute the correlation matrix (Eq. 3.69)
+    Rhh = Ryy - Ruy.T@linsolve(Ruu,Ruy)
+
+    # 2c. Obtain observability matrix using full or partial decomposition 
+    #     (Eqs. 3.72 & 3.74).
+    if full:
+        # Full Decomposition Method
+        un,*_ = np.linalg.svd(Rhh,0)           # Eq. 3.74
+        Observability = un[:,:n]                          # Eq. 3.72
+        A = lsqminnorm(Observability[:(p-1)*m,:], Observability[m:p*m,:])
+        C = Observability[:m,:]
+    else:
+        # Partial Decomposition Method
+        un,*_ = np.linalg.svd(Rhh[:,:(p-1)*m+1],0)
+        Observability = un[:,:n]
+        A = lsqminnorm(Observability[:(p-1)*m,:], Observability[m:p*m,:])
+        C = un[:m,:]
+
+    # Computation of system matrices B & D
+    # Output Error Minimization
+
+    # Setting up the Phi matrix
+    Phi  = np.zeros((m*nsizS, n+m*r+n*r))
+    CA_powers = np.zeros((nsizS, m, A.shape[1]))
+    CA_powers[0, :, :] = C
+    A_p = A
+    for pwr in range(1,nsizS):
+        CA_powers[pwr,:,:] =  C@A_p
+        A_p = A@A_p
+
+    # First block column of Phi
+    for df in range(nsizS):
+        Phi[df*m:(df+1)*m,:n] = CA_powers[df,:,:]
+
+    # Second block column of Phi
+    Imm = np.eye(m)
+    for i in range(nsizS):
+        Phi[i*m:(i+1)*m, n:n+m*r] = np.kron(dati[i,:],Imm)
+
+    # Third block column of Phi
+    In1n1 = np.eye(n)
+    cc = n + m*r + 1
+    dd = n + m*r + n*r
+
+    krn = np.array([np.kron(dati[i,:],In1n1) for i in range(nsizS)])
+
+    with multiprocessing.Pool(pool_size) as pool:
+        for i,res in progress_bar(
+                pool.imap_unordered(
+                    partial(_blk_3,CA=CA_powers,U=np.flip(krn,0)),
+                    range(1,nsizS),
+                    200
+                ),
+                total = nsizS
+            ):
+            Phi[i*m:(i+1)*m,cc-1:dd] = res
+
+    y = dato[:nsizS,:].flatten()
+
+    teta = lsqminnorm(Phi,y)
+
+    x0 = teta[:n1]
+    dcol = teta[n1:n1+m*r]
+    bcol = teta[n1+m*r:n1+m*r+n1*r]
+
+    D = np.zeros((m,r))
+    B = np.zeros((n,r))
+    for wq in range(r):
+        D[:,wq] = dcol[wq*m:(wq+1)*m]
+
+    for ww in range(r):
+        B[:,ww] = bcol[ww*n:(ww+1)*n]
+
+    assert A.shape[0] == A.shape[1] == n
+    if debug:
+        return locals()
     return A,B,C,D
 
+#PY
+# #% 2e. Obtain the modal information from the system matrices A & C
+# # This includes determination of: a) modal frequencies, b) damping ratios & c) mode shapes
+# # c) Determination of mode shapes
+#     mod = C1@vS                 # mode shapes (Eq. 3.40), v is the eigenvectors of matrix A
+# 
+
+#% 2f. Validation Analysis
+
+# Two criteria are used for selection of identified genuine modes, in terms of spatial & temporal consistency.
+# a) Modal Phase Collinearity (MPC) testing spatial consistency of identification results.
+#    Modes having MPC value above 0.5 (mpc parameter below) are considered as genuine modal quantities.
+# b) Extended Modal Amplitude Coherence (EMAC), evaluates temporal consistency of the identification results.
+#    Both output EMAC & input EMAC can be computed. Input EMAC requires the controllability matrix.
+#    Because the controllability matrix is not estimated by all considered SI methods,
+#    this criterion is computed, but not used.
+#    Modes with output EMAC values < 0.5 are considered spurious & therefore not reported.
+
+# a) Modal Phase Collinearity (MPC) [Eqs. 3.85-3.87]
+#Py
+##    for q in range(n):
+##        a = real(mod[:,q])
+##        b = imag(mod[:,q])
+##        sxx[:,q] = a.T*a
+##        syy[:,q] = b.T*b
+##        sxy[:,q] = a.T*b
+##        nu[q] = (syy[:,q]-sxx[:,q])/(2*sxy[:,q])
+##        lam[1,q] = (sxx[:,q]+syy[:,q])/2+sxy[:,q]*(nu(q)**2+1)**0.5
+##        lam[2,q] = (sxx[:,q]+syy[:,q])/2-sxy[:,q]*(nu(q)**2+1)**0.5
+##        mpc[q] = ((lam[0,q]-lam[1,q])/(lam[0,q]+lam[1,q]))**2
+
+
+# b) Extended Modal Amplitude Coherence (EMAC)
+
+# Only EMAC Output is computed as there is no Controllability Matrix
+
+# Note that the computations are commented out as the matrix B is needed
+
+#%KKKKK
+##PY
+##    plin = Op1@vS                # Observability Matrix used for the output-EMAC
+##    lamb = linsolve(vS,A1)*vS
+##    bkh = linsolve(vS,B)
+### Pick the last block row
+##    pto = plin((p-1)*m+1:m*p,:)  # the identified value at T0
+##    for ds in range(n):
+##        ptop[:,ds] = mod[:,ds]*exp(sj1S(ds)*to*(p-1))
+##
+### Computation of rij
+##    for qa in range(n):
+##        for qz in range(m):
+##            Rij(qa,qz) = min((abs(pto(qz,qa))/abs(ptop(qz,qa))),(abs(ptop(qz,qa))/abs(pto(qz,qa))))
+##            Pij = angle(pto(qz,qa)/ptop(qz,qa))
+##            Pijn(qa,qz) = Pij
+##            if abs(Pij) <= pi/4:
+##                Wij[qa,qz] = 1-abs(Pij)/(pi/4)
+##            else:
+##                Wij[qa,qz] = 0
+##
+##            emaco[qa,qz] = Rij[qa,qz]*Wij[qa,qz]
+##
+##
+### Computation of final emac
+##    for xc in range(n):
+##        # Weight for emaco
+##        sumo = 0.0
+##        for la in range(m):
+##            sumo = emaco(xc,la)*abs(mod(la,xc))**2+sumo
+##        emacof[xc] = sumo/((mod[:,xc].T*mod[:,xc]))
+##        emac[xc] = emaco[xc]
+#%KKKKK
+
+# Add the MPC to the matrix freqdampSRIM
+#    for lih = 1:size(freqdmpSRIM,1)
+#        freqdmpSRIM[lih,5] = emacof(freqdmpSRIM(lih,3))
+#        freqdmpSRIM[lih,6] = mpc(freqdmpSRIM(lih,3))
+#        if freqdmpSRIM[lih,5]>0.5 and freqdmpSRIM[lih,6]>0.5:
+#            validationm = ' valid'
+#        else:
+#            validationm = ' not valid'
+#
+#        scroutput = strcat('Mode',num2str(lih), ...
+#            ': Output EMAC =  ',num2str(freqdmpSRIM(lih,5)),...
+#            ', MPC =  ',num2str(freqdmpSRIM(lih,6)),...
+#            ' -->',' SRIM Identified Mode ',...
+#            num2str(lih), ' is',validationm)
+#        sprintf(scroutput)
+
+
+#% 2g. Back calculate (estimate) output accelerations with state-space system &
+#%     check against actual output accelerations
+
+# Note that the computations are commented out as the matrix B is needed
+
+# Prediction using state space model
+#%KKKKK
+##PY
+##    ms1 = modstruc(A1,B,C1,D,zeros(n,m),x0)
+##    th1 = ms2th(ms1,'d')
+##    e,r = resid([dato dati],th1)
+##    simy = idsim([dati],th1);                # simy represents the estimated accelerations
+##
+##    for i in range(m):
+##        temsum = sum((dato[:,i]-simy[:,i]).**2)
+##        Jm[i] = temsum/(sum(dato[:,i].**2));     # Root mean square error of estimated accelerations
+##
+##    RMSEpredSRIM = sum(Jm)/m
+###%KKKKK
+##    return freqdmpSRIM,modeshapeSRIM,RMSEpredSRIM
 
-def validate(freqdmp, v, system, **config):
-    """2e. Validation Analysis
-
-    Two criteria are used for selection of identified genuine modes
-    (in the sense of spatial & temporal consistency).
-
-    a) Modal Phase Collinearity (MPC) testing spatial consistency of identification results.
-       Modes having MPC value above 0.5 (mpc parameter below) are considered as genuine modal quantities.
-
-    b) Exted Modal Amplitude Coherence (EMAC), evaluates temporal consistency of the identification results.
-       Both output EMAC & input EMAC can be computed. Input EMAC requires the controllability matrix.
-       Because the controllability matrix is not estimated by all considered SI methods,
-       this criterion is computed, but not used.
-       Modes with output EMAC values < 0.5 are considered spurious & therefore not reported.
-
-    """
-    mpc = MPC(n, v, system)
-
-    # Add the input EMAC, output EMAC, and MPC to the matrix freqdamp
-    for lih in range(size(freqdmp)[0]):
-        freqdmp[lih,4] = emacif(freqdmp[lih,2])
-        freqdmp[lih,5] = emacof(freqdmp[lih,2])
-        freqdmp[lih,6] = mpc[freqdmp(lih,3)]
-        if freqdmp[lih,5]>0.5 and freqdmp[lih,7]>0.5:
-            validationm=' valid'
-        else:
-            validationm=' not valid'
-
-def MPC(n, v, system):
-    """a) Modal Phase Collinearity (MPC) [Eqs. 3.85-3.87]"""
-    _,__,C,___ = system
-    modes_raw = C@v
-    _, n = modes_raw.shape
-    sxx, syy, sxy = np.zeros((3, *modes_raw.shape))
-    nu, mpc = np.zeros((2, n))
-    lam = np.zeros((2, n))
-    for i in range(n):
-        sxx[:,i] = np.real(modes_raw[:,i]).T@np.real(modes_raw[:,i])
-        syy[:,i] = np.imag(modes_raw[:,i]).T@np.imag(modes_raw[:,i])
-        sxy[:,i] = np.real(modes_raw[:,i]).T@np.imag(modes_raw[:,i])
-        nu[i]    = (syy[:,i]-sxx[:,i])/(2*sxy[:,i])
-        lam[1,i] = (sxx[:,i]+syy[:,i])/2 + sxy[:,i]*np.sqrt(nu[i]**2+1);
-        lam[2,i] = (sxx[:,i]+syy[:,i])/2 - sxy[:,i]*np.sqrt(nu[i]**2+1);
-        mpc[i]   = ((lam[0,i]-lam[1,i])/(lam[0,i]+lam[1,i]))**2;
-    return mpc
-
-def EMAC_Matrix(n, m, pto, ptop):
-    emac = np.zeros((n, m))
-    for i in range(n):
-        for j in range(m):
-            Rij = min(
-                (abs(pto[j,i])/abs(ptop[j,i])),
-                (abs(ptop[j,i])/abs(pto[j,i]))
-            )
-            Pij = np.angle(pto[j,i]/ptop[j,i])
-            if abs(Pij) <= pi/4:
-                Wij = 1 - abs(Pij)/(pi/4)
-            else:
-                Wij = 0
-            emac[i,j] = Rij*Wij
-
-def EMAC_Variation(n,m,pto,ptop):
-    pass
-
-
-def EnergyCondensedEMAC(n,m,emac,phi):
-    "Equation 3.93"
-    return np.array([
-        sum(emac[i,j]*abs(phi[i,j])**2 
-            for j in range(m)
-        )/(phi[i,:].T@phi[i,:])
-        for i in range(n) 
-    ])
-
-def MAC(shape,v, v_inv, A, B):
-    n,m,r,l = shape
-    lamb = v_inv@A@v
-    bkh = v_inv@B
-    for i in range(n):
-        for j in range(l):
-            qhat[i,j*r+1:j*r+r] = bkh[i,:]*(lamb[i,i])**j
-
-    selsiz = min(size(qlin),size(qhat))
-
-    for hnd in range(n):
-        ql = qlin[hnd,:selsiz(2)]
-        qh = qhat[hnd,:selsiz(2)]
-        mac[hnd] = abs(ql*qh.T)/(abs(ql*ql.T)*abs(qh*qh.T))**0.5
-
-
-def EMAC_Validate(shape, kmax, v, d, dt, system):
-    "b) Exted Modal Amplitude Coherence (EMAC)"
-    A,B,C,D = system
-    n,m,r,l = shape
 
-def OutputEMAC(n,m,p,Obsv,A,C):
-    #
-    # Output EMAC (Eqs. 3.88-3.89)
-    # p (kmax)
+if __name__ == "__main__":
+    import sys
+    import quakeio
+    from pathlib import Path
+    method = None
 
-    v, d = A.eigen()
-    plin = Obsv@v;         # Modal observability Matrix used for the output-EMAC
-    modes_raw = C@v
-    sj1 = np.log(d)/dt
-    pto = plin[(p-1)*m+1:m*p,:]  # the identified value at T0 ( last block row)
-    ptop = np.array([
-            modes_raw[:,i]*np.exp(sj1[i]*dt*(p-1))
-        for i in range(n)
-    ]).T
-    emaco  = EMAC_Matrix(n,m,pto,ptop)
-    return EnergyCondensedEMAC(n, m, emaco, modes_raw.T)
+    config, out_ops = parse_args(sys.argv)
 
+    if config["method"] == "test":
+        data_dir = Path("RioDell_Petrolia_Processed_Data")
 
-def InputEMAC(Ctrl,A,B):
-    #
-    # Input EMAC
-    #
-    # # EMAC Input Variation
-    # for i in range(l):
-    #     qtovar = qlin[:,i*r:(i+1)*r]
-    #     qtopvar = (np.diag(d)**i)*inm
-    #     emaci = EMAC_Matrix(n,m,qtovar,qtopvar)
-    #     emacivar[:,i] = EnergyCondensedEMAC(n,m,emaci,inm);
-
-    # Pick the last block column
-    v, d  = A.eigen()
-    v_inv = np.linalg.inv(v)
-    inm   = linsolve(v,B)   # Initial mode contribution
-    qlin  = v_inv@Ctrl;     # Modal controllability Matrix (F' in Pappa 1993)
-    qto   = qlin[:, (l-1)*r+1:l*r]
-    qtop  = d**(l-1)@inm
-    emaci = EMAC_Matrix(n, m, qto, qtop)
-    return EnergyCondensedEMAC(n, m, emaci, inm)
-    
+        first_input = quakeio.read(data_dir/f"CHAN{channels[0][0]:03d}.V2")
+        npoints = len(first_input.accel.data)
+        inputs, outputs = np.zeros((2,npoints,len(channels[0])))
+
+        # Inputs
+        inputs[:,0] = first_input.accel.data
+        for i,inp in enumerate(channels[0][1:]):
+            inputs[:,i+1] = quakeio.read(data_dir/f"CHAN{inp:03d}.V2").accel.data
+
+        # Outputs
+        for i,inp in enumerate(channels[1]):
+            outputs[:,i] = quakeio.read(data_dir/f"CHAN{inp:03d}.V2").accel.data
+
+        dt = first_input.accel["time_step"]
+        config["dt"] = dt
+
+    elif "event_file" in config:
+        event = quakeio.read(config["event_file"])
+        inputs = np.array([
+            event.match("l", station_channel=f"{i}").accel.data for i in channels[0]
+        ]).T
+        outputs = np.array([
+            event.match("l", station_channel=f"{i}").accel.data for i in channels[1]
+        ]).T
+        npoints = len(inputs[:,0])
+        dt = event.match("l", station_channel=f"{channels[0][0]}").accel["time_step"]
+        config["dt"] = dt
+
+    # print(config)
+    # sys.exit()
+
+    A,B,C,D = srim(inputs, outputs, **config)
+
+    freqdmpSRIM, modeshapeSRIM, *_ = ExtractModes.ComposeModes(dt, A, B, C, D)
+
+    if not out_ops:
+        print(f"period: {np.real(1/freqdmpSRIM[:,0])}")
+    elif "freq" in out_ops:
+        print(f"frequency: {freqdmpSRIM[:,0]}")
+    elif "cycl" in out_ops:
+        print(f"cyclic_frequency: {2*np.pi*freqdmpSRIM[:,0]}")
 
 
-if __name__ == "__main__":
-    from pathlib import Path
-    import quakeio
-    # import ssid as si
-    import okid
-    import numpy as np
-    channels = dict( # PAINTER RIO DELL
-        inputs  = [17, 3, 20],
-        outputs = [ 9, 7 , 4]
-    )
-    for file in Path("painter").glob("RioDell_P*.zip"):
-        event = quakeio.read(file)
-        try:
-            inputs = [
-                event.match("r", file_name=f".*{chan}.*").accel
-                for chan in channels["inputs"]
-            ]
-            outpts = [
-                event.match("r", file_name=f".*{chan}.*").accel
-                for chan in channels["outputs"]
-            ]
-        except:
-            print(f"failed {file.name}")
-
-        else:
-            dt = inputs[0]["time_step"]
-            V = OKID.okid(inputs, outpts, dt=dt, kmax=500, mro=10, orm=4, verbose=True)
-            break
-
-            A,B,C,D = OKID.okid(inputs, outpts, dt=dt, kmax=500, mro=10, orm=4, verbose=True)
-            freqdmpSRIM, modeshapeSRIM, *_ = si.ComposeModes(dt, A, B, C, D)
-            # Add validation
-            print(si.IdentifiedSystem(dt, A, B, C, D))
-            # print(file, np.real(1/freqdmpSRIM[:,0]))
```

### Comparing `ssid-0.0.2/src/ssid/srim.py` & `ssid-0.0.3/src/ssid/okid.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,349 +1,300 @@
-__doc__="""
-# ssid : Structural System Identification
-"""
-# Standard library
-import sys
-import json
-import multiprocessing
-from functools import partial
-# Dependencies
-try:
-    from tqdm import tqdm
-except:
-    tqdm = lambda x,*args,**kwds: x
-
-import quakeio
 import numpy as np
-from numpy import pi, log, sign
-from numpy.linalg import eig
-import scipy.linalg as sl
-
-linsolve = np.linalg.solve
-lsqminnorm = lambda *args: np.linalg.lstsq(*args, rcond=None)[0]
+from numpy import zeros, pi, size
+import scipy.linalg
+from scipy.linalg import fractional_matrix_power as matpow
 
-class JSON_Encoder(json.JSONEncoder):
-    def default(self, obj):
-        if isinstance(obj, np.ndarray):
-            return obj.tolist()
-        elif isinstance(obj, np.integer):
-            return int(obj)
-        elif isinstance(obj, np.floating):
-            return float(obj)
-        return json.JSONEncoder.default(self, obj)
-
-REQUIREMENTS = """
-numpy
-scipy
-tqdm
-quakeio
-"""
-
-EXAMPLES="""
-    ssid srim -wABCD event.zip 2,3 4,5
-    ssid okid -pm -i ch02.v2 ch03.v2 -o ch04.v2 ch05.v2
-    ssid okid -wm -i ch02.v2 ch03.v2 -o ch04.v2 ch05.v2
-"""
-
-class IdentifiedSystem:
-    def __init__(self, time_step, A, B, C, D, **kwds):
-        self.system = A, B, C, D
-        self.freqdmp, modeshapeSRIM, *_ = ComposeModes(time_step, A, B, C, D)
+linsolve = scipy.linalg.solve
 
-    def __repr__(self):
-        import textwrap
-        try:
-            nln = "\n                "
-            return textwrap.dedent(f"""
-            Spectral quantities:
-                   T      \N{Mathematical Italic Small F}       \N{Greek Small Letter Zeta}
-                {nln.join(f"{1/i: <6.4}  {i: <6.4}  {j: <6.4}" for i,j in np.real(self.freqdmp[:,:2]))}
-            """)
-        except Exception as e:
-            return f"Error extracting modes: {e}"
-
-def parse_args(args):
-    outputs = []
-    parsers = {
-        "srim": parse_srim,
-        "test": parse_srim,
-        "okid": parse_okid
-    }
-    config = {}
-    argi = iter(args[1:])
-    for arg in argi:
-        if arg == "-p":
-            outputs.append(next(arg))
-        if arg == "--setup":
-            install_me()
-            sys.exit()
-        elif arg in ["--help", "-h"]:
-            print(HELP)
-            sys.exit()
-        else:
-            config["method"] = arg
-            return parsers[arg](argi, config), outputs
-
-#
-# Distribution Utilities
-#
-def install_me(install_opt=None):
-    import os
-    import subprocess
-    if install_opt == "dependencies":
-        subprocess.check_call([
-            sys.executable, "-m", "pip", "install", *REQUIREMENTS.strip().split("\n")
-        ])
-        sys.exit()
-    try:
-        from setuptools import setup
-    except ImportError:
-        from distutils.core import setup
-
-    sys.argv = sys.argv[:1] + sys.argv[2:]
-
-    setup(name = "ssid",
-          version = "0.0.1",
-          description = "Structural system identification",
-          long_description = HELP,
-          author = "",
-          author_email = "",
-          url = "",
-          py_modules = ["ssid"],
-          scripts = ["ssid.py"],
-          license = "",
-          install_requires = [] #*REQUIREMENTS.strip().split("\n")],
-    )
-
-#
-# Computation Utilities
-#
-def condeig(a):
-    """
-    vals, vecs, conds = condeig(A) Computes condition numbers for the
-    eigenvalues of a matrix. The condition numbers are the reciprocals
-    of the cosines of the angles between the left and right eigenvectors.
-    Inspired by Arno Onken's Octave code for condeig.
-
-    https://github.com/macd/rogues/blob/master/rogues/utils/condeig.py
-    """
-    m, n = a.shape
-    # eigenvalues, left and right eigenvectors
-    lamr, vl, vr = sl.eig(a, left=True, right=True)
-    vl = vl.T
-    # Normalize vectors
-    for i in range(n):
-        vl[i, :] = vl[i, :] / np.sqrt(abs(vl[i, :]**2).sum())
-    # Condition numbers are reciprocal of the cosines (dot products) of the
-    # left eignevectors with the right eigenvectors.
-    c = abs(1 / np.diag(np.dot(vl, vr)))
-    return vr, lamr, c
-
-def ComposeModes(dt, A, B, C, D):
-    n = A.shape[0]
-    m = C.shape[0]
-
-    v, d, cnd = condeig(A)  # eigenvectors (d) & eiegenvalues (v) of the matrix A
-    kit = np.log(d)         # logarithm of the eigenvalues
-
-    # a) Determination of modal frequencies (Eqs. 3.46 & 3.39)
-    sj1 = kit/dt            # dt is the time step
-    freq1 = ((sj1*np.conj(sj1))**0.5)/(2*pi)
-
-    roots = []
-
-    # selection of proper roots
-    if freq1[0] == freq1[1]:
-        roots.append(0)
-
-    if freq1[n-1] == freq1[n-2]:
-        roots.append(n-1)
-
-    for i in range(2, n-2):
-        if (freq1[i] == freq1[i+1]) or (freq1[i] == freq1[i-1]):
-            roots.append(i)
-
-    # b) Determination of damping ratios (Eqs. 3.46 & 3.39)
-    damp1 = -np.real(sj1)/(2*pi*freq1)
-    # Represent the identified frequency & damping information
-    # of the proper roots in a matrix
-    freqdmp = np.array([
-            [
-                freq1[lk],   # first column: identified frequency
-                damp1[lk],   # second column: identified damping ratio
-                cnd[lk]      # condition number of the eigenvalue
-            ] for lk in roots
-    ])
-
-    # c) Determination of mode shapes
-    modes_raw = C@v   # mode shapes (Eq. 3.40)
-
-    modeshape = np.zeros((m,len(roots)), dtype=complex)
+lsqminnorm = lambda *args: np.linalg.lstsq(*args, rcond=None)[0]
 
-    # extract mode shapes from mod corresponding to a frequency
-    for q,root in enumerate(roots):
-        modeshape[:m,q] = modes_raw[:m, root]
-
-    for q,root in enumerate(roots):
-        om  = np.argmax(abs(np.real(modeshape[:,q])))
-        mx  = abs(np.real(modeshape[om,q]))
-        modeshape[:,q] = np.real(modeshape[:,q])/mx*sign(np.real(modeshape[om,q]))
-    return freqdmp, modeshape, sj1, v, d
-
-#
-# OKID_ERA_DC
-#
 def parse_okid(args, config):
     """
     p determines order of the observer Kalman ARX filter used in OKID-ERA-DC.
     n determines size of the state-space model used for representing the system.
     """
     return config
 
-#
-# TFE
-#
-def stfe(dati, dato, **config):
-    pass
+# y = output data: forced response. dimensions of y: p x nt, where nt = number of timesteps
+# u = input data: input. dimensions of u: q x nt.
+# m = number of Markov parameters (impulse response timesteps) to solve for
+def get_impulse(y, u):
+    p = y.shape[0]
+    q = u.shape[0]
+    nt = y.shape[1]
+    assert y.shape[1] == u.shape[1]
+    # form a blockwise upper triangular matrix of inputs
+    U = np.zeros((q*nt, nt))
+    for i in range(nt):
+        for j in range(nt-i):
+            U[q*j:q*(j+1),i] = u[:,i]
+    Y_impulse = y @ np.linalg.pinv(U)
+    assert Y_impulse.shape == (p, q*nt)
+    return Y_impulse
+
+def okid2(y, u, m):
+    p = y.shape[0]
+    q = u.shape[0]
+    nt = y.shape[1]
+    assert y.shape[1] == u.shape[1]
+    # form a blockwise upper triangular matrix of inputs
+    U = np.zeros((q*nt, nt))
+    for i in range(nt):
+        for j in range(nt-i):
+            U[q*j:q*(j+1),i] = u[:,i]
+    Y_impulse = y @ np.linalg.pinv(U)
+    assert Y_impulse.shape == (p, q*nt)
+    return Y_impulse
+
+def OKID_brunton(y,u,m):
+    
+    p = y.shape[0]
+    q = u.shape[0]
+    nt = y.shape[1]
+    assert y.shape[1] == u.shape[1]
+    
+    # Form data matrices y and V
+    V = np.zeros((q+(q+p)*m,nt))
+    for i in range(nt):
+        V[:q,i] = u[:q,i]
+        
+    for i in range(1,m+1):
+        for j in range(nt-i):
+            vtemp = np.concatenate((u[:,j],y[:,j]))
+            V[q+(i-1)*(q+p):q+i*(q+p),i+j] = vtemp
+    
+    # Solve for observer Markov parameters Ybar
+    Ybar = y @ np.linalg.pinv(V,rcond=10**(-3))
+    
+    # Isolate system Markov parameters H, and observer gain M
+    D = Ybar[:,:q] # feed-through term (or D matrix) is the first term
+    
+    Y = np.zeros((p,q,m))
+    Ybar1 = np.zeros((p,q,m))
+    Ybar2 = np.zeros((p,q,m))
+    
+    for i in range(m):
+        Ybar1[:,:,i] = Ybar[:,q+(q+p)*i : q+(q+p)*i+q]
+        Ybar2[:,:,i] = Ybar[:,q+(q+p)*i+q : q+(q+p)*(i+1)]
+    
+    Y[:,:,0] = Ybar1[:,:,0] + Ybar2[:,:,0] @ D
+    for k in range(1,m):
+        Y[:,:,k] = Ybar1[:,:,k] + Ybar2[:,:,k] @ D
+        for i in range(k-1):
+            Y[:,:,k] += Ybar2[:,:,i] @ Y[:,:,k-i-1]
+            
+    H = np.zeros((D.shape[0],D.shape[1],m+1))
+    H[:,:,0] = D
+    
+    for k in range(1,m+1):
+        H[:,:,k] = Y[:,:,k-1]
+        
+    return H
+
+# Y = output data: response to unit impulse, or "impulse response," or "Markov parameters".
+# dimensions of Y: p x q x nt, where nt = number of timesteps = number of Markov parameters = number of blocks
+# mc = number of block rows in Hankel matrix = order of controllability matrix
+# mo = number of block columns in Hankel matrix = order of observability matrix
+# p = number of outputs
+# q = number of inputs
+# r = reduced model order = dimension of reduced A = newly assumed dimension of state variable
+def era(Y,mo,mc,p,q,r):
+    # get D from first p x q block of impulse response
+    Dr = Y[:,:,0]  # first block of output data
+    
+    assert Y.shape[:2] == (p,q)  # sanity check that we're passing in the right output data
+    assert Y.shape[2] >= mo+mc   # make sure there are enough timesteps to assemble this size of Hankel matrix
+    
+    # make impulse response into Hankel matrix and shifted Hankel matrix
+    H = np.zeros((p*(mo), q*(mc+1)))
+    for i in range(mo):
+        for j in range(mc+1):
+            H[p*i:p*(i+1), q*j:q*(j+1)] = Y[:,:,i+j+1]
+    H0 = H[:,:-q]
+    H1 = H[:,q:]
+    assert H0.shape == H1.shape == (p*(mo), q*(mc))
+
+    # reduced SVD of Hankel matrix
+    def _svd(*args):
+        U,S,V = scipy.linalg.svd(*args, lapack_driver="gesvd")
+        return U,S,V.T.conj()
+    U,S,V = _svd(H0)
+    SigmaInvSqrt = np.diag(S[:r]**-0.5)
+    SigmaSqrt = np.diag(S[:r]**0.5)
+    Ur = U[:,:r]
+    Vr = V[:,:r]
+
+    # get A from SVD and shifted Hankel matrix
+    Ar = SigmaInvSqrt @ Ur.T.conj() @ H1 @ Vr @ SigmaInvSqrt
+
+    # get B and C
+    Br = (SigmaSqrt @ Vr.T.conj())[:,:q]
+    Cr = (Ur @ SigmaSqrt)[:p,:]
+
+    return (Ar,Br,Cr,Dr,S)
+
+# l = initial lag for data correlations
+# g = lags between correlation matrices
+# a = number of block rows in Hankel of correlation matrix
+# b = number of block columns in Hankel of correlation matrix
+def era_dc(Y,mo,mc,p,q,r,l,g,a,b):
+    # get D from first p x q block of impulse response
+    Dr = Y[:,:,0]  # first block of output data
+    
+    assert Y.shape[:2] == (p,q)  # sanity check that we're passing in the right output data
+    assert Y.shape[2] >= l+(a+1+b+1)*g+mo+mc   # make sure there are enough timesteps to assemble the Hankel matrices
+    
+    # make impulse response into Hankel matrix
+    H = np.zeros((p*(mo), q*(mc+l+(a+1+b+1)*g))) # Hankel of Markov parameters
+    for i in range(mo):
+        for j in range(mc+l+(a+1+b+1)*g):
+            H[p*i:p*(i+1), q*j:q*(j+1)] = Y[:,:,i+j+1]
+    H0 = H[:,:q*mc]
+    assert H0.shape == (p*(mo), q*(mc))
+
+    dimR = p*mo # Dimension of square correlation matrices
+    dimHRl = (dimR*(a+1), dimR*(b+1)) # Dimension of Hankels of correlation matrices
+    HRl = np.zeros(dimHRl) # Hankel of correlation matrices
+    HRl1 = np.zeros(dimHRl) # Shifted Hankel of correlation matrices
+    for i in range(a+1):
+        for j in range(b+1):
+            Hl = H[:, q*(l+1+(i+j)*g):q*(l+1+(i+j)*g+mc)]
+            Hl1 = H[:, q*(l+1+(i+j)*g+1):q*(l+1+(i+j)*g+mc+1)]
+            assert Hl.shape == Hl1.shape == (p*(mo), q*(mc))
+            R = Hl@H0
+            R1 = Hl1@H0
+            assert R.shape == R1.shape == (dimR,dimR)
+            HRl[dimR*i:dimR*(i+1), dimR*j:dimR*(j+1)] = R
+            HRl1[dimR*i:dimR*(i+1), dimR*j:dimR*(j+1)] = R1
+
+    # reduced SVD of Hankel matrix
+    def _svd(*args):
+        U,S,V = scipy.linalg.svd(*args, lapack_driver="gesvd")
+        return U,S,V.T.conj()
+    U,S,V = _svd(HRl)
+    SigmaInvSqrt = np.diag(S[:r]**-0.5)
+    SigmaSqrt = np.diag(S[:r]**0.5)
+    Ur = U[:,:r]
+    Vr = V[:,:r]
+
+    # get A from SVD and shifted Hankel matrix
+    Ar = SigmaInvSqrt @ Ur.T.conj() @ HRl1 @ Vr @ SigmaInvSqrt
+
+    # get B and C
+    Br = ((SigmaInvSqrt @ Ur.T.conj())[:,:dimR] @ H0)[:,:q]
+    Cr = (Ur @ SigmaSqrt)[:p,:]
 
-def ftfe(dati, dato, **config):
-    "Fourier transfer function estimate"
-    pass
-
-#
-# SRIM
-#
-def _blk_3(i, CA, U):
-    return i, np.einsum('kil,klj->ij', CA[:i,:,:], U[-i:,:,:])
+    return (Ar,Br,Cr,Dr,S)
 
 
-def parse_srim(argi, config):
-    help="""
-    SRIM -- System Identification with Information Matrix
-
-    Parameters
-    p           order of the observer Kalman ARX filter.
-    n           size of the state-space model used for 
-                representing the system.
-    """
-    config.update({"p"  :  5, "orm":  4})
-    #argi = iter(args)
-    channels = [[17, 3, 20], [9, 7, 4]]
-    for arg in argi:
-        if arg == "-p":
-            config["p"] = int(next(argi))
-        elif arg == "--dt":
-            config["dt"] = float(next(argi))
-        elif arg == "-n":
-            config["orm"] = int(next(argi))
-        elif arg in ["--help", "-h"]:
-            print(help)
-            sys.exit()
-        elif arg == "--inputs":
-            inputs = next(argi)[1:-1].split(",")
-            if isinstance(inputs, str):
-                channels[0] = [int(inputs)]
-            else:
-                channels[0] = list(map(int, inputs))
-        elif arg == "--outputs":
-            outputs = next(argi)[1:-1].split(",")
-            if isinstance(outputs, str):
-                channels[1] = [int(outputs)]
-            else:
-                channels[1] = list(map(int, outputs))
-        elif arg == "--":
-            continue
+def _era_ya(kmax, m, l, r, Y, n, svd="gesvd"):
+    # ERA/DC
+    #
+    # Form Hankel matrix (H) from the Markov parameters (Y) (Eq. 3.80)
 
-        else:
-            config["event_file"] = arg
+    # Obtain Hankel Matrix of Zeroth Order & First Order
+    H0,H1 = np.zeros((2, kmax*m, l*r))
+    #H0 = hankel(Y,0)
+    for hj in range(kmax):
+        for jh in range(l):
+            H0[hj*m:hj*m+m, jh*r:jh*r+r] = Y[jh+hj+1]
+            H1[hj*m:hj*m+m, jh*r:jh*r+r] = Y[jh+hj+2]
+    
+    if svd in ["gesvd", "gesdd"]:
+        import scipy.linalg
+        def _svd(*args):
+            U,S,V = scipy.linalg.svd(*args, lapack_driver=svd)
+            return U,S,V.T.conj()
+
+    ## 2c. Use H matrix to compute system matrices A, B & C
+    R1,sis,S1 = _svd(H0) # singular value decomposition
+    Sis = np.diag(sis[:n])
+
+    Siv = np.diag(1/np.sqrt(sis[:n]))
+    # A: state transition matrix (Eqs. 3.32 & 3.82)
+    A  = Siv@R1[:,:n].T@H1@S1[:,:n]@Siv
+    # B: input influence matrix (Eqs. 3.32 & 3.83)
+    B = (np.sqrt(Sis)@S1[:,:n].T)[:,:r]
+    Observability = R1[:,:n]@np.sqrt(Sis)
+    # C: output influence matrix (Eqs. 3.34 & 3.84)
+    C  = Observability[:m,:]
 
+    return A,B,C
 
-    event = quakeio.read(config["event_file"])
-    inputs = np.array([
-        event.match("l", station_channel=f"{i}").accel.data for i in channels[0]
-    ]).T
-    outputs = np.array([
-        event.match("l", station_channel=f"{i}").accel.data for i in channels[1]
-        #event.at(file_name=f"CHAN{i:03d}.V2").accel.data for i in channels[1]
-    ]).T
-    npoints = len(inputs[:,0])
-    dt = event.at(station_channel=f"{channels[0][0]}").accel["time_step"]
-    config["dt"] = dt
-
-    #print(config)
-    #sys.exit()
-
-    A,B,C,D = srim(inputs, outputs, **config)
-    freqdmpSRIM, modeshapeSRIM, *_ = ComposeModes(dt, A, B, C, D)
-    output = [
-            {"frequency": np.real(x[0]), "damping": np.real(x[1])} 
-            for x in freqdmpSRIM if all(x > 0.0)
-    ]
-    import json
-    print(json.dumps(output, cls=JSON_Encoder, indent=4))
-    return config
 
-def srim(
-    dati,
-    dato,
-    full     : bool = True,
-    verbose  : bool = False,
-    pool_size: int  = 6,
-    **config
-):
+def okid(dati, dato, svd="gesvd", debug=False, **config):
     """
-    mro $(p)$ determines order of the observer Kalman ARX filter used in OKID-ERA-DC.
-    orm $(n)$ determines size of the state-space model used for representing the system.
-
-    Returns
-    =======
-     freqdampSRIM:
-        variable is a matrix that includes the information of identified
-        frequencies, damping ratios & validation of the modes with MPC & EMAC criteria.
-        Each row of freqdamp corresponds to a mode. Columns are as follows:
-        1) frequency, 2) damping ratio, 3) order index, 4) condition number, 5) MPC.
-        If values in columns 5 is > 0.5, identified mode is valid.
-     modeshapeSRIM:
-         stores the mode shape information for identified modes.
-     RMSEpredSRIM:
-         root mean square error of the predicted output from
-         identified parameters with respect to the actual output
-
-    ## SRIM Methodology
-
-    More information on SRIM algorithm can be found in Sections 3.4.4 & 3.4.5 of
-    (Arici & Mosalam, 2006). Equations below refer to this report. SRIM is a MIMO
-    SI method that is based on state space identification using least squares and
-    consists of the following steps:
-
-
-    2a. Determine output (y) & input (u) vectors [Eqs. 3.58 & 3.60].
-    2b. Compute the correlation terms & the coefficient matrix (Eqs. 3.68 & 3.69).
-    2c. Obtain observability matrix using full or partial decomposition (Eqs. 3.72 & 3.74).
-    2d. Use the observability matrix to compute system matrices A, B & C, in which modal 
-        information is embedded.
-    2e. Obtain the modal information from matrices A, B & C.
-    2f. Spatial & temporal validation of the identified modes.
-    2g. Back calculate (estimate) the output accelerations with the state-space system &
-        check against the actual output accelerations.
+    PART 2: OKID-ERA-DC (Observer Kalman filter Identification -
+            Eigen Realization with Direct Correlations)
+    -----------------------------------------------------------------
+
+    # Inputs
+    Modelparameters
+        div = 1;     # A parameter used for decimating data. 1 uses entire data without downsampling.
+        mro = 10;    # Model reduction order
+        orm = 4;     # Order of the model. # of computed and plotted modes dep on orm.
+                     # For orm = 2, one mode is found, for orm = 4, two modes are found.
+    svd:
+        GESDD: a two-stage algorithm. It first reduces the input matrix to bidiagonal form via 
+        Householder reflection, then divides the bidiagonal matrix into smaller matrices to calculate 
+        singular values and the unitary matrices U and V. Finally, the singular values of the entire 
+        input matrix is simply the those of the smaller sub-matrices.
+        
+        GESVD: also a two-stage algorithm where the first step is identical to GESDD. The second step 
+        can be done using iterative QR decomposition to derive singular values. More mathematical details are available here.
 
-    For orm = 2, one mode is found, for orm = 4, two modes are found.
-    For case 1, one mode is transverse & the other is torsion.
-    For all other cases, the second mode is a higher mode.
     Sometimes higher orm still gives fewer modes, e.g. orm = 8 for case 1 gives
     three modes, but one of them is invalid according to the EMAC & MPC criteria.
-    same orm in OKID-ERA-DC is used. It can be changed if needed.
-
-    """
-    #
-    # Convenience argument handling
-    #
+    kmax = 100;  #Number of computed Markov parameters, indicated as 1000 on page 43 of
+    (Arici & Mosalam, 2006). However, it was input as 100 in the code.
+    kmax = 100 runs much faster & both kmax = 100 & 1000 give the same results.
+
+    # Outputs
+    1. freqdamp variable is a matrix that includes the information of identified
+       frequencies, damping ratios & validation of the modes with MPC & EMAC criteria
+       Each row of freqdamp corresponds to a mode. Columns are as follows:
+       1) frequency, 2) damping ratio, 3) order index, 4) condition number, 5) input EMAC,
+       6) output EMAC, 7) MPC. If values in columns 5-7 are > 0.5, identified mode is valid.
+    2. modeshape stores the mode shape information for identified modes.
+    3. RMSEpred: root mean square error of the predicted output from
+       identified parameters with respect to the actual output.
+    4. Markovparamerror: root mean square error used to validate accurate
+       computation of Markov parameters
+
+    # Description of the Methodology
+    More information on OKID-ERA-DC method can be found in
+    Section 3.4.6 of (Arici & Mosalam, 2006). Equations below refer to this report.
+    OKID-ERA-DC is a Multiple Input - Multiple Output (MIMO) System Identification (SI) method
+    that consists of the following steps:
+    1. Data pre-processing (baseline correction, filtering & decimation)
+    2. Identify observer Kalman filters using Observer Kalman filter Identification (OKID)
+       methodology. This step basically consists of developing a simple observer model of
+       a system from a MIMO ARX structure, Eq. (3.76), which is broken into these 6 steps:
+   
+    3a. Determine Markov parameters (M) in a least squares sense, Eq. (3.76).
+
+    3b. Establish the Hankel matrix (H) from the Markov parameters, (Eq. 3.80).
+    3c. Use H to compute system matrices A, B & C, in which modal information is embedded.
+    // 3d. Obtain the modal information from matrices A, B & C.
+    3e. Spatial & temporal validation of the identified modes.
+    3f. Back calculate (estimate) the output accelerations with the state-space system &
+        check against the actual output accelerations.
+    """ 
     dt = to = config.get("dt", None) or dati["time_step"]
-    p = config.get("p", config.get("mro"))         # # steps used for the identification (ie, prediction horizon)
+    p = config.get("p", config.get("mro")) # # steps used for the identification (ie, prediction horizon)
     n = n1 = config.get("n", config.get("orm", 4))  # Order of the model.
+    
+    if svd in ["gesvd", "gesdd"]:
+        import scipy.linalg
+        def _svd(*args):
+            U,S,V = scipy.linalg.svd(*args, lapack_driver=svd)
+            return U,S,V.T.conj()
+
+    elif svd in ["xla", "jax"]:
+        from jax.scipy.linalg import svd as _svd
 
     if isinstance(dati, list):
         dati = np.array([i.data for i in dati]).T
     elif issubclass(dati.__class__, dict):
         dati = dati.data
 
     if isinstance(dato, list):
@@ -351,299 +302,279 @@
     elif issubclass(dato.__class__, dict):
         dato = dato.data
 
     if len(dati.shape) < 2:
         dati = np.atleast_2d(dati).T
     if len(dato.shape) < 2:
         dato = np.atleast_2d(dato).T
+        
+    dati = dati[:-1,:]
+    dato = dato[:-1,:]
+
+    #verbose = True
+    #dn = config.get("dn", None) or dati.shape[0]
+    kmax    = config["kmax"]
+    n = config["orm"]   # assign order of model input to variable n, consistent with Eqs. 3.81-3.84
+    p = config["mro"]   # assign input model reduction order to variable p, consistent with Eq. 3.76
 
-    if verbose:
-        progress_bar = tqdm
-    else:
-        progress_bar = lambda arg, **kwds: (i for i in arg)
-
-    dn = config.get("dn", None) or dati.shape[0]
-
-    # 2a. Compute y (output) and u (input) vectors (Eqs. 3.58 & 3.60)
-
-    # Note that main Step 2 develops Eq. 3.57.
-    # Therefore, it is not part of the code.
-    # Accordingly, the code continues with Step 2a to compute the output & input vectors.
-
-    # Calculate the usable size of the data matrix
-    # dn = size(dat,1)/div;       # total # time steps after decimating
-    nsizS = dn-1-p+2
 
     l,m = dato.shape # m is the number of output channels
     _,r = dati.shape # r is the number of input channels
 
+    # ASSERT SIZE(DATO,1) == SIZE(DATI,1)
 
-    assert p >= n/m + 1
+    ## 2a. Obtain Observer Markov Parameters
+    # The Markov parameters are computed in two steps:
+    # i)  The Observer Markov matrices are computed from Eq. 3.76 using a linear regression approach
+    # ii) Compute the system Markov parameters from the Markov matrices using recursive relations
+
+    # Compute matrix U that represents ARX equation of current output on p time steps of past output
+    # & input values (Eq. 3.76)
+    U = np.zeros(((m+r)*p+r, l))
+    U[:r,:] = dati.T
+    for b in range(1,p+1):
+        U[(b-1)*(r+m)+r:(b-1)*(r+m)+r+r+m, b:] = [*dati[:-b,:r].T, *dato[:-b, :m].T]
+
+
+    # i) Compute the matrix of Observer Markov Parameter Matrix (M)
+    #    in Eq 3.76 using Linear Regression
+    uu,wr,V = _svd(U,0)
+    pg = (r+m)*p+r
+    for i in range((r+m)*p+r):
+        if wr[i] <= 0.001:
+            pg = i
+            break
+
+    s = np.diag(wr)
+
+    pss = V[:,:pg]@linsolve(s[:pg,:pg], uu[:,:pg].T)
+    M = dato.T@pss           # M: Observer Markov Parameter Matrix
+
+    # Fit for multiple regression
+    # RMSE between actual output & y on left hand side in Eq. 3.76. It should be 
+    # quite small (e.g., 10^-3) for accurately computed Markow parameters.
+    # ypreo = M@U
+    # markovParamError = 1/m*sum((
+    #     sum((dato[:,i] - ypreo[i,:].T)**2)/sum(dato[:,i]**2)
+    #     for i in range(m)
+    # ))  
+
+
+    ## ii) Compute Markov parameters (Y) using recursive relations in Eqs. 3.78 & 3.79
+    #      (Equation 6.21 in Juang 1994)
+
+    # Matrix D is directly equal to the Observer Markov parameter matrix (Eq. 3.77)
+    D = M[:, :r]  # D: Direct Transmission term
+
+    Y = [D]
+    # First p steps (Eq. 3.78)
+    for i in range(p):
+        Y.append(
+            M[:, r+i*(r+m):r+i*(r+m)+r] + sum(
+                M[:, r+j*(r+m)+r:r+j*(r+m)+r+m]@Y[i-j]
+                for j in range(i+1)
+            )
+        )
+    # Remainder (Eq. 3.79)
+    for i in range(p, l+kmax):
+        sumt = zeros((m,r))
+        for j in range(p):
+            sumt += M[:,r+j*(r+m)+r:r+j*(r+m)+r+m]@Y[i-j]
 
-    ypS = np.zeros((m*p,nsizS))
-    upS = np.zeros((r*p,nsizS))
+        Y.append(sumt)
 
-    # Compute Y (output) & U (input) vectors (Eqs. 3.58 & 3.60 Arici 2006)
-    for b in range(p):
-        ypS[b*m:(b+1)*m,:nsizS+1] = dato[b:nsizS+b, :].T
-        upS[b*r:(b+1)*r,:nsizS+1] = dati[b:nsizS+b, :].T
-
-
-    # 2b. Compute the correlation terms and the coefficient matrix 
-    #     (Eqs. 3.68 & 3.69).
-
-    # Compute the correlation terms (Eq. 3.68)
-    Ryy = ypS@ypS.T/nsizS
-    Ruu = upS@upS.T/nsizS
-    Ruy = upS@ypS.T/nsizS
-
-    assert Ryy.shape[0] == Ryy.shape[1] == p*m
-    assert Ruy.shape[0] == p*r
-    assert Ruy.shape[1] == p*m
-
-    # Compute the correlation matrix (Eq. 3.69)
-    Rhh = Ryy - Ruy.T@linsolve(Ruu,Ruy)
-
-    # 2c. Obtain observability matrix using full or partial decomposition 
-    #     (Eqs. 3.72 & 3.74).
-    if full:
-        # Full Decomposition Method
-        un,*_ = np.linalg.svd(Rhh,0)           # Eq. 3.74
-        Op = un[:,:n]                          # Eq. 3.72
-        A = lsqminnorm(Op[:(p-1)*m,:], Op[m:p*m,:])
-        C = Op[:m,:]
-    else:
-        # Partial Decomposition Method
-        un,*_ = np.linalg.svd(Rhh[:,:(p-1)*m+1],0)
-        Op = un[:,:n]
-        A = lsqminnorm(Op[:(p-1)*m,:], Op[m:p*m,:])
-        C = un[:m,:]
-
-    # Computation of system matrices B & D
-    # Output Error Minimization
-
-    # Setting up the Phi matrix
-    Phi  = np.zeros((m*nsizS, n+m*r+n*r))
-    CA_powers = np.zeros((nsizS, m, A.shape[1]))
-    CA_powers[0, :, :] = C
-    A_p = A
-    for pwr in range(1,nsizS):
-        CA_powers[pwr,:,:] =  C@A_p
-        A_p = A@A_p
-
-    # First block column of Phi
-    for df in range(nsizS):
-        Phi[df*m:(df+1)*m,:n] = CA_powers[df,:,:]
-
-    # Second block column of Phi
-    Imm = np.eye(m)
-    for i in range(nsizS):
-        Phi[i*m:(i+1)*m, n:n+m*r] = np.kron(dati[i,:],Imm)
-
-    # Third block column of Phi
-    In1n1 = np.eye(n)
-    cc = n + m*r + 1
-    dd = n + m*r + n*r
-
-    krn = np.array([np.kron(dati[i,:],In1n1) for i in range(nsizS)])
-
-    with multiprocessing.Pool(pool_size) as pool:
-        for i,res in progress_bar(
-                pool.imap_unordered(
-                    partial(_blk_3,CA=CA_powers,U=np.flip(krn,0)),
-                    range(1,nsizS),
-                    200
-                ),
-                total = nsizS
-            ):
-            Phi[i*m:(i+1)*m,cc-1:dd] = res
-
-    y = dato[:nsizS,:].flatten()
-
-    teta = lsqminnorm(Phi,y)
-
-    x0 = teta[:n1]
-    dcol = teta[n1:n1+m*r]
-    bcol = teta[n1+m*r:n1+m*r+n1*r]
-
-    D = np.zeros((m,r))
-    B = np.zeros((n,r))
-    for wq in range(r):
-        D[:,wq] = dcol[wq*m:(wq+1)*m]
+    # The Markow parameters Y have been computed.
 
-    for ww in range(r):
-        B[:,ww] = bcol[ww*n:(ww+1)*n]
+    A,B,C = _era_ya(kmax, m, l, r, Y, _svd, n)
+
+    if debug:
+        return locals()
 
-    assert A.shape[0] == A.shape[1] == n
     return A,B,C,D
 
-#PY
-# #% 2e. Obtain the modal information from the system matrices A & C
-# # This includes determination of: a) modal frequencies, b) damping ratios & c) mode shapes
-# # c) Determination of mode shapes
-#     mod = C1@vS                 # mode shapes (Eq. 3.40), v is the eigenvectors of matrix A
-# 
-
-#% 2f. Validation Analysis
-
-# Two criteria are used for selection of identified genuine modes, in terms of spatial & temporal consistency.
-# a) Modal Phase Collinearity (MPC) testing spatial consistency of identification results.
-#    Modes having MPC value above 0.5 (mpc parameter below) are considered as genuine modal quantities.
-# b) Extended Modal Amplitude Coherence (EMAC), evaluates temporal consistency of the identification results.
-#    Both output EMAC & input EMAC can be computed. Input EMAC requires the controllability matrix.
-#    Because the controllability matrix is not estimated by all considered SI methods,
-#    this criterion is computed, but not used.
-#    Modes with output EMAC values < 0.5 are considered spurious & therefore not reported.
-
-# a) Modal Phase Collinearity (MPC) [Eqs. 3.85-3.87]
-#Py
-##    for q in range(n):
-##        a = real(mod[:,q])
-##        b = imag(mod[:,q])
-##        sxx[:,q] = a.T*a
-##        syy[:,q] = b.T*b
-##        sxy[:,q] = a.T*b
-##        nu[q] = (syy[:,q]-sxx[:,q])/(2*sxy[:,q])
-##        lam[1,q] = (sxx[:,q]+syy[:,q])/2+sxy[:,q]*(nu(q)**2+1)**0.5
-##        lam[2,q] = (sxx[:,q]+syy[:,q])/2-sxy[:,q]*(nu(q)**2+1)**0.5
-##        mpc[q] = ((lam[0,q]-lam[1,q])/(lam[0,q]+lam[1,q]))**2
-
-
-# b) Extended Modal Amplitude Coherence (EMAC)
-
-# Only EMAC Output is computed as there is no Controllability Matrix
-
-# Note that the computations are commented out as the matrix B is needed
-
-#%KKKKK
-##PY
-##    plin = Op1@vS                # Observability Matrix used for the output-EMAC
-##    lamb = linsolve(vS,A1)*vS
-##    bkh = linsolve(vS,B)
-### Pick the last block row
-##    pto = plin((p-1)*m+1:m*p,:)  # the identified value at T0
-##    for ds in range(n):
-##        ptop[:,ds] = mod[:,ds]*exp(sj1S(ds)*to*(p-1))
-##
-### Computation of rij
-##    for qa in range(n):
-##        for qz in range(m):
-##            Rij(qa,qz) = min((abs(pto(qz,qa))/abs(ptop(qz,qa))),(abs(ptop(qz,qa))/abs(pto(qz,qa))))
-##            Pij = angle(pto(qz,qa)/ptop(qz,qa))
-##            Pijn(qa,qz) = Pij
-##            if abs(Pij) <= pi/4:
-##                Wij[qa,qz] = 1-abs(Pij)/(pi/4)
-##            else:
-##                Wij[qa,qz] = 0
-##
-##            emaco[qa,qz] = Rij[qa,qz]*Wij[qa,qz]
-##
-##
-### Computation of final emac
-##    for xc in range(n):
-##        # Weight for emaco
-##        sumo = 0.0
-##        for la in range(m):
-##            sumo = emaco(xc,la)*abs(mod(la,xc))**2+sumo
-##        emacof[xc] = sumo/((mod[:,xc].T*mod[:,xc]))
-##        emac[xc] = emaco[xc]
-#%KKKKK
-
-# Add the MPC to the matrix freqdampSRIM
-#    for lih = 1:size(freqdmpSRIM,1)
-#        freqdmpSRIM[lih,5] = emacof(freqdmpSRIM(lih,3))
-#        freqdmpSRIM[lih,6] = mpc(freqdmpSRIM(lih,3))
-#        if freqdmpSRIM[lih,5]>0.5 and freqdmpSRIM[lih,6]>0.5:
-#            validationm = ' valid'
-#        else:
-#            validationm = ' not valid'
-#
-#        scroutput = strcat('Mode',num2str(lih), ...
-#            ': Output EMAC =  ',num2str(freqdmpSRIM(lih,5)),...
-#            ', MPC =  ',num2str(freqdmpSRIM(lih,6)),...
-#            ' -->',' SRIM Identified Mode ',...
-#            num2str(lih), ' is',validationm)
-#        sprintf(scroutput)
-
-
-#% 2g. Back calculate (estimate) output accelerations with state-space system &
-#%     check against actual output accelerations
-
-# Note that the computations are commented out as the matrix B is needed
-
-# Prediction using state space model
-#%KKKKK
-##PY
-##    ms1 = modstruc(A1,B,C1,D,zeros(n,m),x0)
-##    th1 = ms2th(ms1,'d')
-##    e,r = resid([dato dati],th1)
-##    simy = idsim([dati],th1);                # simy represents the estimated accelerations
-##
-##    for i in range(m):
-##        temsum = sum((dato[:,i]-simy[:,i]).**2)
-##        Jm[i] = temsum/(sum(dato[:,i].**2));     # Root mean square error of estimated accelerations
-##
-##    RMSEpredSRIM = sum(Jm)/m
-###%KKKKK
-##    return freqdmpSRIM,modeshapeSRIM,RMSEpredSRIM
-
-# def parse_args(argv):
-#     argi = iter(argv[1:])
-#     # assert argv[1] in ["srim", "stfe", "ftfe", "okid"]
-#     for arg in argi:
-#         if arg == "":
-#             pass
 
-if __name__ == "__main__":
-    import sys
-    import quakeio
-    from pathlib import Path
-    method = None
+def validate(freqdmp, v, system, **config):
+    """2e. Validation Analysis
+
+    Two criteria are used for selection of identified genuine modes
+    (in the sense of spatial & temporal consistency).
+
+    a) Modal Phase Collinearity (MPC) testing spatial consistency of identification results.
+       Modes having MPC value above 0.5 (mpc parameter below) are considered as genuine modal quantities.
+
+    b) Exted Modal Amplitude Coherence (EMAC), evaluates temporal consistency of the identification results.
+       Both output EMAC & input EMAC can be computed. Input EMAC requires the controllability matrix.
+       Because the controllability matrix is not estimated by all considered SI methods,
+       this criterion is computed, but not used.
+       Modes with output EMAC values < 0.5 are considered spurious & therefore not reported.
+
+    """
+    mpc = MPC(n, v, system)
+
+    # Add the input EMAC, output EMAC, and MPC to the matrix freqdamp
+    for lih in range(size(freqdmp)[0]):
+        freqdmp[lih,4] = emacif(freqdmp[lih,2])
+        freqdmp[lih,5] = emacof(freqdmp[lih,2])
+        freqdmp[lih,6] = mpc[freqdmp(lih,3)]
+        if freqdmp[lih,5]>0.5 and freqdmp[lih,7]>0.5:
+            # valid
+            return True
+        else:
+            # not valid
+            return False
+
+def MPC(n, v, system):
+    """a) Modal Phase Collinearity (MPC) [Eqs. 3.85-3.87]"""
+    _,__,C,___ = system
+    modes_raw = C@v
+    _, n = modes_raw.shape
+    sxx, syy, sxy = np.zeros((3, *modes_raw.shape))
+    nu, mpc = np.zeros((2, n))
+    lam = np.zeros((2, n))
+    for i in range(n):
+        sxx[:,i] = np.real(modes_raw[:,i]).T@np.real(modes_raw[:,i])
+        syy[:,i] = np.imag(modes_raw[:,i]).T@np.imag(modes_raw[:,i])
+        sxy[:,i] = np.real(modes_raw[:,i]).T@np.imag(modes_raw[:,i])
+        nu[i]    = (syy[:,i]-sxx[:,i])/(2*sxy[:,i])
+        lam[1,i] = (sxx[:,i]+syy[:,i])/2 + sxy[:,i]*np.sqrt(nu[i]**2+1);
+        lam[2,i] = (sxx[:,i]+syy[:,i])/2 - sxy[:,i]*np.sqrt(nu[i]**2+1);
+        mpc[i]   = ((lam[0,i]-lam[1,i])/(lam[0,i]+lam[1,i]))**2;
+    return mpc
+
+def EMAC_Matrix(n, m, pto, ptop, debug=False):
+    emac = np.zeros((n, m))
+    for i in range(n):
+        for j in range(m):
+            Rij = min(
+                (abs(pto[j,i])/abs(ptop[j,i])),
+                (abs(ptop[j,i])/abs(pto[j,i]))
+            )
+            Pij = np.angle(pto[j,i]/ptop[j,i])
+            Wij = max(
+                1 - abs(Pij)/(pi/4),
+                0
+            )
+            emac[i,j] = Rij*Wij
+    return emac
+
+def EMAC_Variation(n,m,pto,ptop):
+    pass
+
 
-    config, out_ops = parse_args(sys.argv)
+def EnergyCondensedEMAC(n,m,emac,phi,debug=False):
+    "Equation 3.93"
+    return np.array([
+        sum(emac[i,j]*abs(phi[i,j])**2 
+            for j in range(m)
+        )/np.real(phi[i,:].conjugate().transpose()@phi[i,:])
+        for i in range(n) 
+    ])
+
+def MAC(shape,v, v_inv, A, B):
+    n,m,r,l = shape
+    lamb = v_inv@A@v
+    bkh = v_inv@B
+    for i in range(n):
+        for j in range(l):
+            qhat[i,j*r+1:j*r+r] = bkh[i,:]*(lamb[i,i])**j
+
+    selsiz = min(size(qlin),size(qhat))
 
-    if config["method"] == "test":
-        data_dir = Path("RioDell_Petrolia_Processed_Data")
+    for hnd in range(n):
+        ql = qlin[hnd,:selsiz(2)]
+        qh = qhat[hnd,:selsiz(2)]
+        mac[hnd] = abs(ql*qh.T)/(abs(ql*ql.T)*abs(qh*qh.T))**0.5
+
+
+def EMAC_Validate(shape, kmax, v, d, dt, system):
+    "b) Exted Modal Amplitude Coherence (EMAC)"
+    A,B,C,D = system
+    n,m,r,l = shape
+
+def OutputEMAC(n,m,kmax,A,C,Observability, debug=False,d=None,v=None, **_):
+    """Output EMAC (Eqs. 3.88-3.89)"""
+    if d is None:
+        assert v is None
+        from .ExtractModes import condeig 
+        v, d, _ = condeig(A)
+    pto = Observability[-m:,:]@v # the identified value at T0 ( last block row)
+    ptop = C@v@np.diag(d**(kmax-1))
+    emaco  = EMAC_Matrix(n,m,pto,ptop)
+    if debug:
+        return locals()
+    return EnergyCondensedEMAC(n, m, emaco, (C@v).T)
+
+
+def InputEMAC(Ctrl,A,B):
+    #
+    # Input EMAC
+    #
+    # # EMAC Input Variation
+    # for i in range(l):
+    #     qtovar = qlin[:,i*r:(i+1)*r]
+    #     qtopvar = (np.diag(d)**i)*inm
+    #     emaci = EMAC_Matrix(n,m,qtovar,qtopvar)
+    #     emacivar[:,i] = EnergyCondensedEMAC(n,m,emaci,inm);
+
+    # Pick the last block column
+    v, d  = A.eigen()
+    v_inv = np.linalg.inv(v)
+    inm   = linsolve(v,B)   # Initial mode contribution
+    qlin  = v_inv@Ctrl;     # Modal controllability Matrix (F' in Pappa 1993)
+    qto   = qlin[:, (l-1)*r+1:l*r]
+    qtop  = d**(l-1)@inm
+    emaci = EMAC_Matrix(n, m, qto, qtop)
+    return EnergyCondensedEMAC(n, m, emaci, inm)
+    
 
-        first_input = quakeio.read(data_dir/f"CHAN{channels[0][0]:03d}.V2")
-        npoints = len(first_input.accel.data)
-        inputs, outputs = np.zeros((2,npoints,len(channels[0])))
-
-        # Inputs
-        inputs[:,0] = first_input.accel.data
-        for i,inp in enumerate(channels[0][1:]):
-            inputs[:,i+1] = quakeio.read(data_dir/f"CHAN{inp:03d}.V2").accel.data
-
-        # Outputs
-        for i,inp in enumerate(channels[1]):
-            outputs[:,i] = quakeio.read(data_dir/f"CHAN{inp:03d}.V2").accel.data
-
-        dt = first_input.accel["time_step"]
-        config["dt"] = dt
-
-    elif "event_file" in config:
-        event = quakeio.read(config["event_file"])
-        inputs = np.array([
-            event.match("l", station_channel=f"{i}").accel.data for i in channels[0]
-        ]).T
-        outputs = np.array([
-            event.match("l", station_channel=f"{i}").accel.data for i in channels[1]
-        ]).T
-        npoints = len(inputs[:,0])
-        dt = event.match("l", station_channel=f"{channels[0][0]}").accel["time_step"]
-        config["dt"] = dt
-
-    # print(config)
-    # sys.exit()
-
-    A,B,C,D = srim(inputs, outputs, **config)
-
-    freqdmpSRIM, modeshapeSRIM, *_ = ComposeModes(dt, A, B, C, D)
-
-    if not out_ops:
-        print(f"period: {np.real(1/freqdmpSRIM[:,0])}")
-    elif "freq" in out_ops:
-        print(f"frequency: {freqdmpSRIM[:,0]}")
-    elif "cycl" in out_ops:
-        print(f"cyclic_frequency: {2*np.pi*freqdmpSRIM[:,0]}")
 
+if __name__ == "__main__":
+    from pathlib import Path
+    import quakeio
+    # import ssid as si
+    import okid
+    import numpy as np
+    channels = dict( # PAINTER RIO DELL
+        inputs  = [17, 3, 20],
+        outputs = [ 9, 7 , 4]
+    )
+    channels = dict( # HAYWARD
+        inputs  = [17, 18, 24, 25],
+        outputs = [19, 20 , 22, 23]
+    )
+    for file in Path("hwd_recs").glob("RioDell_P*.zip"):
+        event = quakeio.read(file)
+        try:
+            inputs = [
+                event.match("r", file_name=f".*{chan}.*").accel
+                for chan in channels["inputs"]
+            ]
+            outpts = [
+                event.match("r", file_name=f".*{chan}.*").accel
+                for chan in channels["outputs"]
+            ]
+        except:
+            print(f"failed {file.name}")    
+    for file in Path("painter").glob("RioDell_P*.zip"):
+        event = quakeio.read(file)
+        try:
+            inputs = [
+                event.match("r", file_name=f".*{chan}.*").accel
+                for chan in channels["inputs"]
+            ]
+            outpts = [
+                event.match("r", file_name=f".*{chan}.*").accel
+                for chan in channels["outputs"]
+            ]
+        except:
+            print(f"failed {file.name}")
 
+        else:
+            dt = inputs[0]["time_step"]
+            V = OKID.okid(inputs, outpts, dt=dt, kmax=500, mro=10, orm=4, verbose=True)
+            break
+
+            A,B,C,D = OKID.okid(inputs, outpts, dt=dt, kmax=500, mro=10, orm=4, verbose=True)
+            freqdmpSRIM, modeshapeSRIM, *_ = si.ComposeModes(dt, A, B, C, D)
+            # Add validation
+            print(si.IdentifiedSystem(dt, A, B, C, D))
+            # print(file, np.real(1/freqdmpSRIM[:,0]))
```

