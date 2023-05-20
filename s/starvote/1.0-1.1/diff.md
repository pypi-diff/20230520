# Comparing `tmp/starvote-1.0.tar.gz` & `tmp/starvote-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starvote-1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "starvote-1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `starvote-1.0.tar` & `starvote-1.1.tar`

### file list

```diff
@@ -1,23 +1,39 @@
--rw-r--r--   0        0        0       19 2023-05-20 12:58:10.568731 starvote-1.0/.gitignore
--rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-1.0/LICENSE
--rw-r--r--   0        0        0     2908 2023-05-20 13:14:39.184993 starvote-1.0/README.md
--rw-r--r--   0        0        0      267 2023-05-20 12:47:55.671593 starvote-1.0/example.py
--rw-r--r--   0        0        0      502 2023-05-20 12:55:16.755279 starvote-1.0/pyproject.toml
--rw-r--r--   0        0        0      290 2023-05-20 12:57:25.712356 starvote-1.0/sample_votes/README.md
--rw-r--r--   0        0        0      169 2023-05-20 12:17:24.308288 starvote-1.0/sample_votes/sample_vote_automatic_runoff_breakable_tie.csv
--rw-r--r--   0        0        0      169 2023-05-20 12:16:12.379686 starvote-1.0/sample_votes/sample_vote_automatic_runoff_unbreakable_tie.csv
--rw-r--r--   0        0        0      169 2023-05-20 12:27:44.977476 starvote-1.0/sample_votes/sample_vote_score_round_breakable_tie_between_second_and_third.csv
--rw-r--r--   0        0        0      169 2023-05-20 12:14:18.630735 starvote-1.0/sample_votes/sample_vote_score_round_unbreakable_three_way_tie.csv
--rw-r--r--   0        0        0      169 2023-05-20 12:30:43.458967 starvote-1.0/sample_votes/sample_vote_score_round_unbreakable_tie_between_second_and_third.csv
--rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-1.0/sample_votes/starvote_ballots_4tyx27ks_20230520050434.csv
--rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-1.0/sample_votes/starvote_ballots_9fm5fp2c_20230520033518.csv
--rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-1.0/sample_votes/starvote_ballots_9mm3519w_20230520050438.csv
--rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-1.0/sample_votes/starvote_ballots_9xrw9wch_20230520050429.csv
--rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-1.0/sample_votes/starvote_ballots_dd1wc4yx_20230520050413.csv
--rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-1.0/sample_votes/starvote_ballots_eh3cxxz7_20230520033403.csv
--rw-r--r--   0        0        0   115109 2023-05-20 12:04:19.133723 starvote-1.0/sample_votes/starvote_ballots_p4rs6xn4_20230520050419.csv
--rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-1.0/sample_votes/starvote_ballots_pf69snyx_20230520050425.csv
--rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-1.0/sample_votes/starvote_ballots_swzw2ts6_20230520050422.csv
--rw-r--r--   0        0        0     5227 2023-05-20 12:53:44.562508 starvote-1.0/starvote/__init__.py
--rw-r--r--   0        0        0     1014 2023-05-20 12:53:02.770159 starvote-1.0/starvote/__main__.py
--rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 starvote-1.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-05-20 12:58:10.568731 starvote-1.1/.gitignore
+-rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-1.1/LICENSE
+-rw-r--r--   0        0        0     3776 2023-05-20 14:24:06.899853 starvote-1.1/README.md
+-rw-r--r--   0        0        0      267 2023-05-20 12:47:55.671593 starvote-1.1/example.py
+-rw-r--r--   0        0        0      502 2023-05-20 12:55:16.755279 starvote-1.1/pyproject.toml
+-rw-r--r--   0        0        0      307 2023-05-20 14:24:30.072047 starvote-1.1/sample_polls/README.md
+-rw-r--r--   0        0        0      169 2023-05-20 12:17:24.308288 starvote-1.1/sample_polls/sample_poll_automatic_runoff_breakable_tie.csv
+-rw-r--r--   0        0        0      314 2023-05-20 14:22:01.282802 starvote-1.1/sample_polls/sample_poll_automatic_runoff_breakable_tie.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:16:12.379686 starvote-1.1/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.csv
+-rw-r--r--   0        0        0      382 2023-05-20 14:22:01.298802 starvote-1.1/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:27:44.977476 starvote-1.1/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.csv
+-rw-r--r--   0        0        0      333 2023-05-20 14:22:01.314803 starvote-1.1/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:14:18.630735 starvote-1.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.csv
+-rw-r--r--   0        0        0      198 2023-05-20 14:22:01.330803 starvote-1.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.result.txt
+-rw-r--r--   0        0        0      226 2023-05-20 14:20:22.817978 starvote-1.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.csv
+-rw-r--r--   0        0        0      231 2023-05-20 14:22:01.346803 starvote-1.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:30:43.458967 starvote-1.1/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.csv
+-rw-r--r--   0        0        0      346 2023-05-20 14:22:01.358803 starvote-1.1/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.result.txt
+-rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-1.1/sample_polls/starvote_ballots_4tyx27ks_20230520050434.csv
+-rw-r--r--   0        0        0      869 2023-05-20 14:22:01.378803 starvote-1.1/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.txt
+-rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-1.1/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.csv
+-rw-r--r--   0        0        0     2411 2023-05-20 14:22:01.390803 starvote-1.1/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.txt
+-rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-1.1/sample_polls/starvote_ballots_9mm3519w_20230520050438.csv
+-rw-r--r--   0        0        0      401 2023-05-20 14:22:01.406803 starvote-1.1/sample_polls/starvote_ballots_9mm3519w_20230520050438.result.txt
+-rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-1.1/sample_polls/starvote_ballots_9xrw9wch_20230520050429.csv
+-rw-r--r--   0        0        0      954 2023-05-20 14:22:01.426803 starvote-1.1/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.txt
+-rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-1.1/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv
+-rw-r--r--   0        0        0      954 2023-05-20 14:22:01.446804 starvote-1.1/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.txt
+-rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-1.1/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.csv
+-rw-r--r--   0        0        0     1084 2023-05-20 14:22:01.478804 starvote-1.1/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.txt
+-rw-r--r--   0        0        0   115109 2023-05-20 12:04:19.133723 starvote-1.1/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.csv
+-rw-r--r--   0        0        0     2635 2023-05-20 14:22:01.502804 starvote-1.1/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.txt
+-rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-1.1/sample_polls/starvote_ballots_pf69snyx_20230520050425.csv
+-rw-r--r--   0        0        0      412 2023-05-20 14:22:01.522804 starvote-1.1/sample_polls/starvote_ballots_pf69snyx_20230520050425.result.txt
+-rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-1.1/sample_polls/starvote_ballots_swzw2ts6_20230520050422.csv
+-rw-r--r--   0        0        0      370 2023-05-20 14:22:01.538804 starvote-1.1/sample_polls/starvote_ballots_swzw2ts6_20230520050422.result.txt
+-rw-r--r--   0        0        0     5665 2023-05-20 14:21:09.494369 starvote-1.1/starvote/__init__.py
+-rw-r--r--   0        0        0     1014 2023-05-20 12:53:02.770159 starvote-1.1/starvote/__main__.py
+-rw-r--r--   0        0        0     4194 1970-01-01 00:00:00.000000 starvote-1.1/PKG-INFO
```

