# Comparing `tmp/QuasarCode-0.7.7.tar.gz` & `tmp/QuasarCode-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\chris\source\repos\QuasarCode\QuasarCode_Python\dist\.tmp-shkeiief\QuasarCode-0.7.7.tar", last modified: Thu Apr 27 12:04:09 2023, max compression
+gzip compressed data, was "C:\Users\chris\source\repos\QuasarCode\QuasarCode_Python\dist\.tmp-s3nwrp1r\QuasarCode-0.8.0.tar", last modified: Sat May 20 17:33:33 2023, max compression
```

## Comparing `QuasarCode-0.7.7.tar` & `QuasarCode-0.8.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/
--rw-rw-rw-   0        0        0     1077 2023-03-25 17:43:45.000000 QuasarCode-0.7.7/LICENSE.txt
--rw-rw-rw-   0        0        0      826 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-03-25 17:43:45.000000 QuasarCode-0.7.7/README.md
--rw-rw-rw-   0        0        0      920 2023-04-27 11:50:13.000000 QuasarCode-0.7.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:08.000000 QuasarCode-0.7.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/src/QuasarCode/
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/src/QuasarCode/Games/
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Cards/
--rw-rw-rw-   0        0        0     1549 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Cards/_CardGroup.py
--rw-rw-rw-   0        0        0      830 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Cards/_CardQueue.py
--rw-rw-rw-   0        0        0      829 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Cards/_CardStack.py
--rw-rw-rw-   0        0        0     4886 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Cards/_Deck.py
--rw-rw-rw-   0        0        0      619 2023-03-25 17:43:45.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Cards/_IPlayingCard.py
--rw-rw-rw-   0        0        0     2027 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Cards/_PlayingCard.py
--rw-rw-rw-   0        0        0      212 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Cards/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Dice/
--rw-rw-rw-   0        0        0      259 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Dice/_Dice12.py
--rw-rw-rw-   0        0        0      256 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Dice/_Dice6.py
--rw-rw-rw-   0        0        0      256 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Dice/_Dice8.py
--rw-rw-rw-   0        0        0     2636 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Dice/_DiceCup.py
--rw-rw-rw-   0        0        0      368 2023-03-25 17:43:45.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Dice/_IDice.py
--rw-rw-rw-   0        0        0     1412 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Dice/_NDice.py
--rw-rw-rw-   0        0        0      139 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Dice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Spinners/
--rw-rw-rw-   0        0        0      843 2023-03-25 17:43:45.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Spinners/_ISpinner.py
--rw-rw-rw-   0        0        0     1202 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Spinners/_Spinner.py
--rw-rw-rw-   0        0        0       66 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/Spinners/__init__.py
--rw-rw-rw-   0        0        0       65 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Games/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/src/QuasarCode/IO/
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/src/QuasarCode/IO/Configurations/
--rw-rw-rw-   0        0        0     4296 2023-04-27 12:03:06.000000 QuasarCode-0.7.7/src/QuasarCode/IO/Configurations/_ConfigsBase.py
--rw-rw-rw-   0        0        0      144 2023-03-26 16:22:26.000000 QuasarCode-0.7.7/src/QuasarCode/IO/Configurations/__init__.py
--rw-rw-rw-   0        0        0     1763 2023-03-28 00:44:54.000000 QuasarCode-0.7.7/src/QuasarCode/IO/Configurations/_json.py
--rw-rw-rw-   0        0        0      645 2023-03-28 00:44:22.000000 QuasarCode-0.7.7/src/QuasarCode/IO/Configurations/_properties.py
--rw-rw-rw-   0        0        0     1765 2023-03-28 00:45:09.000000 QuasarCode-0.7.7/src/QuasarCode/IO/Configurations/_yaml.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/src/QuasarCode/IO/Text/
--rw-rw-rw-   0        0        0       23 2023-03-26 16:23:05.000000 QuasarCode-0.7.7/src/QuasarCode/IO/Text/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-03-26 16:33:38.000000 QuasarCode-0.7.7/src/QuasarCode/IO/Text/console.py
--rw-rw-rw-   0        0        0       50 2023-03-26 01:12:29.000000 QuasarCode-0.7.7/src/QuasarCode/IO/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/src/QuasarCode/MPI/
--rw-rw-rw-   0        0        0      989 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/MPI/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/MPI/_mpi_configs.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/src/QuasarCode/Science/
--rw-rw-rw-   0        0        0      290 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Science/__init__.py
--rw-rw-rw-   0        0        0     3751 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Science/data.py
--rw-rw-rw-   0        0        0    15789 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Science/figure.py
--rw-rw-rw-   0        0        0    22484 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Science/fitline.py
--rw-rw-rw-   0        0        0     4177 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Science/graph.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/src/QuasarCode/Tools/
--rw-rw-rw-   0        0        0     1144 2023-03-25 17:43:45.000000 QuasarCode-0.7.7/src/QuasarCode/Tools/StringLiterals.py
--rw-rw-rw-   0        0        0     3144 2023-03-25 17:43:45.000000 QuasarCode-0.7.7/src/QuasarCode/Tools/Validators.py
--rw-rw-rw-   0        0        0      210 2023-03-26 01:50:12.000000 QuasarCode-0.7.7/src/QuasarCode/Tools/__init__.py
--rw-rw-rw-   0        0        0      190 2023-03-26 01:55:09.000000 QuasarCode-0.7.7/src/QuasarCode/Tools/_async.py
--rw-rw-rw-   0        0        0     1393 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Tools/_directorys_and_imports.py
--rw-rw-rw-   0        0        0     1375 2023-03-25 17:43:45.000000 QuasarCode-0.7.7/src/QuasarCode/Tools/_multiItterator.py
--rw-rw-rw-   0        0        0     3261 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/Tools/_networking.py
--rw-rw-rw-   0        0        0    12109 2023-03-29 21:30:30.000000 QuasarCode-0.7.7/src/QuasarCode/Tools/_script_wrapper.py
--rw-rw-rw-   0        0        0      697 2023-04-27 11:50:13.000000 QuasarCode-0.7.7/src/QuasarCode/__init__.py
--rw-rw-rw-   0        0        0     1884 2023-03-26 16:18:21.000000 QuasarCode-0.7.7/src/QuasarCode/_global_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/src/QuasarCode/edp/
--rw-rw-rw-   0        0        0     2028 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/edp/_Event.py
--rw-rw-rw-   0        0        0      254 2023-03-25 17:43:45.000000 QuasarCode-0.7.7/src/QuasarCode/edp/_NotEnoughArgumentsError.py
--rw-rw-rw-   0        0        0      217 2023-03-25 17:43:45.000000 QuasarCode-0.7.7/src/QuasarCode/edp/_SubscriberNotPresentError.py
--rw-rw-rw-   0        0        0      217 2023-03-25 17:43:45.000000 QuasarCode-0.7.7/src/QuasarCode/edp/_UndersubscribedEventError.py
--rw-rw-rw-   0        0        0      391 2023-03-25 22:02:36.000000 QuasarCode-0.7.7/src/QuasarCode/edp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:04:09.000000 QuasarCode-0.7.7/src/QuasarCode.egg-info/
--rw-rw-rw-   0        0        0      826 2023-04-27 12:04:08.000000 QuasarCode-0.7.7/src/QuasarCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2052 2023-04-27 12:04:08.000000 QuasarCode-0.7.7/src/QuasarCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 12:04:08.000000 QuasarCode-0.7.7/src/QuasarCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-27 12:04:08.000000 QuasarCode-0.7.7/src/QuasarCode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-27 12:04:08.000000 QuasarCode-0.7.7/src/QuasarCode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/
+-rw-rw-rw-   0        0        0     1077 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      826 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/README.md
+-rw-rw-rw-   0        0        0      920 2023-05-20 00:29:50.000000 QuasarCode-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/Games/
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/
+-rw-rw-rw-   0        0        0     1549 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_CardGroup.py
+-rw-rw-rw-   0        0        0      830 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_CardQueue.py
+-rw-rw-rw-   0        0        0      829 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_CardStack.py
+-rw-rw-rw-   0        0        0     4878 2023-05-20 14:44:24.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_Deck.py
+-rw-rw-rw-   0        0        0      619 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_IPlayingCard.py
+-rw-rw-rw-   0        0        0     2027 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_PlayingCard.py
+-rw-rw-rw-   0        0        0      212 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Cards/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/
+-rw-rw-rw-   0        0        0      259 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_Dice12.py
+-rw-rw-rw-   0        0        0      256 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_Dice6.py
+-rw-rw-rw-   0        0        0      256 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_Dice8.py
+-rw-rw-rw-   0        0        0     2636 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_DiceCup.py
+-rw-rw-rw-   0        0        0      368 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_IDice.py
+-rw-rw-rw-   0        0        0     1412 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_NDice.py
+-rw-rw-rw-   0        0        0      139 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Dice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Spinners/
+-rw-rw-rw-   0        0        0      843 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Spinners/_ISpinner.py
+-rw-rw-rw-   0        0        0     1202 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Spinners/_Spinner.py
+-rw-rw-rw-   0        0        0       66 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/Spinners/__init__.py
+-rw-rw-rw-   0        0        0       65 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Games/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/IO/
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/
+-rw-rw-rw-   0        0        0     4933 2023-05-20 15:51:12.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_ConfigsBase.py
+-rw-rw-rw-   0        0        0      144 2023-03-26 16:22:26.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/__init__.py
+-rw-rw-rw-   0        0        0     1763 2023-03-28 00:44:54.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_json.py
+-rw-rw-rw-   0        0        0      645 2023-03-28 00:44:22.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_properties.py
+-rw-rw-rw-   0        0        0     1765 2023-05-20 15:54:55.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_yaml.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Text/
+-rw-rw-rw-   0        0        0      388 2023-05-20 16:18:18.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Text/__init__.py
+-rw-rw-rw-   0        0        0     3365 2023-05-20 16:23:22.000000 QuasarCode-0.8.0/src/QuasarCode/IO/Text/_console.py
+-rw-rw-rw-   0        0        0       50 2023-03-26 01:12:29.000000 QuasarCode-0.8.0/src/QuasarCode/IO/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/MPI/
+-rw-rw-rw-   0        0        0      980 2023-05-20 14:46:27.000000 QuasarCode-0.8.0/src/QuasarCode/MPI/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/MPI/_mpi_configs.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/Science/
+-rw-rw-rw-   0        0        0      364 2023-05-20 00:28:18.000000 QuasarCode-0.8.0/src/QuasarCode/Science/__init__.py
+-rw-rw-rw-   0        0        0     1516 2023-05-20 00:30:36.000000 QuasarCode-0.8.0/src/QuasarCode/Science/_plotting.py
+-rw-rw-rw-   0        0        0     4044 2023-05-20 17:21:42.000000 QuasarCode-0.8.0/src/QuasarCode/Science/data.py
+-rw-rw-rw-   0        0        0    15789 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Science/figure.py
+-rw-rw-rw-   0        0        0    22484 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Science/fitline.py
+-rw-rw-rw-   0        0        0     4177 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Science/graph.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/
+-rw-rw-rw-   0        0        0     1144 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/StringLiterals.py
+-rw-rw-rw-   0        0        0     3144 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/Validators.py
+-rw-rw-rw-   0        0        0      210 2023-05-20 16:14:08.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-03-26 01:55:09.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/_async.py
+-rw-rw-rw-   0        0        0     1393 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/_directorys_and_imports.py
+-rw-rw-rw-   0        0        0     1375 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/_multiItterator.py
+-rw-rw-rw-   0        0        0     3261 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/_networking.py
+-rw-rw-rw-   0        0        0    12115 2023-05-20 16:13:07.000000 QuasarCode-0.8.0/src/QuasarCode/Tools/_script_wrapper.py
+-rw-rw-rw-   0        0        0      737 2023-05-20 16:10:55.000000 QuasarCode-0.8.0/src/QuasarCode/__init__.py
+-rw-rw-rw-   0        0        0     1884 2023-03-26 16:18:21.000000 QuasarCode-0.8.0/src/QuasarCode/_global_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode/edp/
+-rw-rw-rw-   0        0        0     2028 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/edp/_Event.py
+-rw-rw-rw-   0        0        0      254 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/edp/_NotEnoughArgumentsError.py
+-rw-rw-rw-   0        0        0      217 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/edp/_SubscriberNotPresentError.py
+-rw-rw-rw-   0        0        0      217 2023-03-25 17:43:45.000000 QuasarCode-0.8.0/src/QuasarCode/edp/_UndersubscribedEventError.py
+-rw-rw-rw-   0        0        0      391 2023-03-25 22:02:36.000000 QuasarCode-0.8.0/src/QuasarCode/edp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode.egg-info/
+-rw-rw-rw-   0        0        0      826 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2089 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-20 17:33:33.000000 QuasarCode-0.8.0/src/QuasarCode.egg-info/top_level.txt
```

### Comparing `QuasarCode-0.7.7/LICENSE.txt` & `QuasarCode-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/PKG-INFO` & `QuasarCode-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuasarCode
-Version: 0.7.7
+Version: 0.8.0
 Summary: A general purpose library for Python applications.
 Author-email: Christopher Rowe <thequasarx1@gmail.com>
 Project-URL: Homepage, https://github.com/QuasarX1/QuasarCode
 Project-URL: Bug Tracker, https://github.com/QuasarX1/QuasarCode/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `QuasarCode-0.7.7/pyproject.toml` & `QuasarCode-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["*"]
 
 [project]
 name = "QuasarCode"
