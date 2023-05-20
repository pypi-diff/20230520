# Comparing `tmp/jcvi-1.3.4.tar.gz` & `tmp/jcvi-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcvi-1.3.4.tar", last modified: Thu Apr 27 08:18:35 2023, max compression
+gzip compressed data, was "jcvi-1.3.5.tar", last modified: Sat May 20 02:09:56 2023, max compression
```

## Comparing `jcvi-1.3.4.tar` & `jcvi-1.3.5.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.621805 jcvi-1.3.4/
--rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.3.4/LICENSE
--rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.3.4/MANIFEST.in
--rw-r--r--   0 bao        (501) staff       (20)     8759 2023-04-27 08:18:35.621885 jcvi-1.3.4/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     8094 2021-04-18 23:59:49.000000 jcvi-1.3.4/README.md
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.589952 jcvi-1.3.4/jcvi/
--rw-r--r--   0 bao        (501) staff       (20)      770 2022-11-26 21:23:29.000000 jcvi-1.3.4/jcvi/__init__.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.592869 jcvi-1.3.4/jcvi/algorithms/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/algorithms/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      263 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/algorithms/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     6422 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/algorithms/ec.py
--rw-r--r--   0 bao        (501) staff       (20)     5678 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/algorithms/formula.py
--rw-r--r--   0 bao        (501) staff       (20)    14132 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/algorithms/graph.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6275 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/algorithms/lis.py
--rwxr-xr-x   0 bao        (501) staff       (20)    24228 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/algorithms/lpsolve.py
--rw-r--r--   0 bao        (501) staff       (20)     6104 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/algorithms/matrix.py
--rw-r--r--   0 bao        (501) staff       (20)     1296 2021-06-19 19:45:56.000000 jcvi-1.3.4/jcvi/algorithms/maxsum.py
--rw-r--r--   0 bao        (501) staff       (20)     1203 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/algorithms/ml.py
--rwxr-xr-x   0 bao        (501) staff       (20)     4999 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/algorithms/supermap.py
--rw-r--r--   0 bao        (501) staff       (20)    12559 2022-11-26 15:55:17.000000 jcvi-1.3.4/jcvi/algorithms/tsp.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.594583 jcvi-1.3.4/jcvi/annotation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/annotation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      261 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/annotation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    21414 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/ahrd.py
--rw-r--r--   0 bao        (501) staff       (20)     7899 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/automaton.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6417 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/depth.py
--rw-r--r--   0 bao        (501) staff       (20)     7042 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/evm.py
--rw-r--r--   0 bao        (501) staff       (20)    14687 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/maker.py
--rw-r--r--   0 bao        (501) staff       (20)    19485 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/pasa.py
--rw-r--r--   0 bao        (501) staff       (20)    12822 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/qc.py
--rw-r--r--   0 bao        (501) staff       (20)    42839 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/reformat.py
--rw-r--r--   0 bao        (501) staff       (20)    12645 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/stats.py
--rw-r--r--   0 bao        (501) staff       (20)     6793 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/annotation/train.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.598898 jcvi-1.3.4/jcvi/apps/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/apps/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      258 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/apps/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    16889 2023-02-19 15:03:46.000000 jcvi-1.3.4/jcvi/apps/align.py
--rw-r--r--   0 bao        (501) staff       (20)    68248 2023-04-27 08:17:23.000000 jcvi-1.3.4/jcvi/apps/base.py
--rw-r--r--   0 bao        (501) staff       (20)    12271 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/biomart.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3554 2021-06-19 19:45:56.000000 jcvi-1.3.4/jcvi/apps/blastplus.py
--rw-r--r--   0 bao        (501) staff       (20)     5219 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/bowtie.py
--rw-r--r--   0 bao        (501) staff       (20)     7695 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/bwa.py
--rw-r--r--   0 bao        (501) staff       (20)     7279 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/cdhit.py
--rw-r--r--   0 bao        (501) staff       (20)     2623 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/emboss.py
--rw-r--r--   0 bao        (501) staff       (20)    21332 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/fetch.py
--rw-r--r--   0 bao        (501) staff       (20)    19459 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/gbsubmit.py
--rw-r--r--   0 bao        (501) staff       (20)     6892 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/gmap.py
--rw-r--r--   0 bao        (501) staff       (20)    18480 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/grid.py
--rw-r--r--   0 bao        (501) staff       (20)    33945 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/ks.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7238 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/lastz.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3004 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/mask.py
--rw-r--r--   0 bao        (501) staff       (20)    35471 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/phylo.py
--rw-r--r--   0 bao        (501) staff       (20)     1896 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/r.py
--rw-r--r--   0 bao        (501) staff       (20)     4901 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/restriction.py
--rw-r--r--   0 bao        (501) staff       (20)     2116 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/apps/script.py
--rw-r--r--   0 bao        (501) staff       (20)     3784 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/softlink.py
--rw-r--r--   0 bao        (501) staff       (20)    33065 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/uclust.py
--rw-r--r--   0 bao        (501) staff       (20)     5208 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/uniprot.py
--rw-r--r--   0 bao        (501) staff       (20)     3661 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/apps/vecscreen.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.602596 jcvi-1.3.4/jcvi/assembly/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/assembly/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      257 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/assembly/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    66136 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)    15451 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/allpaths.py
--rw-r--r--   0 bao        (501) staff       (20)    13265 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/automaton.py
--rw-r--r--   0 bao        (501) staff       (20)     5544 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/base.py
--rw-r--r--   0 bao        (501) staff       (20)    34986 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/ca.py
--rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.3.4/jcvi/assembly/chic.pyx
--rw-r--r--   0 bao        (501) staff       (20)     4581 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/coverage.py
--rw-r--r--   0 bao        (501) staff       (20)     8676 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/gaps.py
--rw-r--r--   0 bao        (501) staff       (20)    20212 2023-02-19 15:03:46.000000 jcvi-1.3.4/jcvi/assembly/geneticmap.py
--rw-r--r--   0 bao        (501) staff       (20)    34693 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/goldenpath.py
--rw-r--r--   0 bao        (501) staff       (20)    57613 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/hic.py
--rw-r--r--   0 bao        (501) staff       (20)    39860 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/kmer.py
--rw-r--r--   0 bao        (501) staff       (20)    12519 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/opticalmap.py
--rw-r--r--   0 bao        (501) staff       (20)    27279 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/patch.py
--rw-r--r--   0 bao        (501) staff       (20)    15741 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/postprocess.py
--rw-r--r--   0 bao        (501) staff       (20)    23470 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/preprocess.py
--rw-r--r--   0 bao        (501) staff       (20)     6287 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/sim.py
--rw-r--r--   0 bao        (501) staff       (20)     8830 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/soap.py
--rw-r--r--   0 bao        (501) staff       (20)    16183 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/assembly/syntenypath.py
--rw-r--r--   0 bao        (501) staff       (20)     5042 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/assembly/trinity.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.604653 jcvi-1.3.4/jcvi/compara/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/compara/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      251 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/compara/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     4210 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/compara/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9796 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/compara/blastfilter.py
--rw-r--r--   0 bao        (501) staff       (20)    27413 2023-04-27 08:17:23.000000 jcvi-1.3.4/jcvi/compara/catalog.py
--rw-r--r--   0 bao        (501) staff       (20)    26355 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/compara/fractionation.py
--rw-r--r--   0 bao        (501) staff       (20)     9216 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/compara/pad.py
--rw-r--r--   0 bao        (501) staff       (20)     3051 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/compara/phylogeny.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7948 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/compara/quota.py
--rw-r--r--   0 bao        (501) staff       (20)    10341 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/compara/reconstruct.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9233 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/compara/synfind.py
--rwxr-xr-x   0 bao        (501) staff       (20)    57574 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/compara/synteny.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.609323 jcvi-1.3.4/jcvi/formats/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/formats/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      262 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/formats/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    63612 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/agp.py
--rw-r--r--   0 bao        (501) staff       (20)    33966 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    72552 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/bed.py
--rw-r--r--   0 bao        (501) staff       (20)    42610 2023-04-27 08:17:23.000000 jcvi-1.3.4/jcvi/formats/blast.py
--rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.3.4/jcvi/formats/cblast.pyx
--rw-r--r--   0 bao        (501) staff       (20)     3193 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/cdt.py
--rw-r--r--   0 bao        (501) staff       (20)     8612 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/chain.py
--rw-r--r--   0 bao        (501) staff       (20)     4644 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/contig.py
--rw-r--r--   0 bao        (501) staff       (20)    15170 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/coords.py
--rw-r--r--   0 bao        (501) staff       (20)     6529 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/excel.py
--rw-r--r--   0 bao        (501) staff       (20)    75590 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/fasta.py
--rw-r--r--   0 bao        (501) staff       (20)    29575 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/fastq.py
--rw-r--r--   0 bao        (501) staff       (20)    15549 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/genbank.py
--rw-r--r--   0 bao        (501) staff       (20)   118976 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/gff.py
--rw-r--r--   0 bao        (501) staff       (20)     3979 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/html.py
--rw-r--r--   0 bao        (501) staff       (20)     4612 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/maf.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2842 2021-07-05 22:45:00.000000 jcvi-1.3.4/jcvi/formats/obo.py
--rw-r--r--   0 bao        (501) staff       (20)     2900 2021-01-11 06:59:36.000000 jcvi-1.3.4/jcvi/formats/paf.py
--rw-r--r--   0 bao        (501) staff       (20)     2785 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/pdf.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10355 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/psl.py
--rw-r--r--   0 bao        (501) staff       (20)     2746 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/formats/pyblast.py
--rw-r--r--   0 bao        (501) staff       (20)    28231 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/sam.py
--rw-r--r--   0 bao        (501) staff       (20)     8041 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/sizes.py
--rw-r--r--   0 bao        (501) staff       (20)    25480 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/formats/vcf.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.613548 jcvi-1.3.4/jcvi/graphics/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/graphics/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      271 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/graphics/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    16271 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/align.py
--rw-r--r--   0 bao        (501) staff       (20)    15265 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/assembly.py
--rw-r--r--   0 bao        (501) staff       (20)    22166 2023-02-23 05:35:25.000000 jcvi-1.3.4/jcvi/graphics/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10006 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/blastplot.py
--rw-r--r--   0 bao        (501) staff       (20)    22427 2023-02-06 05:16:46.000000 jcvi-1.3.4/jcvi/graphics/chromosome.py
--rw-r--r--   0 bao        (501) staff       (20)     7145 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/graphics/coverage.py
--rwxr-xr-x   0 bao        (501) staff       (20)    14873 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/graphics/dotplot.py
--rw-r--r--   0 bao        (501) staff       (20)    21810 2023-02-06 05:16:46.000000 jcvi-1.3.4/jcvi/graphics/glyph.py
--rw-r--r--   0 bao        (501) staff       (20)    23626 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/grabseeds.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2379 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/graphics/graph.py
--rw-r--r--   0 bao        (501) staff       (20)     5025 2021-03-26 15:38:36.000000 jcvi-1.3.4/jcvi/graphics/heatmap.py
--rw-r--r--   0 bao        (501) staff       (20)     9612 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/histogram.py
--rw-r--r--   0 bao        (501) staff       (20)    13375 2023-02-08 03:44:09.000000 jcvi-1.3.4/jcvi/graphics/karyotype.py
--rw-r--r--   0 bao        (501) staff       (20)    31416 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/landscape.py
--rw-r--r--   0 bao        (501) staff       (20)     1276 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/graphics/logo.py
--rw-r--r--   0 bao        (501) staff       (20)     3893 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/mummerplot.py
--rw-r--r--   0 bao        (501) staff       (20)    20888 2023-02-08 03:44:09.000000 jcvi-1.3.4/jcvi/graphics/synteny.py
--rw-r--r--   0 bao        (501) staff       (20)     5488 2021-06-19 19:45:56.000000 jcvi-1.3.4/jcvi/graphics/table.py
--rw-r--r--   0 bao        (501) staff       (20)    20377 2022-11-26 16:06:34.000000 jcvi-1.3.4/jcvi/graphics/tree.py
--rw-r--r--   0 bao        (501) staff       (20)     6194 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/graphics/wheel.py
--rw-r--r--   0 bao        (501) staff       (20)     1675 2021-03-26 15:38:36.000000 jcvi-1.3.4/jcvi/graphics/whisker.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.616232 jcvi-1.3.4/jcvi/projects/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/projects/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/projects/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    22445 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/age.py
--rw-r--r--   0 bao        (501) staff       (20)     1571 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/alfalfa.py
--rw-r--r--   0 bao        (501) staff       (20)    15907 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)     6750 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/bites.py
--rw-r--r--   0 bao        (501) staff       (20)     5679 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/heterosis.py
--rw-r--r--   0 bao        (501) staff       (20)    14136 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/ies.py
--rw-r--r--   0 bao        (501) staff       (20)    22201 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/misc.py
--rw-r--r--   0 bao        (501) staff       (20)    25024 2023-02-06 05:16:46.000000 jcvi-1.3.4/jcvi/projects/napus.py
--rw-r--r--   0 bao        (501) staff       (20)    12754 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/pineapple.py
--rw-r--r--   0 bao        (501) staff       (20)     2367 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/pistachio.py
--rw-r--r--   0 bao        (501) staff       (20)    67857 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/str.py
--rw-r--r--   0 bao        (501) staff       (20)    26165 2023-04-27 08:17:23.000000 jcvi-1.3.4/jcvi/projects/sugarcane.py
--rw-r--r--   0 bao        (501) staff       (20)    23950 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/synfind.py
--rw-r--r--   0 bao        (501) staff       (20)    21554 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/projects/tgbs.py
--rw-r--r--   0 bao        (501) staff       (20)    11941 2023-04-26 05:51:28.000000 jcvi-1.3.4/jcvi/projects/vanilla.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.618577 jcvi-1.3.4/jcvi/utils/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/utils/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    24200 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/utils/aws.py
--rw-r--r--   0 bao        (501) staff       (20)    12512 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/utils/cbook.py
--rw-r--r--   0 bao        (501) staff       (20)      355 2021-01-11 02:34:49.000000 jcvi-1.3.4/jcvi/utils/console.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.620394 jcvi-1.3.4/jcvi/utils/data/
--rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/Airswing.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/Collegia.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/HookedUp.ttf
--rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/Humor-Sans.ttf
--rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/TREDs.meta.csv
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/adapters.fasta
--rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/blosum80.mat
--rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/chrY.hg38.unique_ccn.gc
--rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/colorchecker.txt
--rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/hg38.band.txt
--rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/hg38.chrom.sizes
--rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/utils/data/instance.json
--rw-r--r--   0 bao        (501) staff       (20)     9795 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/utils/db.py
--rw-r--r--   0 bao        (501) staff       (20)     4145 2021-01-09 20:22:53.000000 jcvi-1.3.4/jcvi/utils/ez_setup.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2884 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/utils/grouper.py
--rw-r--r--   0 bao        (501) staff       (20)    10437 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/utils/orderedcollections.py
--rw-r--r--   0 bao        (501) staff       (20)    14595 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/utils/range.py
--rw-r--r--   0 bao        (501) staff       (20)     3946 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/utils/table.py
--rw-r--r--   0 bao        (501) staff       (20)     4687 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/utils/taxonomy.py
--rw-r--r--   0 bao        (501) staff       (20)     1522 2021-07-13 05:06:52.000000 jcvi-1.3.4/jcvi/utils/validator.py
--rwxr-xr-x   0 bao        (501) staff       (20)     1377 2021-01-15 14:44:37.000000 jcvi-1.3.4/jcvi/utils/webcolors.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.621681 jcvi-1.3.4/jcvi/variation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.4/jcvi/variation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      259 2021-06-19 08:23:09.000000 jcvi-1.3.4/jcvi/variation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    45321 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/cnv.py
--rw-r--r--   0 bao        (501) staff       (20)     7036 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/deconvolute.py
--rw-r--r--   0 bao        (501) staff       (20)     9385 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/delly.py
--rw-r--r--   0 bao        (501) staff       (20)    11777 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/impute.py
--rw-r--r--   0 bao        (501) staff       (20)     3478 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/phase.py
--rw-r--r--   0 bao        (501) staff       (20)    10831 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/snp.py
--rw-r--r--   0 bao        (501) staff       (20)    48818 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/str.py
--rw-r--r--   0 bao        (501) staff       (20)     3672 2023-02-06 03:44:04.000000 jcvi-1.3.4/jcvi/variation/tassel.py
--rw-r--r--   0 bao        (501) staff       (20)      176 2023-04-27 08:18:35.000000 jcvi-1.3.4/jcvi/version.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-04-27 08:18:35.590801 jcvi-1.3.4/jcvi.egg-info/
--rw-r--r--   0 bao        (501) staff       (20)     8759 2023-04-27 08:18:35.000000 jcvi-1.3.4/jcvi.egg-info/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     4727 2023-04-27 08:18:35.000000 jcvi-1.3.4/jcvi.egg-info/SOURCES.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2023-04-27 08:18:35.000000 jcvi-1.3.4/jcvi.egg-info/dependency_links.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.3.4/jcvi.egg-info/not-zip-safe
--rw-r--r--   0 bao        (501) staff       (20)      206 2023-04-27 08:18:35.000000 jcvi-1.3.4/jcvi.egg-info/requires.txt
--rw-r--r--   0 bao        (501) staff       (20)        5 2023-04-27 08:18:35.000000 jcvi-1.3.4/jcvi.egg-info/top_level.txt
--rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.3.4/pyproject.toml
--rw-r--r--   0 bao        (501) staff       (20)     1219 2023-04-27 08:18:35.622240 jcvi-1.3.4/setup.cfg
--rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.3.4/setup.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.444485 jcvi-1.3.5/
+-rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.3.5/LICENSE
+-rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.3.5/MANIFEST.in
+-rw-r--r--   0 bao        (501) staff       (20)     8759 2023-05-20 02:09:56.444574 jcvi-1.3.5/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     8094 2021-04-18 23:59:49.000000 jcvi-1.3.5/README.md
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.406541 jcvi-1.3.5/jcvi/
+-rw-r--r--   0 bao        (501) staff       (20)      770 2022-11-26 21:23:29.000000 jcvi-1.3.5/jcvi/__init__.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.411054 jcvi-1.3.5/jcvi/algorithms/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/algorithms/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      263 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/algorithms/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     6422 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/algorithms/ec.py
+-rw-r--r--   0 bao        (501) staff       (20)     5678 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/algorithms/formula.py
+-rw-r--r--   0 bao        (501) staff       (20)    14132 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/algorithms/graph.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6275 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/algorithms/lis.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    24228 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/algorithms/lpsolve.py
+-rw-r--r--   0 bao        (501) staff       (20)     6104 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/algorithms/matrix.py
+-rw-r--r--   0 bao        (501) staff       (20)     1296 2021-06-19 19:45:56.000000 jcvi-1.3.5/jcvi/algorithms/maxsum.py
+-rw-r--r--   0 bao        (501) staff       (20)     1203 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/algorithms/ml.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     4999 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/algorithms/supermap.py
+-rw-r--r--   0 bao        (501) staff       (20)    12559 2022-11-26 15:55:17.000000 jcvi-1.3.5/jcvi/algorithms/tsp.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.415895 jcvi-1.3.5/jcvi/annotation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/annotation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      261 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/annotation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    21414 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/ahrd.py
+-rw-r--r--   0 bao        (501) staff       (20)     7899 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/automaton.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6417 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/depth.py
+-rw-r--r--   0 bao        (501) staff       (20)     7042 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/evm.py
+-rw-r--r--   0 bao        (501) staff       (20)    14687 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/maker.py
+-rw-r--r--   0 bao        (501) staff       (20)    19485 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/pasa.py
+-rw-r--r--   0 bao        (501) staff       (20)    12822 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/qc.py
+-rw-r--r--   0 bao        (501) staff       (20)    42839 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/reformat.py
+-rw-r--r--   0 bao        (501) staff       (20)    12645 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/stats.py
+-rw-r--r--   0 bao        (501) staff       (20)     6793 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/train.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.420105 jcvi-1.3.5/jcvi/apps/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/apps/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      258 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/apps/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    16889 2023-02-19 15:03:46.000000 jcvi-1.3.5/jcvi/apps/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    67790 2023-05-20 01:38:16.000000 jcvi-1.3.5/jcvi/apps/base.py
+-rw-r--r--   0 bao        (501) staff       (20)    12271 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/biomart.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     3554 2021-06-19 19:45:56.000000 jcvi-1.3.5/jcvi/apps/blastplus.py
+-rw-r--r--   0 bao        (501) staff       (20)     5219 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/bowtie.py
+-rw-r--r--   0 bao        (501) staff       (20)     7695 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/bwa.py
+-rw-r--r--   0 bao        (501) staff       (20)     7279 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/cdhit.py
+-rw-r--r--   0 bao        (501) staff       (20)     2623 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/emboss.py
+-rw-r--r--   0 bao        (501) staff       (20)    21332 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/fetch.py
+-rw-r--r--   0 bao        (501) staff       (20)    19459 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/gbsubmit.py
+-rw-r--r--   0 bao        (501) staff       (20)     6892 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/gmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    18476 2023-04-29 14:56:25.000000 jcvi-1.3.5/jcvi/apps/grid.py
+-rw-r--r--   0 bao        (501) staff       (20)    33945 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/ks.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7238 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/lastz.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     3004 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/mask.py
+-rw-r--r--   0 bao        (501) staff       (20)    35471 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/phylo.py
+-rw-r--r--   0 bao        (501) staff       (20)     1896 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/r.py
+-rw-r--r--   0 bao        (501) staff       (20)     4901 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/restriction.py
+-rw-r--r--   0 bao        (501) staff       (20)     2116 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/apps/script.py
+-rw-r--r--   0 bao        (501) staff       (20)     3784 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/softlink.py
+-rw-r--r--   0 bao        (501) staff       (20)    33065 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/uclust.py
+-rw-r--r--   0 bao        (501) staff       (20)     5208 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/uniprot.py
+-rw-r--r--   0 bao        (501) staff       (20)     3661 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/vecscreen.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.423678 jcvi-1.3.5/jcvi/assembly/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/assembly/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      257 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/assembly/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    66136 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    15451 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/allpaths.py
+-rw-r--r--   0 bao        (501) staff       (20)    13265 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/automaton.py
+-rw-r--r--   0 bao        (501) staff       (20)     5544 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/base.py
+-rw-r--r--   0 bao        (501) staff       (20)    34986 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/ca.py
+-rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.3.5/jcvi/assembly/chic.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     4581 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/coverage.py
+-rw-r--r--   0 bao        (501) staff       (20)     8676 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/gaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    20212 2023-02-19 15:03:46.000000 jcvi-1.3.5/jcvi/assembly/geneticmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    34693 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/goldenpath.py
+-rw-r--r--   0 bao        (501) staff       (20)    57613 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/hic.py
+-rw-r--r--   0 bao        (501) staff       (20)    43632 2023-05-05 09:23:28.000000 jcvi-1.3.5/jcvi/assembly/kmer.py
+-rw-r--r--   0 bao        (501) staff       (20)    12519 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/opticalmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    27279 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/patch.py
+-rw-r--r--   0 bao        (501) staff       (20)    15741 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/postprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)    23470 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/preprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)     6287 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/sim.py
+-rw-r--r--   0 bao        (501) staff       (20)     8830 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/soap.py
+-rw-r--r--   0 bao        (501) staff       (20)    16183 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/assembly/syntenypath.py
+-rw-r--r--   0 bao        (501) staff       (20)     5042 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/trinity.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.425737 jcvi-1.3.5/jcvi/compara/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/compara/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      251 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/compara/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     4210 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/compara/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9796 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/compara/blastfilter.py
+-rw-r--r--   0 bao        (501) staff       (20)    27460 2023-05-20 02:09:12.000000 jcvi-1.3.5/jcvi/compara/catalog.py
+-rw-r--r--   0 bao        (501) staff       (20)    26355 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/compara/fractionation.py
+-rw-r--r--   0 bao        (501) staff       (20)     9216 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/compara/pad.py
+-rw-r--r--   0 bao        (501) staff       (20)     3051 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/compara/phylogeny.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7948 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/compara/quota.py
+-rw-r--r--   0 bao        (501) staff       (20)    10341 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/compara/reconstruct.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9233 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/compara/synfind.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    57574 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/compara/synteny.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.430616 jcvi-1.3.5/jcvi/formats/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/formats/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      262 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/formats/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    63612 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/agp.py
+-rw-r--r--   0 bao        (501) staff       (20)    33966 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    72552 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/bed.py
+-rw-r--r--   0 bao        (501) staff       (20)    42967 2023-05-20 02:09:12.000000 jcvi-1.3.5/jcvi/formats/blast.py
+-rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.3.5/jcvi/formats/cblast.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     3193 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/cdt.py
+-rw-r--r--   0 bao        (501) staff       (20)     8612 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/chain.py
+-rw-r--r--   0 bao        (501) staff       (20)     4644 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/contig.py
+-rw-r--r--   0 bao        (501) staff       (20)    15170 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/coords.py
+-rw-r--r--   0 bao        (501) staff       (20)     6529 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/excel.py
+-rw-r--r--   0 bao        (501) staff       (20)    75590 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/fasta.py
+-rw-r--r--   0 bao        (501) staff       (20)    29575 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/fastq.py
+-rw-r--r--   0 bao        (501) staff       (20)    15549 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/genbank.py
+-rw-r--r--   0 bao        (501) staff       (20)   118976 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/gff.py
+-rw-r--r--   0 bao        (501) staff       (20)     3979 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/html.py
+-rw-r--r--   0 bao        (501) staff       (20)     4612 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/maf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2842 2021-07-05 22:45:00.000000 jcvi-1.3.5/jcvi/formats/obo.py
+-rw-r--r--   0 bao        (501) staff       (20)     2900 2021-01-11 06:59:36.000000 jcvi-1.3.5/jcvi/formats/paf.py
+-rw-r--r--   0 bao        (501) staff       (20)     2785 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/pdf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    10355 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/psl.py
+-rw-r--r--   0 bao        (501) staff       (20)     2746 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/formats/pyblast.py
+-rw-r--r--   0 bao        (501) staff       (20)    28231 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/sam.py
+-rw-r--r--   0 bao        (501) staff       (20)     8041 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/sizes.py
+-rw-r--r--   0 bao        (501) staff       (20)    25480 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/vcf.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.435114 jcvi-1.3.5/jcvi/graphics/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/graphics/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      271 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/graphics/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    16271 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    15265 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/assembly.py
+-rw-r--r--   0 bao        (501) staff       (20)    22166 2023-02-23 05:35:25.000000 jcvi-1.3.5/jcvi/graphics/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    10006 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/blastplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    22427 2023-02-06 05:16:46.000000 jcvi-1.3.5/jcvi/graphics/chromosome.py
+-rw-r--r--   0 bao        (501) staff       (20)     7145 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/graphics/coverage.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    14873 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/graphics/dotplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    21810 2023-02-06 05:16:46.000000 jcvi-1.3.5/jcvi/graphics/glyph.py
+-rw-r--r--   0 bao        (501) staff       (20)    23626 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/grabseeds.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2379 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/graphics/graph.py
+-rw-r--r--   0 bao        (501) staff       (20)     5025 2021-03-26 15:38:36.000000 jcvi-1.3.5/jcvi/graphics/heatmap.py
+-rw-r--r--   0 bao        (501) staff       (20)     9612 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/histogram.py
+-rw-r--r--   0 bao        (501) staff       (20)    13375 2023-02-08 03:44:09.000000 jcvi-1.3.5/jcvi/graphics/karyotype.py
+-rw-r--r--   0 bao        (501) staff       (20)    31416 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/landscape.py
+-rw-r--r--   0 bao        (501) staff       (20)     1276 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/graphics/logo.py
+-rw-r--r--   0 bao        (501) staff       (20)     3893 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/mummerplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    20888 2023-02-08 03:44:09.000000 jcvi-1.3.5/jcvi/graphics/synteny.py
+-rw-r--r--   0 bao        (501) staff       (20)     5488 2021-06-19 19:45:56.000000 jcvi-1.3.5/jcvi/graphics/table.py
+-rw-r--r--   0 bao        (501) staff       (20)    20377 2022-11-26 16:06:34.000000 jcvi-1.3.5/jcvi/graphics/tree.py
+-rw-r--r--   0 bao        (501) staff       (20)     6194 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/wheel.py
+-rw-r--r--   0 bao        (501) staff       (20)     1675 2021-03-26 15:38:36.000000 jcvi-1.3.5/jcvi/graphics/whisker.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.437840 jcvi-1.3.5/jcvi/projects/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/projects/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/projects/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    22445 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/age.py
+-rw-r--r--   0 bao        (501) staff       (20)     1571 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/alfalfa.py
+-rw-r--r--   0 bao        (501) staff       (20)    15907 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)     6750 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/bites.py
+-rw-r--r--   0 bao        (501) staff       (20)     5679 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/heterosis.py
+-rw-r--r--   0 bao        (501) staff       (20)    14136 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/ies.py
+-rw-r--r--   0 bao        (501) staff       (20)    22201 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/misc.py
+-rw-r--r--   0 bao        (501) staff       (20)    25024 2023-02-06 05:16:46.000000 jcvi-1.3.5/jcvi/projects/napus.py
+-rw-r--r--   0 bao        (501) staff       (20)    12754 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/pineapple.py
+-rw-r--r--   0 bao        (501) staff       (20)     2367 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/pistachio.py
+-rw-r--r--   0 bao        (501) staff       (20)    67857 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/str.py
+-rw-r--r--   0 bao        (501) staff       (20)    25768 2023-04-29 14:56:25.000000 jcvi-1.3.5/jcvi/projects/sugarcane.py
+-rw-r--r--   0 bao        (501) staff       (20)    23950 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/synfind.py
+-rw-r--r--   0 bao        (501) staff       (20)    21554 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/tgbs.py
+-rw-r--r--   0 bao        (501) staff       (20)    11941 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/projects/vanilla.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.440327 jcvi-1.3.5/jcvi/utils/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/utils/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    24200 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/utils/aws.py
+-rw-r--r--   0 bao        (501) staff       (20)    12512 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/utils/cbook.py
+-rw-r--r--   0 bao        (501) staff       (20)      355 2021-01-11 02:34:49.000000 jcvi-1.3.5/jcvi/utils/console.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.442696 jcvi-1.3.5/jcvi/utils/data/
+-rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/Airswing.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/Collegia.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/HookedUp.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/Humor-Sans.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/TREDs.meta.csv
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/adapters.fasta
+-rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/blosum80.mat
+-rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/chrY.hg38.unique_ccn.gc
+-rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/colorchecker.txt
+-rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/hg38.band.txt
+-rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/hg38.chrom.sizes
+-rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/instance.json
+-rw-r--r--   0 bao        (501) staff       (20)     9795 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/utils/db.py
+-rw-r--r--   0 bao        (501) staff       (20)     4145 2021-01-09 20:22:53.000000 jcvi-1.3.5/jcvi/utils/ez_setup.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2884 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/utils/grouper.py
+-rw-r--r--   0 bao        (501) staff       (20)    10437 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/utils/orderedcollections.py
+-rw-r--r--   0 bao        (501) staff       (20)    14595 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/utils/range.py
+-rw-r--r--   0 bao        (501) staff       (20)     3946 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/utils/table.py
+-rw-r--r--   0 bao        (501) staff       (20)     4687 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/utils/taxonomy.py
+-rw-r--r--   0 bao        (501) staff       (20)     1522 2021-07-13 05:06:52.000000 jcvi-1.3.5/jcvi/utils/validator.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     1377 2021-01-15 14:44:37.000000 jcvi-1.3.5/jcvi/utils/webcolors.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.444323 jcvi-1.3.5/jcvi/variation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/variation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      259 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/variation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    45321 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/cnv.py
+-rw-r--r--   0 bao        (501) staff       (20)     7036 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/deconvolute.py
+-rw-r--r--   0 bao        (501) staff       (20)     9385 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/delly.py
+-rw-r--r--   0 bao        (501) staff       (20)    11777 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/impute.py
+-rw-r--r--   0 bao        (501) staff       (20)     3478 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/phase.py
+-rw-r--r--   0 bao        (501) staff       (20)    10831 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/snp.py
+-rw-r--r--   0 bao        (501) staff       (20)    48818 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/str.py
+-rw-r--r--   0 bao        (501) staff       (20)     3672 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/tassel.py
+-rw-r--r--   0 bao        (501) staff       (20)      176 2023-05-20 02:09:56.000000 jcvi-1.3.5/jcvi/version.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.408609 jcvi-1.3.5/jcvi.egg-info/
+-rw-r--r--   0 bao        (501) staff       (20)     8759 2023-05-20 02:09:56.000000 jcvi-1.3.5/jcvi.egg-info/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     4727 2023-05-20 02:09:56.000000 jcvi-1.3.5/jcvi.egg-info/SOURCES.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2023-05-20 02:09:56.000000 jcvi-1.3.5/jcvi.egg-info/dependency_links.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.3.5/jcvi.egg-info/not-zip-safe
+-rw-r--r--   0 bao        (501) staff       (20)      206 2023-05-20 02:09:56.000000 jcvi-1.3.5/jcvi.egg-info/requires.txt
+-rw-r--r--   0 bao        (501) staff       (20)        5 2023-05-20 02:09:56.000000 jcvi-1.3.5/jcvi.egg-info/top_level.txt
+-rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.3.5/pyproject.toml
+-rw-r--r--   0 bao        (501) staff       (20)     1219 2023-05-20 02:09:56.444952 jcvi-1.3.5/setup.cfg
+-rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.3.5/setup.py
```

### Comparing `jcvi-1.3.4/LICENSE` & `jcvi-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/PKG-INFO` & `jcvi-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jcvi-1.3.4/README.md` & `jcvi-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/__init__.py` & `jcvi-1.3.5/jcvi/__init__.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/algorithms/ec.py` & `jcvi-1.3.5/jcvi/algorithms/ec.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/algorithms/formula.py` & `jcvi-1.3.5/jcvi/algorithms/formula.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/algorithms/graph.py` & `jcvi-1.3.5/jcvi/algorithms/graph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/algorithms/lis.py` & `jcvi-1.3.5/jcvi/algorithms/lis.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/algorithms/lpsolve.py` & `jcvi-1.3.5/jcvi/algorithms/lpsolve.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/algorithms/matrix.py` & `jcvi-1.3.5/jcvi/algorithms/matrix.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/algorithms/maxsum.py` & `jcvi-1.3.5/jcvi/algorithms/maxsum.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/algorithms/ml.py` & `jcvi-1.3.5/jcvi/algorithms/ml.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/algorithms/supermap.py` & `jcvi-1.3.5/jcvi/algorithms/supermap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/algorithms/tsp.py` & `jcvi-1.3.5/jcvi/algorithms/tsp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/annotation/ahrd.py` & `jcvi-1.3.5/jcvi/annotation/ahrd.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/annotation/automaton.py` & `jcvi-1.3.5/jcvi/annotation/automaton.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/annotation/depth.py` & `jcvi-1.3.5/jcvi/annotation/depth.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/annotation/evm.py` & `jcvi-1.3.5/jcvi/annotation/evm.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/annotation/maker.py` & `jcvi-1.3.5/jcvi/annotation/maker.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/annotation/pasa.py` & `jcvi-1.3.5/jcvi/annotation/pasa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/annotation/qc.py` & `jcvi-1.3.5/jcvi/annotation/qc.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/annotation/reformat.py` & `jcvi-1.3.5/jcvi/annotation/reformat.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/annotation/stats.py` & `jcvi-1.3.5/jcvi/annotation/stats.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/annotation/train.py` & `jcvi-1.3.5/jcvi/annotation/train.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/align.py` & `jcvi-1.3.5/jcvi/apps/align.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/base.py` & `jcvi-1.3.5/jcvi/apps/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,32 +164,19 @@
             "--grid",
             dest="grid",
             default=False,
             action="store_true",
             help="Run on the grid",
         )
 