### Comparing `starvote-1.0/LICENSE` & `starvote-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starvote-1.0/README.md` & `starvote-1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,25 @@
 To use, `import starvote`, then instantiate a `starvote.Poll` object.
 Feed in the ballots using `poll.add_ballot(ballot)`; ballots are `dict` objects,
 mapping the candidate to the ballot's vote for the candidate
 (an `int` in the range 0 to 5 inclusive).
 
 Once you've added all the ballots, call `poll.result` to compute the winner.
 If there's an unbreakable tie, `poll.result` will raise an
-`UnbreakableTieError`.
+`UnbreakableTieError`.  The following scenarios can result in an
+unbreakable tie:
+
+* If the top two candidates tie during the automated runoff round
+  *and* their scores are also a tie.
+* If the second and third candidates during the score round tie,
+  and their preference scores are also a tie.
+* If three or more candiates are tied for first *or* second place
+  during the score round.
+
+(These scenarios are highly unlikely with real-world data.)
 
 If you want to see how the vote was tabulated, pass in an argument
 to the `print` keyword-only argument to `poll.result`.  This should
 be a function that behaves like the builtin `print` function; it
 will only ever be called with positional parameters.
 
 Here's an example of computing a poll between Amy, Brian, and Chuck:
@@ -58,15 +68,15 @@
 If the module is executed as a script, it will read a single
 [CSV file](https://en.wikipedia.org/wiki/Comma-separated_values)
 in [*star.vote*](https://star.vote/) format, tabulate, and print
 the result.  For example, you can run this from the root of the
 source-code repository:
 
 ```
-% python3 -m starvote sample_votes/sample_vote_automatic_runoff_breakable_tie.csv
+% python3 -m starvote sample_polls/sample_vote_automatic_runoff_breakable_tie.csv
 ```
 
 to see how **starvote** handles a tie during the automatic runoff round.
 
 ## Limitations
 
 Currently this module only supports single-winner STAR voting;
@@ -82,7 +92,22 @@
 [MIT license.](https://opensource.org/license/mit/)
 See the `LICENSE` file.
 
 The source code repository includes sample ballots downloaded from
 [https://star.vote/](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
+
+## Changelog
+
+**1.1** 2023/05/20
+
+* Bugfix: raise `UnbreakableTieError` if there's a three-way
+  tie for *second* place.  Previously **starvote** only noticed
+  if there was a three-way tie for *first* place.
+* Added sample output for every sample poll in `sample_polls/`.
+  These outputs have been confirmed correct by inspection, and
+  could in the future be used as part of an automated test suite.
+
+**1.0** 2023/05/20
+
+Initial release.
```

### Comparing `starvote-1.0/sample_votes/starvote_ballots_4tyx27ks_20230520050434.csv` & `starvote-1.1/sample_polls/starvote_ballots_4tyx27ks_20230520050434.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.0/sample_votes/starvote_ballots_9fm5fp2c_20230520033518.csv` & `starvote-1.1/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.0/sample_votes/starvote_ballots_9mm3519w_20230520050438.csv` & `starvote-1.1/sample_polls/starvote_ballots_9mm3519w_20230520050438.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.0/sample_votes/starvote_ballots_9xrw9wch_20230520050429.csv` & `starvote-1.1/sample_polls/starvote_ballots_9xrw9wch_20230520050429.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.0/sample_votes/starvote_ballots_dd1wc4yx_20230520050413.csv` & `starvote-1.1/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.0/sample_votes/starvote_ballots_eh3cxxz7_20230520033403.csv` & `starvote-1.1/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.0/sample_votes/starvote_ballots_p4rs6xn4_20230520050419.csv` & `starvote-1.1/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.0/sample_votes/starvote_ballots_pf69snyx_20230520050425.csv` & `starvote-1.1/sample_polls/starvote_ballots_pf69snyx_20230520050425.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.0/sample_votes/starvote_ballots_swzw2ts6_20230520050422.csv` & `starvote-1.1/sample_polls/starvote_ballots_swzw2ts6_20230520050422.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.0/starvote/__init__.py` & `starvote-1.1/starvote/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 __doc__ = "A simple STAR vote tabulator"
 
-__version__ = "1.0"
+__version__ = "1.1"
 
 import math
 
 __all__ = ['Poll', 'UnbreakableTieError']
 
 class UnbreakableTieError(ValueError):
     pass
@@ -99,20 +99,25 @@
             for winner in self.candidates:
                 if print:
                     print(f"  Only one candidate, returning winner {winner!r}")
                 return winner
 
         top_two = rankings[-2:]
         if candidates_count > 2:
-            if rankings[-3][0] == rankings[-2][0]:
+            if (rankings[-3][0] == rankings[-2][0]):
                 if rankings[-2][0] == rankings[-1][0]:
                     candidates = ", ".join(r[1] for r in rankings[-3:])
                     first_two, comma, last_one = candidates.rpartition(",")
                     candidates = f"{first_two}{comma} and{last_one}"
-                    raise UnbreakableTieError("unbreakable three-way tie in score round between " + candidates)
+                    raise UnbreakableTieError("unbreakable three-way tie for first in score round between " + candidates)
+                if (candidates_count > 3) and (rankings[-4][0] == rankings[-3][0]):
+                    candidates = ", ".join(r[1] for r in rankings[-4:-1])
+                    first_two, comma, last_one = candidates.rpartition(",")
+                    candidates = f"{first_two}{comma} and{last_one}"
+                    raise UnbreakableTieError("unbreakable three-way tie for second in score round between " + candidates)
                 if print:
                     print("[Resolving two-way tie between second and third in score round]")
                 preferred = self.preference(rankings[-3][1], rankings[-2][1], print=print, when="preference runoff between second and third in score round")
                 if top_two[0][1] != preferred:
                     top_two[0] = rankings[-3]
         if print:
             print("[Automatic runoff round]")
```

### Comparing `starvote-1.0/starvote/__main__.py` & `starvote-1.1/starvote/__main__.py`

 * *Files identical despite different names*

### Comparing `starvote-1.0/PKG-INFO` & `starvote-1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starvote
-Version: 1.0
+Version: 1.1
 Summary: A simple STAR vote tabulator
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -26,15 +26,25 @@
 To use, `import starvote`, then instantiate a `starvote.Poll` object.
 Feed in the ballots using `poll.add_ballot(ballot)`; ballots are `dict` objects,
 mapping the candidate to the ballot's vote for the candidate
 (an `int` in the range 0 to 5 inclusive).
 
 Once you've added all the ballots, call `poll.result` to compute the winner.
 If there's an unbreakable tie, `poll.result` will raise an
-`UnbreakableTieError`.
+`UnbreakableTieError`.  The following scenarios can result in an
+unbreakable tie:
+
+* If the top two candidates tie during the automated runoff round
+  *and* their scores are also a tie.
+* If the second and third candidates during the score round tie,
+  and their preference scores are also a tie.
+* If three or more candiates are tied for first *or* second place
+  during the score round.
+
+(These scenarios are highly unlikely with real-world data.)
 
 If you want to see how the vote was tabulated, pass in an argument
 to the `print` keyword-only argument to `poll.result`.  This should
 be a function that behaves like the builtin `print` function; it
 will only ever be called with positional parameters.
 
 Here's an example of computing a poll between Amy, Brian, and Chuck:
@@ -70,15 +80,15 @@
 If the module is executed as a script, it will read a single
 [CSV file](https://en.wikipedia.org/wiki/Comma-separated_values)
 in [*star.vote*](https://star.vote/) format, tabulate, and print
 the result.  For example, you can run this from the root of the
 source-code repository:
 
 ```
-% python3 -m starvote sample_votes/sample_vote_automatic_runoff_breakable_tie.csv
+% python3 -m starvote sample_polls/sample_vote_automatic_runoff_breakable_tie.csv
 ```
 
 to see how **starvote** handles a tie during the automatic runoff round.
 
 ## Limitations
 
 Currently this module only supports single-winner STAR voting;
@@ -95,7 +105,22 @@
 See the `LICENSE` file.
 
 The source code repository includes sample ballots downloaded from
 [https://star.vote/](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
+## Changelog
+
+**1.1** 2023/05/20
+
+* Bugfix: raise `UnbreakableTieError` if there's a three-way
+  tie for *second* place.  Previously **starvote** only noticed
+  if there was a three-way tie for *first* place.
+* Added sample output for every sample poll in `sample_polls/`.
+  These outputs have been confirmed correct by inspection, and
+  could in the future be used as part of an automated test suite.
+
+**1.0** 2023/05/20
+
+Initial release.
+
```