-version = "0.7.7"
+version = "0.8.0"
 authors = [
   { name="Christopher Rowe", email="thequasarx1@gmail.com" },
 ]
 description = "A general purpose library for Python applications."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Games/Cards/_CardGroup.py` & `QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_CardGroup.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Games/Cards/_CardQueue.py` & `QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_CardQueue.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Games/Cards/_CardStack.py` & `QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_CardStack.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Games/Cards/_Deck.py` & `QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_Deck.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from QuasarCode.edp import Event
+from ...edp import Event
 from ._CardGroup import CardGroup
 from ._PlayingCard import PlayingCard
 from random import Random
 
 class Deck(CardGroup):
     """
     A collection of 52+ unique playing cards. The exact number can vary dependant on the number of jokers added
```

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Games/Cards/_IPlayingCard.py` & `QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_IPlayingCard.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Games/Cards/_PlayingCard.py` & `QuasarCode-0.8.0/src/QuasarCode/Games/Cards/_PlayingCard.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Games/Dice/_DiceCup.py` & `QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_DiceCup.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Games/Dice/_NDice.py` & `QuasarCode-0.8.0/src/QuasarCode/Games/Dice/_NDice.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Games/Spinners/_ISpinner.py` & `QuasarCode-0.8.0/src/QuasarCode/Games/Spinners/_ISpinner.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Games/Spinners/_Spinner.py` & `QuasarCode-0.8.0/src/QuasarCode/Games/Spinners/_Spinner.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/IO/Configurations/_ConfigsBase.py` & `QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_ConfigsBase.py`

 * *Files 19% similar despite different names*

```diff
@@ -61,17 +61,22 @@
             self.__data[key].lock()
 
     @property
     def writable(self):
         return self.__writable
 
     def _get_keys(self) -> Tuple[Union[str, Dict[str, Tuple]]]:
+        print("WARNING: this method is depreciated and will be removed in a future update! Use object.keys instead.")
         #return ((self.__data[key]._get_keys() if key in self.__sub_mapping_keys else key) for key in self.__data)
         return list(self.__data.keys())
 
+    @property
+    def keys(self):
+        return list(self.__data.keys())
+
 class ConfigsBase(_Mapping, ABC):
     def __init__(self, writable: bool = True, filepath: str = None):
         self.__stringify_storage = None
         self.__stringify_indent = None
 
         super().__init__()
 
@@ -92,30 +97,39 @@
 
     def __str__(self):
         highrarchy = self
 
         self.__stringify_storage = ""
         self.__stringify_indent = 0
         def recursive_writer(sub_highrarchy):
-            nested_item_values = []
-            all_keys = sub_highrarchy._get_keys()
-            max_key_length = max([len(key) for key in all_keys])
-            for key in all_keys:
-                value = sub_highrarchy[key]
-                if isinstance(value, _Mapping):
-                    nested_item_values.append(value)
-                else:
+            all_keys = sub_highrarchy.keys
+
+            if len(all_keys) == 0:
+                return# There is nothing to display here
+
+            non_mapping_key_indexes = [i for i, key in enumerate(all_keys) if not isinstance(sub_highrarchy[key], _Mapping)]
+            if len(non_mapping_key_indexes) > 0:
+                max_key_length = max([len(all_keys[i]) for i in non_mapping_key_indexes])
+
+                # Display non-mapables
+                for key_index in non_mapping_key_indexes:
+                    key = all_keys[key_index]
+                    value = sub_highrarchy[key]
+
                     insert_value = ('"'+value+'"') if isinstance(value, str) else value
                     self.__stringify_storage += (" " * self.__stringify_indent) + f"{key}{' ' * (max_key_length - len(key))} = {insert_value}\n"
 
-            for value in nested_item_values:
+            # Recursivley display mappables
+            for key in (all_keys if len(non_mapping_key_indexes) == 0 else [key for i, key in enumerate(all_keys) if i not in non_mapping_key_indexes]):
+                value = sub_highrarchy[key]
+
                 self.__stringify_storage += (" " * self.__stringify_indent) + "\n"
-                self.__stringify_storage += (" " * self.__stringify_indent) + f"{list(value._get_keys())[0]}:\n"
+                self.__stringify_storage += (" " * self.__stringify_indent) + f"{key}:\n"
                 self.__stringify_indent += 4
                 recursive_writer(value)
                 self.__stringify_indent -= 4
 
         recursive_writer(highrarchy)
-        return self.__stringify_storage
+        return self.__stringify_storage.lstrip("\n")
 
     def __repr__(self):
         return "Configuration Object. Items as follows:\n\n" + self.__str__()
```

### Comparing `QuasarCode-0.7.7/src/QuasarCode/IO/Configurations/_json.py` & `QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_json.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/IO/Configurations/_properties.py` & `QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_properties.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/IO/Configurations/_yaml.py` & `QuasarCode-0.8.0/src/QuasarCode/IO/Configurations/_yaml.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/MPI/__init__.py` & `QuasarCode-0.8.0/src/QuasarCode/MPI/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import warnings
 
-from QuasarCode._global_settings import settings_object as __settings_object
+from .._global_settings import settings_object as __settings_object
 
 try:
     from mpi4py import MPI
     __settings_object._set_mpi_avalible()
     _display_mpi_warning = lambda *args, **kwargs: None
     _raise_mpi_error = lambda *args, **kwargs: None
 except:
```

### Comparing `QuasarCode-0.7.7/src/QuasarCode/MPI/_mpi_configs.py` & `QuasarCode-0.8.0/src/QuasarCode/MPI/_mpi_configs.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Science/data.py` & `QuasarCode-0.8.0/src/QuasarCode/Science/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,42 +64,53 @@
     return num
 
 def standard_form(num: Decimal):
     """
     Determines the value and power for the standard form representation of a number
     """
     num = Decimal(num)
+    power = 0
 
     if num >= 1:
-        power = 0
+        new_num = None
+        new_power = None
         while num > 1:
-            power += 1
-            num /= 10
+            new_num = num
+            new_power = power
+
+            new_power += 1
+            new_num /= 10
+
+            if new_num < 1:
+                break
+            else:
+                num = new_num
+                power = new_power
 
     else:
-        power = 0
         while num < 1:
             power -= 1
             num *= 10
             if num > 1:
                 break
-        power += 1
 
     return num, power
 
-def standard_form_string(num: Decimal, numberSigFig = None):
+def standard_form_string(num: Decimal, numberSigFig = None, latex = False):
     """
     Determines the standard form representation of a number and represents it as a string
     """
     number, power = standard_form(num)
 
-    return "{} * 10^{}".format(float(sig_fig(number, numberSigFig) if numberSigFig is not None else number), power) if power != 0 else str(float(sig_fig(number, numberSigFig) if numberSigFig is not None else number))
+    template = "${}\\times10^{{{}}}$" if latex else "{} * 10^{}"
+
+    return template.format(float(sig_fig(number, numberSigFig) if numberSigFig is not None else number), power) if power != 0 else str(float(sig_fig(number, numberSigFig) if numberSigFig is not None else number))
 
 def standard_form_string_if_nessessary(num: Decimal, numberSigFig = None):
-    if np.abs(num) >= 1000 or np.abs(num) < 0.001:
+    if np.abs(num) >= 9999 or np.abs(num) < 0.001:
         return standard_form_string(num, numberSigFig)
     else:
         return str(float(sig_fig(num, numberSigFig) if numberSigFig is not None else num))
 
 def true_round(number: Decimal, nDigits: int = None):
     """
     Rounds a number according to common rounding principles.
