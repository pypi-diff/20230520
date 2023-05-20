# Comparing `tmp/wgd-2.0.14.tar.gz` & `tmp/wgd-2.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wgd-2.0.14.tar", last modified: Fri May 19 19:43:05 2023, max compression
+gzip compressed data, was "dist/wgd-2.0.15.tar", last modified: Sat May 20 13:46:37 2023, max compression
```

## Comparing `wgd-2.0.14.tar` & `wgd-2.0.15.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-19 19:43:05.427006 wgd-2.0.14/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.14/LICENSE
--rwxrwxrwx   0 heche     (1000) heche     (1000)    36301 2023-05-19 19:43:05.427006 wgd-2.0.14/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)    36063 2023-05-19 19:40:15.000000 wgd-2.0.14/README.md
--rwxrwxrwx   0 heche     (1000) heche     (1000)    49510 2023-05-19 17:07:00.000000 wgd-2.0.14/cli.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-19 19:43:05.428024 wgd-2.0.14/setup.cfg
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1904 2023-05-19 19:42:30.000000 wgd-2.0.14/setup.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-19 19:43:05.402999 wgd-2.0.14/test/
--rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-05-08 19:45:47.000000 wgd-2.0.14/test/test_core.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-19 19:43:05.419001 wgd-2.0.14/wgd/
--rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.14/wgd/__init__.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.14/wgd/beast.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.14/wgd/cluster.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.14/wgd/codeml.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   134238 2023-05-19 10:45:47.000000 wgd-2.0.14/wgd/core.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.14/wgd/mcmctree.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.14/wgd/mix.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   103647 2023-05-10 05:58:49.000000 wgd-2.0.14/wgd/peak.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     8513 2023-05-08 19:45:47.000000 wgd-2.0.14/wgd/syn.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    28648 2022-09-30 07:30:21.000000 wgd-2.0.14/wgd/utils.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    95587 2023-05-19 19:32:45.000000 wgd-2.0.14/wgd/viz.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-19 19:43:05.425025 wgd-2.0.14/wgd.egg-info/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    36301 2023-05-19 19:43:05.000000 wgd-2.0.14/wgd.egg-info/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)      369 2023-05-19 19:43:05.000000 wgd-2.0.14/wgd.egg-info/SOURCES.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-19 19:43:05.000000 wgd-2.0.14/wgd.egg-info/dependency_links.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       32 2023-05-19 19:43:05.000000 wgd-2.0.14/wgd.egg-info/entry_points.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)      749 2023-05-19 19:43:05.000000 wgd-2.0.14/wgd.egg-info/requires.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-05-19 19:43:05.000000 wgd-2.0.14/wgd.egg-info/top_level.txt
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-20 13:46:37.969748 wgd-2.0.15/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.15/LICENSE
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    39373 2023-05-20 13:46:37.969748 wgd-2.0.15/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    39135 2023-05-20 13:42:49.000000 wgd-2.0.15/README.md
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    50452 2023-05-20 10:15:19.000000 wgd-2.0.15/cli.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-20 13:46:37.969748 wgd-2.0.15/setup.cfg
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1904 2023-05-20 13:46:11.000000 wgd-2.0.15/setup.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-20 13:46:37.912264 wgd-2.0.15/test/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-05-08 19:45:47.000000 wgd-2.0.15/test/test_core.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-20 13:46:37.945640 wgd-2.0.15/wgd/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.15/wgd/__init__.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.15/wgd/beast.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.15/wgd/cluster.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.15/wgd/codeml.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   134238 2023-05-19 10:45:47.000000 wgd-2.0.15/wgd/core.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.15/wgd/mcmctree.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.15/wgd/mix.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   103472 2023-05-20 07:48:15.000000 wgd-2.0.15/wgd/peak.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     8513 2023-05-08 19:45:47.000000 wgd-2.0.15/wgd/syn.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    28648 2022-09-30 07:30:21.000000 wgd-2.0.15/wgd/utils.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   113236 2023-05-20 10:17:11.000000 wgd-2.0.15/wgd/viz.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-20 13:46:37.968331 wgd-2.0.15/wgd.egg-info/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    39373 2023-05-20 13:46:37.000000 wgd-2.0.15/wgd.egg-info/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      369 2023-05-20 13:46:37.000000 wgd-2.0.15/wgd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-20 13:46:37.000000 wgd-2.0.15/wgd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       32 2023-05-20 13:46:37.000000 wgd-2.0.15/wgd.egg-info/entry_points.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      749 2023-05-20 13:46:37.000000 wgd-2.0.15/wgd.egg-info/requires.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-05-20 13:46:37.000000 wgd-2.0.15/wgd.egg-info/top_level.txt
```

### Comparing `wgd-2.0.14/LICENSE` & `wgd-2.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `wgd-2.0.14/PKG-INFO` & `wgd-2.0.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: wgd
-Version: 2.0.14
-Summary: wgd
-Home-page: http://github.com/heche-psb/wgd
-Author: Hengchi Chen
-Author-email: heche@psb.vib-ugent.be
-License: GPL
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 
 # `wgd v2` : a suite tool of WGD inference and timing
 
 **Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
 
 [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
@@ -449,37 +438,67 @@
 
 ```
 wgd ksd wgd_globalmrbh/global_MRBH.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
 ```
 
 The file `speciestree.nw` is the text file of species tree in newick that rate correction would be conducted on. Its content is as below. Users need to provide the species pairs to be plotted. We suggest adding the option `--reweight` to recalculate the weight per species pair such that the weight of orthologous gene pairs will become 1 as the paralogous gene pairs. The flag `--plotkde` can be added when the kde curve of orthologous *K*<sub>S</sub> is desired. Extra collinear data can be added by the option `-ap`.
 
+```
+(((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
+```
+
 ![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
 
 As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
 
+If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+
 ```
-(((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
 ```
 
-If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+Note that we can easily show that *Aquilegia coerulea* has higher substitution rate than *Protea cynaroides* and *Vitis vinifera* by comparing their substitution distance in regard to the same divergence event with outgroup species *Acorus_americanus*, using command below.
 
 ```
-wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_viz_Compare_rate --spair "Acorus_americanus;Protea_cynaroides" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Vitis_vinifera;Acorus_americanus" --gsmap gene_species.map --plotkde
 ```
 
+![](data/Raw_Orthologues_Compare_rate.ksd.svg)
+
+As displayed above, the orthologous *K*<sub>S</sub> values bewteen *Aquilegia coerulea* and *Acorus americanus* has the highest mode, indicatingthe faster substitution rate of *Aquilegia coerulea* compared to *Protea cynaroides* and *Vitis vinifera*.
+
 Note that a necessary gene-species map file is needed for its implementation in `wgd viz`, which should be automately produced by the last `wgd ksd` step. The `gene_species.map` has contents as below in which each line is the joined string of gene name and species name by space.
 
 ```
 Aqcoe6G057800.1 Aquilegia_coerulea
 Vvi_VIT_201s0011g01530.1 Vitis_vinifera
 Pcy_Procy01g08510 Protea_cynaroides
 Aam_Acora.04G142900.1 Acorus_americanus
 ```
 
+A more complex plot can be made by add the flag `--plotelmm` such that the ELMM mixture modeling of provided paranome *K*<sub>S</sub> can be superimposed, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Corrected.ksd.svg)
+
+From the mixed *K*<sub>S</sub> plot above, we can see that the optimized lognormal component b with mode 1.2 is younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera* (1.39 and 1.47, respectively).
+
+Besides, we can also add the GMM mixture modeling of anchor *K*<sub>S</sub> values with the flag `--plotapgmm`, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotapgmmm
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Apgmm_Corrected.ksd.svg)
+
+As manifested above, the anchor *K*<sub>S</sub> component 2 with mode 1.28 is also younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera*. But we need to be of course cautious that such distinction comes with the uncertainties introduced from the applied mixture modeling methodology in terms of for instance different initialization points and the issue of overfitting and the sister speciess adopted in that there might be species with more disparate substitution rates than the one we chose.
+
 An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
 
 ```
 wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
 ```
 
 Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
@@ -488,18 +507,18 @@
 wgd ksd wgd_ortho/Orthogroups.sp.tsv -sp speciestree.nw --reweight -o wgd_ortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
 ```
 
 ![](data/Aquilegia_coerulea_OrthoKs_Corrected.ksd.svg)
 
 As shown above, the number of both paralogous gene pairs and orthologous gene pairs is different than the one from global MRBH family in that here we plotted all orthologous gene pairs instead of only global MRBH and potentially new paralogous gene pairs might be produced in the orthogroup inference step, together with different recalculated weights.
 
-If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
+If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, as we have already shown above, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
 
 ```
-wgd ksd wgd_globalmrbh/global_MRBH.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus"
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --gsmap gene_species.map
 ```
 
 We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
 ![](data/Raw_Orthologues.ksd.svg)
 
 ## Citation
```

### Comparing `wgd-2.0.14/README.md` & `wgd-2.0.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: wgd
+Version: 2.0.15
+Summary: wgd
+Home-page: http://github.com/heche-psb/wgd
+Author: Hengchi Chen
+Author-email: heche@psb.vib-ugent.be
+License: GPL
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 
 # `wgd v2` : a suite tool of WGD inference and timing
 
 **Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
 
 [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
@@ -438,37 +449,67 @@
 
 ```
 wgd ksd wgd_globalmrbh/global_MRBH.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
 ```
 
 The file `speciestree.nw` is the text file of species tree in newick that rate correction would be conducted on. Its content is as below. Users need to provide the species pairs to be plotted. We suggest adding the option `--reweight` to recalculate the weight per species pair such that the weight of orthologous gene pairs will become 1 as the paralogous gene pairs. The flag `--plotkde` can be added when the kde curve of orthologous *K*<sub>S</sub> is desired. Extra collinear data can be added by the option `-ap`.
 
+```
+(((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
+```
+
 ![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
 
 As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
 
+If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+
 ```
-(((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
 ```
 
-If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+Note that we can easily show that *Aquilegia coerulea* has higher substitution rate than *Protea cynaroides* and *Vitis vinifera* by comparing their substitution distance in regard to the same divergence event with outgroup species *Acorus_americanus*, using command below.
 
 ```
-wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_viz_Compare_rate --spair "Acorus_americanus;Protea_cynaroides" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Vitis_vinifera;Acorus_americanus" --gsmap gene_species.map --plotkde
 ```
 
+![](data/Raw_Orthologues_Compare_rate.ksd.svg)
+
+As displayed above, the orthologous *K*<sub>S</sub> values bewteen *Aquilegia coerulea* and *Acorus americanus* has the highest mode, indicatingthe faster substitution rate of *Aquilegia coerulea* compared to *Protea cynaroides* and *Vitis vinifera*.
+
 Note that a necessary gene-species map file is needed for its implementation in `wgd viz`, which should be automately produced by the last `wgd ksd` step. The `gene_species.map` has contents as below in which each line is the joined string of gene name and species name by space.
 
 ```
 Aqcoe6G057800.1 Aquilegia_coerulea
 Vvi_VIT_201s0011g01530.1 Vitis_vinifera
 Pcy_Procy01g08510 Protea_cynaroides
 Aam_Acora.04G142900.1 Acorus_americanus
 ```
 
+A more complex plot can be made by add the flag `--plotelmm` such that the ELMM mixture modeling of provided paranome *K*<sub>S</sub> can be superimposed, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Corrected.ksd.svg)
+
+From the mixed *K*<sub>S</sub> plot above, we can see that the optimized lognormal component b with mode 1.2 is younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera* (1.39 and 1.47, respectively).
+
+Besides, we can also add the GMM mixture modeling of anchor *K*<sub>S</sub> values with the flag `--plotapgmm`, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotapgmmm
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Apgmm_Corrected.ksd.svg)
+
+As manifested above, the anchor *K*<sub>S</sub> component 2 with mode 1.28 is also younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera*. But we need to be of course cautious that such distinction comes with the uncertainties introduced from the applied mixture modeling methodology in terms of for instance different initialization points and the issue of overfitting and the sister speciess adopted in that there might be species with more disparate substitution rates than the one we chose.
+
 An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
 
 ```
 wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
 ```
 
 Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
@@ -477,18 +518,18 @@
 wgd ksd wgd_ortho/Orthogroups.sp.tsv -sp speciestree.nw --reweight -o wgd_ortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
 ```
 
 ![](data/Aquilegia_coerulea_OrthoKs_Corrected.ksd.svg)
 
 As shown above, the number of both paralogous gene pairs and orthologous gene pairs is different than the one from global MRBH family in that here we plotted all orthologous gene pairs instead of only global MRBH and potentially new paralogous gene pairs might be produced in the orthogroup inference step, together with different recalculated weights.
 
-If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
+If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, as we have already shown above, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
 
 ```
-wgd ksd wgd_globalmrbh/global_MRBH.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus"
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --gsmap gene_species.map
 ```
 
 We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
 ![](data/Raw_Orthologues.ksd.svg)
 
 ## Citation
```

### Comparing `wgd-2.0.14/cli.py` & `wgd-2.0.15/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,14 +313,15 @@
 @click.option('--weights_outliers_included','-ic', is_flag=True,
     help="include Ks outliers")
 @click.option('--method', '-m', type=click.Choice(['gmm', 'bgmm']), default='gmm', show_default=True, help="mixture modeling method")
 @click.option('--seed',type=int, default=2352890, show_default=True, help="random seed given to initialize parameters")
 @click.option('--em_iter', '-ei',type=int, default=200, show_default=True, help="number of EM iterations to perform")
 @click.option('--n_init', '-ni',type=int, default=200, show_default=True, help="number of initializations to perform")
 @click.option('--components', '-n', nargs=2, default=(1, 4), show_default=True, help="range of number of components to fit")
+@click.option('--gamma', '-g', default=1e-3, show_default=True, help='gamma parameter for bgmm models')
 @click.option('--boots', type=int, default=200, show_default=True, help="number of bootstrap replicates of kde")
 @click.option('--weighted', is_flag=True,help="node-weighted instead of node-averaged method")
 @click.option('--plot', '-p', type=click.Choice(['stacked', 'identical']), default='identical', show_default=True, help="plotting method")
 @click.option('--bw_method', '-bm', type=click.Choice(['silverman', 'ISJ']), default='silverman', show_default=True, help="bandwidth method")
 @click.option('--n_medoids', type=int, default=2, show_default=True, help="number of medoids to generate")
 @click.option('--kdemethod', '-km', type=click.Choice(['scipy', 'naivekde', 'treekde', 'fftkde']), default='scipy', show_default=True, help="kde method")
 @click.option('--n_clusters',type=int, default=5, show_default=True, help="number of clusters to plot Elbow loss function")
@@ -337,15 +338,15 @@
 @click.option('--kscutoff', '-kc', default=5, show_default=True, type=float, help='Ks Saturation cutoff for genes in Dating')
 def peak(**kwargs):
     """
     Infer peak and CI of Ks distribution.
     """
     _peak(**kwargs)
 
-def _peak(ks_distribution, anchorpoints, outdir, alignfilter, ksrange, bin_width, weights_outliers_included, method, seed, em_iter, n_init, components, boots, weighted, plot, bw_method, n_medoids, kdemethod, n_clusters, kmedoids, guide, prominence_cutoff, kstodate, family, rel_height, ci,manualset,segments,hdr,heuristic,listelements,multipliconpairs,kscutoff):
+def _peak(ks_distribution, anchorpoints, outdir, alignfilter, ksrange, bin_width, weights_outliers_included, method, seed, em_iter, n_init, components, boots, weighted, plot, bw_method, n_medoids, kdemethod, n_clusters, kmedoids, guide, prominence_cutoff, kstodate, family, rel_height, ci,manualset,segments,hdr,heuristic,listelements,multipliconpairs,kscutoff,gamma):
     from wgd.peak import alnfilter, group_dS, log_trans, fit_gmm, fit_bgmm, add_prediction, bootstrap_kde, default_plot, get_kde, draw_kde_CI, draw_components_kde_bootstrap, fit_kmedoids, default_plot_kde, fit_apgmm_guide, fit_apgmm_ap, find_apeak, find_mpeak, retreive95CI, formatv2
     from wgd.core import _mkdir
     outpath = _mkdir(outdir)
     ksdf = pd.read_csv(ks_distribution,header=0,index_col=0,sep='\t')
     ksdf = formatv2(ksdf)
     if len(ksdf.columns) <4:
         logging.info("Begin to analyze peak of WGD dates")
@@ -358,28 +359,28 @@
         exit()
     fn_ksdf, weight_col = group_dS(ksdf_filtered)
     train_in = log_trans(fn_ksdf)
     if anchorpoints!= None:
         if kmedoids:
             df_ap = fit_kmedoids(guide, anchorpoints, boots, kdemethod, bin_width, weighted, ksdf, ksdf_filtered, outdir, seed, n_medoids, em_iter=em_iter, plot=plot, n_kmedoids = n_clusters, segment = segments, multipliconpairs=multipliconpairs,listelement=listelements)
         else:
-            df_ap_mp = fit_apgmm_guide(hdr,guide,anchorpoints,ksdf,ksdf_filtered,seed,components,em_iter,n_init,outdir,method,weighted,plot,segment=segments,multipliconpairs=multipliconpairs,listelement=listelements,cutoff = kscutoff)
-            df_ap = fit_apgmm_ap(hdr,anchorpoints,ksdf_filtered,seed,components,em_iter,n_init,outdir,method,weighted,plot)
+            df_ap_mp = fit_apgmm_guide(hdr,guide,anchorpoints,ksdf,ksdf_filtered,seed,components,em_iter,n_init,outdir,method,gamma,weighted,plot,segment=segments,multipliconpairs=multipliconpairs,listelement=listelements,cutoff = kscutoff)
+            df_ap = fit_apgmm_ap(hdr,anchorpoints,ksdf_filtered,seed,components,em_iter,n_init,outdir,method,gamma,weighted,plot)
         if heuristic:
             find_apeak(df_ap,anchorpoints,os.path.basename(ks_distribution),outdir,peak_threshold=prominence_cutoff,na=False,rel_height=rel_height,ci=ci,user_low=kstodate[0],user_upp=kstodate[1],user=manualset)
             find_apeak(df_ap,anchorpoints,os.path.basename(ks_distribution),outdir,peak_threshold=prominence_cutoff,na=True,rel_height=rel_height,ci=ci,user_low=kstodate[0],user_upp=kstodate[1],user=manualset)
             find_mpeak(df_ap_mp,anchorpoints,os.path.basename(ks_distribution),outdir,guide,peak_threshold=prominence_cutoff,rel_height=rel_height,ci=ci,user_low=kstodate[0],user_upp=kstodate[1],user=manualset)
         logging.info('Done')
         exit()
     get_kde(kdemethod,outdir,fn_ksdf,ksdf_filtered,weighted,ksrange[0],ksrange[1])
     if method == 'gmm':
         out_file = os.path.join(outdir, "AIC_BIC.pdf")
         models, aic, bic, besta, bestb, N = fit_gmm(out_file, train_in, seed, components[0], components[1], em_iter=em_iter, n_init=n_init)
     if method == 'bgmm':
-        models, N = fit_bgmm(train_in, seed, components[0], components[1], em_iter=em_iter, n_init=n_init)
+        models, N = fit_bgmm(train_in, seed, gamma, components[0], components[1], em_iter=em_iter, n_init=n_init)
     for n, m in zip(N,models):
         fname = os.path.join(outpath, "Ks_{0}_{1}components_prediction.tsv".format(method,n))
         ksdf_predict = add_prediction(ksdf,fn_ksdf,train_in,m)
         ksdf_predict.to_csv(fname,header=True,index=True,sep='\t')
         logging.info("Plotting components-annotated Ks distribution for {} components model".format(n))
         #fig = default_plot(ksdf_predict, title=os.path.basename(fname), bins=50, ylabel="Duplication events", nums = int(n),plot = plot)
         #fig.savefig(fname + "_Ks.svg")
@@ -423,14 +424,16 @@
 @click.option('--spair', '-sr', multiple=True, default=None, show_default=True,help='species pair to be plotted')
 @click.option('--speciestree', '-sp', default=None, show_default=True,help='species tree to perform rate correction')
 @click.option('--reweight', '-rw', is_flag=True, help='recalculate the weight per species pair')
 @click.option('--onlyrootout', '-or', is_flag=True, help='only consider the outgroup at root')
 @click.option('--extraparanomeks', '-epk', default=None, help='extra paranome ks data')
 @click.option('--anchorpoints', '-ap', default=None, show_default=True, help='anchorpoints.txt file')
 @click.option('--plotkde', '-pk', is_flag=True, help='plot kde curve over histogram')
+@click.option('--plotapgmm', '-pag', is_flag=True, help='plot mixture modeling of anchor pairs')
+@click.option('--components', '-n', nargs=2, default=(1, 4), show_default=True, help="range of number of components to fit")
 def ksd(**kwargs):
     """
     Paranome and one-to-one ortholog Ks distribution inference pipeline.
 
     Example 1 - whole-paranome:
 
         wgd ksd families.mcl cds.fasta
@@ -441,15 +444,15 @@
 
     If you want to keep intermediate (temporary) files, please provide a directory
     name for the `--tmpdir` option.
     """
     _ksd(**kwargs)
 
 def _ksd(families, sequences, outdir, tmpdir, nthreads, to_stop, cds, pairwise,
-        strip_gaps, tree_method,spair, speciestree, reweight, onlyrootout, extraparanomeks, anchorpoints, plotkde):
+        strip_gaps, tree_method,spair, speciestree, reweight, onlyrootout, extraparanomeks, anchorpoints, plotkde, plotapgmm, components):
     from wgd.core import get_gene_families, SequenceData, KsDistributionBuilder
     from wgd.core import read_gene_families, merge_seqs
     from wgd.viz import default_plot, apply_filters,multi_sp_plot
     start = timer()
     if tmpdir != None and not os.path.isdir(tmpdir): os.mkdir(tmpdir)
     if len(sequences) == 0: 
         logging.error("Please provide at least one sequence file")
@@ -476,15 +479,15 @@
     logging.info("Making plots")
     df = apply_filters(ksdb.df, [("dS", 0., 5.)])
     ylabel = "Duplications"
     if len(sequences) == 2:
         ylabel = "RBH orthologs"
     elif len(sequences) > 2:
         ylabel = "Homologous pairs"
-    if len(spair)!= 0:  multi_sp_plot(df,spair,spgenemap,outdir,onlyrootout,title=prefix,ylabel=ylabel,ksd=True,reweight=reweight,sptree=speciestree,extraparanomeks=extraparanomeks, ap = anchorpoints,plotkde=plotkde)
+    if len(spair)!= 0:  multi_sp_plot(df,spair,spgenemap,outdir,onlyrootout,title=prefix,ylabel=ylabel,ksd=True,reweight=reweight,sptree=speciestree,extraparanomeks=extraparanomeks, ap = anchorpoints,plotkde=plotkde,plotapgmm=plotapgmm,components=components)
     fig = default_plot(df, title=prefix, bins=50, ylabel=ylabel)
     fig.savefig(os.path.join(outdir, "{}.ksd.svg".format(prefix)))
     fig.savefig(os.path.join(outdir, "{}.ksd.pdf".format(prefix)))
     plt.close()
     if tmpdir is None:
         [x.remove_tmp(prompt=False) for x in seqs]
     end = timer()
@@ -510,21 +513,24 @@
 @click.option('--anchorpoints', '-ap', default=None, show_default=True, help='anchorpoints.txt file')
 @click.option('--multiplicon', '-mt', default=None, show_default=True, help='multiplicons.txt file')
 @click.option('--genetable', '-gt', default=None, show_default=True, help='gene-table.csv file')
 @click.option('--rel_height', '-rh', type=float, default=0.4, show_default=True, help='relative height at which the peak width is measured')
 @click.option('--minseglen', '-mg', default=10000, show_default=True, help="minimum length (ratio if <=1) of segments to show in marco-synteny")
 @click.option('--keepredun', '-kr', is_flag=True, help='keep redundant multiplicons')
 @click.option('--extraparanomeks', '-epk', default=None, help='extra paranome ks data')
+@click.option('--plotapgmm', '-pag', is_flag=True, help='plot mixture modeling of anchor pairs')
+@click.option('--plotelmm', '-pem', is_flag=True, help='plot elmm mixture modeling')
+@click.option('--components', '-n', nargs=2, default=(1, 4), show_default=True, help="range of number of components to fit")
 def viz(**kwargs):
     """
     Visualization of Ks distribution or synteny
     """
     _viz(**kwargs)
 
-def _viz(datafile,spair,outdir,gsmap,plotkde,reweight,em_iterations,em_initializations,prominence_cutoff,segments,minlen,maxsize,anchorpoints,multiplicon,genetable,rel_height,speciestree,onlyrootout,minseglen,keepredun,extraparanomeks):
+def _viz(datafile,spair,outdir,gsmap,plotkde,reweight,em_iterations,em_initializations,prominence_cutoff,segments,minlen,maxsize,anchorpoints,multiplicon,genetable,rel_height,speciestree,onlyrootout,minseglen,keepredun,extraparanomeks,plotapgmm,plotelmm,components):
     from wgd.viz import elmm_plot, apply_filters, multi_sp_plot, default_plot,all_dotplots,filter_by_minlength
     from wgd.core import _mkdir
     from wgd.syn import get_anchors,get_multi,get_segments_profile
     if datafile!=None: prefix = os.path.basename(datafile)
     _mkdir(outdir)
     if datafile ==None:
         table = pd.read_csv(genetable,header=0,index_col=0,sep=',')
@@ -537,15 +543,15 @@
             v.savefig(os.path.join(outdir, "{}.dot.pdf".format(k)))
             v.savefig(os.path.join(outdir, "{}.dot.png".format(k)))
         logging.info('Done')
         exit()
     ksdb_df = pd.read_csv(datafile,header=0,index_col=0,sep='\t')
     df = apply_filters(ksdb_df, [("dS", 0., 5.)])
     ylabel = "Duplications" if spair == () else "Homologous pairs"
-    if len(spair)!= 0: multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title=prefix,ylabel=ylabel,viz=True,plotkde=plotkde,reweight=reweight,sptree=speciestree,ap = anchorpoints, extraparanomeks=extraparanomeks)
+    if len(spair)!= 0: multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title=prefix,ylabel=ylabel,viz=True,plotkde=plotkde,reweight=reweight,sptree=speciestree,ap = anchorpoints, extraparanomeks=extraparanomeks,plotapgmm=plotapgmm,plotelmm=plotelmm,components=components,max_EM_iterations=em_iterations,num_EM_initializations=em_initializations,peak_threshold=prominence_cutoff,rel_height=rel_height)
     fig = default_plot(df, title=prefix, bins=50, ylabel=ylabel)
     fig.savefig(os.path.join(outdir, "{}.ksd.svg".format(prefix)))
     fig.savefig(os.path.join(outdir, "{}.ksd.pdf".format(prefix)))
     plt.close()
     if spair == ():
         logging.info('Exponential-Lognormal mixture modeling on node-weighted Ks distribution')
         elmm_plot(df,prefix,outdir,max_EM_iterations=em_iterations,num_EM_initializations=em_initializations,peak_threshold=prominence_cutoff,rel_height=rel_height)
```

### Comparing `wgd-2.0.14/setup.py` & `wgd-2.0.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='wgd',
-    version='2.0.14',
+    version='2.0.15',
     packages=['wgd'],
     url='http://github.com/heche-psb/wgd',
     license='GPL',
     author='Hengchi Chen',
     author_email='heche@psb.vib-ugent.be',
     description='wgd',
     long_description=long_description,
```

### Comparing `wgd-2.0.14/test/test_core.py` & `wgd-2.0.15/test/test_core.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.14/wgd/__init__.py` & `wgd-2.0.15/wgd/__init__.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.14/wgd/beast.py` & `wgd-2.0.15/wgd/beast.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.14/wgd/cluster.py` & `wgd-2.0.15/wgd/cluster.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.14/wgd/codeml.py` & `wgd-2.0.15/wgd/codeml.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.14/wgd/core.py` & `wgd-2.0.15/wgd/core.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.14/wgd/mcmctree.py` & `wgd-2.0.15/wgd/mcmctree.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.14/wgd/mix.py` & `wgd-2.0.15/wgd/mix.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.14/wgd/peak.py` & `wgd-2.0.15/wgd/peak.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import warnings
 from KDEpy import NaiveKDE,TreeKDE,FFTKDE
 from sklearn.utils import resample
 import itertools
 import os
 from wgd.core import _mkdir
 from sklearn_extra.cluster import KMedoids
-from wgd.viz import reflect_logks,find_peak_init_parameters,get_deconvoluted_data
+from wgd.viz import reflect_logks,find_peak_init_parameters
 from io import StringIO
 from sklearn import metrics
 warnings.filterwarnings("ignore", category=np.VisibleDeprecationWarning)
 
 def alnfilter(df,weights_outliers_included, identity, aln_len, coverage, min_ks, max_ks):
     """
     Filter alignment stats and Ks
@@ -171,14 +171,15 @@
     #X = X[(X<5) & (X>0)]
     colors = cm.viridis(np.linspace(0, 1, n))
     kdesity = 100
     kde_x = np.linspace(0,5,num=bins*kdesity)
     fig, ax = plt.subplots()
     df = pd.DataFrame.from_dict({'label':labels,'dS':X})
     for i,color in enumerate(colors):
+        # here I recover the std by sqrt
         mean,std,weight = means[i][0],np.sqrt(stds[i][0][0]),weights[i]
         df_comp = df[df['label']==i]
         x = np.array(list(df_comp['dS']))
         y = x[np.isfinite(x)]
         Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, alpha=0.5, rwidth=0.8, label = "component {}".format(i))
         CHF = get_totalH(Hs)
         scaling = CHF*0.1
@@ -229,15 +230,16 @@
 
 def plot_ak_component(df,nums,bins=50,plot = 'identical',ylabel="Duplication events",weighted=True,regime='multiplicon'):
     colors = cm.viridis(np.linspace(0, 1, nums))
     fig, ax = plt.subplots()
     if plot == 'identical':
         if weighted:
             for num,color in zip(range(nums),colors):
-                if nums == 1: df_comp = df.drop_duplicates(subset=['family','node'])
+                if nums == 1: df_comp = df
+                #if nums == 1: df_comp = df.drop_duplicates(subset=['family','node'])
                 else: df_comp = df[df['AnchorKs_GMM_Component']==num]
                 w = df_comp['weightoutlierexcluded']
                 x = np.array(list(df_comp['dS']))
                 y = x[np.isfinite(x)]
                 w = w[np.isfinite(x)]
                 ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, weights=w, alpha=0.5, rwidth=0.8, label = "component {}".format(num))
         else:
@@ -277,14 +279,15 @@
 def plot_ak_component_lognormal(df,means,stds,weights,nums,bins=50,ylabel="Duplication events",weighted=True,regime='multiplicon'):
     colors = cm.viridis(np.linspace(0, 1, nums))
     kdesity = 100
     kde_x = np.linspace(0,5,num=bins*kdesity)
     fig, ax = plt.subplots()
     if weighted:
         for num,color in zip(range(nums),colors):
+            # here I recover the std by sqrt
             mean,std,weight = means[num][0],np.sqrt(stds[num][0][0]),weights[num]
             if nums == 1: df_comp = df.copy()
             else: df_comp = df[df['AnchorKs_GMM_Component']==num]
             w = df_comp['weightoutlierexcluded']
             x = np.array(list(df_comp['dS']))
             y = x[np.isfinite(x)]
             w = w[np.isfinite(x)]
@@ -606,14 +609,15 @@
     ksdf_predict = ksdf_reset.merge(predict_column, on = ['family','node'])
     return ksdf_predict.set_index('pair')
 
 def fit_gmm(out_file,X, seed, n1, n2, em_iter=100, n_init=1):
     """
     Compute Gaussian mixtures for different numbers of components
     """
+    # The EM algorithm can't deal with weighted data, so we're actually ignoring all the associated weights.
     N = np.arange(n1, n2 + 1)
     models = [None for i in N]
     info_table = {}
     for i in N:
         logging.info("Fitting GMM with {} components".format(i))
         models[i-n1] = mixture.GaussianMixture(n_components = i, covariance_type='full', max_iter = em_iter, n_init = n_init, random_state = seed).fit(X)
         if models[i-n1].converged_:
@@ -626,31 +630,24 @@
     logging.info("The best fitted model via AIC is with {} components".format(np.argmin(aic)+n1))
     aic_info(aic,n1)
     logging.info("The best fitted model via BIC is with {} components".format(np.argmin(bic)+n1))
     bic_info(bic,n1)
     plot_aic_bic(aic, bic, n1, n2, out_file)
     return models, aic, bic, besta, bestb, N
 
-def fit_bgmm(X, seed, n1, n2, em_iter=100, n_init=1):
+def fit_bgmm(X, seed, gamma, n1, n2, em_iter=100, n_init=1):
     """
     Variational Bayesian estimation of a Gaussian mixture
     """
     N = np.arange(n1, n2 + 1)
     models = [None for i in N]
     info_table = {}
     for i in N:
         logging.info("Fitting BGMM with {} components".format(i))
-        #'dirichlet_distribution' (can favor more uniform weights) while 'dirichlet_process' (default weight_concentration_prior_type)
-        #(using the Stick-breaking representation) seems better
-        # default weight_concentration_prior is 1/n_components
-        # default mean_precision_prior is 1
-        # default mean_prior is the mean of X
-        # default degrees_of_freedom_prior is n_features
-        # default covariance_prior is the covariance of X
-        models[i-n1] = mixture.GaussianMixture(n_components = i, covariance_type='full', max_iter = em_iter, n_init = n_init, random_state = seed).fit(X)
+        models[i-n1] = mixture.BayesianGaussianMixture(n_components = i, covariance_type='full', max_iter = em_iter, n_init = n_init, random_state = seed, weight_concentration_prior=gamma).fit(X)
         if models[i-n1].converged_:
             logging.info("Convergence reached")
         info_components(models[i-n1],i,info_table)
     return models, N
 
 def get_gaussian_kde(train_nonan, ks_lower, ks_upper, bin_width, ksdf_filtered, weight_col, weighted=False):
     #default bw_method is 'scott'
@@ -1597,29 +1594,29 @@
     #        lower_bound_indice = i
     #        break
     for (x,y) in itertools.product(np.arange(0,lower_bound_indice,1,dtype=int), np.arange(upper_bound_indice,len(sorted_in),1,dtype=int)):
         if (y-x+1) >= cutoff: candidates.append((sorted_in[y] - sorted_in[x],(x,y)))
     lower,upper = sorted(candidates, key=lambda y: y[0])[0][1][0],sorted(candidates, key=lambda y: y[0])[0][1][1]
     return sorted_in[upper],sorted_in[lower]
 
-def fit_apgmm_guide(hdr,guide,anchor,df_nofilter,dfor,seed,components,em_iter,n_init,outdir,method,weighted,plot,segment=None,multipliconpairs=None,listelement=None,cutoff=None):
+def fit_apgmm_guide(hdr,guide,anchor,df_nofilter,dfor,seed,components,em_iter,n_init,outdir,method,gamma,weighted,plot,segment=None,multipliconpairs=None,listelement=None,cutoff=None):
     if anchor == None:
         logging.error('Please provide anchorpoints.txt file for Anchor Ks GMM Clustering')
         exit(0)
     df_ap = get_anchors(anchor)
     df = get_anchor_ksd(dfor, df_ap)
     df_nofilter = df_nofilter[df_nofilter['dS']>0]
     if segment!= None:
         df = add_seg(df_nofilter,listelement,multipliconpairs,segment)
         df.to_csv(os.path.join(outdir, "Segment_Ks.tsv"),header=True,index=True,sep='\t')
     df_withindex,X = bc_group_anchor(df,regime=guide)
     X_log = np.log(X).reshape(-1, 1)
     out_file = os.path.join(outdir, "{}_Ks_GMM_AIC_BIC.pdf".format(guide))
     if method == 'gmm': models, aic, bic, besta, bestb, N = fit_gmm(out_file, X_log, seed, components[0], components[1], em_iter=em_iter, n_init=n_init)
-    if method == 'bgmm': models, N = fit_bgmm(X_log, seed, components[0], components[1], em_iter=em_iter, n_init=n_init)
+    if method == 'bgmm': models, N = fit_bgmm(X_log, seed, gamma, components[0], components[1], em_iter=em_iter, n_init=n_init)
     if components[0] == 1 and components[1] > 1:
         plot_silhouette_score(X_log,components[0]+1,components[1],[m.predict(X_log) for m in models][1:],outdir,guide+'_Ks','GMM')
         significance_test_cluster(X_log,components[0]+1,components[1],[m.predict(X_log) for m in models][1:])
     else:
         plot_silhouette_score(X_log,components[0],components[1],[m.predict(X_log) for m in models],outdir,guide+'_Ks','GMM')
         significance_test_cluster(X_log,components[0],components[1],[m.predict(X_log) for m in models])
     Losses = []
@@ -1656,26 +1653,26 @@
     for num in HDRs.keys():
         df_tmp = df_c[df_c['AnchorKs_GMM_Component']==num]
         df_tmp = df_tmp.loc[(df_tmp['dS']<=min([cutoff,HDRs[num][1]])) & (df_tmp['dS']>=HDRs[num][0]),:]
         df_tmp = df_tmp.loc[:,['gene1','gene2','dS','Segment_dS','AnchorKs_GMM_Component']].rename(columns={"gene1":"gene_x","gene2":"gene_y"})
         fname = os.path.join(outdir,"{}_guided_{}%HDR_Syntelogs_Component{}_Model{}_WGDating.tsv".format(regime,hdr,num,n))
         df_tmp.to_csv(fname,sep='\t',header=True,index=True)
 
-def fit_apgmm_ap(hdr,anchor,df,seed,components,em_iter,n_init,outdir,method,weighted,plot):
+def fit_apgmm_ap(hdr,anchor,df,seed,components,em_iter,n_init,outdir,method,gamma,weighted,plot):
     if anchor == None:
         logging.error('Please provide anchorpoints.txt file for Anchor Ks GMM Clustering')
         exit(0)
     df_ap = get_anchors(anchor)
     df = get_anchor_ksd(df, df_ap)
     df_withindex,X = df.index,getX(df,'dS')
     X_log = np.log(X).reshape(-1, 1)
     out_file = os.path.join(outdir, "Original_AnchorKs_GMM_AIC_BIC.pdf")
     logging.info("GMM modeling on Log-scale original anchor Ks data")
     if method == 'gmm': models, aic, bic, besta, bestb, N = fit_gmm(out_file, X_log, seed, components[0], components[1], em_iter=em_iter, n_init=n_init)
-    if method == 'bgmm': models, N = fit_bgmm(X_log, seed, components[0], components[1], em_iter=em_iter, n_init=n_init)
+    if method == 'bgmm': models, N = fit_bgmm(X_log, seed, gamma, components[0], components[1], em_iter=em_iter, n_init=n_init)
     if components[0] == 1 and components[1] > 1:
         plot_silhouette_score(X_log,components[0]+1,components[1],[m.predict(X_log) for m in models][1:],outdir,'Original_AnchorKs','GMM')
         significance_test_cluster(X_log,components[0]+1,components[1],[m.predict(X_log) for m in models][1:])
     else:
         plot_silhouette_score(X_log,components[0],components[1],[m.predict(X_log) for m in models],outdir,'Original_AnchorKs','GMM')
         significance_test_cluster(X_log,components[0],components[1],[m.predict(X_log) for m in models])
     Losses = []
```

### Comparing `wgd-2.0.14/wgd/syn.py` & `wgd-2.0.15/wgd/syn.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.14/wgd/utils.py` & `wgd-2.0.15/wgd/utils.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.14/wgd/viz.py` & `wgd-2.0.15/wgd/viz.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from matplotlib.patches import Rectangle
 from matplotlib.path import Path
 import matplotlib.patches as patches
 from matplotlib.pyplot import cm
 from scipy import stats,interpolate,signal
 from io import StringIO
 from Bio import Phylo
+from sklearn import mixture
 
 def node_averages(df):
     # note that this returns a df with fewer rows, i.e. one for every
     # node in the gene family trees.
     return df.groupby(["family", "node"])["dS"].mean()
 
 def node_weights(df):
@@ -191,15 +192,291 @@
     maxy_iloc = np.argmax(kde_y)
     mode = kde_x[maxy_iloc]
     return mode, max(kde_y)
 
 def reweighted(df_per):
     return 1 / df_per.groupby(["family", "node"])["dS"].transform('count')
 
-def multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title='',ylabel='',viz=False,plotkde=False,reweight=True,sptree=None,ksd=False,ap=None,extraparanomeks=None):
+def fit_gmm(out_file,X, seed, n1, n2, em_iter=100, n_init=1):
+    """
+    Compute Gaussian mixtures for different numbers of components
+    """
+    # The EM algorithm can't deal with weighted data, so we're actually ignoring all the associated weights.
+    N = np.arange(n1, n2 + 1)
+    models = [None for i in N]
+    info_table = {}
+    for i in N:
+        logging.info("Fitting GMM with {} components".format(i))
+        models[i-n1] = mixture.GaussianMixture(n_components = i, covariance_type='full', max_iter = em_iter, n_init = n_init, random_state = seed).fit(X)
+        if models[i-n1].converged_:
+            logging.info("Convergence reached")
+        info_components(models[i-n1],i,info_table)
+    aic = [m.aic(X) for m in models]
+    bic = [m.bic(X) for m in models]
+    besta = models[np.argmin(aic)]
+    bestb = models[np.argmin(bic)]
+    logging.info("The best fitted model via AIC is with {} components".format(np.argmin(aic)+n1))
+    aic_info(aic,n1)
+    logging.info("The best fitted model via BIC is with {} components".format(np.argmin(bic)+n1))
+    bic_info_wgd(bic,n1)
+    plot_aic_bic(aic, bic, n1, n2, out_file)
+    return models, aic, bic, besta, bestb, N
+
+def fit_bgmm(X, seed, gamma, n1, n2, em_iter=100, n_init=1):
+    """
+    Variational Bayesian estimation of a Gaussian mixture
+    """
+    N = np.arange(n1, n2 + 1)
+    models = [None for i in N]
+    info_table = {}
+    for i in N:
+        logging.info("Fitting BGMM with {} components".format(i))
+        models[i-n1] = mixture.BayesianGaussianMixture(n_components = i, covariance_type='full', max_iter = em_iter, n_init = n_init, random_state = seed, weight_concentration_prior=gamma).fit(X)
+        if models[i-n1].converged_:
+            logging.info("Convergence reached")
+        info_components(models[i-n1],i,info_table)
+    return models, N
+
+def info_components(m,i,info_table):
+    means = []
+    covariances = []
+    weights = []
+    precisions = []
+    stds = []
+    for j in range(i):
+        mean = np.exp(m.means_[j][0])
+        covariance = m.covariances_[j][0][0]
+        std = np.sqrt(covariance)
+        weight = m.weights_[j]
+        precision = m.precisions_[j][0][0]
+        means.append(mean)
+        covariances.append(covariance)
+        stds.append(std)
+        weights.append(weight)
+        precisions.append(precision)
+        logging.info("Component {0} has mean {1:.3f} ,std {2:.3f} ,weight {3:.3f}, precision {4:.3f}".format(j+1,mean,std,weight,precision))
+    info_table['{}component'.format(i)] = {'mean':means,'covariance':covariances,'weight':weights,'precision':precisions,'stds':stds}
+
+def aic_info(aic,n1):
+    besta_loc = np.argmin(aic)
+    logging.info("Rules-of-thumb (Burnham & Anderson, 2002) compares the AIC-best model and remaining:")
+    for i, aic_i in enumerate(aic):
+        if i != besta_loc:
+            ABS = abs(aic[besta_loc] - aic_i)
+            if ABS <= 2:
+                logging.info("model with {} components also gets substantial support comparing to the AIC-best model".format(i+n1))
+            elif 2<ABS<4:
+                logging.info("model with {} components gets not-so-trivial support comparing to the AIC-best model".format(i+n1))
+            elif 4<=ABS<=7:
+                logging.info("model with {} components gets considerably less support comparing to the AIC-best model".format(i+n1))
+            elif 7<ABS<=10:
+                logging.info("model with {} components gets few support comparing to the AIC-best model".format(i+n1))
+            else:
+                logging.info("model with {} components gets essentially no support comparing to the AIC-best model".format(i+n1))
+
+def bic_info_wgd(bic,n1):
+    bestb_loc = np.argmin(bic)
+    logging.info("Rules-of-thumb (Kass & Raftery, 1995) evaluates the outperformance of the BIC-best model over remaining:")
+    for i, bic_i in enumerate(bic):
+        if i != bestb_loc:
+            ABS = abs(bic[bestb_loc] - bic_i)
+            if ABS < 2:
+                logging.info("Such outperformance is not worth more than a bare mention for model with {} components".format(i+n1))
+            elif 2<=ABS<6:
+                logging.info("Such outperformance is positively evidenced for model with {} components".format(i+n1))
+            elif 6<=ABS<=10:
+                logging.info("Such outperformance is strongly evidenced for model with {} components".format(i+n1))
+            else:
+                logging.info("Such outperformance is very strongly evidenced for model with {} components".format(i+n1))
+
+def plot_aic_bic(aic, bic, n1, n2, out_file):
+    x_range = list(range(n1, n2 + 1))
+    fig, axes = plt.subplots(1, 2, figsize=(12, 3))
+    axes[0].plot(np.arange(1, len(aic) + 1), aic, color='k', marker='o')
+    axes[0].set_xticks(list(range(1, len(aic) + 1)))
+    axes[0].set_xticklabels(x_range)
+    axes[0].grid(ls=":")
+    axes[0].set_ylabel("AIC")
+    axes[0].set_xlabel("# components")
+    axes[1].plot(np.arange(1, len(bic) + 1), bic, color='k', marker='o')
+    axes[1].set_xticks(list(range(1, len(bic) + 1)))
+    axes[1].set_xticklabels(x_range)
+    axes[1].grid(ls=":")
+    axes[1].set_ylabel("BIC")
+    axes[1].set_xlabel("# components")
+    fig.tight_layout()
+    fig.savefig(out_file)
+    plt.close()
+
+def addapgmm(ax,X,W,components,outdir,Hs):
+    kde_x = np.linspace(0,5,num=5000)
+    X_log = np.log(np.array(X)).reshape(-1, 1)
+    aic_bic_fplot = os.path.join(outdir,"AIC_BIC.pdf")
+    models, aic, bic, besta, bestb, N = fit_gmm(aic_bic_fplot, X_log, 2352890, components[0], components[1], em_iter=200, n_init=200)
+    means,covariances,weights = besta.means_,besta.covariances_,besta.weights_
+    CHF = get_totalH(Hs)
+    scaling = CHF*0.1
+    cs = cm.tab20b(np.linspace(0, 1, len(weights)))
+    for num in range(len(weights)):
+        mean,std,weight = means[num][0],np.sqrt(covariances[num][0][0]),weights[num]
+        ax.plot(kde_x,scaling*weight*stats.lognorm.pdf(kde_x, scale=np.exp(mean),s=std), c=cs[num], ls='-', lw=1, alpha=0.8, label='Anchor Ks component {} mode {:.2f}'.format(num+1,np.exp(mean - std**2)))
+    return ax
+
+def addelmm(ax,df,max_EM_iterations=200,num_EM_initializations=200,peak_threshold=0.1,rel_height=0.4):
+    df = df.dropna(subset=['dS','weightoutlierexcluded'])
+    df = df.loc[(df['dS']>0) & (df['dS']<5),:]
+    ks_or = np.array(df['dS'])
+    w = np.array(df['weightoutlierexcluded'])
+    deconvoluted_data = get_deconvoluted_data(ks_or,w)
+    hist_property = np.histogram(ks_or, weights=w, bins=50, density=True)
+    init_lambd = hist_property[0][0]
+    ks = np.log(ks_or)
+    max_ks,min_ks = ks.max(),ks.min()
+    ks_refed,cutoff,w_refed = reflect_logks(ks,w)
+    kde = stats.gaussian_kde(ks_refed, bw_method="scott", weights=w_refed)
+    bw_modifier = 0.4
+    kde.set_bandwidth(kde.factor * bw_modifier)
+    kde_x = np.linspace(min_ks-cutoff, max_ks+cutoff,num=500)
+    kde_y = kde(kde_x)
+    spl = interpolate.UnivariateSpline(kde_x, kde_y)
+    spl.set_smoothing_factor(0.01)
+    spl_x = np.linspace(min_ks, max_ks+0.1, num=int(round((abs(min_ks) + (max_ks+0.1)) *100)))
+    spl_y = spl(spl_x)
+    peaks, properties = signal.find_peaks(spl_y)
+    prominences = signal.peak_prominences(spl_y, peaks)[0]
+    prominences_refed_R1,width_refed_R1,prominences_refed_L1,width_refed_L1 = [],[],[],[]
+    for i in range(len(peaks)):
+        peak_index = peaks[i]
+        spl_peak_refl_y = np.concatenate((np.flip(spl_y[peak_index+1:]), spl_y[peak_index:]))
+        spl_peak_refl_x = np.concatenate((np.flip(spl_x[peak_index+1:] * -1 + 2 * spl_x[peak_index]), spl_x[peak_index:]))
+        current_peak_index = int((len(spl_peak_refl_x)-1)/2)
+        new_prominences = signal.peak_prominences(spl_peak_refl_y,[current_peak_index])[0][0]
+        new_width,new_height,left_ips,right_ips = signal.peak_widths(spl_peak_refl_y, [current_peak_index], rel_height=rel_height)
+        if new_width[0] > 150: new_width[0] = 150
+        prominences_refed_R1.append(new_prominences)
+        width_refed_R1.append(new_width[0])
+        c = "r" if new_prominences >= peak_threshold else 'gray'
+        w = new_width[0]/2/100
+        spl_peak_refl_y_L = np.concatenate((spl_y[:peak_index+1], np.flip(spl_y[:peak_index])))
+        spl_peak_refl_x_L = np.concatenate((spl_x[:peak_index+1], np.flip(spl_x[:peak_index]) * -1 + 2*spl_x[peak_index]))
+        current_peak_index = int((len(spl_peak_refl_x_L)-1)/2)
+        new_prominences = signal.peak_prominences(spl_peak_refl_y_L,[current_peak_index])[0][0]
+        new_width,new_height,left_ips,right_ips = signal.peak_widths(spl_peak_refl_y_L, [current_peak_index], rel_height=rel_height)
+        if new_width[0] > 150: new_width[0] = 150
+        prominences_refed_L1.append(new_prominences)
+        width_refed_L1.append(new_width[0])
+        c = "r" if new_prominences >= peak_threshold else 'gray'
+        w = new_width[0]/2/100
+    good_peaks_R1,good_peaks_L1 = [i>=peak_threshold for i in prominences_refed_R1],[i>=peak_threshold for i in prominences_refed_L1]
+    good_prominences,init_means,init_stdevs = [],[],[]
+    for i in range(len(peaks)):
+        if good_peaks_R1[i] or good_peaks_L1[i]:
+            init_means.append(spl_x[peaks[i]])
+            best = np.argmax((prominences_refed_R1[i], prominences_refed_L1[i]))
+            good_prominences.append(max([prominences_refed_R1[i], prominences_refed_L1[i]]))
+            width = [width_refed_R1[i], width_refed_L1[i]][best]
+            init_stdevs.append(width/2/100)
+    reduced_gaussians = False
+    if len(init_stdevs) > 4:
+        sor_by_prom = [(m,s) for m,s,_ in sorted(zip(init_means,init_stdevs,good_prominences), key=lambda y: y[2])]
+        init_means,init_stdevs = [i for i,j in sor_by_prom[:4]],[j for i,j in sor_by_prom[:4]]
+        reduced_gaussians = True
+        logging.info('Too many peak signals detected among which only 4 with highest prominences are retained')
+    buffer_maxks,buffer_std = 5,0.3
+    logging.info('An extra buffer lognormal component with mean {:.2f} and std 0.30 is appended'.format(buffer_maxks))
+    init_means.append(np.log(buffer_maxks))
+    init_stdevs.append(buffer_std)
+    logging.info('Found {} likely peak signals'.format(len(init_means)))
+    for m,s in zip(init_means,init_stdevs): logging.info('The initiative means and stds is {:.2f} {:.2f}'.format(np.exp(m),s))
+    num_comp = len(init_means)+1
+    init_weights = [1/num_comp] * num_comp
+    all_models_init_parameters,bic_dict,all_models_fitted_parameters = {},{},{}
+    all_models_init_parameters['Model1'] = [init_means, init_stdevs, init_lambd, init_weights]
+    num_comp = len(init_means) + 1
+    logging.info("Performing EM algorithm from initializated data (Model1)")
+    bic, new_means, new_stdevs, new_lambd, new_weights, convergence = EM_step(num_comp,deconvoluted_data,init_means, init_stdevs, init_lambd, init_weights,max_EM_iterations=max_EM_iterations,max_num_comp = 5, reduced_gaussians_flag=reduced_gaussians)
+    #if convergence: logging.info('The EM algorithm has reached convergence')
+    #else: logging.info("The EM algorithm hasn't reached convergence")
+    all_models_fitted_parameters['Model1'] = [new_means, new_stdevs, new_lambd, new_weights]
+    bic_dict['Model1'] = bic
+    logging.info('BIC of Model1: {:.2f}'.format(bic))
+    bic_from_same_num_comp,start_parameters,final_parameters = [],[],[]
+    logging.info("Performing EM algorithm from initializated data plus a random lognormal component (Model2)")
+    for i in range(num_EM_initializations):
+        if len(init_means) > 4:
+            updated_means,updated_stdevs = init_means[:4]+[init_means[-1]],init_stdevs[:4]+init_stdevs[-1]
+            reduced_gaussians = True
+        else:
+            updated_means,updated_stdevs = init_means.copy(), init_stdevs.copy()
+            reduced_gaussians = False
+        updated_means.append(round(np.random.choice(np.arange(-0.5, 1, 0.1)), 1))
+        updated_stdevs.append(round(np.random.choice(np.arange(0.3, 0.9, 0.1)), 1))
+        num_comp = len(updated_means) + 1
+        updated_weights = [1/num_comp] * num_comp
+        start_parameters.append([updated_means, updated_stdevs, init_lambd, updated_weights])
+        bic, new_means, new_stdevs, new_lambd, new_weights, convergence = EM_step(num_comp,deconvoluted_data,updated_means, updated_stdevs, init_lambd, updated_weights,max_EM_iterations=max_EM_iterations,max_num_comp = 5, reduced_gaussians_flag=reduced_gaussians)
+        bic_from_same_num_comp.append(bic)
+        final_parameters.append([new_means, new_stdevs, new_lambd, new_weights])
+    updated_means, updated_stdevs, init_lambd, updated_weights = start_parameters[np.argmin(bic_from_same_num_comp)]
+    all_models_init_parameters['Model2'] = [updated_means, updated_stdevs, init_lambd, updated_weights]
+    final_means, final_stdevs, final_lambd, final_weights = final_parameters[np.argmin(bic_from_same_num_comp)]
+    all_models_fitted_parameters['Model2'] = [final_means, final_stdevs, final_lambd, final_weights]
+    bic_dict['Model2'] = min(bic_from_same_num_comp)
+    logging.info('BIC of Model2 : {:.2f}'.format(min(bic_from_same_num_comp)))
+    min_num_comp,max_num_comp = 2,5
+    num_comp_list = np.arange(min_num_comp, max_num_comp + 1)
+    model_ids = num_comp_list+1
+    for num_comp, model_id in zip(num_comp_list, model_ids):
+        logging.info("Performing EM algorithm from random initialization with {0} components (Model{1})".format(num_comp,model_id))
+        bic_from_same_num_comp = []
+        start_parameters, final_parameters = [], []
+        for i in range(num_EM_initializations):
+            init_means, init_stdevs, init_weights = [], [], [1/num_comp] * num_comp
+            init_lambd = round(np.random.choice(np.arange(0.2, 1, 0.1)), 2)
+            for j in range(num_comp-2):
+                init_means.append(round(np.random.choice(np.arange(-0.5, 1, 0.01)),1))
+                init_stdevs.append(round(np.random.choice(np.arange(0.3, 0.9, 0.01)),1))
+            init_means.append(np.log(5))
+            init_stdevs.append(0.3)
+            start_parameters.append([init_means, init_stdevs, init_lambd, init_weights])
+            bic, new_means, new_stdevs, new_lambd, new_weights, convergence = EM_step(num_comp,deconvoluted_data,init_means, init_stdevs, init_lambd, init_weights,max_EM_iterations=max_EM_iterations,max_num_comp = 5)
+            bic_from_same_num_comp.append(bic)
+            final_parameters.append([new_means, new_stdevs, new_lambd, new_weights])
+        init_means, init_stdevs, init_lambd, init_weights = start_parameters[np.argmin(bic_from_same_num_comp)]
+        all_models_init_parameters["Model{}".format(model_id)] = [init_means, init_stdevs, init_lambd, init_weights]
+        final_means, final_stdevs, final_lambd, final_weights = final_parameters[np.argmin(bic_from_same_num_comp)]
+        all_models_fitted_parameters["Model{}".format(model_id)] = [final_means, final_stdevs, final_lambd, final_weights]
+        bic_dict["Model{}".format(model_id)] = min(bic_from_same_num_comp)
+        logging.info('BIC of Model{} : {:.2f}'.format(model_id,min(bic_from_same_num_comp)))
+    logging.info("Models are evaluated according to BIC scores")
+    model_bic = [(k,v) for k,v in bic_dict.items()]
+    modelist, bic_list = [k for k,v in model_bic],[v for k,v in model_bic]
+    best_model_id = modelist[np.argmin(bic_list)]
+    logging.info("The best fitted model via BIC is {}".format(best_model_id))
+    bic_info(modelist, bic_list)
+    model_bic_ordered = [(k,v) for k,v in sorted(bic_dict.items(), key=lambda y:y[0])]
+    model_ordered, bic_ordered = [k for k,v in model_bic_ordered],[v for k,v in model_bic_ordered]
+    final_means, final_stdevs, final_lambd, final_weights = all_models_fitted_parameters[best_model_id]
+    bin_width = 0.1
+    scaling = 0.1 * len(deconvoluted_data[deconvoluted_data <= 5])
+    x_points = np.linspace(-5, 5, int((5 + 5) *100))
+    x_points_strictly_positive = np.linspace(0, 5, int(5 * 100))
+    total_pdf = final_weights[0] * stats.expon.pdf(x_points_strictly_positive, scale=1/final_lambd)
+    ax.plot(x_points_strictly_positive,scaling*final_weights[0]*stats.expon.pdf(x_points_strictly_positive, scale=1/final_lambd), c='g', ls='-', lw=1.5, alpha=0.8, label='Exponential optimized')
+    lognormal_peaks = {i:round(np.exp(final_means[i] - pow(final_stdevs[i], 2)), 2) for i in range(len(final_stdevs))}
+    lognormals_sorted_by_peak = [k for k,v in sorted(lognormal_peaks.items(), key=lambda y:y[1])]
+    letter_dict = dict(zip(lognormals_sorted_by_peak, [ "a", "b", "c", "d", "e", "f", "g"][:len(final_stdevs)]))
+    colors = ["b", "r", "c", "m", "k"][:len(final_stdevs)-1] + ["y"]
+    for comp, color in zip(lognormals_sorted_by_peak, colors):
+        ax.plot(x_points_strictly_positive,scaling*final_weights[comp+1]*stats.lognorm.pdf(x_points_strictly_positive, scale=np.exp(final_means[comp]),s=final_stdevs[comp]), c=color, ls='-', lw=1.5, alpha=0.8, label=f'Lognormal {letter_dict[comp]} optimized (mode {lognormal_peaks[comp]})')
+        total_pdf = total_pdf + final_weights[comp+1]*stats.lognorm.pdf(x_points_strictly_positive,scale=np.exp(final_means[comp]),s=final_stdevs[comp])
+    ax.plot(x_points_strictly_positive, scaling*total_pdf, "k-", lw=1.5, label=f'Exp-lognormal mixture model')
+    return ax
+
+def multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title='',ylabel='',viz=False,plotkde=False,reweight=True,sptree=None,ksd=False,ap=None,extraparanomeks=None,plotapgmm=False,components=(1,4),plotelmm=False,max_EM_iterations=200,num_EM_initializations=200,peak_threshold=0.1,rel_height=0.4):
     if extraparanomeks != None:
         df_para = pd.read_csv(extraparanomeks,header=0,index_col=0,sep='\t')
         df_para = apply_filters(df_para, [("dS", 0., 5.)])
         df_para["family"] = df_para["family"].apply(lambda x:"ExtraParalog_"+x)
         df = pd.concat([df,df_para])
     # I add this dropduplicates to prevent the same paralogous pair from occuring twice and also use preferentially paranome
     df = df[~df.index.duplicated(keep='last')]
@@ -233,14 +510,15 @@
         #for ax, k, f in zip(axs.flatten(), keys, funs):
         w = reweighted(df_per) if reweight else df_per['weightoutlierexcluded']
         x = df_per['dS']
         y = x[np.isfinite(x)]
         w = w[np.isfinite(x)]
         if pair in paralog_pair:
             Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=51,dtype=int)/10, weights=w, color=cs[i], alpha=0.8, rwidth=0.8,label=pair,edgecolor='black',linewidth=0.8)
+            if plotelmm: ax = addelmm(ax,df_para,max_EM_iterations=max_EM_iterations,num_EM_initializations=num_EM_initializations,peak_threshold=peak_threshold,rel_height=rel_height)
         else:
             Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=51,dtype=int)/10, weights=w, color=cs[i], alpha=0.5, rwidth=0.8,label=pair)
         if corrected_ks_spair != None:
             if pair in corrected_ks_spair.keys():
                 #since paralogous genes and orthologous genes between focus and outgroup speices have no corrected Ks data
                 ax.axvline(x = corrected_ks_spair[pair], color = cs[i], alpha = 0.8, ls = '-.', lw = 1,label = 'Corrected mode {:.2f} of {}'.format(corrected_ks_spair[pair],pair))
                 logging.info('The corrected mode of species pair {} is {:.2f}'.format(pair,corrected_ks_spair[pair]))
@@ -260,15 +538,16 @@
         df_ap = pd.read_csv(ap,header=0,index_col=0,sep='\t')
         df_ap.loc[:,"pair"] = df_ap[["gene_x", "gene_y"]].apply(lambda x: "__".join(sorted([x[0], x[1]])), axis=1)
         df_working = df_ap.set_index('pair').join(df).dropna(subset=['dS','weightoutlierexcluded'])
         w = reweighted(df_working) if reweight else df_working['weightoutlierexcluded']
         x = df_working['dS']
         y = x[np.isfinite(x)]
         w = w[np.isfinite(x)]
-        ax.hist(y, bins = np.linspace(0, 50, num=51,dtype=int)/10, weights=w, fill=False, rwidth=0.8,label='Anchor pairs',linewidth=0,hatch = '////////',edgecolor='black')
+        Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=51,dtype=int)/10, weights=w, fill=False, rwidth=0.8,label='Anchor pairs',linewidth=0,hatch = '////////',edgecolor='black')
+        if plotapgmm: ax = addapgmm(ax,y,w,components,outdir,Hs)
     ax.set_xlabel(_labels["dS"])
     #ax.legend(loc=1,fontsize=5,bbox_to_anchor=(0.95, 0.95),frameon=False)
     ax.legend(loc='center left',bbox_to_anchor=(1.0, 0.5),frameon=False)
     ax.set_ylabel(ylabel)
     ax.set_xticks([0,1,2,3,4,5])
     sns.despine(offset=1)
     if len(paralog_pair) !=0: title = 'Corrected $K_\mathrm{S}$ ' + 'distribution of {}'.format(paralog_pair[0].split('__')[0])
@@ -294,15 +573,15 @@
 
 def elmm_plot(df,sp,outdir,max_EM_iterations=200,num_EM_initializations=200,peak_threshold=0.1,na=False,rel_height=0.4):
     if na:
         df = df.drop_duplicates(subset=['family','node'])
         df = df.loc[:,['node_averaged_dS_outlierexcluded']].copy().rename(columns={'node_averaged_dS_outlierexcluded':'dS'})
         df['weightoutlierexcluded'] = 1
     df = df.dropna(subset=['dS','weightoutlierexcluded'])
-    df = df.loc[(df['dS']>0) & (df['dS']<=5),:]
+    df = df.loc[(df['dS']>0) & (df['dS']<5),:]
     ks_or = np.array(df['dS'])
     w = np.array(df['weightoutlierexcluded'])
     if na: deconvoluted_data = ks_or.copy()
     else: deconvoluted_data = get_deconvoluted_data(ks_or,w)
     hist_property = np.histogram(ks_or, weights=w, bins=50, density=True)
     init_lambd = hist_property[0][0]
     ks = np.log(ks_or)
@@ -370,16 +649,16 @@
     all_models_init_parameters,bic_dict,all_models_fitted_parameters = {},{},{}
     all_models_init_parameters['Model1'] = [init_means, init_stdevs, init_lambd, init_weights]
     plot_init_model(axes[0,0], axes[0,1],init_means, init_stdevs, init_lambd, init_weights)
     num_comp = len(init_means) + 1
     logging.info("Performing EM algorithm from initializated data (Model1)")
     bic, new_means, new_stdevs, new_lambd, new_weights, convergence = EM_step(num_comp,deconvoluted_data,init_means, init_stdevs, init_lambd, init_weights,max_EM_iterations=max_EM_iterations,max_num_comp = 5, reduced_gaussians_flag=reduced_gaussians)
     #for m,s in zip(new_means,new_stdevs): logging.info('The optimized means and stds is {:.2f} {:.2f}'.format(np.exp(m),s))
-    if convergence: logging.info('The EM algorithm has reached convergence')
-    else: logging.info("The EM algorithm hasn't reached convergence")
+    #if convergence: logging.info('The EM algorithm has reached convergence')
+    #else: logging.info("The EM algorithm hasn't reached convergence")
     all_models_fitted_parameters['Model1'] = [new_means, new_stdevs, new_lambd, new_weights]
     bic_dict['Model1'] = bic
     logging.info('BIC of Model1: {:.2f}'.format(bic))
     plot_fitted_model(axes[0,0], axes[0,1],new_means, new_stdevs, new_lambd, new_weights)
     logging.info("Performing EM algorithm from initializated data plus a random lognormal component (Model2)")
     axes[1,0].set_title("Model 2")
     bic_from_same_num_comp,start_parameters,final_parameters = [],[],[]
```

### Comparing `wgd-2.0.14/wgd.egg-info/PKG-INFO` & `wgd-2.0.15/wgd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wgd
-Version: 2.0.14
+Version: 2.0.15
 Summary: wgd
 Home-page: http://github.com/heche-psb/wgd
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -449,37 +449,67 @@
 
 ```
 wgd ksd wgd_globalmrbh/global_MRBH.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
 ```
 
 The file `speciestree.nw` is the text file of species tree in newick that rate correction would be conducted on. Its content is as below. Users need to provide the species pairs to be plotted. We suggest adding the option `--reweight` to recalculate the weight per species pair such that the weight of orthologous gene pairs will become 1 as the paralogous gene pairs. The flag `--plotkde` can be added when the kde curve of orthologous *K*<sub>S</sub> is desired. Extra collinear data can be added by the option `-ap`.
 
+```
+(((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
+```
+
 ![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
 
 As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
 
+If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+
 ```
-(((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
 ```
 
-If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+Note that we can easily show that *Aquilegia coerulea* has higher substitution rate than *Protea cynaroides* and *Vitis vinifera* by comparing their substitution distance in regard to the same divergence event with outgroup species *Acorus_americanus*, using command below.
 
 ```
-wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_viz_Compare_rate --spair "Acorus_americanus;Protea_cynaroides" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Vitis_vinifera;Acorus_americanus" --gsmap gene_species.map --plotkde
 ```
 
+![](data/Raw_Orthologues_Compare_rate.ksd.svg)
+
+As displayed above, the orthologous *K*<sub>S</sub> values bewteen *Aquilegia coerulea* and *Acorus americanus* has the highest mode, indicatingthe faster substitution rate of *Aquilegia coerulea* compared to *Protea cynaroides* and *Vitis vinifera*.
+
 Note that a necessary gene-species map file is needed for its implementation in `wgd viz`, which should be automately produced by the last `wgd ksd` step. The `gene_species.map` has contents as below in which each line is the joined string of gene name and species name by space.
 
 ```
 Aqcoe6G057800.1 Aquilegia_coerulea
 Vvi_VIT_201s0011g01530.1 Vitis_vinifera
 Pcy_Procy01g08510 Protea_cynaroides
 Aam_Acora.04G142900.1 Acorus_americanus
 ```
 
+A more complex plot can be made by add the flag `--plotelmm` such that the ELMM mixture modeling of provided paranome *K*<sub>S</sub> can be superimposed, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Corrected.ksd.svg)
+
+From the mixed *K*<sub>S</sub> plot above, we can see that the optimized lognormal component b with mode 1.2 is younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera* (1.39 and 1.47, respectively).
+
+Besides, we can also add the GMM mixture modeling of anchor *K*<sub>S</sub> values with the flag `--plotapgmm`, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotapgmmm
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Apgmm_Corrected.ksd.svg)
+
+As manifested above, the anchor *K*<sub>S</sub> component 2 with mode 1.28 is also younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera*. But we need to be of course cautious that such distinction comes with the uncertainties introduced from the applied mixture modeling methodology in terms of for instance different initialization points and the issue of overfitting and the sister speciess adopted in that there might be species with more disparate substitution rates than the one we chose.
+
 An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
 
 ```
 wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
 ```
 
 Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
@@ -488,18 +518,18 @@
 wgd ksd wgd_ortho/Orthogroups.sp.tsv -sp speciestree.nw --reweight -o wgd_ortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
 ```
 
 ![](data/Aquilegia_coerulea_OrthoKs_Corrected.ksd.svg)
 
 As shown above, the number of both paralogous gene pairs and orthologous gene pairs is different than the one from global MRBH family in that here we plotted all orthologous gene pairs instead of only global MRBH and potentially new paralogous gene pairs might be produced in the orthogroup inference step, together with different recalculated weights.
 
-If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
+If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, as we have already shown above, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
 
 ```
-wgd ksd wgd_globalmrbh/global_MRBH.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus"
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --gsmap gene_species.map
 ```
 
 We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
 ![](data/Raw_Orthologues.ksd.svg)
 
 ## Citation
```

### Comparing `wgd-2.0.14/wgd.egg-info/requires.txt` & `wgd-2.0.15/wgd.egg-info/requires.txt`

 * *Files identical despite different names*