-    def set_grid_opts(self, array=False, vcode="99999"):
-        queue_choices = ("default", "fast", "medium", "himem")
-        valid_pcodes = popen("qconf -sprjl", debug=False).read().strip().split("\n")
-        valid_pcodes.append(vcode)
-
+    def set_grid_opts(self, array=False):
         group = OptionGroup(self, "Grid parameters")
         group.add_option(
-            "-P",
-            dest="pcode",
-            default=vcode,
-            choices=valid_pcodes,
-            help="Specify accounting project code",
-        )
-        group.add_option(
             "-l",
             dest="queue",
-            default="default",
-            choices=queue_choices,
             help="Name of the queue",
         )
         group.add_option(
             "-t",
             dest="threaded",
             default=None,
             type="int",
```

### Comparing `jcvi-1.3.4/jcvi/apps/biomart.py` & `jcvi-1.3.5/jcvi/apps/biomart.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/blastplus.py` & `jcvi-1.3.5/jcvi/apps/blastplus.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/bowtie.py` & `jcvi-1.3.5/jcvi/apps/bowtie.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/bwa.py` & `jcvi-1.3.5/jcvi/apps/bwa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/cdhit.py` & `jcvi-1.3.5/jcvi/apps/cdhit.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/emboss.py` & `jcvi-1.3.5/jcvi/apps/emboss.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/fetch.py` & `jcvi-1.3.5/jcvi/apps/fetch.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/gbsubmit.py` & `jcvi-1.3.5/jcvi/apps/gbsubmit.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/gmap.py` & `jcvi-1.3.5/jcvi/apps/gmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/grid.py` & `jcvi-1.3.5/jcvi/apps/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,38 +416,37 @@
 
     def run(self):
         for pi in self:
             pi.start()
 
 
 PBS_STANZA = """
-#PBS -q standard
-#PBS -J 1-{0}
-#PBS -l select=1:ncpus={1}:mem=23gb
+#PBS -q {0}
+#PBS -J 1-{1}
+#PBS -l select=1:ncpus={2}:mem=23gb
 #PBS -l pvmem=23gb
 #PBS -l walltime=100:00:00
-#PBS -W group_list=genomeanalytics
 """
 
 arraysh = """
 CMD=`awk "NR==$SGE_TASK_ID" {0}`
 $CMD"""
 
 arraysh_ua = (
     PBS_STANZA
     + """
 cd $PBS_O_WORKDIR
-CMD=`awk "NR==$PBS_ARRAY_INDEX" {2}`
+CMD=`awk "NR==$PBS_ARRAY_INDEX" {3}`
 $CMD"""
 )
 
 
 def get_grid_engine():
     cmd = "qsub --version"
-    ret = popen(cmd, debug=False).read()
+    ret = popen(cmd, debug=False).read().decode("utf-8").upper()
     return "PBS" if "PBS" in ret else "SGE"
 
 
 def main():
 
     actions = (
         ("run", "run a normal command on grid"),
@@ -483,15 +482,15 @@
     assert runfile != cmds, "Commands list file should not have a `.sh` extension"
 
     engine = get_grid_engine()
     threaded = opts.threaded or 1
     contents = (
         arraysh.format(cmds)
         if engine == "SGE"
-        else arraysh_ua.format(N, threaded, cmds)
+        else arraysh_ua.format(opts.queue, N, threaded, cmds)
     )
     write_file(runfile, contents)
 
     if engine == "PBS":
         return
 
     outfile = "{0}.{1}.out".format(pf, r"\$TASK_ID")
```

### Comparing `jcvi-1.3.4/jcvi/apps/ks.py` & `jcvi-1.3.5/jcvi/apps/ks.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/lastz.py` & `jcvi-1.3.5/jcvi/apps/lastz.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/mask.py` & `jcvi-1.3.5/jcvi/apps/mask.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/phylo.py` & `jcvi-1.3.5/jcvi/apps/phylo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/r.py` & `jcvi-1.3.5/jcvi/apps/r.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/restriction.py` & `jcvi-1.3.5/jcvi/apps/restriction.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/script.py` & `jcvi-1.3.5/jcvi/apps/script.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/softlink.py` & `jcvi-1.3.5/jcvi/apps/softlink.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/uclust.py` & `jcvi-1.3.5/jcvi/apps/uclust.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/uniprot.py` & `jcvi-1.3.5/jcvi/apps/uniprot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/apps/vecscreen.py` & `jcvi-1.3.5/jcvi/apps/vecscreen.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/allmaps.py` & `jcvi-1.3.5/jcvi/assembly/allmaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/allpaths.py` & `jcvi-1.3.5/jcvi/assembly/allpaths.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/automaton.py` & `jcvi-1.3.5/jcvi/assembly/automaton.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/base.py` & `jcvi-1.3.5/jcvi/assembly/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/ca.py` & `jcvi-1.3.5/jcvi/assembly/ca.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/chic.pyx` & `jcvi-1.3.5/jcvi/assembly/chic.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/coverage.py` & `jcvi-1.3.5/jcvi/assembly/coverage.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/gaps.py` & `jcvi-1.3.5/jcvi/assembly/gaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/geneticmap.py` & `jcvi-1.3.5/jcvi/assembly/geneticmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/goldenpath.py` & `jcvi-1.3.5/jcvi/assembly/goldenpath.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/hic.py` & `jcvi-1.3.5/jcvi/assembly/hic.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/kmer.py` & `jcvi-1.3.5/jcvi/assembly/kmer.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import os.path as op
 import sys
 import logging
 import math
 import numpy as np
 
 from collections import defaultdict
+from more_itertools import chunked
+from typing import List
 
 from jcvi.graphics.base import (
     plt,
     adjust_spines,
     asciiplot,
     set_human_axis,
     savefig,
@@ -113,15 +115,15 @@
         MAX_OPTIMIZED_SIZE = 9.9e9
 
         # Generate bins for the decomposed negative binomial distributions
         bins = [
             (i, i) for i in range(1, 9)
         ]  # The first 8 CN are critical often determines ploidy
         for i in (8, 16, 32, 64, 128, 256, 512):  # 14 geometricly sized bins
-            a, b = i + 1, int(round(i * 2 ** 0.5))
+            a, b = i + 1, int(round(i * 2**0.5))
             bins.append((a, b))
             a, b = b + 1, i * 2
             bins.append((a, b))
 
         # Convert histogram to np array so we can index by CN
         kf_ceil = max([cov for cov, _ in self.data])
         N = kf_ceil + 1
@@ -491,27 +493,80 @@
         return {}
 
 
 class KMCComplex(object):
     def __init__(self, indices):
         self.indices = indices
 
-    def write(self, outfile, filename="stdout", action="union"):
+    def write(
+        self,
+        outfile: str,
+        action: str = "union",
+        ci_in: int = 0,
+        ci_out: int = 0,
+        batch: int = 0,
+    ):
         assert action in ("union", "intersect")
         op = " + sum " if action == "union" else " * "
+        mm = MakeManager()
+        if batch > 1:
+            filename = outfile + ".{}.def"
+            # Divide indices into batches
+            batches = []
+            batchsize = (len(self.indices) + batch - 1) // batch
+            logging.debug("Use batchsize of %d", batchsize)
+            for i, indices in enumerate(chunked(self.indices, batchsize)):
+                filename_i = filename.format(i + 1)
+                outfile_i = outfile + ".{}".format(i + 1)
+                self.write_definitions(
+                    filename_i, indices, outfile_i, op, ci_in=ci_in, ci_out=0
+                )
+                cmd = "kmc_tools complex {}".format(filename_i)
+                outfile_suf = outfile_i + ".kmc_suf"
+                mm.add(indices, outfile_suf, cmd)
+                batches.append(outfile_suf)
+        else:
+            batches = self.indices
+
+        # Merge batches into one
+        filename = outfile + ".def"
+        self.write_definitions(
+            filename, batches, outfile, op, ci_in=ci_in, ci_out=ci_out
+        )
+        outfile_suf = outfile + ".kmc_suf"
+        mm.add(batches, outfile_suf, "kmc_tools complex {}".format(filename))
+
+        # Write makefile
+        mm.write()
+
+    def write_definitions(
+        self,
+        filename: str,
+        indices: List[str],
+        outfile: str,
+        op: str,
+        ci_in: int,
+        ci_out: int,
+    ):
         fw = must_open(filename, "w")
         print("INPUT:", file=fw)
         ss = []
-        pad = len(str(len(self.indices)))
-        for i, e in enumerate(self.indices):
+        pad = len(str(len(indices)))
+        for i, e in enumerate(indices):
             s = "s{0:0{1}d}".format(i + 1, pad)
             ss.append(s)
-            print("{} = {}".format(s, e.rsplit(".", 1)[0]), file=fw)
+            msg = "{} = {}".format(s, e.rsplit(".", 1)[0])
+            if ci_in:
+                msg += f" -ci{ci_in}"
+            print(msg, file=fw)
         print("OUTPUT:", file=fw)
         print("{} = {}".format(outfile, op.join(ss)), file=fw)
+        if ci_out:
+            print("OUTPUT_PARAMS:", file=fw)
+            print(f"-ci{ci_out}", file=fw)
         fw.close()
 
 
 def main():
 
     actions = (
         # K-mer counting
@@ -621,54 +676,122 @@
     """
     %prog kmcop *.kmc_suf
 
     Intersect or union kmc indices.
     """
     p = OptionParser(kmcop.__doc__)
     p.add_option(
-        "--action", choices=("union", "intersect"), default="union", help="Action"
+        "--action",
+        choices=("union", "intersect", "reduce"),
+        default="union",
+        help="Action",
+    )
+    p.add_option(
+        "--ci_in",
+        default=0,
+        type="int",
+        help="Exclude input kmers with less than ci_in counts",
+    )
+    p.add_option(
+        "--cs",
+        default=0,
+        type="int",
+        help="Maximal value of a counter, only used when action is reduce",
+    )
+    p.add_option(
+        "--ci_out",
+        default=0,
+        type="int",
+        help="Exclude output kmers with less than ci_out counts",
+    )
+    p.add_option(
+        "--batch",
+        default=1,
+        type="int",
+        help="Number of batch, useful to reduce memory usage",
     )
+    p.add_option("--exclude", help="Exclude accessions from this list")
     p.add_option("-o", default="results", help="Output name")
     opts, args = p.parse_args(args)
 
     if len(args) < 2:
         sys.exit(not p.print_help())
 
     indices = args
-    ku = KMCComplex(indices)
-    ku.write(opts.o, action=opts.action)
+    if opts.exclude:
+        before = set(indices)
+        exclude_ids = set(x.strip() for x in open(opts.exclude))
+        indices = [x for x in indices if x.rsplit(".", 2)[0] not in exclude_ids]
+        after = set(indices)
+        if before > after:
+            logging.debug(
+                "Excluded accessions %d → %d (%s)",
+                len(before),
+                len(after),
+                ",".join(before - after),
+            )
+    if opts.action == "reduce":
+        mm = MakeManager()
+        ci = opts.ci_in
+        cs = opts.cs
+        suf = ""
+        if ci:
+            suf += f"_ci{ci}"
+        if cs:
+            suf += f"_cs{cs}"
+        for index in indices:
+            idx = index.rsplit(".", 1)[0]
+            reduced_idx = idx + suf
+            cmd = f"kmc_tools transform {idx} reduce {reduced_idx}"
+            if ci:
+                cmd += f" -ci{ci}"
+            if cs:
+                cmd += f" -cs{cs}"
+            reduced_index = reduced_idx + ".kmc_suf"
+            mm.add(index, reduced_index, cmd)
+        mm.write()
+    else:
+        ku = KMCComplex(indices)
+        ku.write(
+            opts.o,
+            action=opts.action,
+            ci_in=opts.ci_in,
+            ci_out=opts.ci_out,
+            batch=opts.batch,
+        )
 
 
 def kmc(args):
     """
     %prog kmc folder
 
     Run kmc3 on Illumina reads.
     """
     p = OptionParser(kmc.__doc__)
-    p.add_option("-k", default=21, type="int", help="Kmer size")
+    p.add_option("-k", default=27, type="int", help="Kmer size")
     p.add_option(
         "--ci", default=2, type="int", help="Exclude kmers with less than ci counts"
     )
-    p.add_option("--cs", default=2, type="int", help="Maximal value of a counter")
-    p.add_option(
-        "--cx", default=None, type="int", help="Exclude kmers with more than cx counts"
-    )
+    p.add_option("--cs", default=0, type="int", help="Maximal value of a counter")
+    p.add_option("--cx", type="int", help="Exclude kmers with more than cx counts")
     p.add_option(
         "--single",
         default=False,
         action="store_true",
         help="Input is single-end data, only one FASTQ/FASTA",
     )
     p.add_option(
         "--fasta",
         default=False,
         action="store_true",
         help="Input is FASTA instead of FASTQ",
     )
+    p.add_option(
+        "--mem", default=48, type="int", help="Max amount of RAM in GB (`kmc -m`)"
+    )
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (folder,) = args
@@ -684,16 +807,18 @@
     for p, pf in iter_project(folder, pattern=pattern, n=n, commonprefix=False):
         pf = pf.split("_")[0] + ".ms{}".format(K)
         infiles = pf + ".infiles"
         fw = open(infiles, "w")
         print("\n".join(p), file=fw)
         fw.close()
 
-        cmd = "kmc -k{} -m64 -t{}".format(K, opts.cpus)
-        cmd += " -ci{} -cs{}".format(opts.ci, opts.cs)
+        cmd = "kmc -k{} -m{} -t{}".format(K, opts.mem, opts.cpus)
+        cmd += " -ci{}".format(opts.ci)
+        if opts.cs:
+            cmd += " -cs{}".format(opts.cs)
         if opts.cx:
             cmd += " -cx{}".format(opts.cx)
         if opts.fasta:
             cmd += " -fm"
         cmd += " @{} {} .".format(infiles, pf)
         outfile = pf + ".kmc_suf"
         mm.add(p, outfile, cmd)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jcvi-1.3.4/jcvi/assembly/opticalmap.py` & `jcvi-1.3.5/jcvi/assembly/opticalmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/patch.py` & `jcvi-1.3.5/jcvi/assembly/patch.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/postprocess.py` & `jcvi-1.3.5/jcvi/assembly/postprocess.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/preprocess.py` & `jcvi-1.3.5/jcvi/assembly/preprocess.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/sim.py` & `jcvi-1.3.5/jcvi/assembly/sim.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/soap.py` & `jcvi-1.3.5/jcvi/assembly/soap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/syntenypath.py` & `jcvi-1.3.5/jcvi/assembly/syntenypath.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/assembly/trinity.py` & `jcvi-1.3.5/jcvi/assembly/trinity.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/compara/base.py` & `jcvi-1.3.5/jcvi/compara/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/compara/blastfilter.py` & `jcvi-1.3.5/jcvi/compara/blastfilter.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/compara/catalog.py` & `jcvi-1.3.5/jcvi/compara/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
             size = len(component)
             if size > 1:
                 bb.add(component)
         return bb
 
 
 def main():
-
     actions = (
         ("tandem", "identify tandem gene groups within certain distance"),
         ("ortholog", "run a combined synteny and RBH pipeline to call orthologs"),
         ("group", "cluster the anchors into ortho-groups"),
         ("omgprepare", "prepare weights file to run Sankoff OMG algorithm"),
         ("omg", "generate a series of Sankoff OMG algorithm inputs"),
         ("omgparse", "parse the OMG outputs to get gene lists"),
@@ -609,15 +608,15 @@
     such predictions. Extra orthologs will be recruited from reciprocal best
     match (RBH).
     """
     from jcvi.apps.align import last as last_main
     from jcvi.compara.blastfilter import main as blastfilter_main
     from jcvi.compara.quota import main as quota_main
     from jcvi.compara.synteny import scan, mcscan, liftover
-    from jcvi.formats.blast import cscore, filter
+    from jcvi.formats.blast import cscore, filter, filtered_blastfile_name
 
     p = OptionParser(ortholog.__doc__)
     p.add_option(
         "--dbtype",
         default="nucl",
         choices=("nucl", "prot"),
         help="Molecule type of subject database",
@@ -691,15 +690,15 @@
     qprefix = ".".join((bprefix, aprefix))
     last = pprefix + ".last"
     if need_update((afasta, bfasta), last, warn=True):
         last_main([bfasta, afasta, cpus_flag], dbtype)
 
     self_remove = opts.self_remove
     if a == b:
-        lastself = last + f".P{self_remove}L0.inverse"
+        lastself = filtered_blastfile_name(last, self_remove, 0, inverse=True)
         if need_update(last, lastself, warn=True):
             filter(
                 [last, "--hitlen=0", f"--pctid={self_remove}", "--inverse", "--noself"]
             )
         last = lastself
 
     filtered_last = last + ".filtered"
@@ -792,15 +791,14 @@
     P=50,
     is_self=True,
     evalue=0.01,
     strip_name=".",
     ofile=sys.stderr,
     genefam=False,
 ):
-
     if genefam:
         N = 1e5
 
     # get the sizes for the CDS first
     f = Fasta(cds_file)
     sizes = dict(f.itersizes())
```

### Comparing `jcvi-1.3.4/jcvi/compara/fractionation.py` & `jcvi-1.3.5/jcvi/compara/fractionation.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/compara/pad.py` & `jcvi-1.3.5/jcvi/compara/pad.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/compara/phylogeny.py` & `jcvi-1.3.5/jcvi/compara/phylogeny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/compara/quota.py` & `jcvi-1.3.5/jcvi/compara/quota.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/compara/reconstruct.py` & `jcvi-1.3.5/jcvi/compara/reconstruct.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/compara/synfind.py` & `jcvi-1.3.5/jcvi/compara/synfind.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/compara/synteny.py` & `jcvi-1.3.5/jcvi/compara/synteny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/agp.py` & `jcvi-1.3.5/jcvi/formats/agp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/base.py` & `jcvi-1.3.5/jcvi/formats/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/bed.py` & `jcvi-1.3.5/jcvi/formats/bed.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/blast.py` & `jcvi-1.3.5/jcvi/formats/blast.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,14 @@
 class BlastLineByConversion(BlastLine):
     """
     make BlastLine object from tab delimited line objects with
     BlastLine-like up to 12 fields formats
     """
 
     def __init__(self, sline, mode="1" * 12):
-
         if int(mode, 2) == 4095:
             super(BlastLineByConversion, self).__init__(sline)
         elif 3072 <= int(mode, 2) < 4095:
             args = sline.split("\t")
             atoms = args[:2]
             mode = list(mode)
             if len(args) == 12:
@@ -261,14 +260,30 @@
     alignstats = AlignStats(
         filename, qrycovered, refcovered, qryspan, refspan, identicals, AL50
     )
 
     return alignstats
 
 
+def filtered_blastfile_name(
+    blastfile: str,
+    pctid: float,
+    hitlen: int,
+    inverse: bool = False,
+) -> str:
+    """
+    Return a filtered filename for LAST output, with the given similarity cutoff.
+    """
+    pctid_str = f"{pctid:.1f}".replace(".", "_").replace("_0", "")
+    newblastfile = blastfile + ".P{0}L{1}".format(pctid_str, hitlen)
+    if inverse:
+        newblastfile += ".inverse"
+    return newblastfile
+
+
 def filter(args):
     """
     %prog filter test.blast
 
     Produce a new blast file and filter based on:
     - score: >= cutoff
     - pctid: >= cutoff
@@ -307,29 +322,25 @@
             row = row.replace(",", "\t")
             ids.update(row.split())
     else:
         ids = None
 
     (blastfile,) = args
     inverse = opts.inverse
-    outfile = opts.outfile
     fp = must_open(blastfile)
 
     score, pctid, hitlen, evalue, noself = (
         opts.score,
         opts.pctid,
         opts.hitlen,
         opts.evalue,
         opts.noself,
     )
-    newblastfile = (
-        blastfile + ".P{0}L{1}".format(pctid, hitlen) if outfile is None else outfile
-    )
-    if inverse:
-        newblastfile += ".inverse"
+    blastfile = opts.outfile or blastfile
+    newblastfile = filtered_blastfile_name(blastfile, pctid, hitlen, inverse)
     fw = must_open(newblastfile, "w")
     for row in fp:
         if row[0] == "#":
             continue
         c = BlastLine(row)
 
         if ids:
@@ -358,15 +369,14 @@
 
     fw.close()
 
     return newblastfile
 
 
 def main():
-
     actions = (
         ("summary", "provide summary on id% and cov%"),
         ("completeness", "print completeness statistics for each query"),
         ("annotation", "create tabular file with the annotations"),
         ("top10", "count the most frequent 10 hits"),
         ("filter", "filter BLAST file (based on score, id%, alignlen)"),
         ("covfilter", "filter BLAST file (based on id% and cov%)"),
@@ -1144,15 +1154,15 @@
         mismatches += this_mismatches
         gaps += this_gaps
         alignlen += this_alignlen
 
     if opts.list:
         if qspair:
             allpairs = defaultdict(list)
-            for (q, s) in covidstore:
+            for q, s in covidstore:
                 allpairs[q].append((q, s))
                 allpairs[s].append((q, s))
 
             for id, size in sz.iter_sizes():
                 if id not in allpairs:
                     print("\t".join((id, "na", "0", "0")))
                 else:
```

### Comparing `jcvi-1.3.4/jcvi/formats/cblast.pyx` & `jcvi-1.3.5/jcvi/formats/cblast.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/cdt.py` & `jcvi-1.3.5/jcvi/formats/cdt.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/chain.py` & `jcvi-1.3.5/jcvi/formats/chain.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/contig.py` & `jcvi-1.3.5/jcvi/formats/contig.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/coords.py` & `jcvi-1.3.5/jcvi/formats/coords.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/excel.py` & `jcvi-1.3.5/jcvi/formats/excel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/fasta.py` & `jcvi-1.3.5/jcvi/formats/fasta.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/fastq.py` & `jcvi-1.3.5/jcvi/formats/fastq.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/genbank.py` & `jcvi-1.3.5/jcvi/formats/genbank.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/gff.py` & `jcvi-1.3.5/jcvi/formats/gff.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/html.py` & `jcvi-1.3.5/jcvi/formats/html.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/maf.py` & `jcvi-1.3.5/jcvi/formats/maf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/obo.py` & `jcvi-1.3.5/jcvi/formats/obo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/paf.py` & `jcvi-1.3.5/jcvi/formats/paf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/pdf.py` & `jcvi-1.3.5/jcvi/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/psl.py` & `jcvi-1.3.5/jcvi/formats/psl.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/pyblast.py` & `jcvi-1.3.5/jcvi/formats/pyblast.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/sam.py` & `jcvi-1.3.5/jcvi/formats/sam.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/sizes.py` & `jcvi-1.3.5/jcvi/formats/sizes.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/formats/vcf.py` & `jcvi-1.3.5/jcvi/formats/vcf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/align.py` & `jcvi-1.3.5/jcvi/graphics/align.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/assembly.py` & `jcvi-1.3.5/jcvi/graphics/assembly.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/base.py` & `jcvi-1.3.5/jcvi/graphics/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/blastplot.py` & `jcvi-1.3.5/jcvi/graphics/blastplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/chromosome.py` & `jcvi-1.3.5/jcvi/graphics/chromosome.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/coverage.py` & `jcvi-1.3.5/jcvi/graphics/coverage.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/dotplot.py` & `jcvi-1.3.5/jcvi/graphics/dotplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/glyph.py` & `jcvi-1.3.5/jcvi/graphics/glyph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/grabseeds.py` & `jcvi-1.3.5/jcvi/graphics/grabseeds.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/graph.py` & `jcvi-1.3.5/jcvi/graphics/graph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/heatmap.py` & `jcvi-1.3.5/jcvi/graphics/heatmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/histogram.py` & `jcvi-1.3.5/jcvi/graphics/histogram.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/karyotype.py` & `jcvi-1.3.5/jcvi/graphics/karyotype.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/landscape.py` & `jcvi-1.3.5/jcvi/graphics/landscape.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/logo.py` & `jcvi-1.3.5/jcvi/graphics/logo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/mummerplot.py` & `jcvi-1.3.5/jcvi/graphics/mummerplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/synteny.py` & `jcvi-1.3.5/jcvi/graphics/synteny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/table.py` & `jcvi-1.3.5/jcvi/graphics/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/tree.py` & `jcvi-1.3.5/jcvi/graphics/tree.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/wheel.py` & `jcvi-1.3.5/jcvi/graphics/wheel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/graphics/whisker.py` & `jcvi-1.3.5/jcvi/graphics/whisker.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/projects/age.py` & `jcvi-1.3.5/jcvi/projects/age.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/projects/alfalfa.py` & `jcvi-1.3.5/jcvi/projects/alfalfa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/projects/allmaps.py` & `jcvi-1.3.5/jcvi/projects/allmaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/projects/bites.py` & `jcvi-1.3.5/jcvi/projects/bites.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/projects/heterosis.py` & `jcvi-1.3.5/jcvi/projects/heterosis.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/projects/ies.py` & `jcvi-1.3.5/jcvi/projects/ies.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/projects/misc.py` & `jcvi-1.3.5/jcvi/projects/misc.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/projects/napus.py` & `jcvi-1.3.5/jcvi/projects/napus.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/projects/pineapple.py` & `jcvi-1.3.5/jcvi/projects/pineapple.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/projects/pistachio.py` & `jcvi-1.3.5/jcvi/projects/pistachio.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/projects/str.py` & `jcvi-1.3.5/jcvi/projects/str.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/projects/sugarcane.py` & `jcvi-1.3.5/jcvi/projects/sugarcane.py`

 * *Files 4% similar despite different names*

```diff
@@ -658,48 +658,39 @@
         pct.append(identicals * 100 / qrycovered)
         pct.append(identicals * 100 / refcovered)
     return pct
 
 
 def divergence(args):
     """
-    %prog divergence SS_SR_SO.summary.txt anchors
+    %prog divergence SS_SR_SO.summary.txt
 
     Plot divergence between and within SS/SR/SO genomes.
     """
     sns.set_style("white")
 
     p = OptionParser(divergence.__doc__)
-    _, args, iopts = p.set_image_options(args, figsize="8x8")
-    if len(args) != 2:
+    p.add_option("--title", default="Gapless", help="Plot title")
+    p.add_option(
+        "--xmin",
+        default=94,
+        type="int",
+        help="Minimum percent identity in the histogram",
+    )
+    opts, args, iopts = p.set_image_options(args, figsize="8x8")
+    if len(args) != 1:
         sys.exit(not p.print_help())
 
-    (summary, anchors_dir) = args
+    (summary,) = args
     data_by_genomes = get_genome_wide_pct(summary)
     # Print summary statistics
     print("Genome-wide ungapped percent identity:")
     for (genome1, genome2), pct in sorted(data_by_genomes.items()):
         print(genome1, genome2, np.mean(pct), np.std(pct))
 
-    # Find CDS matches
-    """
-    anchors_last_files = glob(op.join(anchors_dir, "*.anchors.last"))
-    anchors_by_genomes = defaultdict(list)
-    GENOME_NAME_MAPPER = {"robustum": "SR", "officinarum": "SO", "spontaneum": "SS"}
-    for filename in anchors_last_files:
-        genome1, genome2 = op.basename(filename).split(".")[:2]
-        genome1, genome2 = GENOME_NAME_MAPPER[genome1], GENOME_NAME_MAPPER[genome2]
-        pct = get_anchors_pct(filename)
-        anchors_by_genomes[(genome1, genome2)] = pct
-    # Print summary statistics
-    print("CDS anchors ungapped percent identity:")
-    for (genome1, genome2), pct in sorted(anchors_by_genomes.items()):
-        print(genome1, genome2, np.mean(pct), np.std(pct))
-    """
-
     # Plotting genome-wide divergence
     fig = plt.figure(figsize=(iopts.w, iopts.h))
     root = fig.add_axes([0, 0, 1, 1])
     SPECIES_CONFIG = {
         "SS": {"label": "S. spontaneum", "pos": (0.5, 0.67)},
         "SR": {"label": "S. robustum", "pos": (0.2, 0.3)},
         "SO": {"label": "S. officinarum", "pos": (0.8, 0.3)},
@@ -737,37 +728,41 @@
         ("SR", "SR"): {"pos": (0.1, 0.2)},
         ("SO", "SO"): {"pos": (0.9, 0.2)},
         ("SR", "SS"): {"pos": (0.3 - PAD, 0.55)},
         ("SO", "SS"): {"pos": (0.7 + PAD, 0.55)},
         ("SO", "SR"): {"pos": (0.5, 0.18)},
     }
     HIST_WIDTH = 0.15
+    xmin = opts.xmin
     for genome_pair, config in PCT_CONFIG.items():
         x, y = config["pos"]
         ax = fig.add_axes(
             [x - HIST_WIDTH / 2, y - HIST_WIDTH / 2, HIST_WIDTH, HIST_WIDTH]
         )
         d = data_by_genomes[genome_pair]
-        sns.histplot(d, ax=ax, bins=5, kde=False)
-        ax.set_xlim(95, 100)
+        binwidth = (100 - xmin) / 20
+        sns.histplot(d, ax=ax, binwidth=binwidth, kde=False)
+        ax.set_xlim(xmin, 100)
         ax.get_yaxis().set_visible(False)
-        ax.set_xticks([95, 100])
+        ax.set_xticks([xmin, 100])
         adjust_spines(ax, ["bottom"], outward=True)
         ax.spines["bottom"].set_color("lightslategray")
 
+    title = opts.title
+    italic_title = markup(f"*{title}*")
     root.text(
         0.5,
         0.95,
-        "Gapless identities between and within SS/SR/SO genomes",
+        f"{italic_title} identities between and within SS/SR/SO genomes",
         size=14,
         ha="center",
         va="center",
     )
     normalize_axes(root)
-    image_name = "SO_SR_SS.pct_id." + iopts.format
+    image_name = f"SO_SR_SS.{title}." + iopts.format
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def main():
 
     actions = (
         ("prepare", "Calculate lengths from real sugarcane data"),
```

### Comparing `jcvi-1.3.4/jcvi/projects/synfind.py` & `jcvi-1.3.5/jcvi/projects/synfind.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/projects/tgbs.py` & `jcvi-1.3.5/jcvi/projects/tgbs.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/projects/vanilla.py` & `jcvi-1.3.5/jcvi/projects/vanilla.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/aws.py` & `jcvi-1.3.5/jcvi/utils/aws.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/cbook.py` & `jcvi-1.3.5/jcvi/utils/cbook.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/data/Airswing.ttf` & `jcvi-1.3.5/jcvi/utils/data/Airswing.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/data/Collegia.ttf` & `jcvi-1.3.5/jcvi/utils/data/Collegia.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/data/HookedUp.ttf` & `jcvi-1.3.5/jcvi/utils/data/HookedUp.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/data/Humor-Sans.ttf` & `jcvi-1.3.5/jcvi/utils/data/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/data/TREDs.meta.csv` & `jcvi-1.3.5/jcvi/utils/data/TREDs.meta.csv`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/data/adapters.fasta` & `jcvi-1.3.5/jcvi/utils/data/adapters.fasta`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/data/blosum80.mat` & `jcvi-1.3.5/jcvi/utils/data/blosum80.mat`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/data/chrY.hg38.unique_ccn.gc` & `jcvi-1.3.5/jcvi/utils/data/chrY.hg38.unique_ccn.gc`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/data/hg38.band.txt` & `jcvi-1.3.5/jcvi/utils/data/hg38.band.txt`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/data/hg38.chrom.sizes` & `jcvi-1.3.5/jcvi/utils/data/hg38.chrom.sizes`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/data/instance.json` & `jcvi-1.3.5/jcvi/utils/data/instance.json`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/db.py` & `jcvi-1.3.5/jcvi/utils/db.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/ez_setup.py` & `jcvi-1.3.5/jcvi/utils/ez_setup.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/grouper.py` & `jcvi-1.3.5/jcvi/utils/grouper.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/orderedcollections.py` & `jcvi-1.3.5/jcvi/utils/orderedcollections.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/range.py` & `jcvi-1.3.5/jcvi/utils/range.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/table.py` & `jcvi-1.3.5/jcvi/utils/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/taxonomy.py` & `jcvi-1.3.5/jcvi/utils/taxonomy.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/validator.py` & `jcvi-1.3.5/jcvi/utils/validator.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/utils/webcolors.py` & `jcvi-1.3.5/jcvi/utils/webcolors.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/variation/cnv.py` & `jcvi-1.3.5/jcvi/variation/cnv.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/variation/deconvolute.py` & `jcvi-1.3.5/jcvi/variation/deconvolute.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/variation/delly.py` & `jcvi-1.3.5/jcvi/variation/delly.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/variation/impute.py` & `jcvi-1.3.5/jcvi/variation/impute.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/variation/phase.py` & `jcvi-1.3.5/jcvi/variation/phase.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/variation/snp.py` & `jcvi-1.3.5/jcvi/variation/snp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/variation/str.py` & `jcvi-1.3.5/jcvi/variation/str.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi/variation/tassel.py` & `jcvi-1.3.5/jcvi/variation/tassel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/jcvi.egg-info/PKG-INFO` & `jcvi-1.3.5/jcvi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jcvi-1.3.4/jcvi.egg-info/SOURCES.txt` & `jcvi-1.3.5/jcvi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/setup.cfg` & `jcvi-1.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.4/setup.py` & `jcvi-1.3.5/setup.py`

 * *Files identical despite different names*