```

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Science/figure.py` & `QuasarCode-0.8.0/src/QuasarCode/Science/figure.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Science/fitline.py` & `QuasarCode-0.8.0/src/QuasarCode/Science/fitline.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Science/graph.py` & `QuasarCode-0.8.0/src/QuasarCode/Science/graph.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Tools/StringLiterals.py` & `QuasarCode-0.8.0/src/QuasarCode/Tools/StringLiterals.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Tools/Validators.py` & `QuasarCode-0.8.0/src/QuasarCode/Tools/Validators.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Tools/_directorys_and_imports.py` & `QuasarCode-0.8.0/src/QuasarCode/Tools/_directorys_and_imports.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Tools/_multiItterator.py` & `QuasarCode-0.8.0/src/QuasarCode/Tools/_multiItterator.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Tools/_networking.py` & `QuasarCode-0.8.0/src/QuasarCode/Tools/_networking.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/Tools/_script_wrapper.py` & `QuasarCode-0.8.0/src/QuasarCode/Tools/_script_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import traceback
 
-from QuasarCode.IO.Text.console import print_info, print_verbose_info, print_warning, print_verbose_warning, print_error, print_verbose_error, print_debug
-from QuasarCode._global_settings import settings_object as _settings_object
-from QuasarCode.MPI import get_mpi_rank
-from QuasarCode.Tools._async import start_main_async
+from ..IO.Text._console import Console# print_info, print_verbose_info, print_warning, print_verbose_warning, print_error, print_verbose_error, print_debug
+from .._global_settings import settings_object as _settings_object
+from ..MPI import get_mpi_rank
+from ..Tools._async import start_main_async
 
 
 class ScriptWrapper(object):
     """
     Singelton that handles command argument parsing for the currently running program.
     Constructor Arguments:
               str filename                 --> The name of the entrypoint file.
@@ -156,19 +156,19 @@
                     # MPI active and not the first process
                     is_root_process = False
                     return func(self, *args, **kwargs)
                     
             except Exception as e:
                 if is_root_process or self.MPI_print_non_root_process_errors:
                     has_message = e.__str__() != ""
-                    print_error(f"Execution encountered an error{(':' if has_message else ' (no details avalible).') if _settings_object.debug or _settings_object.verbose else '.'}")
-                    print_debug("Traceback (most recent call last):\n" + "".join(traceback.format_tb(e.__traceback__)) + type(e).__name__ + (f": {e.__str__()}" if has_message else ""))
+                    Console.print_error(f"Execution encountered an error{(':' if has_message else ' (no details avalible).') if _settings_object.debug or _settings_object.verbose else '.'}")
+                    Console.print_debug("Traceback (most recent call last):\n" + "".join(traceback.format_tb(e.__traceback__)) + type(e).__name__ + (f": {e.__str__()}" if has_message else ""))
                     if has_message and not _settings_object.debug:
-                        print_error(e.__str__())
-                    print_info("Terminating.")
+                        Console.print_error(e.__str__())
+                    Console.print_info("Terminating.")
 
         return inner
 
     @__run
     def run(self, func):
         kwargs = { param.replace("-", "_"): self.params[param] for param in self.params if param not in ("help", "debug", "verbose") }
         return func(**kwargs)
```

### Comparing `QuasarCode-0.7.7/src/QuasarCode/__init__.py` & `QuasarCode-0.8.0/src/QuasarCode/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Adds functionality to Python along with wrapers for existing modules for ease of use
 
 Credits:
     Written by Christopher Rowe
     Notable contribusions taken from code written by Tim Greenshaw 10/2018
 
-Version: 0.7.7
+Version: 0.8.0
 """
 
 from ._global_settings import settings_object as Settings
 
 from . import edp
 
 from . import Games
@@ -21,11 +21,12 @@
 from . import MPI
 
 from . import Science
 
 from . import Tools
 
 from .Tools._directorys_and_imports import source_file_relitive_add_to_path
-from .IO.Text.console import pause as console_pause
-from .IO.Text import console
+from .IO.Text import Console
+from .IO.Text import console# Depreciated!!!
+console_pause = console.pause# Depreciated!!!
 from .edp import Event
 from .Tools._async import start_main_async
```

### Comparing `QuasarCode-0.7.7/src/QuasarCode/_global_settings.py` & `QuasarCode-0.8.0/src/QuasarCode/_global_settings.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode/edp/_Event.py` & `QuasarCode-0.8.0/src/QuasarCode/edp/_Event.py`

 * *Files identical despite different names*

### Comparing `QuasarCode-0.7.7/src/QuasarCode.egg-info/PKG-INFO` & `QuasarCode-0.8.0/src/QuasarCode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuasarCode
-Version: 0.7.7
+Version: 0.8.0
 Summary: A general purpose library for Python applications.
 Author-email: Christopher Rowe <thequasarx1@gmail.com>
 Project-URL: Homepage, https://github.com/QuasarX1/QuasarCode
 Project-URL: Bug Tracker, https://github.com/QuasarX1/QuasarCode/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `QuasarCode-0.7.7/src/QuasarCode.egg-info/SOURCES.txt` & `QuasarCode-0.8.0/src/QuasarCode.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,19 @@
 src/QuasarCode/IO/__init__.py
 src/QuasarCode/IO/Configurations/_ConfigsBase.py
 src/QuasarCode/IO/Configurations/__init__.py
 src/QuasarCode/IO/Configurations/_json.py
 src/QuasarCode/IO/Configurations/_properties.py
 src/QuasarCode/IO/Configurations/_yaml.py
 src/QuasarCode/IO/Text/__init__.py
-src/QuasarCode/IO/Text/console.py
+src/QuasarCode/IO/Text/_console.py
 src/QuasarCode/MPI/__init__.py
 src/QuasarCode/MPI/_mpi_configs.py
 src/QuasarCode/Science/__init__.py
+src/QuasarCode/Science/_plotting.py
 src/QuasarCode/Science/data.py
 src/QuasarCode/Science/figure.py
 src/QuasarCode/Science/fitline.py
 src/QuasarCode/Science/graph.py
 src/QuasarCode/Tools/StringLiterals.py
 src/QuasarCode/Tools/Validators.py
 src/QuasarCode/Tools/__init__.py
```

