# Comparing `tmp/gwcelery-2.0.6.tar.gz` & `tmp/gwcelery-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwcelery-2.0.6.tar", max compression
+gzip compressed data, was "gwcelery-2.1.0.tar", max compression
```

## Comparing `gwcelery-2.0.6.tar` & `gwcelery-2.1.0.tar`

### file list

```diff
@@ -1,229 +1,232 @@
--rw-r--r--   0        0        0    92247 2023-05-10 21:15:58.258618 gwcelery-2.0.6/CHANGES.rst
--rw-r--r--   0        0        0       64 2023-05-08 19:41:16.838727 gwcelery-2.0.6/CONTRIBUTING.rst
--rw-r--r--   0        0        0    19716 2023-05-08 19:41:16.838727 gwcelery-2.0.6/LICENSE.rst
--rw-r--r--   0        0        0     1351 2023-05-08 19:41:16.839727 gwcelery-2.0.6/README.rst
--rw-r--r--   0        0        0      634 2023-05-08 19:41:16.839727 gwcelery-2.0.6/doc/Makefile
--rw-r--r--   0        0        0   191486 2023-05-08 19:41:16.841727 gwcelery-2.0.6/doc/_static/acceptance-tests-checklist.png
--rw-r--r--   0        0        0   241593 2023-05-08 19:41:16.842727 gwcelery-2.0.6/doc/_static/celeryevent-screenshot.png
--rw-r--r--   0        0        0   206465 2023-05-08 19:41:16.844727 gwcelery-2.0.6/doc/_static/deployment-screenshot.png
--rw-r--r--   0        0        0   161306 2023-05-08 19:41:16.845727 gwcelery-2.0.6/doc/_static/flask-screenshot.png
--rw-r--r--   0        0        0   328056 2023-05-08 19:41:16.848727 gwcelery-2.0.6/doc/_static/flower-screenshot.png
--rw-r--r--   0        0        0   114719 2023-05-08 19:41:16.849727 gwcelery-2.0.6/doc/_static/logo-0.5x.png
--rw-r--r--   0        0        0   351955 2023-05-08 19:41:16.851727 gwcelery-2.0.6/doc/_static/logo.png
--rw-r--r--   0        0        0   230777 2023-05-08 19:41:16.853727 gwcelery-2.0.6/doc/_static/sentry-screenshot.png
--rwxr-xr-x   0        0        0     7356 2023-05-08 19:41:16.854728 gwcelery-2.0.6/doc/conf.py
--rw-r--r--   0        0        0     4351 2023-05-08 19:41:16.854728 gwcelery-2.0.6/doc/configuration.rst
--rw-r--r--   0        0        0     5698 2023-05-08 19:41:16.854728 gwcelery-2.0.6/doc/contributing.rst
--rw-r--r--   0        0        0     7204 2023-05-08 19:41:16.854728 gwcelery-2.0.6/doc/deployment.rst
--rw-r--r--   0        0        0    10176 2023-05-08 19:41:16.854728 gwcelery-2.0.6/doc/design.rst
--rw-r--r--   0        0        0      486 2023-05-08 19:41:16.854728 gwcelery-2.0.6/doc/gwcelery.conf.rst
--rw-r--r--   0        0        0      284 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.email.rst
--rw-r--r--   0        0        0      329 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.igwn_alert.rst
--rw-r--r--   0        0        0      227 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.rst
--rw-r--r--   0        0        0       79 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.sentry.rst
--rw-r--r--   0        0        0       97 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.tasks.alerts.rst
--rw-r--r--   0        0        0      103 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.tasks.bayestar.rst
--rw-r--r--   0        0        0      107 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.tasks.circulars.rst
--rw-r--r--   0        0        0       98 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.tasks.condor.rst
--rw-r--r--   0        0        0     2404 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.tasks.detchar.rst
--rw-r--r--   0        0        0     1110 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.em_bright.rst
--rw-r--r--   0        0        0      129 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.external_skymaps.rst
--rw-r--r--   0        0        0     6738 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.external_triggers.rst
--rw-r--r--   0        0        0      112 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.first2years.rst
--rw-r--r--   0        0        0       88 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.gcn.rst
--rw-r--r--   0        0        0      100 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.gracedb.rst
--rw-r--r--   0        0        0      109 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.igwn_alert.rst
--rw-r--r--   0        0        0      109 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.inference.rst
--rw-r--r--   0        0        0     8111 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.orchestrator.rst
--rw-r--r--   0        0        0      100 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.p_astro.rst
--rw-r--r--   0        0        0       94 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tasks.raven.rst
--rw-r--r--   0        0        0      628 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tasks.rst
--rw-r--r--   0        0        0      100 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tasks.skymaps.rst
--rw-r--r--   0        0        0     7161 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tasks.superevents.rst
--rw-r--r--   0        0        0       97 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tools.condor.rst
--rw-r--r--   0        0        0       94 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tools.flask.rst
--rw-r--r--   0        0        0       97 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tools.nagios.rst
--rw-r--r--   0        0        0      185 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tools.rst
--rw-r--r--   0        0        0       73 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.util.rst
--rw-r--r--   0        0        0      507 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.voevent.rst
--rw-r--r--   0        0        0     3564 2023-05-08 19:41:16.858728 gwcelery-2.0.6/doc/htcondor.rst
--rw-r--r--   0        0        0     1576 2023-05-08 19:41:16.858728 gwcelery-2.0.6/doc/index.rst
--rw-r--r--   0        0        0      800 2023-05-08 19:41:16.858728 gwcelery-2.0.6/doc/make.bat
--rw-r--r--   0        0        0     4416 2023-05-08 19:41:16.858728 gwcelery-2.0.6/doc/monitoring.rst
--rw-r--r--   0        0        0     5312 2023-05-08 19:41:16.858728 gwcelery-2.0.6/doc/quickstart.rst
--rw-r--r--   0        0        0     1149 2023-05-08 19:41:16.858728 gwcelery-2.0.6/gwcelery/__init__.py
--rw-r--r--   0        0        0    18447 2023-05-08 19:41:16.859728 gwcelery-2.0.6/gwcelery/_version.py
--rw-r--r--   0        0        0    14975 2023-05-09 19:30:07.793112 gwcelery-2.0.6/gwcelery/conf/__init__.py
--rw-r--r--   0        0        0      403 2023-05-08 19:41:16.859728 gwcelery-2.0.6/gwcelery/conf/development.py
--rw-r--r--   0        0        0     1026 2023-05-08 19:41:16.859728 gwcelery-2.0.6/gwcelery/conf/minikube.py
--rw-r--r--   0        0        0     1722 2023-05-08 19:41:16.859728 gwcelery-2.0.6/gwcelery/conf/playground.py
--rw-r--r--   0        0        0     3541 2023-05-10 21:15:58.259619 gwcelery-2.0.6/gwcelery/conf/production.py
--rw-r--r--   0        0        0     2040 2023-05-08 19:41:16.860728 gwcelery-2.0.6/gwcelery/conf/test.py
--rw-r--r--   0        0        0        0 2023-05-10 21:15:58.344621 gwcelery-2.0.6/gwcelery/data/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 21:15:58.346621 gwcelery-2.0.6/gwcelery/data/first2years/__init__.py
--rw-r--r--   0        0        0   731421 2023-05-08 19:41:16.863728 gwcelery-2.0.6/gwcelery/data/first2years/gstlal.xml.gz
--rwxr-xr-x   0        0        0     2519 2023-05-08 19:41:16.863728 gwcelery-2.0.6/gwcelery/data/gwcelery.sub
--rw-r--r--   0        0        0      505 2023-05-08 19:41:16.863728 gwcelery-2.0.6/gwcelery/email/__init__.py
--rw-r--r--   0        0        0     3317 2023-05-08 19:41:16.863728 gwcelery-2.0.6/gwcelery/email/bootsteps.py
--rw-r--r--   0        0        0      995 2023-05-08 19:41:16.863728 gwcelery-2.0.6/gwcelery/email/signals.py
--rw-r--r--   0        0        0     1457 2023-05-08 19:41:16.863728 gwcelery-2.0.6/gwcelery/flask.py
--rw-r--r--   0        0        0      529 2023-05-08 19:41:16.864728 gwcelery-2.0.6/gwcelery/igwn_alert/__init__.py
--rw-r--r--   0        0        0     4484 2023-05-08 19:41:16.864728 gwcelery-2.0.6/gwcelery/igwn_alert/bootsteps.py
--rw-r--r--   0        0        0      608 2023-05-08 19:41:16.864728 gwcelery-2.0.6/gwcelery/igwn_alert/signals.py
--rw-r--r--   0        0        0      275 2023-05-08 19:41:16.864728 gwcelery-2.0.6/gwcelery/jinja.py
--rw-r--r--   0        0        0      305 2023-05-08 19:41:16.864728 gwcelery-2.0.6/gwcelery/kafka/__init__.py
--rw-r--r--   0        0        0    10431 2023-05-08 19:41:16.864728 gwcelery-2.0.6/gwcelery/kafka/bootsteps.py
--rw-r--r--   0        0        0      522 2023-05-08 19:41:16.864728 gwcelery-2.0.6/gwcelery/kafka/signals.py
--rw-r--r--   0        0        0     2567 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/sentry/__init__.py
--rw-r--r--   0        0        0       34 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/sentry/integrations/__init__.py
--rw-r--r--   0        0        0      832 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/sentry/integrations/condor.py
--rw-r--r--   0        0        0      836 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/sentry/integrations/requests.py
--rw-r--r--   0        0        0      939 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/sentry/integrations/subprocess.py
--rw-r--r--   0        0        0     1302 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/static/typeahead.css
--rw-r--r--   0        0        0     4124 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/static/vega/index.html
--rw-r--r--   0        0        0      515 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/tasks/__init__.py
--rw-r--r--   0        0        0    13067 2023-05-10 21:15:58.260619 gwcelery-2.0.6/gwcelery/tasks/alerts.py
--rw-r--r--   0        0        0     2672 2023-05-08 19:41:16.866728 gwcelery-2.0.6/gwcelery/tasks/bayestar.py
--rw-r--r--   0        0        0     1296 2023-05-08 19:41:16.866728 gwcelery-2.0.6/gwcelery/tasks/circulars.py
--rw-r--r--   0        0        0     7502 2023-05-08 19:41:16.866728 gwcelery-2.0.6/gwcelery/tasks/condor.py
--rw-r--r--   0        0        0     2692 2023-05-08 19:41:16.866728 gwcelery-2.0.6/gwcelery/tasks/core.py
--rw-r--r--   0        0        0    21082 2023-05-09 03:39:39.191337 gwcelery-2.0.6/gwcelery/tasks/detchar.py
--rw-r--r--   0        0        0     4863 2023-05-08 19:41:16.867728 gwcelery-2.0.6/gwcelery/tasks/em_bright.py
--rw-r--r--   0        0        0    21951 2023-05-08 19:41:16.867728 gwcelery-2.0.6/gwcelery/tasks/external_skymaps.py
--rw-r--r--   0        0        0    22552 2023-05-10 21:15:58.261619 gwcelery-2.0.6/gwcelery/tasks/external_triggers.py
--rw-r--r--   0        0        0     6832 2023-05-08 19:41:16.867728 gwcelery-2.0.6/gwcelery/tasks/first2years.py
--rw-r--r--   0        0        0     6384 2023-05-08 19:41:16.868728 gwcelery-2.0.6/gwcelery/tasks/first2years_external.py
--rw-r--r--   0        0        0     4831 2023-05-08 19:41:16.868728 gwcelery-2.0.6/gwcelery/tasks/gcn.py
--rw-r--r--   0        0        0    11079 2023-05-08 19:41:16.868728 gwcelery-2.0.6/gwcelery/tasks/gracedb.py
--rw-r--r--   0        0        0     2453 2023-05-08 19:41:16.868728 gwcelery-2.0.6/gwcelery/tasks/igwn_alert.py
--rw-r--r--   0        0        0    39761 2023-05-08 19:41:16.868728 gwcelery-2.0.6/gwcelery/tasks/inference.py
--rw-r--r--   0        0        0     1406 2023-05-08 19:41:16.869728 gwcelery-2.0.6/gwcelery/tasks/legacy_gracedb.py
--rw-r--r--   0        0        0     7772 2023-05-08 19:41:16.869728 gwcelery-2.0.6/gwcelery/tasks/notice_text.py
--rw-r--r--   0        0        0    46680 2023-05-08 19:41:16.869728 gwcelery-2.0.6/gwcelery/tasks/orchestrator.py
--rw-r--r--   0        0        0     5796 2023-05-08 19:41:16.870728 gwcelery-2.0.6/gwcelery/tasks/p_astro.py
--rw-r--r--   0        0        0    19693 2023-05-08 19:41:16.870728 gwcelery-2.0.6/gwcelery/tasks/raven.py
--rw-r--r--   0        0        0     2242 2023-05-08 19:41:16.870728 gwcelery-2.0.6/gwcelery/tasks/rrt_utils.py
--rw-r--r--   0        0        0    12528 2023-05-08 19:41:16.870728 gwcelery-2.0.6/gwcelery/tasks/skymaps.py
--rw-r--r--   0        0        0    23386 2023-05-08 19:41:16.871728 gwcelery-2.0.6/gwcelery/tasks/superevents.py
--rw-r--r--   0        0        0     1084 2023-05-08 19:41:16.871728 gwcelery-2.0.6/gwcelery/templates/fits_header.jinja2
--rw-r--r--   0        0        0    34059 2023-05-08 19:41:16.871728 gwcelery-2.0.6/gwcelery/templates/index.jinja2
--rw-r--r--   0        0        0     8505 2023-05-08 19:41:16.872728 gwcelery-2.0.6/gwcelery/templates/lalinference.jinja2
--rw-r--r--   0        0        0     8939 2023-05-08 19:41:16.872728 gwcelery-2.0.6/gwcelery/templates/rapidpe.jinja2
--rw-r--r--   0        0        0      806 2023-05-08 19:41:16.872728 gwcelery-2.0.6/gwcelery/templates/vector_table.jinja2
--rw-r--r--   0        0        0        0 2023-05-10 21:15:58.348621 gwcelery-2.0.6/gwcelery/tests/__init__.py
--rw-r--r--   0        0        0     4388 2023-05-08 19:41:16.872728 gwcelery-2.0.6/gwcelery/tests/conftest.py
--rw-r--r--   0        0        0      976 2023-05-08 19:41:16.872728 gwcelery-2.0.6/gwcelery/tests/data/G000012_S0040_preferred.json
--rw-r--r--   0        0        0     6258 2023-05-08 19:41:16.873728 gwcelery-2.0.6/gwcelery/tests/data/G298048-1-Initial.xml
--rw-r--r--   0        0        0      599 2023-05-08 19:41:16.873728 gwcelery-2.0.6/gwcelery/tests/data/G298048_log.json
--rw-r--r--   0        0        0      150 2023-05-08 19:41:16.873728 gwcelery-2.0.6/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
--rw-r--r--   0        0        0      974 2023-05-08 19:41:16.873728 gwcelery-2.0.6/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
--rw-r--r--   0        0        0    17572 2023-05-08 19:41:16.873728 gwcelery-2.0.6/gwcelery/tests/data/MS220722v.xml
--rw-r--r--   0        0        0   777600 2023-05-08 19:41:16.879728 gwcelery-2.0.6/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
--rw-r--r--   0        0        0     8220 2023-05-08 19:41:16.879728 gwcelery-2.0.6/gwcelery/tests/data/S230413b.json
--rw-r--r--   0        0        0     7255 2023-05-08 19:41:16.880728 gwcelery-2.0.6/gwcelery/tests/data/S230413g.json
--rw-r--r--   0        0        0     7721 2023-05-08 19:41:16.880728 gwcelery-2.0.6/gwcelery/tests/data/S230413h.json
--rw-r--r--   0        0        0     3387 2023-05-08 19:41:16.880728 gwcelery-2.0.6/gwcelery/tests/data/T0212_S0039_preferred.json
--rw-r--r--   0        0        0     3384 2023-05-08 19:41:16.880728 gwcelery-2.0.6/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
--rw-r--r--   0        0        0     5210 2023-05-08 19:41:16.880728 gwcelery-2.0.6/gwcelery/tests/data/T0219_S0041_nopreferred.json
--rw-r--r--   0        0        0        0 2023-05-10 21:15:58.349621 gwcelery-2.0.6/gwcelery/tests/data/__init__.py
--rw-r--r--   0        0        0     2290 2023-05-08 19:41:16.880728 gwcelery-2.0.6/gwcelery/tests/data/agile_grb_gcn.xml
--rw-r--r--   0        0        0   854036 2023-05-08 19:41:16.886729 gwcelery-2.0.6/gwcelery/tests/data/coinc.xml
--rw-r--r--   0        0        0     6175 2023-05-08 19:41:16.886729 gwcelery-2.0.6/gwcelery/tests/data/externaltrigger_original_data.xml
--rw-r--r--   0        0        0     5482 2023-05-08 19:41:16.886729 gwcelery-2.0.6/gwcelery/tests/data/fermi_grb_gcn.xml
--rw-r--r--   0        0        0     5469 2023-05-08 19:41:16.886729 gwcelery-2.0.6/gwcelery/tests/data/fermi_initial_grb_gcn.xml
--rw-r--r--   0        0        0     5865 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/fermi_noise_gcn.xml
--rw-r--r--   0        0        0     5864 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/fermi_noise_gcn_2.xml
--rw-r--r--   0        0        0     4914 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
--rw-r--r--   0        0        0     4914 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
--rw-r--r--   0        0        0     3407 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/fits_header_result.html
--rw-r--r--   0        0        0      882 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/gracedb_externaltrigger_log.json
--rw-r--r--   0        0        0      446 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/gracedb_setrigger_log.json
--rw-r--r--   0        0        0      870 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_detchar.json
--rw-r--r--   0        0        0     2025 2023-05-08 19:41:16.888729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_exttrig_creation.json
--rw-r--r--   0        0        0     2007 2023-05-08 19:41:16.888729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
--rw-r--r--   0        0        0      166 2023-05-08 19:41:16.888729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_fits.json
--rw-r--r--   0        0        0      101 2023-05-08 19:41:16.888729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_label_dqv.json
--rw-r--r--   0        0        0      743 2023-05-08 19:41:16.888729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_psd.json
--rw-r--r--   0        0        0     2020 2023-05-08 19:41:16.888729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_snews_creation.json
--rw-r--r--   0        0        0     2012 2023-05-08 19:41:16.888729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_snews_test_creation.json
--rw-r--r--   0        0        0     2028 2023-05-08 19:41:16.889729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_subgrb_creation.json
--rw-r--r--   0        0        0     1235 2023-05-08 19:41:16.889729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_superevent_creation.json
--rw-r--r--   0        0        0      107 2023-05-08 19:41:16.889729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_superevent_label.json
--rw-r--r--   0        0        0     5021 2023-05-08 19:41:16.889729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_voevent.json
--rw-r--r--   0        0        0     4429 2023-05-08 19:41:16.889729 gwcelery-2.0.6/gwcelery/tests/data/integral_grb_gcn.xml
--rw-r--r--   0        0        0     4295 2023-05-08 19:41:16.889729 gwcelery-2.0.6/gwcelery/tests/data/integral_mdc_gcn.xml
--rw-r--r--   0        0        0        0 2023-05-10 21:15:58.350622 gwcelery-2.0.6/gwcelery/tests/data/llhoft/__init__.py
--rw-r--r--   0        0        0    14622 2023-05-08 19:41:16.890729 gwcelery-2.0.6/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-05-10 21:15:58.350622 gwcelery-2.0.6/gwcelery/tests/data/llhoft/fail/L1/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 21:15:58.350622 gwcelery-2.0.6/gwcelery/tests/data/llhoft/fail/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 21:15:58.350622 gwcelery-2.0.6/gwcelery/tests/data/llhoft/omegascan/__init__.py
--rw-r--r--   0        0        0   516419 2023-05-08 19:41:16.891729 gwcelery-2.0.6/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
--rw-r--r--   0        0        0    14630 2023-05-08 19:41:16.892729 gwcelery-2.0.6/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-05-10 21:15:58.350622 gwcelery-2.0.6/gwcelery/tests/data/llhoft/pass/H1/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 21:15:58.350622 gwcelery-2.0.6/gwcelery/tests/data/llhoft/pass/__init__.py
--rw-r--r--   0        0        0    13099 2023-05-08 19:41:16.892729 gwcelery-2.0.6/gwcelery/tests/data/lvalert_event_creation.json
--rw-r--r--   0        0        0     9060 2023-05-08 19:41:16.892729 gwcelery-2.0.6/gwcelery/tests/data/lvalert_xmpp.xml
--rw-r--r--   0        0        0      864 2023-05-08 19:41:16.892729 gwcelery-2.0.6/gwcelery/tests/data/mock_superevent_object.json
--rw-r--r--   0        0        0   445440 2023-05-08 19:41:16.894729 gwcelery-2.0.6/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
--rw-r--r--   0        0        0   294426 2023-05-08 19:41:16.895729 gwcelery-2.0.6/gwcelery/tests/data/psd.xml.gz
--rw-r--r--   0        0        0    11520 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/rrt_small_area.fits
--rw-r--r--   0        0        0     2964 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/sample_events.json
--rw-r--r--   0        0        0     3648 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/samples.hdf5
--rw-r--r--   0        0        0      616 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/scaler_set_all.pickle
--rw-r--r--   0        0        0     6169 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/snews_gcn.xml
--rw-r--r--   0        0        0     6161 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/snews_gcn_test.xml
--rw-r--r--   0        0        0     9583 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/superevents.json
--rw-r--r--   0        0        0     7713 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/swift_grb_gcn.xml
--rw-r--r--   0        0        0   581918 2023-05-08 19:41:16.899729 gwcelery-2.0.6/gwcelery/tests/data/test_classifier.pickle
--rw-r--r--   0        0        0     4042 2023-05-08 19:41:16.899729 gwcelery-2.0.6/gwcelery/tests/process.py
--rw-r--r--   0        0        0     2307 2023-05-08 19:41:16.900729 gwcelery-2.0.6/gwcelery/tests/test_sentry.py
--rw-r--r--   0        0        0     1705 2023-05-08 19:41:16.900729 gwcelery-2.0.6/gwcelery/tests/test_tasks_alerts.py
--rw-r--r--   0        0        0     4916 2023-05-08 19:41:16.900729 gwcelery-2.0.6/gwcelery/tests/test_tasks_alerts_validate.py
--rw-r--r--   0        0        0     1439 2023-05-08 19:41:16.900729 gwcelery-2.0.6/gwcelery/tests/test_tasks_bayestar.py
--rw-r--r--   0        0        0     2416 2023-05-08 19:41:16.900729 gwcelery-2.0.6/gwcelery/tests/test_tasks_circulars.py
--rw-r--r--   0        0        0     4550 2023-05-08 19:41:16.900729 gwcelery-2.0.6/gwcelery/tests/test_tasks_condor.py
--rw-r--r--   0        0        0    11688 2023-05-08 19:41:16.901729 gwcelery-2.0.6/gwcelery/tests/test_tasks_detchar.py
--rw-r--r--   0        0        0     2317 2023-05-08 19:41:16.901729 gwcelery-2.0.6/gwcelery/tests/test_tasks_em_bright.py
--rw-r--r--   0        0        0    12322 2023-05-08 19:41:16.901729 gwcelery-2.0.6/gwcelery/tests/test_tasks_external_skymaps.py
--rw-r--r--   0        0        0    32406 2023-05-10 21:15:58.262619 gwcelery-2.0.6/gwcelery/tests/test_tasks_external_triggers.py
--rw-r--r--   0        0        0     1816 2023-05-08 19:41:16.901729 gwcelery-2.0.6/gwcelery/tests/test_tasks_first2years.py
--rw-r--r--   0        0        0     4555 2023-05-08 19:41:16.901729 gwcelery-2.0.6/gwcelery/tests/test_tasks_first2years_external.py
--rw-r--r--   0        0        0     1826 2023-05-08 19:41:16.902729 gwcelery-2.0.6/gwcelery/tests/test_tasks_gcn.py
--rw-r--r--   0        0        0     1655 2023-05-08 19:41:16.902729 gwcelery-2.0.6/gwcelery/tests/test_tasks_gcn_validate.py
--rw-r--r--   0        0        0     5739 2023-05-08 19:41:16.902729 gwcelery-2.0.6/gwcelery/tests/test_tasks_gracedb.py
--rw-r--r--   0        0        0     3662 2023-05-08 19:41:16.902729 gwcelery-2.0.6/gwcelery/tests/test_tasks_igwn_alert.py
--rw-r--r--   0        0        0    21593 2023-05-08 19:41:16.903729 gwcelery-2.0.6/gwcelery/tests/test_tasks_inference.py
--rw-r--r--   0        0        0    33299 2023-05-08 19:41:16.903729 gwcelery-2.0.6/gwcelery/tests/test_tasks_orchestrator.py
--rw-r--r--   0        0        0     1647 2023-05-08 19:41:16.903729 gwcelery-2.0.6/gwcelery/tests/test_tasks_p_astro.py
--rw-r--r--   0        0        0    26044 2023-05-08 19:41:16.904729 gwcelery-2.0.6/gwcelery/tests/test_tasks_raven.py
--rw-r--r--   0        0        0     4724 2023-05-08 19:41:16.904729 gwcelery-2.0.6/gwcelery/tests/test_tasks_rrt_utils.py
--rw-r--r--   0        0        0     5035 2023-05-08 19:41:16.904729 gwcelery-2.0.6/gwcelery/tests/test_tasks_skymaps.py
--rw-r--r--   0        0        0    39981 2023-05-08 19:41:16.904729 gwcelery-2.0.6/gwcelery/tests/test_tasks_superevents.py
--rw-r--r--   0        0        0      637 2023-05-08 19:41:16.905729 gwcelery-2.0.6/gwcelery/tests/test_tempfile.py
--rw-r--r--   0        0        0     3520 2023-05-08 19:41:16.905729 gwcelery-2.0.6/gwcelery/tests/test_tools_condor.py
--rw-r--r--   0        0        0     1098 2023-05-08 19:41:16.905729 gwcelery-2.0.6/gwcelery/tests/test_tools_condor_submit_helper.py
--rw-r--r--   0        0        0      633 2023-05-08 19:41:16.905729 gwcelery-2.0.6/gwcelery/tests/test_tools_flask.py
--rw-r--r--   0        0        0     9658 2023-05-08 19:41:16.905729 gwcelery-2.0.6/gwcelery/tests/test_tools_nagios.py
--rw-r--r--   0        0        0      269 2023-05-08 19:41:16.905729 gwcelery-2.0.6/gwcelery/tests/test_util.py
--rw-r--r--   0        0        0    21450 2023-05-08 19:41:16.905729 gwcelery-2.0.6/gwcelery/tests/test_views.py
--rw-r--r--   0        0        0      216 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/tools/__init__.py
--rw-r--r--   0        0        0     2948 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/tools/condor.py
--rw-r--r--   0        0        0     1120 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/tools/condor_submit_helper.py
--rw-r--r--   0        0        0     1938 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/tools/flask.py
--rw-r--r--   0        0        0     6624 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/tools/nagios.py
--rw-r--r--   0        0        0      413 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/util/__init__.py
--rw-r--r--   0        0        0     1007 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/util/cmdline.py
--rw-r--r--   0        0        0      453 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/util/matplotlib.py
--rw-r--r--   0        0        0      390 2023-05-08 19:41:16.907729 gwcelery-2.0.6/gwcelery/util/proxy.py
--rw-r--r--   0        0        0      514 2023-05-08 19:41:16.907729 gwcelery-2.0.6/gwcelery/util/resources.py
--rw-r--r--   0        0        0      253 2023-05-08 19:41:16.907729 gwcelery-2.0.6/gwcelery/util/sphinx.py
--rw-r--r--   0        0        0      941 2023-05-08 19:41:16.907729 gwcelery-2.0.6/gwcelery/util/tempfile.py
--rw-r--r--   0        0        0    18472 2023-05-08 19:41:16.907729 gwcelery-2.0.6/gwcelery/views.py
--rw-r--r--   0        0        0      365 2023-05-08 19:41:16.907729 gwcelery-2.0.6/gwcelery/voevent/__init__.py
--rw-r--r--   0        0        0     6387 2023-05-08 19:41:16.908729 gwcelery-2.0.6/gwcelery/voevent/bootsteps.py
--rw-r--r--   0        0        0     1063 2023-05-08 19:41:16.908729 gwcelery-2.0.6/gwcelery/voevent/logging.py
--rw-r--r--   0        0        0      779 2023-05-08 19:41:16.908729 gwcelery-2.0.6/gwcelery/voevent/signals.py
--rw-r--r--   0        0        0      852 2023-05-08 19:41:16.908729 gwcelery-2.0.6/gwcelery/voevent/subscriber.py
--rw-r--r--   0        0        0     1454 2023-05-08 19:41:16.908729 gwcelery-2.0.6/gwcelery/voevent/util.py
--rw-r--r--   0        0        0     5956 2023-05-10 21:16:17.400233 gwcelery-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     4628 1970-01-01 00:00:00.000000 gwcelery-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0    94846 2023-05-20 06:06:22.743731 gwcelery-2.1.0/CHANGES.rst
+-rw-r--r--   0        0        0       64 2023-05-18 19:27:39.643149 gwcelery-2.1.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0    19716 2023-05-18 19:27:39.643149 gwcelery-2.1.0/LICENSE.rst
+-rw-r--r--   0        0        0     1351 2023-05-18 19:27:39.643149 gwcelery-2.1.0/README.rst
+-rw-r--r--   0        0        0      634 2023-05-18 19:27:39.644149 gwcelery-2.1.0/doc/Makefile
+-rw-r--r--   0        0        0   191486 2023-05-18 19:27:39.645149 gwcelery-2.1.0/doc/_static/acceptance-tests-checklist.png
+-rw-r--r--   0        0        0   241593 2023-05-18 19:27:39.647149 gwcelery-2.1.0/doc/_static/celeryevent-screenshot.png
+-rw-r--r--   0        0        0   206465 2023-05-18 19:27:39.649149 gwcelery-2.1.0/doc/_static/deployment-screenshot.png
+-rw-r--r--   0        0        0   161306 2023-05-18 19:27:39.650149 gwcelery-2.1.0/doc/_static/flask-screenshot.png
+-rw-r--r--   0        0        0   328056 2023-05-18 19:27:39.653149 gwcelery-2.1.0/doc/_static/flower-screenshot.png
+-rw-r--r--   0        0        0   114719 2023-05-18 19:27:39.654149 gwcelery-2.1.0/doc/_static/logo-0.5x.png
+-rw-r--r--   0        0        0   351955 2023-05-18 19:27:39.657150 gwcelery-2.1.0/doc/_static/logo.png
+-rw-r--r--   0        0        0   230777 2023-05-18 19:27:39.659150 gwcelery-2.1.0/doc/_static/sentry-screenshot.png
+-rwxr-xr-x   0        0        0     7356 2023-05-18 19:27:39.659150 gwcelery-2.1.0/doc/conf.py
+-rw-r--r--   0        0        0     4346 2023-05-18 19:27:39.659150 gwcelery-2.1.0/doc/configuration.rst
+-rw-r--r--   0        0        0     5698 2023-05-18 19:27:39.659150 gwcelery-2.1.0/doc/contributing.rst
+-rw-r--r--   0        0        0     7202 2023-05-18 19:27:39.659150 gwcelery-2.1.0/doc/deployment.rst
+-rw-r--r--   0        0        0    10176 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/design.rst
+-rw-r--r--   0        0        0      486 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.conf.rst
+-rw-r--r--   0        0        0      284 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.email.rst
+-rw-r--r--   0        0        0      329 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.igwn_alert.rst
+-rw-r--r--   0        0        0      227 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.rst
+-rw-r--r--   0        0        0       79 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.sentry.rst
+-rw-r--r--   0        0        0       97 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.tasks.alerts.rst
+-rw-r--r--   0        0        0      103 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.tasks.bayestar.rst
+-rw-r--r--   0        0        0      107 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.tasks.circulars.rst
+-rw-r--r--   0        0        0       98 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.tasks.condor.rst
+-rw-r--r--   0        0        0     2404 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.tasks.detchar.rst
+-rw-r--r--   0        0        0     1110 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.em_bright.rst
+-rw-r--r--   0        0        0      129 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.external_skymaps.rst
+-rw-r--r--   0        0        0     6738 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.external_triggers.rst
+-rw-r--r--   0        0        0      112 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.first2years.rst
+-rw-r--r--   0        0        0       88 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.gcn.rst
+-rw-r--r--   0        0        0      100 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.gracedb.rst
+-rw-r--r--   0        0        0      109 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.igwn_alert.rst
+-rw-r--r--   0        0        0      109 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.inference.rst
+-rw-r--r--   0        0        0     8111 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.orchestrator.rst
+-rw-r--r--   0        0        0      100 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.p_astro.rst
+-rw-r--r--   0        0        0       94 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.raven.rst
+-rw-r--r--   0        0        0      628 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.tasks.rst
+-rw-r--r--   0        0        0      100 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.tasks.skymaps.rst
+-rw-r--r--   0        0        0     7161 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.tasks.superevents.rst
+-rw-r--r--   0        0        0       97 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.tools.condor.rst
+-rw-r--r--   0        0        0       94 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.tools.flask.rst
+-rw-r--r--   0        0        0       97 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.tools.nagios.rst
+-rw-r--r--   0        0        0      185 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.tools.rst
+-rw-r--r--   0        0        0       73 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.util.rst
+-rw-r--r--   0        0        0      507 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.voevent.rst
+-rw-r--r--   0        0        0     3564 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/htcondor.rst
+-rw-r--r--   0        0        0     1576 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/index.rst
+-rw-r--r--   0        0        0      800 2023-05-18 19:27:39.663150 gwcelery-2.1.0/doc/make.bat
+-rw-r--r--   0        0        0     4416 2023-05-18 19:27:39.663150 gwcelery-2.1.0/doc/monitoring.rst
+-rw-r--r--   0        0        0     5312 2023-05-18 19:27:39.663150 gwcelery-2.1.0/doc/quickstart.rst
+-rw-r--r--   0        0        0     1149 2023-05-18 19:27:39.663150 gwcelery-2.1.0/gwcelery/__init__.py
+-rw-r--r--   0        0        0    18447 2023-05-18 19:27:39.663150 gwcelery-2.1.0/gwcelery/_version.py
+-rw-r--r--   0        0        0    15596 2023-05-19 03:09:23.772937 gwcelery-2.1.0/gwcelery/conf/__init__.py
+-rw-r--r--   0        0        0     1014 2023-05-18 19:27:39.664150 gwcelery-2.1.0/gwcelery/conf/dev.py
+-rw-r--r--   0        0        0      403 2023-05-18 19:27:39.664150 gwcelery-2.1.0/gwcelery/conf/development.py
+-rw-r--r--   0        0        0     1026 2023-05-18 19:27:39.664150 gwcelery-2.1.0/gwcelery/conf/minikube.py
+-rw-r--r--   0        0        0     1722 2023-05-18 19:27:39.664150 gwcelery-2.1.0/gwcelery/conf/playground.py
+-rw-r--r--   0        0        0     3541 2023-05-18 19:27:39.664150 gwcelery-2.1.0/gwcelery/conf/production.py
+-rw-r--r--   0        0        0     2040 2023-05-18 19:27:39.664150 gwcelery-2.1.0/gwcelery/conf/test.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:06:22.811733 gwcelery-2.1.0/gwcelery/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:06:22.813733 gwcelery-2.1.0/gwcelery/data/first2years/__init__.py
+-rw-r--r--   0        0        0   731421 2023-05-18 19:27:39.667150 gwcelery-2.1.0/gwcelery/data/first2years/gstlal.xml.gz
+-rwxr-xr-x   0        0        0     2785 2023-05-18 19:27:39.668150 gwcelery-2.1.0/gwcelery/data/gwcelery.sub
+-rw-r--r--   0        0        0      505 2023-05-18 19:27:39.668150 gwcelery-2.1.0/gwcelery/email/__init__.py
+-rw-r--r--   0        0        0     3317 2023-05-18 19:27:39.668150 gwcelery-2.1.0/gwcelery/email/bootsteps.py
+-rw-r--r--   0        0        0      995 2023-05-18 19:27:39.668150 gwcelery-2.1.0/gwcelery/email/signals.py
+-rw-r--r--   0        0        0     1457 2023-05-18 19:27:39.668150 gwcelery-2.1.0/gwcelery/flask.py
+-rw-r--r--   0        0        0      529 2023-05-18 19:27:39.668150 gwcelery-2.1.0/gwcelery/igwn_alert/__init__.py
+-rw-r--r--   0        0        0     4484 2023-05-18 19:27:39.668150 gwcelery-2.1.0/gwcelery/igwn_alert/bootsteps.py
+-rw-r--r--   0        0        0      608 2023-05-18 19:27:39.669150 gwcelery-2.1.0/gwcelery/igwn_alert/signals.py
+-rw-r--r--   0        0        0      275 2023-05-18 19:27:39.669150 gwcelery-2.1.0/gwcelery/jinja.py
+-rw-r--r--   0        0        0      305 2023-05-18 19:27:39.669150 gwcelery-2.1.0/gwcelery/kafka/__init__.py
+-rw-r--r--   0        0        0    10431 2023-05-18 19:27:39.669150 gwcelery-2.1.0/gwcelery/kafka/bootsteps.py
+-rw-r--r--   0        0        0      522 2023-05-18 19:27:39.669150 gwcelery-2.1.0/gwcelery/kafka/signals.py
+-rw-r--r--   0        0        0     2567 2023-05-18 19:27:39.669150 gwcelery-2.1.0/gwcelery/sentry/__init__.py
+-rw-r--r--   0        0        0       34 2023-05-18 19:27:39.669150 gwcelery-2.1.0/gwcelery/sentry/integrations/__init__.py
+-rw-r--r--   0        0        0      832 2023-05-18 19:27:39.670150 gwcelery-2.1.0/gwcelery/sentry/integrations/condor.py
+-rw-r--r--   0        0        0      836 2023-05-18 19:27:39.670150 gwcelery-2.1.0/gwcelery/sentry/integrations/requests.py
+-rw-r--r--   0        0        0      939 2023-05-18 19:27:39.670150 gwcelery-2.1.0/gwcelery/sentry/integrations/subprocess.py
+-rw-r--r--   0        0        0     1302 2023-05-18 19:27:39.670150 gwcelery-2.1.0/gwcelery/static/typeahead.css
+-rw-r--r--   0        0        0     4124 2023-05-18 19:27:39.670150 gwcelery-2.1.0/gwcelery/static/vega/index.html
+-rw-r--r--   0        0        0      515 2023-05-18 19:27:39.670150 gwcelery-2.1.0/gwcelery/tasks/__init__.py
+-rw-r--r--   0        0        0    13597 2023-05-19 06:44:52.288984 gwcelery-2.1.0/gwcelery/tasks/alerts.py
+-rw-r--r--   0        0        0     2672 2023-05-18 19:27:39.671150 gwcelery-2.1.0/gwcelery/tasks/bayestar.py
+-rw-r--r--   0        0        0     1535 2023-05-19 06:44:52.288984 gwcelery-2.1.0/gwcelery/tasks/circulars.py
+-rw-r--r--   0        0        0     7502 2023-05-18 19:27:39.671150 gwcelery-2.1.0/gwcelery/tasks/condor.py
+-rw-r--r--   0        0        0     2692 2023-05-18 19:27:39.671150 gwcelery-2.1.0/gwcelery/tasks/core.py
+-rw-r--r--   0        0        0    21515 2023-05-19 21:39:54.349367 gwcelery-2.1.0/gwcelery/tasks/detchar.py
+-rw-r--r--   0        0        0     4863 2023-05-18 19:27:39.671150 gwcelery-2.1.0/gwcelery/tasks/em_bright.py
+-rw-r--r--   0        0        0    21951 2023-05-18 19:27:39.672150 gwcelery-2.1.0/gwcelery/tasks/external_skymaps.py
+-rw-r--r--   0        0        0    23806 2023-05-20 00:18:20.105305 gwcelery-2.1.0/gwcelery/tasks/external_triggers.py
+-rw-r--r--   0        0        0     6832 2023-05-18 19:27:39.672150 gwcelery-2.1.0/gwcelery/tasks/first2years.py
+-rw-r--r--   0        0        0     6384 2023-05-18 19:27:39.672150 gwcelery-2.1.0/gwcelery/tasks/first2years_external.py
+-rw-r--r--   0        0        0     4831 2023-05-18 19:27:39.672150 gwcelery-2.1.0/gwcelery/tasks/gcn.py
+-rw-r--r--   0        0        0    11079 2023-05-18 19:27:39.673150 gwcelery-2.1.0/gwcelery/tasks/gracedb.py
+-rw-r--r--   0        0        0     6105 2023-05-19 19:57:48.392739 gwcelery-2.1.0/gwcelery/tasks/gwskynet.py
+-rw-r--r--   0        0        0     2453 2023-05-18 19:27:39.673150 gwcelery-2.1.0/gwcelery/tasks/igwn_alert.py
+-rw-r--r--   0        0        0    41859 2023-05-20 02:48:26.929777 gwcelery-2.1.0/gwcelery/tasks/inference.py
+-rw-r--r--   0        0        0     1406 2023-05-18 19:27:39.673150 gwcelery-2.1.0/gwcelery/tasks/legacy_gracedb.py
+-rw-r--r--   0        0        0     7772 2023-05-18 19:27:39.674150 gwcelery-2.1.0/gwcelery/tasks/notice_text.py
+-rw-r--r--   0        0        0    46819 2023-05-19 16:53:56.117563 gwcelery-2.1.0/gwcelery/tasks/orchestrator.py
+-rw-r--r--   0        0        0     5796 2023-05-18 19:27:39.674150 gwcelery-2.1.0/gwcelery/tasks/p_astro.py
+-rw-r--r--   0        0        0    20999 2023-05-20 00:18:20.106305 gwcelery-2.1.0/gwcelery/tasks/raven.py
+-rw-r--r--   0        0        0     2242 2023-05-18 19:27:39.675150 gwcelery-2.1.0/gwcelery/tasks/rrt_utils.py
+-rw-r--r--   0        0        0    12528 2023-05-18 19:27:39.675150 gwcelery-2.1.0/gwcelery/tasks/skymaps.py
+-rw-r--r--   0        0        0    23631 2023-05-18 19:27:39.675150 gwcelery-2.1.0/gwcelery/tasks/superevents.py
+-rw-r--r--   0        0        0     1084 2023-05-18 19:27:39.676150 gwcelery-2.1.0/gwcelery/templates/fits_header.jinja2
+-rw-r--r--   0        0        0    35556 2023-05-19 06:44:52.290984 gwcelery-2.1.0/gwcelery/templates/index.jinja2
+-rw-r--r--   0        0        0     8505 2023-05-18 19:27:39.676150 gwcelery-2.1.0/gwcelery/templates/lalinference.jinja2
+-rw-r--r--   0        0        0     9496 2023-05-19 03:09:23.773937 gwcelery-2.1.0/gwcelery/templates/rapidpe.jinja2
+-rw-r--r--   0        0        0      806 2023-05-18 19:27:39.676150 gwcelery-2.1.0/gwcelery/templates/vector_table.jinja2
+-rw-r--r--   0        0        0        0 2023-05-20 06:06:22.815733 gwcelery-2.1.0/gwcelery/tests/__init__.py
+-rw-r--r--   0        0        0     4388 2023-05-18 19:27:39.677150 gwcelery-2.1.0/gwcelery/tests/conftest.py
+-rw-r--r--   0        0        0      976 2023-05-18 19:27:39.677150 gwcelery-2.1.0/gwcelery/tests/data/G000012_S0040_preferred.json
+-rw-r--r--   0        0        0     6258 2023-05-18 19:27:39.677150 gwcelery-2.1.0/gwcelery/tests/data/G298048-1-Initial.xml
+-rw-r--r--   0        0        0      599 2023-05-18 19:27:39.677150 gwcelery-2.1.0/gwcelery/tests/data/G298048_log.json
+-rw-r--r--   0        0        0      150 2023-05-18 19:27:39.677150 gwcelery-2.1.0/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
+-rw-r--r--   0        0        0      974 2023-05-18 19:27:39.677150 gwcelery-2.1.0/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
+-rw-r--r--   0        0        0    17572 2023-05-18 19:27:39.677150 gwcelery-2.1.0/gwcelery/tests/data/MS220722v.xml
+-rw-r--r--   0        0        0   777600 2023-05-18 19:27:39.683150 gwcelery-2.1.0/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
+-rw-r--r--   0        0        0     8220 2023-05-18 19:27:39.683150 gwcelery-2.1.0/gwcelery/tests/data/S230413b.json
+-rw-r--r--   0        0        0     7255 2023-05-18 19:27:39.683150 gwcelery-2.1.0/gwcelery/tests/data/S230413g.json
+-rw-r--r--   0        0        0     7721 2023-05-18 19:27:39.683150 gwcelery-2.1.0/gwcelery/tests/data/S230413h.json
+-rw-r--r--   0        0        0     3387 2023-05-18 19:27:39.683150 gwcelery-2.1.0/gwcelery/tests/data/T0212_S0039_preferred.json
+-rw-r--r--   0        0        0     3384 2023-05-18 19:27:39.683150 gwcelery-2.1.0/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
+-rw-r--r--   0        0        0     5210 2023-05-18 19:27:39.683150 gwcelery-2.1.0/gwcelery/tests/data/T0219_S0041_nopreferred.json
+-rw-r--r--   0        0        0        0 2023-05-20 06:06:22.815733 gwcelery-2.1.0/gwcelery/tests/data/__init__.py
+-rw-r--r--   0        0        0     2290 2023-05-18 19:27:39.684150 gwcelery-2.1.0/gwcelery/tests/data/agile_grb_gcn.xml
+-rw-r--r--   0        0        0   854036 2023-05-18 19:27:39.689151 gwcelery-2.1.0/gwcelery/tests/data/coinc.xml
+-rw-r--r--   0        0        0     6175 2023-05-18 19:27:39.689151 gwcelery-2.1.0/gwcelery/tests/data/externaltrigger_original_data.xml
+-rw-r--r--   0        0        0     5482 2023-05-18 19:27:39.689151 gwcelery-2.1.0/gwcelery/tests/data/fermi_grb_gcn.xml
+-rw-r--r--   0        0        0     5469 2023-05-18 19:27:39.689151 gwcelery-2.1.0/gwcelery/tests/data/fermi_initial_grb_gcn.xml
+-rw-r--r--   0        0        0     5865 2023-05-18 19:27:39.689151 gwcelery-2.1.0/gwcelery/tests/data/fermi_noise_gcn.xml
+-rw-r--r--   0        0        0     5864 2023-05-18 19:27:39.689151 gwcelery-2.1.0/gwcelery/tests/data/fermi_noise_gcn_2.xml
+-rw-r--r--   0        0        0     4914 2023-05-18 19:27:39.689151 gwcelery-2.1.0/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
+-rw-r--r--   0        0        0     4914 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
+-rw-r--r--   0        0        0     3407 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/fits_header_result.html
+-rw-r--r--   0        0        0      882 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/gracedb_externaltrigger_log.json
+-rw-r--r--   0        0        0      446 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/gracedb_setrigger_log.json
+-rw-r--r--   0        0        0      870 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_detchar.json
+-rw-r--r--   0        0        0     2025 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_exttrig_creation.json
+-rw-r--r--   0        0        0     2007 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
+-rw-r--r--   0        0        0      166 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_fits.json
+-rw-r--r--   0        0        0      101 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_label_dqv.json
+-rw-r--r--   0        0        0      743 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_psd.json
+-rw-r--r--   0        0        0     2020 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_snews_creation.json
+-rw-r--r--   0        0        0     2012 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_snews_test_creation.json
+-rw-r--r--   0        0        0     2028 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_subgrb_creation.json
+-rw-r--r--   0        0        0     1235 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_superevent_creation.json
+-rw-r--r--   0        0        0      107 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_superevent_label.json
+-rw-r--r--   0        0        0     5021 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_voevent.json
+-rw-r--r--   0        0        0     4429 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/integral_grb_gcn.xml
+-rw-r--r--   0        0        0     4295 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/integral_mdc_gcn.xml
+-rw-r--r--   0        0        0        0 2023-05-20 06:06:22.817733 gwcelery-2.1.0/gwcelery/tests/data/llhoft/__init__.py
+-rw-r--r--   0        0        0    14614 2023-05-18 19:27:39.692151 gwcelery-2.1.0/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-05-20 06:06:22.817733 gwcelery-2.1.0/gwcelery/tests/data/llhoft/fail/L1/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:06:22.817733 gwcelery-2.1.0/gwcelery/tests/data/llhoft/fail/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:06:22.817733 gwcelery-2.1.0/gwcelery/tests/data/llhoft/omegascan/__init__.py
+-rw-r--r--   0        0        0   516419 2023-05-18 19:27:39.693151 gwcelery-2.1.0/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
+-rw-r--r--   0        0        0    14630 2023-05-18 19:27:39.694151 gwcelery-2.1.0/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-05-20 06:06:22.818733 gwcelery-2.1.0/gwcelery/tests/data/llhoft/pass/H1/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:06:22.818733 gwcelery-2.1.0/gwcelery/tests/data/llhoft/pass/__init__.py
+-rw-r--r--   0        0        0    13099 2023-05-18 19:27:39.694151 gwcelery-2.1.0/gwcelery/tests/data/lvalert_event_creation.json
+-rw-r--r--   0        0        0     9060 2023-05-18 19:27:39.694151 gwcelery-2.1.0/gwcelery/tests/data/lvalert_xmpp.xml
+-rw-r--r--   0        0        0      864 2023-05-18 19:27:39.694151 gwcelery-2.1.0/gwcelery/tests/data/mock_superevent_object.json
+-rw-r--r--   0        0        0   445440 2023-05-18 19:27:39.696151 gwcelery-2.1.0/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
+-rw-r--r--   0        0        0   294426 2023-05-18 19:27:39.697151 gwcelery-2.1.0/gwcelery/tests/data/psd.xml.gz
+-rw-r--r--   0        0        0    11520 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/rrt_small_area.fits
+-rw-r--r--   0        0        0     2964 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/sample_events.json
+-rw-r--r--   0        0        0     3648 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/samples.hdf5
+-rw-r--r--   0        0        0      616 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/scaler_set_all.pickle
+-rw-r--r--   0        0        0     6169 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/snews_gcn.xml
+-rw-r--r--   0        0        0     6161 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/snews_gcn_test.xml
+-rw-r--r--   0        0        0     9583 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/superevents.json
+-rw-r--r--   0        0        0     7713 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/swift_grb_gcn.xml
+-rw-r--r--   0        0        0   581918 2023-05-18 19:27:39.701151 gwcelery-2.1.0/gwcelery/tests/data/test_classifier.pickle
+-rw-r--r--   0        0        0     4042 2023-05-18 19:27:39.701151 gwcelery-2.1.0/gwcelery/tests/process.py
+-rw-r--r--   0        0        0     2307 2023-05-18 19:27:39.702151 gwcelery-2.1.0/gwcelery/tests/test_sentry.py
+-rw-r--r--   0        0        0     1705 2023-05-18 19:27:39.702151 gwcelery-2.1.0/gwcelery/tests/test_tasks_alerts.py
+-rw-r--r--   0        0        0     4916 2023-05-18 19:27:39.702151 gwcelery-2.1.0/gwcelery/tests/test_tasks_alerts_validate.py
+-rw-r--r--   0        0        0     1439 2023-05-18 19:27:39.702151 gwcelery-2.1.0/gwcelery/tests/test_tasks_bayestar.py
+-rw-r--r--   0        0        0     3007 2023-05-19 06:44:52.291984 gwcelery-2.1.0/gwcelery/tests/test_tasks_circulars.py
+-rw-r--r--   0        0        0     4550 2023-05-18 19:27:39.702151 gwcelery-2.1.0/gwcelery/tests/test_tasks_condor.py
+-rw-r--r--   0        0        0    15811 2023-05-19 21:39:54.350367 gwcelery-2.1.0/gwcelery/tests/test_tasks_detchar.py
+-rw-r--r--   0        0        0     2317 2023-05-18 19:27:39.703151 gwcelery-2.1.0/gwcelery/tests/test_tasks_em_bright.py
+-rw-r--r--   0        0        0    12322 2023-05-18 19:27:39.703151 gwcelery-2.1.0/gwcelery/tests/test_tasks_external_skymaps.py
+-rw-r--r--   0        0        0    34773 2023-05-20 00:18:20.108305 gwcelery-2.1.0/gwcelery/tests/test_tasks_external_triggers.py
+-rw-r--r--   0        0        0     1816 2023-05-18 19:27:39.703151 gwcelery-2.1.0/gwcelery/tests/test_tasks_first2years.py
+-rw-r--r--   0        0        0     4555 2023-05-18 19:27:39.703151 gwcelery-2.1.0/gwcelery/tests/test_tasks_first2years_external.py
+-rw-r--r--   0        0        0     1826 2023-05-18 19:27:39.703151 gwcelery-2.1.0/gwcelery/tests/test_tasks_gcn.py
+-rw-r--r--   0        0        0     1655 2023-05-18 19:27:39.704151 gwcelery-2.1.0/gwcelery/tests/test_tasks_gcn_validate.py
+-rw-r--r--   0        0        0     5739 2023-05-18 19:27:39.704151 gwcelery-2.1.0/gwcelery/tests/test_tasks_gracedb.py
+-rw-r--r--   0        0        0     9591 2023-05-18 19:27:39.704151 gwcelery-2.1.0/gwcelery/tests/test_tasks_gwskynet.py
+-rw-r--r--   0        0        0     3662 2023-05-18 19:27:39.704151 gwcelery-2.1.0/gwcelery/tests/test_tasks_igwn_alert.py
+-rw-r--r--   0        0        0    22955 2023-05-20 02:48:26.929777 gwcelery-2.1.0/gwcelery/tests/test_tasks_inference.py
+-rw-r--r--   0        0        0    33299 2023-05-18 19:27:39.705151 gwcelery-2.1.0/gwcelery/tests/test_tasks_orchestrator.py
+-rw-r--r--   0        0        0     1647 2023-05-18 19:27:39.705151 gwcelery-2.1.0/gwcelery/tests/test_tasks_p_astro.py
+-rw-r--r--   0        0        0    25523 2023-05-20 00:18:20.109305 gwcelery-2.1.0/gwcelery/tests/test_tasks_raven.py
+-rw-r--r--   0        0        0     4724 2023-05-18 19:27:39.705151 gwcelery-2.1.0/gwcelery/tests/test_tasks_rrt_utils.py
+-rw-r--r--   0        0        0     5035 2023-05-18 19:27:39.705151 gwcelery-2.1.0/gwcelery/tests/test_tasks_skymaps.py
+-rw-r--r--   0        0        0    40127 2023-05-18 19:27:39.706151 gwcelery-2.1.0/gwcelery/tests/test_tasks_superevents.py
+-rw-r--r--   0        0        0      637 2023-05-18 19:27:39.706151 gwcelery-2.1.0/gwcelery/tests/test_tempfile.py
+-rw-r--r--   0        0        0     3520 2023-05-18 19:27:39.706151 gwcelery-2.1.0/gwcelery/tests/test_tools_condor.py
+-rw-r--r--   0        0        0     1098 2023-05-18 19:27:39.706151 gwcelery-2.1.0/gwcelery/tests/test_tools_condor_submit_helper.py
+-rw-r--r--   0        0        0      633 2023-05-18 19:27:39.706151 gwcelery-2.1.0/gwcelery/tests/test_tools_flask.py
+-rw-r--r--   0        0        0     9668 2023-05-18 19:27:39.706151 gwcelery-2.1.0/gwcelery/tests/test_tools_nagios.py
+-rw-r--r--   0        0        0      269 2023-05-18 19:27:39.706151 gwcelery-2.1.0/gwcelery/tests/test_util.py
+-rw-r--r--   0        0        0    22392 2023-05-19 06:44:52.292984 gwcelery-2.1.0/gwcelery/tests/test_views.py
+-rw-r--r--   0        0        0      216 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/tools/__init__.py
+-rw-r--r--   0        0        0     2948 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/tools/condor.py
+-rw-r--r--   0        0        0     1120 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/tools/condor_submit_helper.py
+-rw-r--r--   0        0        0     1938 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/tools/flask.py
+-rw-r--r--   0        0        0     6624 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/tools/nagios.py
+-rw-r--r--   0        0        0      413 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/util/__init__.py
+-rw-r--r--   0        0        0     1007 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/util/cmdline.py
+-rw-r--r--   0        0        0      453 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/util/matplotlib.py
+-rw-r--r--   0        0        0      390 2023-05-18 19:27:39.708151 gwcelery-2.1.0/gwcelery/util/proxy.py
+-rw-r--r--   0        0        0      514 2023-05-18 19:27:39.708151 gwcelery-2.1.0/gwcelery/util/resources.py
+-rw-r--r--   0        0        0      253 2023-05-18 19:27:39.708151 gwcelery-2.1.0/gwcelery/util/sphinx.py
+-rw-r--r--   0        0        0      941 2023-05-18 19:27:39.708151 gwcelery-2.1.0/gwcelery/util/tempfile.py
+-rw-r--r--   0        0        0    19058 2023-05-19 06:44:52.293984 gwcelery-2.1.0/gwcelery/views.py
+-rw-r--r--   0        0        0      365 2023-05-18 19:27:39.708151 gwcelery-2.1.0/gwcelery/voevent/__init__.py
+-rw-r--r--   0        0        0     6387 2023-05-18 19:27:39.708151 gwcelery-2.1.0/gwcelery/voevent/bootsteps.py
+-rw-r--r--   0        0        0     1063 2023-05-18 19:27:39.709151 gwcelery-2.1.0/gwcelery/voevent/logging.py
+-rw-r--r--   0        0        0      779 2023-05-18 19:27:39.709151 gwcelery-2.1.0/gwcelery/voevent/signals.py
+-rw-r--r--   0        0        0      852 2023-05-18 19:27:39.709151 gwcelery-2.1.0/gwcelery/voevent/subscriber.py
+-rw-r--r--   0        0        0     1454 2023-05-18 19:27:39.709151 gwcelery-2.1.0/gwcelery/voevent/util.py
+-rw-r--r--   0        0        0     6035 2023-05-20 06:06:36.345167 gwcelery-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4519 1970-01-01 00:00:00.000000 gwcelery-2.1.0/PKG-INFO
```

### Comparing `gwcelery-2.0.6/CHANGES.rst` & `gwcelery-2.1.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,73 @@
 Changelog
 =========
 
+2.1.0 "Jersey Devil" (2023-05-19)
+---------------------------------
+
+-   Add GWSkyNet to annotate CBC all-sky search superevents. Only the
+    superevents that meet the following conditions will be annotated by
+    GWSkyNet: 1. A network of signal-to-noise ratio of greater
+    than or equal to 7.0; 2. The SNRs in at least two detectors are no less
+    than 4.5; 3. The FAR is below 1 / 21600Hz. In addition, superevents
+    that meet the above conditions will also be annotated if there is a change
+    of preferred event.
+
+-   Only check iDQ for detectors that are on.
+
+-   Update IGWN alert authentication documentation.
+
+-   Clean up large bilby data files after the run for MDC injections.
+
+-   Add pe tag to pesummary uploads.
+
+-   Add new emfollow-dev deployment.
+
+-   Ignore SSM search for superevents until decision about dedicated notice type
+    and other details from OpsDiv are decided.
+
+-   Update rapidpe-rift-pipe to v0.3.0. Adding config options to calculate
+    pastro. Uploading rapidpe pastro to gracedb. Adding a link to
+    rapidpe summary page in logs. Moving the config option to cprofile the
+    jobs to the General section of config. Increasing the number of grid points
+    per intrinsic coordinate to 10.  Adding a config option to specify
+    the type of run (`online` vs `o3replay`) when choosing channel names, the
+    same as `bilby_pipe` does.  Modified `inference.py` to set this config
+    option based on the GraceDB URL.
+
+-   Increase request memory of bilby runs for BBH.
+
+-   Update bilby filenames in acceptance test.
+
+-   Reduce GW FAR requirement for SOG_READY to 1/10 years.
+
+-   Handle ValueErrors from checking iDQ channels, such as if the configured
+    iDQ channel name is not the same as that in the frames. This happened for
+    S230518h during ER15 and broke the alert pipeline.
+
+-   Update the Kafka topic that we consume Fermi alerts from.
+
+-   Fix the triple circular uploads by rearranging the alerts canvas and
+    moving tasks into the second group.
+
+-   Add ability to create circular for medium-latency GRB followup by PyGRB
+    and X-pipeline from the dashboard.
+
+-   Add pe tag to EM-bright probabilities calculated from bilby samples.
+
+-   Add an automatic retry for the check_vectors task if requested data is not
+    yet available in the caches due to data transfer latency. This will retry
+    every five seconds up to four times, for a maximum total of 20 seconds.
+
+-   Rerun the RAVEN sky map comparison whenever the GW preferred event changes.
+
+-   Upgrade bilby to v2.1.1
+
+-   Update ligo-raven to v3.2 and ligo-followup-advocate to v1.2.2.
+
 2.0.6 "Spaghetti Tree" (2023-05-10)
 -----------------------------------
 
 -   Add `HIGH_PROFILE` label for rapid response team.
 
 -   Ensure that external events are not already associated with a superevent
     when triggering Raven off of superevents.
@@ -44,14 +107,15 @@
     event rather than the superevent.
 
 -   Fix bug where the external sky map was created with out-of-date external
     GCN information.
 
 -   Require em-bright >= 1.1.2.
 
+
 2.0.5 "Mothman" (2023-04-20)
 ----------------------------
 
 -   Add Mattermost channel creation for the RRT to discuss a superevent
     candidate.
 
 -   Use Online_PE_MDC nodes for bilby jobs on O3-Replay injections.
@@ -74,15 +138,15 @@
     triggers. Previous workflow only accounted for blocking in presence of
     significant events.
 
 -   Update rapidpe-rift-pipe version to 0.0.12. Use mchirp and q as the
     coordinates for the rectilinear intrinsic grid. Update accounting_group to
     ligo.dev.o4.cbc.pe.lalinferencerapid and add accouting_group_user. Add
     an option to map the events to an injection. Upload only a select set
-    of log files to gracedb. 
+    of log files to gracedb.
 
 -   Prevent alternative collating method for O3 replay and MDC events with INTEGRAL.
 
 -   Pick RAVEN_ALERT preferred external event over one that doesn't pass the joint
     alert publishing criteria.
 
 -   Avoid updating values in the combined sky map if missing in the GW sky map.
@@ -98,15 +162,15 @@
 
 -   Populate the duration and central_frequency fields in Kafka notices for
     burst events.
 
 -   Add periodic SNEWS MDC events to test the corresponding IGWN alert
     listener.
 
--   Use sky map from preferred event rather than superevent, triggering off 
+-   Use sky map from preferred event rather than superevent, triggering off
     EM_READY label instead of SKYMAP_READY. If SKYMAP_READY is applied or if a
     sky map file is added to the superevent, we will once again try to get the
     GW sky map from the superevent.
 
 -   Update bilby and bilby_pipe to 2.1.0 and 1.0.10 respectively. The number of
     spline nodes for calibration errors is increased to 10 thanks to the bilby
     optimizations. Change sampler settings into naccept=60, nlive=500.
@@ -163,15 +227,15 @@
     alert pipeline is blocked by the presence of ``EM_SelectedConfident``.
 
 -   Enable public early warning alerts. The superevent manager now applies the
     ``EARLY_WARNING`` label to the superevent when a significant EW event is added
     to the superevent. The automated pipeline is launched and is blocked before sending
     if ``EM_SelectedConfident`` is found to be applied.
 
--   Add O3 replay MDC testing with RAVEN pipeline. This will run on the 
+-   Add O3 replay MDC testing with RAVEN pipeline. This will run on the
     emfollow-playground server, creating mock coincidences with a frequency
     given by the ``joint_O3_replay_freq`` variable.
 
 -   Require sky map information to publish coincidence with a GRB candidate.
 
 -   Fix collation of INTEGRAL notices by getting the GCN ID from the IVORN
     field.
@@ -290,31 +354,31 @@
 
 -   Change web directory for PE outputs. Use Online PE nodes for bilby. Do not upload lalinference ini files.
 
 -   Add RIFT analysis only for gstlal triggers.
 
 -   Use the exttring worker for RAVEN tasks.
 
--   Bump ligo.em-bright to 1.1.0.dev1 to add HasMassGap. 
+-   Bump ligo.em-bright to 1.1.0.dev1 to add HasMassGap.
     Review page: https://git.ligo.org/emfollow/em-properties/em-bright/-/wikis/Mass-gap-review
-    
+
 -   Compute source properties uniformly across all CBC pipelines.
 
 -   Don't compute p-astro for MBTA because they now compute and upload their
     own.
 
 -   Change expected p-astro filename from ``p_astro.json`` to
     ``pipeline.p_astro.json``, where pipeline is the name of the pipeline that
     uploaded the event.
 
 -   Indicate a joint CBC-GRB event should be used for a measurement of the
-    speed of gravity by applying the SOG_READY label to the superevent. This pipeline is launched is the right conditions are met after ADVOK label. 
+    speed of gravity by applying the SOG_READY label to the superevent. This pipeline is launched is the right conditions are met after ADVOK label.
 
 -   Add button to apply RAVEN alert labels to flask app. This will manually
-    trigger a RAVEN alert. 
+    trigger a RAVEN alert.
 
 -   Update messages from RAVEN alert pipeline to be more informative.
 
 -   Fix bug where updated GRB events couldn't create sky maps.
 
 -   Filter out test GCNs from updating external events.
 
@@ -410,15 +474,15 @@
     decreased by a median of about 0.5 s.
 
 -   Set the preliminary alert timeout to 0 s.
 
 -   Use multi-resolution GW sky maps when calculating the joint false alarm
     rate. Use single pixel RA/dec when evaluating for Swift coincidences.
 
--   Filter BBH/IMBH events from burst-GRB searches. 
+-   Filter BBH/IMBH events from burst-GRB searches.
 
 1.0.1 (2022-05-09)
 ------------------
 
 -   Added ``request_disk`` specification for gwcelery condor submission
 
 -   Bump ``p-astro`` to pre-release ``v1.0.0dev1``. This version is a stop gap to
@@ -550,15 +614,15 @@
 -   Identify early-warning events using the ``EARLY_WARNING`` label rather than
     the ``EarlyWarning`` search type. The search type is already used to
     distinguish mock (``MDC``) events, so it cannot also be used to indicate
     early-warning events.
 
 -   Inhibit GCNs for superevents with the INJ label.
 
--   Add configuration variable to disable all but MDC alerts from GCN, and 
+-   Add configuration variable to disable all but MDC alerts from GCN, and
     set that variable to True on the production instance.
 
 -   Skip the preliminary alert timeout for early warning events.
 
 -   Update the documentation on RAVEN functions and external triggers flow
     chart.
 
@@ -605,15 +669,15 @@
     REST API calls involved in uploading and download the additional file.
 
 0.12.2 (2020-03-20)
 -------------------
 
 -   Skip detchar checks for events which occur in the future.
 
--   Delay omegascans until data are available for events in the future. 
+-   Delay omegascans until data are available for events in the future.
 
 -   Enable Zstandard compression of tasks and results to reduce bandwidth into
     and out of Redis.
 
 -   Enable receipt confirmation of early warning GCN notices.
 
 -   If available, use spatial coincidence FAR to determine when to publish a
```

### Comparing `gwcelery-2.0.6/LICENSE.rst` & `gwcelery-2.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/README.rst` & `gwcelery-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/Makefile` & `gwcelery-2.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/_static/acceptance-tests-checklist.png` & `gwcelery-2.1.0/doc/_static/acceptance-tests-checklist.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/_static/celeryevent-screenshot.png` & `gwcelery-2.1.0/doc/_static/celeryevent-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/_static/deployment-screenshot.png` & `gwcelery-2.1.0/doc/_static/deployment-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/_static/flask-screenshot.png` & `gwcelery-2.1.0/doc/_static/flask-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/_static/flower-screenshot.png` & `gwcelery-2.1.0/doc/_static/flower-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/_static/logo-0.5x.png` & `gwcelery-2.1.0/doc/_static/logo-0.5x.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/_static/logo.png` & `gwcelery-2.1.0/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/_static/sentry-screenshot.png` & `gwcelery-2.1.0/doc/_static/sentry-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/conf.py` & `gwcelery-2.1.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/configuration.rst` & `gwcelery-2.1.0/doc/configuration.rst`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 it in a location such as ``~/.globus/userkey.pem`` and
 ``~/.globus/usercert.pem``.
 
 .. rubric:: IGWN Alert
 
 You must provide a valid username and password for :doc:`IGWN Alert <igwn-alert:index>`. You can request an
 account using the `SCiMMA Auth portal`_. To get started, see :doc:`IGWN Alert Userguide <igwn-alert:guide>`.
-The IGWN Alert username and password should be stored in your `netrc file`_.
+The IGWN Alert username and password should be stored in your `auth.toml`_ file.
 
 .. rubric:: Kafka
 
 You must provide a file named ``kafka_credential_map.json`` that maps
 deployment specific usernames for Kafka credentials to the logical names given
 in the configuration files. This file should be saved in the GWCelery XDG
 config directory (``${HOME}/.config/gwcelery/`` by default on many Linux and
@@ -72,15 +72,15 @@
 Note that one user can be specified multiple times. ``hop auth`` must have
 information about each user specified in this file. Every Kafka producer and
 consumer configuration key must have an entry in this file.
 
 .. _`LSC DataGrid Client`: https://www.lsc-group.phys.uwm.edu/lscdatagrid/doc/installclient.html
 .. _`obtain a robot certificate`: https://robots.ligo.org
 .. _`SCiMMA Auth portal`: https://my.hop.scimma.org/
-.. _`netrc file`: https://www.gnu.org/software/inetutils/manual/html_node/The-_002enetrc-file.html
+.. _`auth.toml`: https://hop-client.readthedocs.io/en/latest/user/auth.html#configuration
 
 .. _redis-configuration:
 
 Redis
 -----
 
 We recommend that you make the following settings in your Redis server
```

### Comparing `gwcelery-2.0.6/doc/contributing.rst` & `gwcelery-2.1.0/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/deployment.rst` & `gwcelery-2.1.0/doc/deployment.rst`

 * *Files 1% similar despite different names*

```diff
@@ -125,16 +125,16 @@
 
 8.  Wait a couple minutes, and then verify that the new release has been
     published on our PyPI project page, https://pypi.org/project/gwcelery/.
 
 9.  If desired, navigate to the GitLab project's `Environments`_ page and
     trigger a deployment to production.
 
-    Each pipeline has an interface which enables deployment to the 
-    available environments. 
+    Each pipeline has an interface which enables deployment to the
+    available environments.
 
     .. image:: _static/deployment-screenshot.png
        :alt: Screen shot of deployment options
 
 .. _`Environments`: https://git.ligo.org/emfollow/gwcelery/environments
 .. _`.gitlab-ci.yml`: https://git.ligo.org/emfollow/gwcelery/blob/main/.gitlab-ci.yml
 .. _`poetry`: https://python-poetry.org/
```

### Comparing `gwcelery-2.0.6/doc/design.rst` & `gwcelery-2.1.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/gwcelery.tasks.detchar.rst` & `gwcelery-2.1.0/doc/gwcelery.tasks.detchar.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/gwcelery.tasks.em_bright.rst` & `gwcelery-2.1.0/doc/gwcelery.tasks.em_bright.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/gwcelery.tasks.external_triggers.rst` & `gwcelery-2.1.0/doc/gwcelery.tasks.external_triggers.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/gwcelery.tasks.orchestrator.rst` & `gwcelery-2.1.0/doc/gwcelery.tasks.orchestrator.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/gwcelery.tasks.rst` & `gwcelery-2.1.0/doc/gwcelery.tasks.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/gwcelery.tasks.superevents.rst` & `gwcelery-2.1.0/doc/gwcelery.tasks.superevents.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/htcondor.rst` & `gwcelery-2.1.0/doc/htcondor.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/index.rst` & `gwcelery-2.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/make.bat` & `gwcelery-2.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/monitoring.rst` & `gwcelery-2.1.0/doc/monitoring.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/doc/quickstart.rst` & `gwcelery-2.1.0/doc/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/__init__.py` & `gwcelery-2.1.0/gwcelery/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/_version.py` & `gwcelery-2.1.0/gwcelery/_version.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/conf/__init__.py` & `gwcelery-2.1.0/gwcelery/conf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 variable to the fully qualified name of any Python module that can be located
 in :obj:`sys.path`, including any of the following presets:
 
  * :mod:`gwcelery.conf.development`
  * :mod:`gwcelery.conf.playground` (the default)
  * :mod:`gwcelery.conf.production`
  * :mod:`gwcelery.conf.test`
+ * :mod:`gwcelery.conf.dev`
 """
 
 import getpass
 import os
 
 # Celery application settings.
 
@@ -64,27 +65,41 @@
 
 igwn_alert_group = 'gracedb-playground'
 """IGWN alert group."""
 
 gracedb_host = 'gracedb-playground.ligo.org'
 """GraceDB host."""
 
+gwskynet_upper_far_threshold = 1 / 21600
+"""GWSkyNet will only annotate events with FARs below this value."""
+
+gwskynet_snr_threshold = 4.5
+"""GWSkyNet will only annotate events with individual SNRs above this value."""
+
+gwskynet_network_snr_threshold = 7.0
+"""GWSkyNet will only annotate events with network SNRs above this value."""
+
 create_mattermost_channel = False
 """Do not create Mattermost channel."""
 
 kafka_consumer_config = {
     'fermi': {'url': 'kafka://kafka.test.gcn.nasa.gov/'
-              'fermi.gbm.targeted.private', 'suffix': 'json'},
+              'fermi.gbm.targeted.private.igwn', 'suffix': 'json'},
     'swift': {'url': 'kafka://kafka.test.gcn.nasa.gov/swift.bat.guano',
               'suffix': 'json'}
 }
 """Kafka consumer configuration details. The keys describe the senders of the
 messages to be consumed. The values are a dictionary of the URL to listen to
 and information about the message serializer."""
 
+views_manual_preferred_event_log_message = 'User {} queued a preferred event' \
+                                           ' change to {}.'
+"""Log message that is uploaded to GraceDB when a user manually changes the
+preferred event in the dashboard."""
+
 voevent_broadcaster_address = ':5342'
 """The VOEvent broker will bind to this address to send GCNs.
 This should be a string of the form `host:port`. If `host` is empty,
 then listen on all available interfaces."""
 
 voevent_broadcaster_whitelist = []
 """List of hosts from which the broker will accept connections.
@@ -155,15 +170,15 @@
 preliminary_alert_trials_factor = dict(cbc=8.0, burst=8.0)
 """Trials factor for less significant alerts."""
 
 snews_gw_far_threshold = 1 / (3600 * 24)
 """Maximum false alarm rate for a superevent to send out a coincidence alert
 between an external SNEWS alert and the superevent."""
 
-sog_paper_far_threshold = {'gw': 1 / (1000 * 365 * 86400),
+sog_paper_far_threshold = {'gw': 1 / (10 * 365 * 86400),
                            'joint': 1 / (10000 * 365 * 86400)}
 """False alarm rate thresholds for producing a manuscript of speed of gravity
 measurement in low-latency."""
 
 superevent_clean_up_timeout = 270.
 """The orchestrator will wait this many seconds from the time of the
 application of the GCN_PRELIM_SENT label to revise the preferred
```

### Comparing `gwcelery-2.0.6/gwcelery/conf/minikube.py` & `gwcelery-2.1.0/gwcelery/conf/minikube.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/conf/playground.py` & `gwcelery-2.1.0/gwcelery/conf/playground.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/conf/production.py` & `gwcelery-2.1.0/gwcelery/conf/production.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/conf/test.py` & `gwcelery-2.1.0/gwcelery/conf/test.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/data/first2years/gstlal.xml.gz` & `gwcelery-2.1.0/gwcelery/data/first2years/gstlal.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/data/gwcelery.sub` & `gwcelery-2.1.0/gwcelery/data/gwcelery.sub`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env condor_submit
-accounting_group_user = leo.singer
+accounting_group_user = cody.messick
 universe = local
 getenv = true
 executable = /usr/bin/env
 log = gwcelery-condor.log
 on_exit_remove = false
 request_disk = 7GB
 JobBatchName = gwcelery
@@ -60,7 +60,14 @@
 arguments = "gwcelery-condor-submit-helper gwcelery worker -l info -n gwcelery-multiprocessing-worker@%h -f %n.log -Q multiprocessing -c 1 --prefetch-multiplier 1"
 description = gwcelery-multiprocessing-worker
 queue
 
 arguments = "--unset OMP_NUM_THREADS gwcelery-condor-submit-helper gwcelery worker -l info -n gwcelery-openmp-worker-$(Process)@%h -f %n.log -Q openmp -c 1 --prefetch-multiplier 1"
 description = gwcelery-openmp-worker-$(Process)
 queue 15
+
++Online_GWSkyNet = True
+Requirements = (TARGET.Online_GWSkyNet =?= True)
+
+arguments = "gwcelery-condor-submit-helper gwcelery worker -l info -n gwcelery-skynet-worker@%h -f %n.log -Q skynet -c 1 --prefetch-multiplier 1"
+description = gwcelery-skynet-worker
+queue
```

### Comparing `gwcelery-2.0.6/gwcelery/email/bootsteps.py` & `gwcelery-2.1.0/gwcelery/email/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/email/signals.py` & `gwcelery-2.1.0/gwcelery/email/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/flask.py` & `gwcelery-2.1.0/gwcelery/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/igwn_alert/__init__.py` & `gwcelery-2.1.0/gwcelery/igwn_alert/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/igwn_alert/bootsteps.py` & `gwcelery-2.1.0/gwcelery/igwn_alert/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/igwn_alert/signals.py` & `gwcelery-2.1.0/gwcelery/igwn_alert/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/kafka/bootsteps.py` & `gwcelery-2.1.0/gwcelery/kafka/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/kafka/signals.py` & `gwcelery-2.1.0/gwcelery/kafka/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/sentry/__init__.py` & `gwcelery-2.1.0/gwcelery/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/sentry/integrations/condor.py` & `gwcelery-2.1.0/gwcelery/sentry/integrations/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/sentry/integrations/requests.py` & `gwcelery-2.1.0/gwcelery/sentry/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/sentry/integrations/subprocess.py` & `gwcelery-2.1.0/gwcelery/sentry/integrations/subprocess.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/static/typeahead.css` & `gwcelery-2.1.0/gwcelery/static/typeahead.css`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/static/vega/index.html` & `gwcelery-2.1.0/gwcelery/static/vega/index.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/__init__.py` & `gwcelery-2.1.0/gwcelery/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/alerts.py` & `gwcelery-2.1.0/gwcelery/tasks/alerts.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,34 @@
 
 
 class _KafkaDispatchHandler(DispatchHandler):
 
     def process_args(self, name, record):
         return name, (record,), {}
 
+    def __call__(self, *keys, **kwargs):
+        r"""Create a new task and register it as a callback for handling the
+        given keys.
+
+        Parameters
+        ----------
+        \*keys : list
+            Keys to match
+        \*\*kwargs
+            Additional keyword arguments for `celery.Celery.task`.
+
+        """
+        def wrap(f):
+            f = gracedb.task(ignore_result=True, **kwargs)(f)
+            for key in keys:
+                self.setdefault(key, []).append(f)
+            return f
+
+        return wrap
+
 
 handler = _KafkaDispatchHandler()
 r"""Function decorator to register a handler callback for specified Kafka URLs.
 The decorated function is turned into a Celery task, which will be
 automatically called whenever a message is received from a matching URL.
 
 Parameters
```

### Comparing `gwcelery-2.0.6/gwcelery/tasks/bayestar.py` & `gwcelery-2.1.0/gwcelery/tasks/bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/circulars.py` & `gwcelery-2.1.0/gwcelery/tasks/circulars.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 def create_emcoinc_circular(graceid):
     """Create and return the em_coinc circular txt."""
     return ligo.followup_advocate.compose_raven(graceid,
                                                 client=gracedb.client)
 
 
 @gracedb.task(shared=False)
+def create_medium_latency_circular(graceid):
+    """Create and return the em_coinc circular txt."""
+    return ligo.followup_advocate.compose_grb_medium_latency(
+               graceid, client=gracedb.client)
+
+
+@gracedb.task(shared=False)
 def create_update_circular(graceid, update_types=['sky_localization',
                                                   'em_bright',
                                                   'p_astro']):
     """Create and return update circular txt."""
     return ligo.followup_advocate.compose_update(graceid,
                                                  update_types=update_types,
                                                  client=gracedb.client)
```

### Comparing `gwcelery-2.0.6/gwcelery/tasks/condor.py` & `gwcelery-2.1.0/gwcelery/tasks/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/core.py` & `gwcelery-2.1.0/gwcelery/tasks/core.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/detchar.py` & `gwcelery-2.1.0/gwcelery/tasks/detchar.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,18 +292,16 @@
 
     """
     if cache:
         try:
             idq_fap = TimeSeries.read(
                 cache, channel, start=start, end=end)
             return (channel, float(idq_fap.min().value))
-        except (IndexError, RuntimeError):
-            # FIXME: Change from log.exception to log.warning until this fixed,
-            # because it's saturating Sentry.
-            log.warning('Failed to read from low-latency iDQ frame files')
+        except (IndexError, RuntimeError, ValueError):
+            log.exception('Failed to read from low-latency iDQ frame files')
     # FIXME: figure out how to get access to low-latency frames outside
     # of the cluster. Until we figure that out, actual I/O errors have
     # to be non-fatal.
     return (channel, None)
 
 
 def check_vector(cache, channel, start, end, bits, logic_type='all'):
@@ -372,16 +370,16 @@
     # FIXME: figure out how to get access to low-latency frames outside
     # of the cluster. Until we figure that out, actual I/O errors have
     # to be non-fatal.
     return {bitname.format(channel.split(':')[0], key):
             None for key in bits if key is not None}
 
 
-@app.task(shared=False)
-def check_vectors(event, graceid, start, end):
+@app.task(shared=False, bind=True, default_retry_delay=5)
+def check_vectors(self, event, graceid, start, end):
     """Perform data quality checks for an event and labels/logs results to
     GraceDB.
 
     Depending on the pipeline, a certain amount of time (specified in
     :obj:`~gwcelery.conf.check_vector_prepost`) is appended to either side of
     the superevent start and end time. This is to catch DQ issues slightly
     before and after the event, such as that appearing in L1 just before
@@ -450,50 +448,60 @@
     # Do not analyze DMT-DQ_VECTOR if pipeline uses gated h(t)
     states = {}
     analysis_channels = app.conf['llhoft_channels'].items()
     if app.conf['uses_gatedhoft'][pipeline]:
         analysis_channels = {k: v for k, v in analysis_channels
                              if k[3:] != 'DMT-DQ_VECTOR'}.items()
     for channel, bits in analysis_channels:
-        states.update(check_vector(caches[channel.split(':')[0]], channel,
-                                   start, end, bit_defs[bits]))
+        try:
+            states.update(check_vector(
+                caches[channel.split(':')[0]], channel,
+                start, end, bit_defs[bits]))
+        except ValueError as exc:
+            # check_vector likely failed to find the requested data
+            # in the cache because it has yet to arrive
+            raise self.retry(exc=exc, max_retries=4)
     # Pick out DQ and injection states, then filter for active detectors
     dq_states = {key: value for key, value in states.items()
                  if key.split('_')[-1] != 'INJ'}
     inj_states = {key: value for key, value in states.items()
                   if key.split('_')[-1] == 'INJ'}
     active_dq_states = {key: value for key, value in dq_states.items()
                         if key.split(':')[0] in instruments}
     active_inj_states = {key: value for key, value in inj_states.items()
                          if key.split(':')[0] in instruments}
 
-    # Check iDQ states
+    # Check iDQ states and filter for active instruments
     idq_faps = dict(check_idq(caches[channel.split(':')[0]],
                     channel, start, end)
-                    for channel in app.conf['idq_channels'])
+                    for channel in app.conf['idq_channels']
+                    if channel.split(':')[0] in instruments)
 
     # Logging iDQ to GraceDB
-    if None not in idq_faps.values():
+    if None not in idq_faps.values() and len(idq_faps) > 0:
         idq_faps_readable = {k: round(v, 3) for k, v in idq_faps.items()}
         if min(idq_faps.values()) <= app.conf['idq_fap_thresh']:
-            idq_msg = ("iDQ false alarm probability is low: "
+            idq_msg = ("iDQ false alarm probability is low "
+                       "(below {} threshold), "
+                       "i.e., there could be a data quality issue: "
                        "minimum FAP is {}. ").format(
+                app.conf['idq_fap_thresh'],
                 json.dumps(idq_faps_readable)[1:-1])
             # If iDQ FAP is low and pipeline enabled, apply DQV
             if app.conf['idq_veto'][pipeline]:
                 gracedb.remove_label('DQOK', graceid)
                 gracedb.create_label('DQV', graceid)
                 # Add labels to return value to avoid querying GraceDB again.
                 event = dict(event, labels=event.get('labels', []) + ['DQV'])
                 try:
                     event['labels'].remove('DQOK')
                 except ValueError:  # not in list
                     pass
         else:
-            idq_msg = ("iDQ false alarm probabilities at both H1 and L1 "
+            idq_msg = ("iDQ false alarm probabilities for active detectors "
                        "are good (above {} threshold). "
                        "Minimum FAP is {}. ").format(
                            app.conf['idq_fap_thresh'],
                            json.dumps(idq_faps_readable)[1:-1])
     else:
         idq_msg = "iDQ false alarm probabilities unknown. "
     gracedb.upload.delay(
```

### Comparing `gwcelery-2.0.6/gwcelery/tasks/em_bright.py` & `gwcelery-2.1.0/gwcelery/tasks/em_bright.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/external_skymaps.py` & `gwcelery-2.1.0/gwcelery/tasks/external_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/external_triggers.py` & `gwcelery-2.1.0/gwcelery/tasks/external_triggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,20 +384,39 @@
             # Rerun for all eligible external events
             for ext_id in superevent['em_events']:
                 external_event = gracedb.get_event(ext_id)
                 if REQUIRED_LABELS_BY_TASK['compare'].issubset(
                         set(external_event['labels'])):
                     _relaunch_raven_pipeline_with_skymaps(
                         superevent, external_event, graceid,
-                        use_superevent=True)
+                        use_superevent_skymap=True)
         else:
             if REQUIRED_LABELS_BY_TASK['compare'].issubset(
                     set(external_event['labels'])):
                 _relaunch_raven_pipeline_with_skymaps(
                     superevent, external_event, graceid)
+    # Rerun the coincidence FAR calculation if possible with combined sky map
+    # if the preferred event changes
+    # We don't want to run this logic if PE results are present
+    elif alert['alert_type'] == 'log' and \
+            'PE_READY' not in alert['object']['labels'] and \
+            'EM_COINC' in alert['object']['labels']:
+        new_log_comment = alert['data'].get('comment', '')
+        if 'S' in graceid and \
+            new_log_comment.startswith('Updated superevent parameters: '
+                                       'preferred_event: '):
+            superevent = alert['object']
+            # Rerun for all eligible external events
+            for ext_id in superevent['em_events']:
+                external_event = gracedb.get_event(ext_id)
+                if REQUIRED_LABELS_BY_TASK['compare'].issubset(
+                        set(external_event['labels'])):
+                    _relaunch_raven_pipeline_with_skymaps(
+                        superevent, external_event, graceid,
+                        use_superevent_skymap=False)
     elif alert['alert_type'] == 'label_removed' and \
             alert['object'].get('group') == 'External':
         if alert['data']['name'] == 'NOT_GRB' and \
                 'EM_COINC' in alert['object']['labels']:
             # if NOT_GRB is removed, re-check publishing conditions
             superevent_id = alert['object']['superevent']
             superevent = gracedb.get_superevent(superevent_id)
@@ -486,47 +505,49 @@
         end = start + integration_time
     detchar.check_vectors.si(event, event['graceid'], start, end).delay()
 
     return event
 
 
 def _relaunch_raven_pipeline_with_skymaps(superevent, ext_event, graceid,
-                                          use_superevent=False):
+                                          use_superevent_skymap=None):
     """Relaunch the RAVEN sky map comparison workflow, include recalculating
     the joint FAR with updated sky map info and create a new combined sky map.
 
     Parameters
     ----------
     superevent: dict
         superevent dictionary
     exttrig: dict
         external event dictionary
     graceid: str
         GraceDB ID of event
-    use_superevent: bool
-        If True, always use skymap info from superevent
-        regardless of SKYMAP_READY label.
+    use_superevent_skymap: bool
+        If True/False, use/don't use skymap info from superevent.
+        Else if None, check SKYMAP_READY label in external event.
 
     """
     gw_group = superevent['preferred_event_data']['group']
     tl, th = raven._time_window(graceid, gw_group,
                                 [ext_event['pipeline']],
                                 [ext_event['search']])
     # FIXME: both overlap integral and combined sky map could be
     # done by the same function since they are so similar
+    use_superevent = (use_superevent_skymap
+                      if use_superevent_skymap is not None else
+                      'SKYMAP_READY' in ext_event['labels'])
     canvas = raven.raven_pipeline.si(
                  [ext_event] if 'S' in graceid else [superevent],
                  graceid,
                  superevent if 'S' in graceid else ext_event,
-                 tl, th, gw_group)
+                 tl, th, gw_group, use_superevent_skymap=use_superevent)
     # Swift localizations are incredibly well localized and require
     # a different method from Fermi/Integral/AGILE
     # FIXME: Add Swift localization information in the future
     if ext_event['pipeline'] != 'Swift':
         # Create new updated combined sky map
         canvas |= external_skymaps.create_combined_skymap.si(
                       superevent['superevent_id'], ext_event['graceid'],
                       preferred_event=(
-                          None if 'SKYMAP_READY' in ext_event['labels']
-                          or use_superevent
+                          None if use_superevent
                           else superevent['preferred_event']))
     canvas.delay()
```

### Comparing `gwcelery-2.0.6/gwcelery/tasks/first2years.py` & `gwcelery-2.1.0/gwcelery/tasks/first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/first2years_external.py` & `gwcelery-2.1.0/gwcelery/tasks/first2years_external.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/gcn.py` & `gwcelery-2.1.0/gwcelery/tasks/gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/gracedb.py` & `gwcelery-2.1.0/gwcelery/tasks/gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/igwn_alert.py` & `gwcelery-2.1.0/gwcelery/tasks/igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/inference.py` & `gwcelery-2.1.0/gwcelery/tasks/inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -491,15 +491,16 @@
 
     path_to_settings = os.path.join(rundir, 'settings.json')
     setup_arg = ['bilby_pipe_gracedb', '--webdir', path_to_webdir,
                  '--outdir', rundir, '--json', path_to_json,
                  '--psd-file', path_to_psd, '--settings', path_to_settings]
     settings = {'summarypages_arguments': {'gracedb': event['graceid'],
                                            'no_ligo_skymap': True},
-                'accounting_user': 'soichiro.morisaki'}
+                'accounting_user': 'soichiro.morisaki',
+                'enforce_signal_duration': False}
     if app.conf['gracedb_host'] != 'gracedb.ligo.org':
         settings['queue'] = 'Online_PE_MDC'
     else:
         settings['queue'] = 'Online_PE'
     # FIXME: using live data for gracedb-test events should be reconsidered
     # when we have a better idea to differentiate MDC and real events.
     if app.conf['gracedb_host'] not in [
@@ -538,15 +539,16 @@
         # range where IMRPhenomXPHM ROQ bases are not available
         elif trigger_chirp_mass < 12:
             likelihood_mode = os.path.join(rundir, "likelihood_mode.json")
             _dump_high_mass_ratio_pv2_settings(likelihood_mode)
         else:
             likelihood_mode = os.path.join(rundir, "likelihood_mode.json")
             _dump_xphm_settings(likelihood_mode)
-            settings['request_memory_generation'] = 16.0
+            settings['request_memory_generation'] = 36.0
+            settings['request_memory'] = 16.0
         setup_arg += ['--cbc-likelihood-mode', likelihood_mode]
     elif mode == 'fast_test':
         setup_arg += ["--sampler-kwargs", "FastTest"]
         if trigger_chirp_mass < 3.9:
             setup_arg += ['--cbc-likelihood-mode', 'phenompv2_bns_roq']
             settings['request_memory_generation'] = 8.0
     else:
@@ -599,33 +601,32 @@
 
     Returns
     -------
     path_to_dag : str
         The path to the .dag file
 
     """
-    # dump SVD depth file
-    path_to_svd_file = os.path.join(rundir, 'svd_depth_methods.json')
-    with open(path_to_svd_file, 'w') as f:
-        json.dump(
-            [{'bounds': {}, 'fudge_factors': {'mchirp': 0.2, 'eta': 0.1},
-             'svd_depth': 1}],
-            f)
+    if app.conf['gracedb_host'] not in {
+        'gracedb.ligo.org', 'gracedb-test.ligo.org'
+    }:
+        run_mode = 'o3replay'
+    else:
+        run_mode = 'online'
 
     # dump ini file
     ini_template = env.get_template('rapidpe.jinja2')
     ini_contents = ini_template.render(
         {'rundir': rundir,
          'webdir': os.path.join(
              app.conf['pe_results_path'], superevent_id, 'rapidpe'
          ),
          'gracedb_url': f'https://{app.conf["gracedb_host"]}/api',
          'superevent_id': superevent_id,
-         'frame_data_types': frametype_dict,
-         'svd_depth_json': os.path.abspath(path_to_svd_file)})
+         'run_mode': run_mode,
+         'frame_data_types': frametype_dict})
     path_to_ini = os.path.join(rundir, 'rapidpe.ini')
     with open(path_to_ini, 'w') as f:
         f.write(ini_contents)
     gracedb.upload.delay(
         ini_contents, filename=os.path.basename(path_to_ini),
         graceid=superevent_id,
         message=('Automatically generated RapidPE-RIFT configuration file'
@@ -720,14 +721,33 @@
         Paths to the target files or directories
 
     """
     return glob.iglob(os.path.join(directory, '**', name), recursive=True)
 
 
 @app.task(ignore_result=True, shared=False)
+def _clean_up_bilby(rundir):
+    """Remove large data products produced by bilby
+
+    Parameters
+    ----------
+    rundir : str
+
+    """
+    for p in glob.glob(
+        os.path.join(rundir, "data/*_generation_roq_weights.hdf5")
+    ):
+        os.remove(p)
+    for p in glob.glob(
+        os.path.join(rundir, "data/*_generation_data_dump.pickle")
+    ):
+        os.remove(p)
+
+
+@app.task(ignore_result=True, shared=False)
 def job_error_notification(request, exc, traceback,
                            superevent_id, rundir, analysis):
     """Upload notification when condor.submit terminates unexpectedly.
 
     Parameters
     ----------
     request : Context (placeholder)
@@ -739,14 +759,19 @@
     superevent_id : str
         The GraceDB ID of a target superevent
     rundir : str
         The run directory for PE
     analysis : str
         Analysis name used as a label in uploaded messages
 
+    Notes
+    -----
+    Some large bilby data products are cleaned up after the notification if the
+    gracedb host is different from `gracedb.ligo.org`.
+
     """
     if isinstance(exc, condor.JobRunning):
         subprocess.run(['condor_rm', str(exc.args[0]['Cluster'])])
         canvas = gracedb.upload.si(
             filecontents=None, filename=None, graceid=superevent_id, tags='pe',
             message=f'The {analysis} condor job was aborted by gwcelery, '
                     'due to its long run time.'
@@ -783,14 +808,17 @@
                     filename=os.path.basename(path) + '.log',
                     graceid=superevent_id,
                     message=f'A log file for {analysis} condor job.',
                     tags='pe'
                 ))
         canvas |= group(tasks)
 
+    if "bilby" in analysis and app.conf['gracedb_host'] != 'gracedb.ligo.org':
+        canvas |= _clean_up_bilby.si(rundir)
+
     canvas.delay()
 
 
 def _upload_tasks_lalinference(rundir, superevent_id):
     """Return canvas of tasks to upload LALInference results
 
     Parameters
@@ -885,14 +913,19 @@
         Analysis mode
 
     Returns
     -------
     tasks : canvas
         The work-flow for uploading Bilby results
 
+    Notes
+    -----
+    Some large bilby data products are cleaned up after posteterior file is
+    uploaded if the gracedb host is different from `gracedb.ligo.org`.
+
     """
     # convert bilby sample file into one compatible with ligo-skymap
     samples_dir = os.path.join(rundir, 'final_result')
     if mode == 'production':
         samples_filename = 'Bilby.posterior_samples.hdf5'
     else:
         samples_filename = f'Bilby.{mode}.posterior_samples.hdf5'
@@ -903,14 +936,17 @@
     )
 
     with open(out_samples, 'rb') as f:
         canvas = gracedb.upload.si(
             f.read(), samples_filename,
             superevent_id, f'{mode}-mode Bilby posterior samples', 'pe')
 
+    if app.conf['gracedb_host'] != 'gracedb.ligo.org':
+        canvas |= _clean_up_bilby.si(rundir)
+
     # pesummary
     pesummary_kwargs = {}
     path_to_ini, = glob.glob(os.path.join(rundir, "*_complete.ini"))
     pesummary_kwargs["config"] = path_to_ini
     config_parser = BilbyConfigFileParser()
     with open(path_to_ini, "r") as f:
         config_content, _, _, _ = config_parser.parse(f)
@@ -934,22 +970,62 @@
     )
     canvas = group(
         canvas,
         _pesummary_task(webdir, in_samples, **pesummary_kwargs)
         |
         gracedb.upload.si(
             None, None, superevent_id,
-            'PESummary page for {mode}-mode Bilby is available '
-            f'<a href={url}>here</a>'
+            f'PESummary page for {mode}-mode Bilby is available '
+            f'<a href={url}>here</a>',
+            'pe'
         )
     )
 
     return canvas
 
 
+def _upload_tasks_rapidpe(rundir, superevent_id):
+    summary_path = os.path.join(rundir, "summary")
+
+    url = urllib.parse.urljoin(
+        app.conf['pe_results_url'],
+        os.path.join(superevent_id, 'rapidpe', 'summarypage.html')
+    )
+    canvas = gracedb.upload.si(
+        None, None, superevent_id,
+        f'Summary page for RapidPE-RIFT is available <a href={url}>here</a>',
+        ('pe',))
+
+    to_upload = [
+        (
+            "p_astro.json", "RapidPE_RIFT.p_astro.json",
+            "RapidPE-RIFT Pastro results",
+            ("pe", "lvem", "public", "p_astro"),
+        ),
+        (
+            "p_astro.png", "RapidPE_RIFT.p_astro.png",
+            "RapidPE-RIFT Pastro results",
+            ("pe", "lvem", "public", "p_astro"),
+        ),
+    ]
+    tasks = []
+    for src_basename, dst_filename, description, tags in to_upload:
+        src_filename = os.path.join(summary_path, src_basename)
+        if os.path.isfile(src_filename):
+            with open(src_filename, "rb") as f:
+                tasks.append(
+                    gracedb.upload.si(
+                        f.read(), dst_filename,
+                        superevent_id, description, tags))
+
+    canvas |= group(tasks)
+
+    return canvas
+
+
 @app.task(ignore_result=True, shared=False)
 def dag_finished(rundir, superevent_id, pe_pipeline, **kwargs):
     """Upload PE results
 
     Parameters
     ----------
     rundir : str
@@ -963,23 +1039,21 @@
     """
     if pe_pipeline == 'lalinference':
         canvas = _upload_tasks_lalinference(rundir, superevent_id)
     elif pe_pipeline == 'bilby':
         canvas = _upload_tasks_bilby(
             rundir, superevent_id, kwargs['bilby_mode'])
     elif pe_pipeline == 'rapidpe':
-        # TODO: upload rapidpe posterior samples
-        canvas = gracedb.upload.si(
-            None, None, superevent_id,
-            'Online RapidPE-RIFT parameter estimation finished.', 'pe')
+        canvas = _upload_tasks_rapidpe(rundir, superevent_id)
     else:
         raise NotImplementedError(f'Unknown PE pipeline {pe_pipeline}.')
 
     canvas.delay()
 
+    # NOTE: check if this should include rapidpe as well
     if pe_pipeline == 'bilby':
         gracedb.create_label.delay('PE_READY', superevent_id)
 
 
 def _pesummary_task(webdir, samples, **pesummary_kwargs):
     """Return a celery task to submit a pesummary condor job.
```

### Comparing `gwcelery-2.0.6/gwcelery/tasks/legacy_gracedb.py` & `gwcelery-2.1.0/gwcelery/tasks/legacy_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/notice_text.py` & `gwcelery-2.1.0/gwcelery/tasks/notice_text.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/orchestrator.py` & `gwcelery-2.1.0/gwcelery/tasks/orchestrator.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,15 +437,16 @@
     (
         gracedb.download.si(filename, superevent_id)
         |
         em_bright.em_bright_posterior_samples.s()
         |
         gracedb.upload.s(
             '{}.em_bright.json'.format(prefix), superevent_id,
-            'em-bright computed from "{}"'.format(info)
+            'em-bright computed from "{}"'.format(info),
+            'pe'
         )
     ).delay()
 
 
 @app.task(bind=True, shared=False)
 def _create_mattermost_channel(self, superevent_id):
     """
@@ -1173,22 +1174,29 @@
         )
     elif alert_type == 'preliminary':
         sent_label_canvas = gracedb.create_label.si(
             'GCN_PRELIM_SENT',
             superevent_id
         )
 
+    # NOTE: The following canvas structure was used to fix #480
     canvas = (
         group(download_andor_expose_group)
         |
-        group(voevent_canvas, kafka_alert_canvas)
-        |
         group(
-            sent_label_canvas,
-            circular_canvas,
+            voevent_canvas
+            |
+            group(
+                circular_canvas,
+
+                sent_label_canvas
+            ),
+
+            kafka_alert_canvas,
+
             high_profile_canvas
         )
     )
 
     canvas.apply_async()
```

### Comparing `gwcelery-2.0.6/gwcelery/tasks/p_astro.py` & `gwcelery-2.1.0/gwcelery/tasks/p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/raven.py` & `gwcelery-2.1.0/gwcelery/tasks/raven.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 """Search for GRB-GW coincidences with ligo-raven."""
 import ligo.raven.search
 from celery import group
 from celery.utils.log import get_task_logger
 
 from ..import app
+from .core import identity
 from . import external_skymaps
 from . import gracedb
 
 log = get_task_logger(__name__)
 
 
 @app.task(queue='exttrig',
           shared=False)
-def calculate_coincidence_far(superevent, exttrig, tl, th):
+def calculate_coincidence_far(superevent, exttrig, tl, th,
+                              use_superevent_skymap=None):
     """Compute coincidence FAR for external trigger and superevent
     coincidence by calling ligo.raven.search.calc_signif_gracedb,
     using sky map info if available.
 
     Parameters
     ----------
     superevent: dict
         superevent dictionary
     exttrig: dict
         external event dictionary
     tl: float
         start of coincident time window
     th: float
         end of coincident time window
+    use_superevent_skymap: bool
+        If True/False, use/don't use skymap info from superevent.
+        Else if None, check SKYMAP_READY label in external event.
 
     """
     superevent_id = superevent['superevent_id']
     exttrig_id = exttrig['graceid']
 
     #  Don't compute coinc FAR for SNEWS coincidences
     if exttrig['pipeline'] == 'SNEWS':
         return {}
 
     if ({'EXT_SKYMAP_READY', 'SKYMAP_READY'}.issubset(exttrig['labels']) or
             {'EXT_SKYMAP_READY', 'EM_READY'}.issubset(exttrig['labels'])):
         #  if both sky maps available, calculate spatial coinc far
-        use_preferred_event_skymap = 'SKYMAP_READY' not in exttrig['labels']
+        use_preferred_event_skymap = (
+            not use_superevent_skymap
+            if use_superevent_skymap is not None else
+            'SKYMAP_READY' not in exttrig['labels'])
         se_skymap = external_skymaps.get_skymap_filename(
             (superevent['preferred_event'] if use_preferred_event_skymap
              else superevent_id), is_gw=True)
         ext_skymap = external_skymaps.get_skymap_filename(
             exttrig_id, is_gw=False)
 
         return ligo.raven.search.calc_signif_gracedb(
@@ -183,15 +191,15 @@
                                     searches=searches,
                                     se_searches=se_searches)
 
 
 @app.task(queue='exttrig',
           shared=False)
 def raven_pipeline(raven_search_results, gracedb_id, alert_object, tl, th,
-                   gw_group):
+                   gw_group, use_superevent_skymap=None):
     """Executes much of the full raven pipeline, including adding
     the external trigger to the superevent, calculating the
     coincidence false alarm rate, and applying 'EM_COINC' to the
     appropriate events. Also a preimlinary alert will be triggered
     if the coincidence passes threshold.
 
     Parameters
@@ -200,14 +208,17 @@
         list of dictionaries of each related gracedb trigger
     gracedb_id: str
         ID of either a superevent or external trigger
     alert_object: dict
         Alert dictionary, either a superevent or an external event
     gw_group: str
         Burst or CBC
+    use_superevent_skymap: bool
+        If True/False, use/don't use skymap info from superevent.
+        Else if None, check SKYMAP_READY label in external event.
 
     """
     if not raven_search_results:
         return
     if 'S' not in gracedb_id:
         raven_search_results = preferred_superevent(raven_search_results)
     for result in raven_search_results:
@@ -225,24 +236,23 @@
         if ext_event['superevent'] is not None \
                 and ext_event['superevent'] != superevent['superevent_id']:
             return
 
         canvas = (
             gracedb.add_event_to_superevent.si(superevent_id, exttrig_id)
             |
-            calculate_coincidence_far.si(superevent, ext_event, tl, th)
-            |
-            update_coinc_far.s(superevent, ext_event)
+            calculate_coincidence_far.si(
+                superevent, ext_event, tl, th,
+                use_superevent_skymap=use_superevent_skymap
+            )
             |
             group(gracedb.create_label.si('EM_COINC', superevent_id),
                   gracedb.create_label.si('EM_COINC', exttrig_id),
                   trigger_raven_alert.s(superevent, gracedb_id,
-                                        ext_event, gw_group),
-                  external_skymaps.plot_overlap_integral.s(
-                      superevent, ext_event))
+                                        ext_event, gw_group))
         )
         canvas.delay()
 
 
 @app.task(queue='exttrig',
           shared=False)
 def preferred_superevent(raven_search_results):
@@ -378,14 +388,15 @@
     preferred_gwevent_id = superevent['preferred_event']
     superevent_id = superevent['superevent_id']
     ext_id = ext_event['graceid']
     gw_group = gw_group.lower()
     pipeline = ext_event['pipeline']
     trials_factor = app.conf['significant_alert_trials_factor'][gw_group]
     missing_skymap = True
+    comments = []
     messages = []
 
     #  Since the significance of SNEWS triggers is so high, we will publish
     #  any trigger coincident with a decently significant GW candidate
     if 'SNEWS' == pipeline:
         gw_far = superevent['far']
         far_type = 'gw'
@@ -426,52 +437,72 @@
                      ext_event['group'] == 'Test')
 
     #  If publishable, trigger an alert by applying `RAVEN_ALERT` label to
     #  preferred event
     if pass_far_threshold and not is_ext_subthreshold and \
             likely_real_ext_event and not missing_skymap and \
             not is_test_event and no_previous_alert:
-        messages.append(('RAVEN: publishing criteria met for {0}-{1}. '
+        comments.append(('RAVEN: publishing criteria met for {0}-{1}. '
                          'Triggering RAVEN alert'.format(
                              preferred_gwevent_id, ext_id)))
-        (
+        # Add label to local dictionary and to event on GraceDB server
+        # NOTE: We may prefer to apply the superevent label first and the grab
+        # labels to refresh in the future
+        superevent['labels'] += 'RAVEN_ALERT'
+        # Add RAVEN_ALERT to preferred event last to avoid race conditions
+        # where superevent is expected to have it once alert is issued
+        alert_canvas = (
             gracedb.create_label.si('RAVEN_ALERT', superevent_id)
             |
             gracedb.create_label.si('HIGH_PROFILE', superevent_id)
             |
             gracedb.create_label.si('RAVEN_ALERT', ext_id)
             |
             gracedb.create_label.si('RAVEN_ALERT', preferred_gwevent_id)
-        ).delay()
+        )
+    else:
+        alert_canvas = identity.si()
     if not pass_far_threshold:
-        messages.append(('RAVEN: publishing criteria not met for {0}-{1},'
+        comments.append(('RAVEN: publishing criteria not met for {0}-{1},'
                          ' {2} FAR (w/ trials) too large '
                          '({3:.4g} > {4:.4g})'.format(
                              preferred_gwevent_id, ext_id, far_type,
                              coinc_far_f, far_threshold)))
     if is_ext_subthreshold:
-        messages.append(('RAVEN: publishing criteria not met for {0}-{1},'
+        comments.append(('RAVEN: publishing criteria not met for {0}-{1},'
                          ' {1} is subthreshold'.format(preferred_gwevent_id,
                                                        ext_id)))
     if not likely_real_ext_event:
-        messages.append(('RAVEN: publishing criteria not met for {0}-{1},'
+        comments.append(('RAVEN: publishing criteria not met for {0}-{1},'
                          ' {1} is likely non-astrophysical.'.format(
                              preferred_gwevent_id, ext_id)))
     if is_test_event:
-        messages.append('RAVEN: {0}-{1} is non-astrophysical, '
+        comments.append('RAVEN: {0}-{1} is non-astrophysical, '
                         'at least one event is a Test event'.format(
                             preferred_gwevent_id, ext_id))
     if missing_skymap:
-        messages.append('RAVEN: Will only publish GRB coincidence '
+        comments.append('RAVEN: Will only publish GRB coincidence '
                         'if spatial-temporal FAR is present. '
                         'Waiting for both sky maps to be available '
                         'first.')
-    for message in messages:
-        gracedb.upload.si(None, None, superevent_id, message,
-                          tags=['ext_coinc']).delay()
+    for comment in comments:
+        messages.append(gracedb.upload.si(None, None, superevent_id, comment,
+                                          tags=['ext_coinc']))
+
+    # Update coincidence FAR with latest info, including the application of
+    # RAVEN_ALERT, then issue alert
+    (
+        update_coinc_far.si(coinc_far_dict, superevent, ext_event)
+        |
+        group(
+            alert_canvas,
+            external_skymaps.plot_overlap_integral.s(superevent, ext_event),
+            *messages
+        )
+    ).delay()
 
 
 @app.task(queue='exttrig',
           shared=False)
 def sog_paper_pipeline(ext_event, superevent):
     """Determine whether an a speed of gravity measurment manuscript should be
     triggered for a given coincidence.
```

### Comparing `gwcelery-2.0.6/gwcelery/tasks/rrt_utils.py` & `gwcelery-2.1.0/gwcelery/tasks/rrt_utils.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/skymaps.py` & `gwcelery-2.1.0/gwcelery/tasks/skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tasks/superevents.py` & `gwcelery-2.1.0/gwcelery/tasks/superevents.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,19 @@
 
 EARLY_WARNING_LABEL = 'EARLY_WARNING'
 """This label indicates that the superevent contains a significant
 early warning event."""
 
 EARLY_WARNING_SEARCH_NAME = 'EarlyWarning'
 """Search name for Early Warning searches. Only significant events
-result in
-consideration by the superevent manager."""
+result in consideration by the superevent manager."""
+
+SUBSOLAR_SEARCH_NAME = 'SSM'
+"""Search name for subsolar mass search. These are ignored by
+the superevent manager."""
 
 READY_LABEL = 'EM_READY'
 """This label indicates that a preferred event has been assigned and it
 has all data products required to make it ready for annotations."""
 
 
 @igwn_alert.handler('cbc_gstlal',
@@ -75,14 +78,17 @@
             far > app.conf['early_warning_alert_far_threshold'] / \
             app.conf['early_warning_alert_trials_factor']:
         log.info(
             "Skipping processing EW event %s because it does not"
             "meet significant event criterion", gid
         )
         return
+    elif search == SUBSOLAR_SEARCH_NAME:
+        log.info("Skipping processing subsolar search event %s", gid)
+        return
 
     priority = 1
     if alert_type == 'label_added':
         priority = 0
         label = payload['data']['name']
         group = payload['object']['group'].lower()
         if label == 'RAVEN_ALERT':
```

### Comparing `gwcelery-2.0.6/gwcelery/templates/fits_header.jinja2` & `gwcelery-2.1.0/gwcelery/templates/fits_header.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/templates/index.jinja2` & `gwcelery-2.1.0/gwcelery/templates/index.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,43 @@
                     </div>
                 </div>
             </form>
         </div>
     </div>
     <div class="card mb-3">
         <div class=card-header>
+            Create Medium Latency GRB GCN Circular
+        </div>
+        <div class=card-body>
+            <form method=post action="{{ url_for('create_medium_latency_gcn_circular') }}">
+                <div class="form-row">
+                    <div class=form-group>
+                        <div class=form-text>Print out a medium latency GRB GCN circular, either a detection or distance exclusion based on the false alarm probability.</div>
+                    </div>
+                </div>
+                <div class="form-row">
+                    <div class=form-group>
+                        <p class="text-danger">Warning: this will only work properly if either PyGRB or X-pipeline has uploaded files to the external event.</p>
+                    </div>
+                </div>
+                <div class="form-row">
+                    <div class="cform-group">
+                        <label class="sr-only" for=ext_event_id>External event ID</label>
+                        <input required name=ext_event_id class="form-control typeahead" placeholder="External event ID">
+                    </div>
+                    <div class="form-group">
+                        <label for=submit-button>&nbsp;</label>
+                        <button type=submit id=submit-button name=submit-button class="btn btn-primary">Submit</button>
+                    </div>
+                </div>
+            </form>
+        </div>
+    </div>
+    <div class="card mb-3">
+        <div class=card-header>
             Change Preferred Event in Superevent
         </div>
         <div class=card-body>
             <form method=post action="{{ url_for('change_preferred_event') }}">
                 <div class=form-row>
                     <div class=form-group>
                         <div class=form-text>Change the preferred event of a superevent. Do not send any preliminary or update GCN Notice.</div>
```

#### html2text {}

```diff
@@ -48,14 +48,21 @@
 using the above form.
 Superevent ID [superevent_id       ]
 ⁰ Sky Localization
 ⁰ EM_Bright
 ⁰ P_Astro
 ⁰ RAVEN Coincidence
   Submit
+Create Medium Latency GRB GCN Circular
+Print out a medium latency GRB GCN circular, either a detection or distance
+exclusion based on the false alarm probability.
+Warning: this will only work properly if either PyGRB or X-pipeline has
+uploaded files to the external event.
+External event ID [ext_event_id        ]
+  Submit
 Change Preferred Event in Superevent
 Change the preferred event of a superevent. Do not send any preliminary or
 update GCN Notice.
 Superevent ID [superevent_id       ]
 Preferred event ID [event_id            ]
   Submit
 ** Really Change Preferred Event? **
```

### Comparing `gwcelery-2.0.6/gwcelery/templates/lalinference.jinja2` & `gwcelery-2.1.0/gwcelery/templates/lalinference.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/templates/rapidpe.jinja2` & `gwcelery-2.1.0/gwcelery/templates/rapidpe.jinja2`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [General]
 output_parent_directory={{ rundir }}
 #submit_only_at_exact_signal_position=1
 #Note: if use_skymap is set, set the skymap directory/file pattern to match in the [Event] section
 use_skymap=0
 use_event_spin=True
+cProfile=True
 
 gracedb_url={{ gracedb_url }}
 
 #If you want to perform multiple studies on a single event, you can set this. And command line arguments passed to create_submit_dag will be ignored. If you do NOT set this = 1, the [Event] section in the config file will be ignored, and command line arguments with event specific information is required
 event_parameters_in_config_file=0
 
 #was n_samples_per_job in old RIT code. This defines how many iterations of rapidPE are run. Before each new iteration a new grid is generated which is finer than the previous grid, and covers a smaller region of intrinsic parameter space (hopefully around the signal)
@@ -48,22 +49,23 @@
 #WARNING: this needs to be sed here and in [GridRefine], unless you want it to refine only in mass space
 intrinsic_param_to_search=[mass1,mass2]
 
 web_dir={{ webdir }}
 
 [Event]
 superevent_id={{ superevent_id }}
+run_mode={{ run_mode }}
 frame_data_types={{ frame_data_types | tojson }}
 mdc_event_injection_file =/home/vinaya.valsan/rapidPE/RapidPE_RIFT_Developments/RapidPE-RIFT_fork/gracedb_playground_events/injection_campaign_studies/lowlatency-replay-distributions/minSNR-4/injections-minSNR-4.xml.gz
 mdc_time_offset=101760000
 #Anything specified in this section is passed verbatim to rapidpe_compute_intrinsic_grid in generate_initial_grid_based_of_gstlal_O2_overlaps.py
 [InitialGridOnly]
 #mc-min = 5
 #mc-max = 61
-points-per-side=5
+points-per-side=10
 
 [InitialGridSetup]
 #The arguments in this section are passed directly to the command line in the condor dag job which does the grid refinement. Do not include any arguments which change per iteration or per node.
 ##NOTE: The script is currently setup to work with rapidpe_compute_intrinsic_grid or util_ConstructIntrinsicPosterior.py
 
 [GridRefine]
 no-exact-match=
@@ -130,9 +132,17 @@
 distance-marginalization=
 # TODO: determine where to store the look-up table
 distance-marginalization-lookup-table=/home/vinaya.valsan/rapidPE/RapidPE_RIFT/generate_dist_lookup/distance_marginalization_lookup.npz
 vectorized=
 gpu=
 force-xpy=
 sampler-method=adaptive_cartesian_gpu
-cProfile=
 manual-logarithm-offset=
+
+[Pastro]
+category_rates={"R_bns": 3.040442568596489e-07,"R_nsbh": 2.187249638130701e-07,"R_bbh": 2.1323454514234493e-06}
+
+category_rates_inj={"R_bns": 3.040442568596489e-07,"R_nsbh": 2.187249638130701e-07,"R_bbh": 2.1323454514234493e-06}
+
+far_threshold=0.0002777777777777778
+prior_boundary={"m_max_bank": 200.0,"m_min_bank": 0.98,"m_max_ns": 3.0,"q_min_bank": 0.05,"q_max_bank": 1}
+rankstat_pdf_file=/home/gstlalcbc.online/observing/4/pre-engineering/runs/trigs.renee_Apr21/dist_stat_pdfs/H1L1-GSTLAL_DIST_STAT_PDFS-0-0.xml.gz
```

### Comparing `gwcelery-2.0.6/gwcelery/templates/vector_table.jinja2` & `gwcelery-2.1.0/gwcelery/templates/vector_table.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/conftest.py` & `gwcelery-2.1.0/gwcelery/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/G000012_S0040_preferred.json` & `gwcelery-2.1.0/gwcelery/tests/data/G000012_S0040_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/G298048-1-Initial.xml` & `gwcelery-2.1.0/gwcelery/tests/data/G298048-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/G298048_log.json` & `gwcelery-2.1.0/gwcelery/tests/data/G298048_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json` & `gwcelery-2.1.0/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/MS220722v.xml` & `gwcelery-2.1.0/gwcelery/tests/data/MS220722v.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits` & `gwcelery-2.1.0/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/S230413b.json` & `gwcelery-2.1.0/gwcelery/tests/data/S230413b.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/S230413g.json` & `gwcelery-2.1.0/gwcelery/tests/data/S230413g.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/S230413h.json` & `gwcelery-2.1.0/gwcelery/tests/data/S230413h.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/T0212_S0039_preferred.json` & `gwcelery-2.1.0/gwcelery/tests/data/T0212_S0039_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json` & `gwcelery-2.1.0/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/T0219_S0041_nopreferred.json` & `gwcelery-2.1.0/gwcelery/tests/data/T0219_S0041_nopreferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/agile_grb_gcn.xml` & `gwcelery-2.1.0/gwcelery/tests/data/agile_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/coinc.xml` & `gwcelery-2.1.0/gwcelery/tests/data/coinc.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/externaltrigger_original_data.xml` & `gwcelery-2.1.0/gwcelery/tests/data/externaltrigger_original_data.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/fermi_grb_gcn.xml` & `gwcelery-2.1.0/gwcelery/tests/data/fermi_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/fermi_initial_grb_gcn.xml` & `gwcelery-2.1.0/gwcelery/tests/data/fermi_initial_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/fermi_noise_gcn.xml` & `gwcelery-2.1.0/gwcelery/tests/data/fermi_noise_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/fermi_noise_gcn_2.xml` & `gwcelery-2.1.0/gwcelery/tests/data/fermi_noise_gcn_2.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml` & `gwcelery-2.1.0/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml` & `gwcelery-2.1.0/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/fits_header_result.html` & `gwcelery-2.1.0/gwcelery/tests/data/fits_header_result.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/gracedb_externaltrigger_log.json` & `gwcelery-2.1.0/gwcelery/tests/data/gracedb_externaltrigger_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_detchar.json` & `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_detchar.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_exttrig_creation.json` & `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_exttrig_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json` & `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_psd.json` & `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_psd.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_snews_creation.json` & `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_snews_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_snews_test_creation.json` & `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_snews_test_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_subgrb_creation.json` & `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_subgrb_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_superevent_creation.json` & `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_superevent_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_voevent.json` & `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_voevent.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/integral_grb_gcn.xml` & `gwcelery-2.1.0/gwcelery/tests/data/integral_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/integral_mdc_gcn.xml` & `gwcelery-2.1.0/gwcelery/tests/data/integral_mdc_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.1.0/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf`

 * *Files 1% similar despite different names*

```diff
@@ -146,22 +146,22 @@
 00000910: 2066 6f72 2074 6865 2066 6972 7374 2061   for the first a
 00000920: 7578 696c 6961 7279 2074 6162 6c65 2064  uxiliary table d
 00000930: 6174 6100 209f 3edd 3600 0000 0000 0000  ata. .>.6.......
 00000940: 0102 1500 0000 0700 6368 6b53 756d 0007  ........chkSum..
 00000950: 0049 4e54 5f34 5500 1000 5374 7275 6374  .INT_4U...Struct
 00000960: 2063 6865 636b 7375 6d00 bccb b902 8500   checksum.......
 00000970: 0000 0000 0000 0103 0000 0000 0500 6777  ..............gw
-00000980: 7079 0000 0000 0082 7f00 0070 8d74 30b8  py.........p.t0.
+00000980: 7079 0000 0000 0000 0000 0000 0000 00b8  py..............
 00000990: 8183 4800 0000 0025 0000 0000 0000 0010  ..H....%........
 000009a0: 4000 0000 0000 0000 0000 0000 0000 0000  @...............
 000009b0: 0000 0005 0000 0000 0000 0000 0000 0000  ................
 000009c0: 0000 0000 000b 0000 0000 0000 0000 0000  ................
 000009d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000009e0: 0000 0000 0000 0000 0000 0000 0000 00ec  ................
-000009f0: d052 c43b 0000 0000 0000 0001 0101 0000  .R.;............
+000009e0: 0000 0000 0000 0000 0000 0000 0000 0047  ...............G
+000009f0: 6661 b63b 0000 0000 0000 0001 0101 0000  fa.;............
 00000a00: 000b 0046 7244 6574 6563 746f 7200 0500  ...FrDetector...
 00000a10: 1800 4465 7465 6374 6f72 2044 6174 6120  ..Detector Data 
 00000a20: 5374 7275 6374 7572 6500 94bd 3e10 2500  Structure...>.%.
 00000a30: 0000 0000 0000 0102 1600 0000 0500 6e61  ..............na
 00000a40: 6d65 0007 0053 5452 494e 4700 0100 006c  me...STRING....l
 00000a50: ebf8 8528 0000 0000 0000 0001 0217 0000  ...(............
 00000a60: 0007 0070 7265 6669 7800 0800 4348 4152  ...prefix...CHAR
@@ -421,494 +421,494 @@
 00001a40: 4641 505f 4f56 4c5f 3332 5f32 3034 3800  FAP_OVL_32_2048.
 00001a50: 1700 4c31 3a49 4451 2d46 4150 5f4f 564c  ..L1:IDQ-FAP_OVL
 00001a60: 5f33 325f 3230 3438 0001 0000 0000 0000  _32_2048........
 00001a70: 0000 0000 0000 0000 0000 0010 4000 0000  ............@...
 00001a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001a90: 0000 0000 0000 0000 0000 0014 0002 0000  ................
 00001aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ab0: 0000 0000 0000 0000 0017 3b04 fb8f 0000  ..........;.....
+00001ab0: 0000 0000 0000 0000 0017 3b04 fb87 0000  ..........;.....
 00001ac0: 0000 0000 0001 1402 0000 0017 004c 313a  .............L1:
 00001ad0: 4944 512d 4641 505f 4f56 4c5f 3332 5f32  IDQ-FAP_OVL_32_2
 00001ae0: 3034 3800 0101 0500 0004 0000 0000 0000  048.............
-00001af0: 2700 0000 0000 0000 789c edc5 310d 0000  '.......x...1...
-00001b00: 0c03 a0d5 bfe9 1d55 d104 1e72 15db b66d  .......U...r...m
-00001b10: dbb6 6ddb b66d dbb6 3dfb 0333 c004 0101  ..m..m..=..3....
-00001b20: 0000 0000 0400 0000 0000 0000 0000 0000  ................
-00001b30: 0070 3f00 0000 0000 0000 0002 0073 0001  .p?..........s..
-00001b40: 0000 0000 0000 0000 7459 7945 4100 0000  ........tYyEA...
-00001b50: 0000 0000 0101 0400 0000 0d00 4672 456e  ............FrEn
-00001b60: 644f 6646 7261 6d65 0007 001c 0045 6e64  dOfFrame.....End
-00001b70: 206f 6620 4672 616d 6520 4461 7461 2053   of Frame Data S
-00001b80: 7472 7563 7475 7265 009c ab33 e258 0000  tructure...3.X..
-00001b90: 0000 0000 0001 0247 0000 0004 0072 756e  .......G.....run
-00001ba0: 0007 0049 4e54 5f34 5300 3500 5275 6e20  ...INT_4S.5.Run 
-00001bb0: 6e75 6d62 6572 3b20 7361 6d65 2061 7320  number; same as 
-00001bc0: 696e 2046 7261 6d65 4865 6164 6572 2072  in FrameHeader r
-00001bd0: 756e 206e 756d 6265 7220 6461 7475 6d2e  un number datum.
-00001be0: 000b 9641 5b87 0000 0000 0000 0001 0248  ...A[..........H
-00001bf0: 0000 0006 0066 7261 6d65 0007 0049 4e54  .....frame...INT
-00001c00: 5f34 5500 6200 4672 616d 6520 6e75 6d62  _4U.b.Frame numb
-00001c10: 6572 2c20 6d6f 6e6f 746f 6e69 6361 6c6c  er, monotonicall
-00001c20: 7920 696e 6372 6561 7369 6e67 2075 6e74  y increasing unt
-00001c30: 696c 2065 6e64 206f 6620 7275 6e3b 2073  il end of run; s
-00001c40: 616d 6520 6173 2069 6e20 4672 616d 6520  ame as in Frame 
-00001c50: 4865 6164 6572 2072 756e 206e 756d 6265  Header run numbe
-00001c60: 7220 6461 7475 6d00 ba5a b3d1 4700 0000  r datum..Z..G...
-00001c70: 0000 0000 0102 4900 0000 0700 4754 696d  ......I.....GTim
-00001c80: 6553 0007 0049 4e54 5f34 5500 2100 4672  eS...INT_4U.!.Fr
-00001c90: 616d 6520 7374 6172 7420 7469 6d65 2069  ame start time i
-00001ca0: 6e20 4750 5320 5365 636f 6e64 732e 0018  n GPS Seconds...
-00001cb0: add0 ff56 0000 0000 0000 0001 024a 0000  ...V.........J..
-00001cc0: 0007 0047 5469 6d65 4e00 0700 494e 545f  ...GTimeN...INT_
-00001cd0: 3455 0030 0046 7261 6d65 2073 7461 7274  4U.0.Frame start
-00001ce0: 2074 696d 6520 7265 7369 6475 616c 2c20   time residual, 
-00001cf0: 696e 7465 6765 7220 6e61 6e6f 7365 636f  integer nanoseco
-00001d00: 6e64 732e 0064 338f ba36 0000 0000 0000  nds..d3..6......
-00001d10: 0001 024b 0000 0007 0063 686b 5375 6d00  ...K.....chkSum.
-00001d20: 0700 494e 545f 3455 0010 0053 7472 7563  ..INT_4U...Struc
-00001d30: 7420 6368 6563 6b73 756d 0022 ca11 6222  t checksum."..b"
-00001d40: 0000 0000 0000 0001 0700 0000 0000 0000  ................
-00001d50: 0082 7f00 0000 0000 0000 0000 007a 9554  .............z.T
-00001d60: 1f37 0000 0000 0000 0001 0100 0000 0006  .7..............
-00001d70: 0046 7254 4f43 0013 0019 0053 696d 756c  .FrTOC.....Simul
-00001d80: 6174 6564 2044 6174 6120 5374 7275 6374  ated Data Struct
-00001d90: 7572 6500 7c69 656b 4800 0000 0000 0000  ure.|iekH.......
-00001da0: 0102 0000 0000 0700 554c 6561 7053 0007  ........ULeapS..
-00001db0: 0049 4e54 5f32 5300 2200 4672 6f6d 2074  .INT_2S.".From t
-00001dc0: 6865 2066 6972 7374 2046 7261 6d65 4820  he first FrameH 
-00001dd0: 696e 2074 6865 2066 696c 6500 0087 5256  in the file...RV
-00001de0: 4300 0000 0000 0000 0102 0100 0000 0700  C...............
-00001df0: 6e46 7261 6d65 0007 0049 4e54 5f34 5500  nFrame...INT_4U.
-00001e00: 1d00 4e75 6d62 6572 206f 6620 6672 616d  ..Number of fram
-00001e10: 6573 2069 6e20 7468 6520 6669 6c65 00cc  es in the file..
-00001e20: 3d5f 7370 0000 0000 0000 0001 0202 0000  =_sp............
-00001e30: 000c 0064 6174 6151 7561 6c69 7479 000f  ...dataQuality..
-00001e40: 0049 4e54 5f34 555b 6e46 7261 6d65 5d00  .INT_4U[nFrame].
-00001e50: 3d00 4172 7261 7920 6f66 2069 6e74 6567  =.Array of integ
-00001e60: 6572 2051 4120 776f 7264 7320 6672 6f6d  er QA words from
-00001e70: 2065 6163 6820 4672 616d 6548 2028 7369   each FrameH (si
-00001e80: 7a65 206f 6620 6e46 7261 6d65 7329 0088  ze of nFrames)..
-00001e90: 6738 c05f 0000 0000 0000 0001 0203 0000  g8._............
-00001ea0: 0007 0047 5469 6d65 5300 0f00 494e 545f  ...GTimeS...INT_
-00001eb0: 3455 5b6e 4672 616d 655d 0031 0041 7272  4U[nFrame].1.Arr
-00001ec0: 6179 206f 6620 696e 7465 6765 7220 4750  ay of integer GP
-00001ed0: 5320 6672 6165 2074 696d 6573 2028 7369  S frae times (si
-00001ee0: 7a65 206f 6620 6e46 7261 6d65 7300 d5b2  ze of nFrames...
-00001ef0: 6755 7600 0000 0000 0000 0102 0400 0000  gUv.............
-00001f00: 0700 4754 696d 654e 000f 0049 4e54 5f34  ..GTimeN...INT_4
-00001f10: 555b 6e46 7261 6d65 5d00 4800 4172 7261  U[nFrame].H.Arra
-00001f20: 7920 6f66 2069 6e74 6567 6572 2047 5053  y of integer GPS
-00001f30: 2072 6573 6964 7561 6c20 6e61 6e6f 7365   residual nanose
-00001f40: 636f 6e64 7320 666f 7220 7468 6520 6672  conds for the fr
-00001f50: 616d 6520 2873 697a 6520 6f66 206e 4672  ame (size of nFr
-00001f60: 616d 6500 154d fabb 6000 0000 0000 0000  ame..M..`.......
-00001f70: 0102 0500 0000 0300 6474 000f 0052 4541  ........dt...REA
-00001f80: 4c5f 385b 6e46 7261 6d65 5d00 3600 4172  L_8[nFrame].6.Ar
-00001f90: 7261 7920 6f66 2066 7261 6d65 2064 7572  ray of frame dur
-00001fa0: 6174 696f 6e73 2069 6e20 7365 636f 6e64  ations in second
-00001fb0: 7328 2073 697a 6520 6f66 206e 4672 616d  s( size of nFram
-00001fc0: 6573 2900 0d06 b877 5200 0000 0000 0000  es)....wR.......
-00001fd0: 0102 0600 0000 0500 7275 6e73 000f 0049  ........runs...I
-00001fe0: 4e54 5f34 535b 6e46 7261 6d65 5d00 2600  NT_4S[nFrame].&.
-00001ff0: 4172 7261 7920 6f66 2072 756e 206e 756d  Array of run num
-00002000: 6265 7273 2028 7369 7a65 206f 6620 6e46  bers (size of nF
-00002010: 7261 6d65 2900 ca0b 9f5c 5500 0000 0000  rame)....\U.....
-00002020: 0000 0102 0700 0000 0600 6672 616d 6500  ..........frame.
-00002030: 0f00 494e 545f 3455 5b6e 4672 616d 655d  ..INT_4U[nFrame]
-00002040: 0028 0041 7272 6179 206f 6620 6672 616d  .(.Array of fram
-00002050: 6520 6e75 6d62 6572 7320 2873 697a 6520  e numbers (size 
-00002060: 6f66 206e 4672 616d 6529 0031 285d 2581  of nFrame).1(]%.
-00002070: 0000 0000 0000 0001 0208 0000 000a 0070  ...............p
-00002080: 6f73 6974 696f 6e48 000f 0049 4e54 5f38  ositionH...INT_8
-00002090: 555b 6e46 7261 6d65 5d00 5000 4172 7261  U[nFrame].P.Arra
-000020a0: 7920 6f66 2046 7261 6d65 4820 706f 7369  y of FrameH posi
-000020b0: 7469 6f6e 732c 2069 6e20 6279 7465 732c  tions, in bytes,
-000020c0: 2066 726f 6d20 7468 6520 6267 696e 6e69   from the bginni
-000020d0: 6e67 206f 6620 6669 6c65 2028 7369 7a65  ng of file (size
-000020e0: 206f 6620 6e46 7261 6d65 2900 db18 22e8   of nFrame)...".
-000020f0: 8700 0000 0000 0000 0102 0900 0000 0a00  ................
-00002100: 6e46 6972 7374 4144 4300 0f00 494e 545f  nFirstADC...INT_
-00002110: 3855 5b6e 4672 616d 655d 0056 0041 7272  8U[nFrame].V.Arr
-00002120: 6179 206f 6620 6669 7273 7420 4672 4144  ay of first FrAD
-00002130: 4344 6174 6120 706f 7369 7469 6f6e 732c  CData positions,
-00002140: 2069 6e20 6279 7465 732c 2066 726f 6d20   in bytes, from 
-00002150: 6265 6769 6e6e 696e 6720 6f66 2066 696c  beginning of fil
-00002160: 6520 2873 697a 6520 6f66 206e 4672 616d  e (size of nFram
-00002170: 6529 00b7 d5cd 8b86 0000 0000 0000 0001  e)..............
-00002180: 020a 0000 000a 006e 4669 7273 7453 6572  .......nFirstSer
-00002190: 000f 0049 4e54 5f38 555b 6e46 7261 6d65  ...INT_8U[nFrame
-000021a0: 5d00 5500 4172 7261 7920 6f66 2066 6972  ].U.Array of fir
-000021b0: 7374 2046 7253 6572 4461 7461 2070 6f73  st FrSerData pos
-000021c0: 6974 696f 6e73 2069 6e20 6279 7465 732c  itions in bytes,
-000021d0: 2066 726f 6d20 6265 6769 6e6e 696e 6720   from beginning 
-000021e0: 6f66 2066 696c 6520 2873 697a 6520 6f66  of file (size of
-000021f0: 206e 4672 616d 6529 00fa c761 6b87 0000   nFrame)...ak...
-00002200: 0000 0000 0001 020b 0000 000c 006e 4669  .............nFi
-00002210: 7273 7454 6162 6c65 000f 0049 4e54 5f38  rstTable...INT_8
-00002220: 555b 6e46 7261 6d65 5d00 5400 4172 7261  U[nFrame].T.Arra
-00002230: 7920 6f66 2066 6972 7374 2046 7254 6162  y of first FrTab
-00002240: 6c65 2070 6f73 6974 696f 6e73 2c20 696e  le positions, in
-00002250: 2062 7974 6573 2c20 6672 6f6d 2062 6567   bytes, from beg
-00002260: 696e 6e69 6e67 206f 6620 6669 6c65 2028  inning of file (
-00002270: 7369 7a65 206f 6620 6e46 7261 6d65 2900  size of nFrame).
-00002280: 1016 52a6 8300 0000 0000 0000 0102 0c00  ..R.............
-00002290: 0000 0a00 6e46 6972 7374 4d73 6700 0f00  ....nFirstMsg...
-000022a0: 494e 545f 3855 5b6e 4672 616d 655d 0052  INT_8U[nFrame].R
-000022b0: 0041 7272 6179 206f 6620 6669 7273 7420  .Array of first 
-000022c0: 4672 4d73 6720 706f 7369 7469 6f6e 732c  FrMsg positions,
-000022d0: 2069 6e20 6279 7465 732c 2066 726f 6d20   in bytes, from 
-000022e0: 6265 6769 6e6e 696e 6720 6f66 2066 696c  beginning of fil
-000022f0: 6520 2873 697a 6520 6f66 206e 4672 616d  e (size of nFram
-00002300: 6529 00b9 e1c6 f949 0000 0000 0000 0001  e).....I........
-00002310: 020d 0000 0004 006e 5348 0007 0049 4e54  .......nSH...INT
-00002320: 5f34 5500 2600 4e75 6d62 6572 206f 6620  _4U.&.Number of 
-00002330: 4672 5348 2073 7472 7563 7475 7265 7320  FrSH structures 
-00002340: 696e 2074 6865 2066 696c 6500 f46c 0bb0  in the file..l..
-00002350: 4900 0000 0000 0000 0102 0e00 0000 0500  I...............
-00002360: 5348 6964 000c 0049 4e54 5f32 555b 6e53  SHid...INT_2U[nS
-00002370: 485d 0020 0041 7272 6179 206f 6620 4672  H]. .Array of Fr
-00002380: 5348 2049 4473 2028 7369 7a65 206f 6620  SH IDs (size of 
-00002390: 6e53 4829 0010 5b23 074d 0000 0000 0000  nSH)..[#.M......
-000023a0: 0001 020f 0000 0007 0053 486e 616d 6500  .........SHname.
-000023b0: 0c00 5354 5249 4e47 5b6e 5348 5d00 2200  ..STRING[nSH].".
-000023c0: 4172 7261 7920 6f66 2046 7253 4820 6e61  Array of FrSH na
-000023d0: 6d65 7320 2873 697a 6520 6f66 206e 5348  mes (size of nSH
-000023e0: 2900 a664 b4df 5c00 0000 0000 0000 0102  )..d..\.........
-000023f0: 1000 0000 0a00 6e44 6574 6563 746f 7200  ......nDetector.
-00002400: 0700 494e 545f 3455 0033 004e 756d 6265  ..INT_4U.3.Numbe
-00002410: 7220 6f66 2064 6973 7469 6e63 7420 7479  r of distinct ty
-00002420: 7065 7320 6f66 2046 7244 6574 6563 746f  pes of FrDetecto
-00002430: 7220 696e 2074 6865 2066 696c 6500 fa46  r in the file..F
-00002440: 0067 8100 0000 0000 0000 0102 1100 0000  .g..............
-00002450: 0d00 6e61 6d65 4465 7465 6374 6f72 0012  ..nameDetector..
-00002460: 0053 5452 494e 475b 6e44 6574 6563 746f  .STRING[nDetecto
-00002470: 725d 004a 0041 7272 6179 206f 6620 4672  r].J.Array of Fr
-00002480: 4465 7465 6374 6f72 206e 616d 6573 2028  Detector names (
-00002490: 7369 7a65 206f 6620 6e44 6574 6563 746f  size of nDetecto
-000024a0: 7229 2e20 5468 6579 2061 7070 6561 7220  r). They appear 
-000024b0: 616c 7068 6162 6574 6963 616c 6c79 0011  alphabetically..
-000024c0: 11d2 a589 0000 0000 0000 0001 0212 0000  ................
-000024d0: 0011 0070 6f73 6974 696f 6e44 6574 6563  ...positionDetec
-000024e0: 746f 7200 1200 494e 545f 3855 5b6e 4465  tor...INT_8U[nDe
-000024f0: 7465 6374 6f72 5d00 4e00 4172 7261 7920  tector].N.Array 
-00002500: 6f66 2046 7244 6574 6563 746f 7220 706f  of FrDetector po
-00002510: 7369 7469 6f6e 7320 6672 6f6d 2074 6865  sitions from the
-00002520: 2062 6567 696e 6e69 6e67 206f 6620 6669   beginning of fi
-00002530: 6c65 2028 7369 7a65 206f 6620 6e44 6574  le (size of nDet
-00002540: 6563 746f 7229 2e00 8345 9ff0 5800 0000  ector)...E..X...
-00002550: 0000 0000 0102 1300 0000 0a00 6e53 7461  ............nSta
-00002560: 7454 7970 6500 0700 494e 545f 3455 002f  tType...INT_4U./
-00002570: 004e 756d 6265 7220 6f66 2073 7461 7469  .Number of stati
-00002580: 6320 6461 7461 2062 6c6f 636b 2074 7970  c data block typ
-00002590: 6573 2069 6e20 7468 6520 6669 6c65 2e00  es in the file..
-000025a0: 0f05 6246 6000 0000 0000 0000 0102 1400  ..bF`...........
-000025b0: 0000 0900 6e61 6d65 5374 6174 0012 0053  ....nameStat...S
-000025c0: 5452 494e 475b 6e53 7461 7454 7970 655d  TRING[nStatType]
-000025d0: 002d 0041 7272 6179 206f 6620 4672 5374  .-.Array of FrSt
-000025e0: 6174 4461 7461 206e 616d 6520 2873 697a  atData name (siz
-000025f0: 6520 6f66 206e 5374 6174 5479 7065 2900  e of nStatType).
-00002600: a3bf 4547 5d00 0000 0000 0000 0102 1500  ..EG]...........
-00002610: 0000 0900 6465 7465 6374 6f72 0012 0053  ....detector...S
-00002620: 5452 494e 475b 6e53 7461 7454 7970 655d  TRING[nStatType]
-00002630: 002a 0041 7272 6179 206f 6620 4465 7465  .*.Array of Dete
-00002640: 6374 6f72 206e 616d 6528 7369 7a65 206f  ctor name(size o
-00002650: 6620 6e53 7461 7454 7970 6529 0041 b642  f nStatType).A.B
-00002660: 9d7b 0000 0000 0000 0001 0216 0000 000e  .{..............
-00002670: 006e 5374 6174 496e 7374 616e 6365 0012  .nStatInstance..
-00002680: 0049 4e54 5f34 555b 6e53 7461 7454 7970  .INT_4U[nStatTyp
-00002690: 655d 0043 0041 7272 6179 206f 6620 6e75  e].C.Array of nu
-000026a0: 6d62 6572 206f 6620 696e 7374 616e 6365  mber of instance
-000026b0: 2066 6f72 2065 6163 6820 4672 5374 6174   for each FrStat
-000026c0: 4461 7461 2873 697a 6520 6f66 206e 5374  Data(size of nSt
-000026d0: 6174 5479 7065 2900 66b8 774f 4b00 0000  atType).f.wOK...
-000026e0: 0000 0000 0102 1700 0000 0b00 6e54 6f74  ............nTot
-000026f0: 616c 5374 6174 0007 0049 4e54 5f34 5500  alStat...INT_4U.
-00002700: 2100 5375 6d6d 6174 696f 6e20 6f66 206e  !.Summation of n
-00002710: 5374 6174 496e 7374 616e 6365 2061 7272  StatInstance arr
-00002720: 6179 0089 b4e7 f874 0000 0000 0000 0001  ay.....t........
-00002730: 0218 0000 0007 0074 5374 6172 7400 1300  .......tStart...
-00002740: 494e 545f 3455 5b6e 546f 7461 6c53 7461  INT_4U[nTotalSta
-00002750: 745d 0042 0041 7272 6179 206f 6620 4750  t].B.Array of GP
-00002760: 5320 696e 7465 6765 7220 7374 6172 7420  S integer start 
-00002770: 7469 6d65 732c 2069 6e20 7365 636f 6e64  times, in second
-00002780: 7320 2873 697a 6520 6f66 206e 546f 7461  s (size of nTota
-00002790: 6c53 7461 7429 001a 531d 0970 0000 0000  lStat)..S..p....
-000027a0: 0000 0001 0219 0000 0005 0074 456e 6400  ...........tEnd.
-000027b0: 1300 494e 545f 3455 5b6e 546f 7461 6c53  ..INT_4U[nTotalS
-000027c0: 7461 745d 0040 0041 7272 6179 206f 6620  tat].@.Array of 
-000027d0: 4750 5320 696e 7465 6765 7220 656e 6420  GPS integer end 
-000027e0: 7469 6d65 732c 2069 6e20 7365 636f 6e64  times, in second
-000027f0: 7320 2873 697a 6520 6f66 206e 546f 7461  s (size of nTota
-00002800: 6c53 7461 7429 0045 668b 4d5e 0000 0000  lStat).Ef.M^....
-00002810: 0000 0001 021a 0000 0008 0076 6572 7369  ...........versi
-00002820: 6f6e 0013 0049 4e54 5f34 555b 6e54 6f74  on...INT_4U[nTot
-00002830: 616c 5374 6174 5d00 2b00 4172 7261 7920  alStat].+.Array 
-00002840: 6f66 2076 6572 7369 6f6e 2074 696d 6520  of version time 
-00002850: 2873 697a 6520 6f66 206e 546f 7461 6c53  (size of nTotalS
-00002860: 7461 7429 0093 e259 1d82 0000 0000 0000  tat)...Y........
-00002870: 0001 021b 0000 000d 0070 6f73 6974 696f  .........positio
-00002880: 6e53 7461 7400 1300 494e 545f 3855 5b6e  nStat...INT_8U[n
-00002890: 546f 7461 6c53 7461 745d 004a 0041 7272  TotalStat].J.Arr
-000028a0: 6179 206f 6620 4672 5374 6174 4461 7461  ay of FrStatData
-000028b0: 2070 6f73 6974 696f 6e73 2066 726f 6d20   positions from 
-000028c0: 6265 6769 6e6e 696e 6720 6f66 2066 696c  beginning of fil
-000028d0: 6520 2873 697a 6520 6f66 206e 546f 7461  e (size of nTota
-000028e0: 6c53 7461 7429 002e 51de 564e 0000 0000  lStat)..Q.VN....
-000028f0: 0000 0001 021c 0000 0005 006e 4144 4300  ...........nADC.
-00002900: 0700 494e 545f 3455 002a 004e 756d 6265  ..INT_4U.*.Numbe
-00002910: 7220 6f66 2075 6e69 7175 6520 4672 4164  r of unique FrAd
-00002920: 6344 6174 6120 6e61 6d65 7320 696e 2066  cData names in f
-00002930: 696c 652e 0007 54ee e143 0000 0000 0000  ile...T..C......
-00002940: 0001 021d 0000 0005 006e 616d 6500 0d00  .........name...
-00002950: 5354 5249 4e47 5b6e 4144 435d 0019 0041  STRING[nADC]...A
-00002960: 7272 6179 206f 6620 4672 4164 6344 6174  rray of FrAdcDat
-00002970: 6120 6e61 6d65 7300 89b1 c3ad 4800 0000  a names.....H...
-00002980: 0000 0000 0102 1e00 0000 0a00 6368 616e  ............chan
-00002990: 6e65 6c49 4400 0d00 494e 545f 3455 5b6e  nelID...INT_4U[n
-000029a0: 4144 435d 0019 0041 7272 6179 206f 6620  ADC]...Array of 
-000029b0: 4144 4320 6368 616e 6e65 6c20 4944 7300  ADC channel IDs.
-000029c0: 251b 8f78 4400 0000 0000 0000 0102 1f00  %..xD...........
-000029d0: 0000 0800 6772 6f75 7049 4400 0d00 494e  ....groupID...IN
-000029e0: 545f 3455 5b6e 4144 435d 0017 0041 7272  T_4U[nADC]...Arr
-000029f0: 6179 206f 6620 4144 4320 6772 6f75 7020  ay of ADC group 
-00002a00: 4944 7300 ec33 7c9e 9e00 0000 0000 0000  IDs..3|.........
-00002a10: 0102 2000 0000 0c00 706f 7369 7469 6f6e  .. .....position
-00002a20: 4144 4300 1500 494e 545f 3855 5b6e 4144  ADC...INT_8U[nAD
-00002a30: 435d 5b6e 4672 616d 655d 0065 0041 7272  C][nFrame].e.Arr
-00002a40: 6179 206f 6620 6c69 7374 7320 6f66 2046  ay of lists of F
-00002a50: 7241 6463 4461 7461 206f 6666 7365 7420  rAdcData offset 
-00002a60: 706f 7369 7469 6f6e 732c 2069 6e20 6279  positions, in by
-00002a70: 7465 732c 2066 726f 6d20 6265 6769 6e6e  tes, from beginn
-00002a80: 696e 6720 6f66 2066 696c 6520 2873 697a  ing of file (siz
-00002a90: 6520 6f66 206e 4672 616d 652a 6e41 4443  e of nFrame*nADC
-00002aa0: 2900 6d54 ccf2 5000 0000 0000 0000 0102  ).mT..P.........
-00002ab0: 2100 0000 0600 6e50 726f 6300 0700 494e  !.....nProc...IN
-00002ac0: 545f 3455 002b 004e 756d 6265 7220 6f66  T_4U.+.Number of
-00002ad0: 2075 6e69 7175 6520 4672 5072 6f63 4461   unique FrProcDa
-00002ae0: 7461 206e 616d 6573 2069 6e20 6669 6c65  ta names in file
-00002af0: 2e00 feef 7499 4900 0000 0000 0000 0102  ....t.I.........
-00002b00: 2200 0000 0900 6e61 6d65 5072 6f63 000e  ".....nameProc..
-00002b10: 0053 5452 494e 475b 6e50 726f 635d 001a  .STRING[nProc]..
-00002b20: 0041 7272 6179 206f 6620 4672 5072 6f63  .Array of FrProc
-00002b30: 4461 7461 206e 616d 6573 0092 f0ec 64a2  Data names....d.
-00002b40: 0000 0000 0000 0001 0223 0000 000d 0070  .........#.....p
-00002b50: 6f73 6974 696f 6e50 726f 6300 1600 494e  ositionProc...IN
-00002b60: 545f 3855 5b6e 5072 6f63 5d5b 6e46 7261  T_8U[nProc][nFra
-00002b70: 6d65 5d00 6700 4172 7261 7920 6f66 206c  me].g.Array of l
-00002b80: 6973 7473 206f 6620 4672 5072 6f63 4461  ists of FrProcDa
-00002b90: 7461 206f 6666 7365 7420 706f 7369 7469  ta offset positi
-00002ba0: 6f6e 732c 2069 6e20 6279 7465 732c 2066  ons, in bytes, f
-00002bb0: 726f 6d20 6265 6769 6e6e 696e 6720 6f66  rom beginning of
-00002bc0: 2066 696c 6520 2873 697a 6520 6f66 206e   file (size of n
-00002bd0: 4672 616d 652a 6e50 726f 6329 00f2 b9e4  Frame*nProc)....
-00002be0: a64e 0000 0000 0000 0001 0224 0000 0005  .N.........$....
-00002bf0: 006e 5369 6d00 0700 494e 545f 3455 002a  .nSim...INT_4U.*
-00002c00: 004e 756d 6265 7220 6f66 2075 6e69 7175  .Number of uniqu
-00002c10: 6520 4672 5369 6d44 6174 6120 6e61 6d65  e FrSimData name
-00002c20: 7320 696e 2066 696c 652e 0008 01bc 3746  s in file.....7F
-00002c30: 0000 0000 0000 0001 0225 0000 0008 006e  .........%.....n
-00002c40: 616d 6553 696d 000d 0053 5452 494e 475b  ameSim...STRING[
-00002c50: 6e53 696d 5d00 1900 4172 7261 7920 6f66  nSim]...Array of
-00002c60: 2046 7253 696d 4461 7461 206e 616d 6573   FrSimData names
-00002c70: 00c4 a72b f69e 0000 0000 0000 0001 0226  ...+...........&
-00002c80: 0000 000c 0070 6f73 6974 696f 6e53 696d  .....positionSim
-00002c90: 0015 0049 4e54 5f38 555b 6e53 696d 5d5b  ...INT_8U[nSim][
-00002ca0: 6e46 7261 6d65 5d00 6500 4172 7261 7920  nFrame].e.Array 
-00002cb0: 6f66 206c 6973 7473 206f 6620 4672 5369  of lists of FrSi
-00002cc0: 6d44 6174 6120 6f66 6673 6574 2070 6f73  mData offset pos
-00002cd0: 6974 696f 6e73 2c20 696e 2062 7974 6573  itions, in bytes
-00002ce0: 2c20 6672 6f6d 2062 6567 696e 6e69 6e67  , from beginning
-00002cf0: 206f 6620 6669 6c65 2028 7369 7a65 206f   of file (size o
-00002d00: 6620 6e46 7261 6d65 2a6e 5369 6d29 00d3  f nFrame*nSim)..
-00002d10: 40ba c14e 0000 0000 0000 0001 0227 0000  @..N.........'..
-00002d20: 0005 006e 5365 7200 0700 494e 545f 3455  ...nSer...INT_4U
-00002d30: 002a 004e 756d 6265 7220 6f66 2075 6e69  .*.Number of uni
-00002d40: 7175 6520 4672 5365 7244 6174 6120 6e61  que FrSerData na
-00002d50: 6d65 7320 696e 2066 696c 652e 000f 814d  mes in file....M
-00002d60: 9046 0000 0000 0000 0001 0228 0000 0008  .F.........(....
-00002d70: 006e 616d 6553 6572 000d 0053 5452 494e  .nameSer...STRIN
-00002d80: 475b 6e53 6572 5d00 1900 4172 7261 7920  G[nSer]...Array 
-00002d90: 6f66 2046 7253 6572 4461 7461 206e 616d  of FrSerData nam
-00002da0: 6573 00bd 2d79 109e 0000 0000 0000 0001  es..-y..........
-00002db0: 0229 0000 000c 0070 6f73 6974 696f 6e53  .).....positionS
-00002dc0: 6572 0015 0049 4e54 5f38 555b 6e53 6572  er...INT_8U[nSer
-00002dd0: 5d5b 6e46 7261 6d65 5d00 6500 4172 7261  ][nFrame].e.Arra
-00002de0: 7920 6f66 206c 6973 7473 206f 6620 4672  y of lists of Fr
-00002df0: 5365 7244 6174 6120 6f66 6673 6574 2070  SerData offset p
-00002e00: 6f73 6974 696f 6e73 2c20 696e 2062 7974  ositions, in byt
-00002e10: 6573 2c20 6672 6f6d 2062 6567 696e 6e69  es, from beginni
-00002e20: 6e67 206f 6620 6669 6c65 2028 7369 7a65  ng of file (size
-00002e30: 206f 6620 6e46 7261 6d65 2a6e 5365 7229   of nFrame*nSer)
-00002e40: 001c 5003 fb52 0000 0000 0000 0001 022a  ..P..R.........*
-00002e50: 0000 0009 006e 5375 6d6d 6172 7900 0700  .....nSummary...
-00002e60: 494e 545f 3455 002a 004e 756d 6265 7220  INT_4U.*.Number 
-00002e70: 6f66 2075 6e69 7175 6520 4672 5375 6d6d  of unique FrSumm
-00002e80: 6172 7920 6e61 6d65 7320 696e 2066 696c  ary names in fil
-00002e90: 652e 0034 77a5 e94b 0000 0000 0000 0001  e..4w..K........
-00002ea0: 022b 0000 0009 006e 616d 6553 5375 6d00  .+.....nameSSum.
-00002eb0: 1100 5354 5249 4e47 5b6e 5375 6d6d 6172  ..STRING[nSummar
-00002ec0: 795d 0019 0041 7272 6179 206f 6620 4672  y]...Array of Fr
-00002ed0: 5375 6d6d 6172 7920 6e61 6d65 7300 0684  Summary names...
-00002ee0: 574e a200 0000 0000 0000 0102 2c00 0000  WN..........,...
-00002ef0: 0c00 706f 7369 7469 6f6e 5365 7200 1900  ..positionSer...
-00002f00: 494e 545f 3855 5b6e 5375 6d6d 6172 795d  INT_8U[nSummary]
-00002f10: 5b6e 4672 616d 655d 0065 0041 7272 6179  [nFrame].e.Array
-00002f20: 206f 6620 6c69 7374 7320 6f66 2046 7253   of lists of FrS
-00002f30: 756d 6d61 7279 206f 6666 7365 7420 706f  ummary offset po
-00002f40: 7369 7469 6f6e 732c 2069 6e20 6279 7465  sitions, in byte
-00002f50: 732c 2066 726f 6d20 6265 6769 6e6e 696e  s, from beginnin
-00002f60: 6720 6f66 2066 696c 6520 2873 697a 6520  g of file (size 
-00002f70: 6f66 206e 4672 616d 652a 6e53 6572 2900  of nFrame*nSer).
-00002f80: c376 da95 4800 0000 0000 0000 0102 2d00  .v..H.........-.
-00002f90: 0000 0b00 6e45 7665 6e74 5479 7065 0007  ....nEventType..
-00002fa0: 0049 4e54 5f34 5500 1e00 4e75 6d62 6572  .INT_4U...Number
-00002fb0: 206f 6620 4672 4576 656e 7420 696e 2074   of FrEvent in t
-00002fc0: 6865 2066 696c 6500 cb0b 34f7 4c00 0000  he file...4.L...
-00002fd0: 0000 0000 0102 2e00 0000 0a00 6e61 6d65  ............name
-00002fe0: 4576 656e 7400 1300 5354 5249 4e47 5b6e  Event...STRING[n
-00002ff0: 4576 656e 7454 7970 655d 0017 0041 7272  EventType]...Arr
-00003000: 6179 206f 6620 4672 4576 656e 7420 6e61  ay of FrEvent na
-00003010: 6d65 7300 8aec 7442 7200 0000 0000 0000  mes...tBr.......
-00003020: 0102 2f00 0000 0700 6e45 7665 6e74 0013  ../.....nEvent..
-00003030: 0049 4e54 5f34 555b 6e45 7665 6e74 5479  .INT_4U[nEventTy
-00003040: 7065 5d00 4000 4e75 6d62 6572 206f 6620  pe].@.Number of 
-00003050: 4672 4576 656e 7420 666f 7220 6561 6368  FrEvent for each
-00003060: 2074 7970 6520 6f66 2046 7245 7665 6e74   type of FrEvent
-00003070: 2028 7369 7a65 206f 6620 6e45 7665 6e74   (size of nEvent
-00003080: 5479 7065 2900 aebb 6fd3 4300 0000 0000  Type)...o.C.....
-00003090: 0000 0102 3000 0000 0c00 6e54 6f74 616c  ....0.....nTotal
-000030a0: 4576 656e 7400 0700 494e 545f 3455 0018  Event...INT_4U..
-000030b0: 0054 6f74 616c 206e 756d 6265 7220 6f66  .Total number of
-000030c0: 2046 7245 7665 6e74 0074 8af4 4a54 0000   FrEvent.t..JT..
-000030d0: 0000 0000 0001 0231 0000 000c 0047 5469  .......1.....GTi
-000030e0: 6d65 5345 7665 6e74 0014 0049 4e54 5f34  meSEvent...INT_4
-000030f0: 555b 6e54 6f74 616c 4576 656e 745d 001c  U[nTotalEvent]..
-00003100: 0047 5053 2074 696d 6520 696e 2069 6e74  .GPS time in int
-00003110: 6567 6572 2073 6563 6f6e 6473 0015 3513  eger seconds..5.
-00003120: 2961 0000 0000 0000 0001 0232 0000 000c  )a.........2....
-00003130: 0047 5469 6d65 4e45 7665 6e74 0014 0049  .GTimeNEvent...I
-00003140: 4e54 5f34 555b 6e54 6f74 616c 4576 656e  NT_4U[nTotalEven
-00003150: 745d 0029 0052 6573 6964 7561 6c20 4750  t].).Residual GP
-00003160: 5320 7469 6d65 2069 6e20 696e 7465 6765  S time in intege
-00003170: 7220 6e61 6e6f 7365 636f 6e64 7300 157d  r nanoseconds..}
-00003180: 335d 4b00 0000 0000 0000 0102 3300 0000  3]K.........3...
-00003190: 0f00 616d 706c 6974 7564 6545 7665 6e74  ..amplitudeEvent
-000031a0: 0014 0052 4541 4c5f 345b 6e54 6f74 616c  ...REAL_4[nTotal
-000031b0: 4576 656e 745d 0010 0045 7665 6e74 2061  Event]...Event a
-000031c0: 6d70 6c69 7475 6465 00c2 ba16 4177 0000  mplitude....Aw..
-000031d0: 0000 0000 0001 0234 0000 000e 0070 6f73  .......4.....pos
-000031e0: 6974 696f 6e45 7665 6e74 0014 0049 4e54  itionEvent...INT
-000031f0: 5f38 555b 6e54 6f74 616c 4576 656e 745d  _8U[nTotalEvent]
-00003200: 003d 0041 7272 6179 206f 6620 4672 4576  .=.Array of FrEv
-00003210: 656e 7420 706f 7369 7469 6f6e 732c 2069  ent positions, i
-00003220: 6e20 6279 7465 732c 2066 726f 6d20 6265  n bytes, from be
-00003230: 6769 6e6e 696e 6720 6f66 2066 696c 6500  ginning of file.
-00003240: 46be 4b47 4e00 0000 0000 0000 0102 3500  F.KGN.........5.
-00003250: 0000 0e00 6e53 696d 4576 656e 7454 7970  ....nSimEventTyp
-00003260: 6500 0700 494e 545f 3455 0021 004e 756d  e...INT_4U.!.Num
-00003270: 6265 7220 6f66 2046 7253 696d 4576 656e  ber of FrSimEven
-00003280: 7420 696e 2074 6865 2066 696c 6500 d601  t in the file...
-00003290: de2b 5500 0000 0000 0000 0102 3600 0000  .+U.........6...
-000032a0: 0d00 6e61 6d65 5369 6d45 7665 6e74 0016  ..nameSimEvent..
-000032b0: 0053 5452 494e 475b 6e53 696d 4576 656e  .STRING[nSimEven
-000032c0: 7454 7970 655d 001a 0041 7272 6179 206f  tType]...Array o
-000032d0: 6620 4672 5369 6d45 7665 6e74 206e 616d  f FrSimEvent nam
-000032e0: 6573 00c3 e4da a081 0000 0000 0000 0001  es..............
-000032f0: 0237 0000 000a 006e 5369 6d45 7665 6e74  .7.....nSimEvent
-00003300: 0016 0049 4e54 5f34 555b 6e53 696d 4576  ...INT_4U[nSimEv
-00003310: 656e 7454 7970 655d 0049 004e 756d 6265  entType].I.Numbe
-00003320: 7220 6f66 2046 7253 696d 4576 656e 7420  r of FrSimEvent 
-00003330: 666f 7220 6561 6368 2074 7970 6520 6f66  for each type of
-00003340: 2046 7253 696d 4576 656e 7420 2873 697a   FrSimEvent (siz
-00003350: 6520 6f66 206e 5369 6d45 7665 6e74 5479  e of nSimEventTy
-00003360: 7065 2900 4e11 c946 4700 0000 0000 0000  pe).N..FG.......
-00003370: 0102 3800 0000 0d00 6e54 6f74 616c 5345  ..8.....nTotalSE
-00003380: 7665 6e74 0007 0049 4e54 5f34 5500 1b00  vent...INT_4U...
-00003390: 546f 7461 6c20 6e75 6d62 6572 206f 6620  Total number of 
-000033a0: 4672 5369 6d45 7665 6e74 00de 86a5 7e53  FrSimEvent....~S
-000033b0: 0000 0000 0000 0001 0239 0000 000a 0047  .........9.....G
-000033c0: 5469 6d65 5353 696d 0015 0049 4e54 5f34  TimeSSim...INT_4
-000033d0: 555b 6e54 6f74 616c 5345 7665 6e74 5d00  U[nTotalSEvent].
-000033e0: 1c00 4750 5320 7469 6d65 2069 6e20 696e  ..GPS time in in
-000033f0: 7465 6765 7220 7365 636f 6e64 7300 8b64  teger seconds..d
-00003400: 9181 6000 0000 0000 0000 0102 3a00 0000  ..`.........:...
-00003410: 0a00 4754 696d 654e 5369 6d00 1500 494e  ..GTimeNSim...IN
-00003420: 545f 3455 5b6e 546f 7461 6c53 4576 656e  T_4U[nTotalSEven
-00003430: 745d 0029 0052 6573 6964 7561 6c20 4750  t].).Residual GP
-00003440: 5320 7469 6d65 2069 6e20 696e 7465 6765  S time in intege
-00003450: 7220 6e61 6e6f 7365 636f 6e64 7300 6127  r nanoseconds.a'
-00003460: db26 5200 0000 0000 0000 0102 3b00 0000  .&R.........;...
-00003470: 1200 616d 706c 6974 7564 6553 696d 4576  ..amplitudeSimEv
-00003480: 656e 7400 1500 5245 414c 5f34 5b6e 546f  ent...REAL_4[nTo
-00003490: 7461 6c53 4576 656e 745d 0013 0053 696d  talSEvent]...Sim
-000034a0: 4576 656e 7420 616d 706c 6974 7564 6500  Event amplitude.
-000034b0: 2410 90c2 7e00 0000 0000 0000 0102 3c00  $...~.........<.
-000034c0: 0000 1100 706f 7369 7469 6f6e 5369 6d45  ....positionSimE
-000034d0: 7665 6e74 0015 0049 4e54 5f38 555b 6e54  vent...INT_8U[nT
-000034e0: 6f74 616c 5345 7665 6e74 5d00 4000 4172  otalSEvent].@.Ar
-000034f0: 7261 7920 6f66 2046 7253 696d 4576 656e  ray of FrSimEven
-00003500: 7420 706f 7369 7469 6f6e 732c 2069 6e20  t positions, in 
-00003510: 6279 7465 732c 2066 726f 6d20 6265 6769  bytes, from begi
-00003520: 6e6e 696e 6720 6f66 2066 696c 6500 9f96  nning of file...
-00003530: 37f5 3600 0000 0000 0000 0102 3d00 0000  7.6.........=...
-00003540: 0700 6368 6b53 756d 0007 0049 4e54 5f34  ..chkSum...INT_4
-00003550: 5500 1000 5374 7275 6374 2063 6865 636b  U...Struct check
-00003560: 7375 6d00 8e79 d77a 5001 0000 0000 0000  sum..y.zP.......
-00003570: 0113 0000 0000 2500 0100 0000 708d 7430  ......%.....p.t0
-00003580: b881 8348 0000 0000 0000 0000 0000 1040  ...H...........@
-00003590: 0000 0000 827f 0000 6e09 0000 0000 0000  ........n.......
+00001af0: 1f00 0000 0000 0000 789c edc1 010d 0000  ........x.......
+00001b00: 00c2 a0f7 4f6d 0e37 a000 0000 0000 0000  ....Om.7........
+00001b10: 8077 0320 0000 0101 0000 0000 0400 0000  .w. ............
+00001b20: 0000 0000 0000 0000 0070 3f00 0000 0000  .........p?.....
+00001b30: 0000 0002 0073 0001 0000 0000 0000 0000  .....s..........
+00001b40: 913f 116f 4100 0000 0000 0000 0101 0400  .?.oA...........
+00001b50: 0000 0d00 4672 456e 644f 6646 7261 6d65  ....FrEndOfFrame
+00001b60: 0007 001c 0045 6e64 206f 6620 4672 616d  .....End of Fram
+00001b70: 6520 4461 7461 2053 7472 7563 7475 7265  e Data Structure
+00001b80: 009c ab33 e258 0000 0000 0000 0001 0247  ...3.X.........G
+00001b90: 0000 0004 0072 756e 0007 0049 4e54 5f34  .....run...INT_4
+00001ba0: 5300 3500 5275 6e20 6e75 6d62 6572 3b20  S.5.Run number; 
+00001bb0: 7361 6d65 2061 7320 696e 2046 7261 6d65  same as in Frame
+00001bc0: 4865 6164 6572 2072 756e 206e 756d 6265  Header run numbe
+00001bd0: 7220 6461 7475 6d2e 000b 9641 5b87 0000  r datum....A[...
+00001be0: 0000 0000 0001 0248 0000 0006 0066 7261  .......H.....fra
+00001bf0: 6d65 0007 0049 4e54 5f34 5500 6200 4672  me...INT_4U.b.Fr
+00001c00: 616d 6520 6e75 6d62 6572 2c20 6d6f 6e6f  ame number, mono
+00001c10: 746f 6e69 6361 6c6c 7920 696e 6372 6561  tonically increa
+00001c20: 7369 6e67 2075 6e74 696c 2065 6e64 206f  sing until end o
+00001c30: 6620 7275 6e3b 2073 616d 6520 6173 2069  f run; same as i
+00001c40: 6e20 4672 616d 6520 4865 6164 6572 2072  n Frame Header r
+00001c50: 756e 206e 756d 6265 7220 6461 7475 6d00  un number datum.
+00001c60: ba5a b3d1 4700 0000 0000 0000 0102 4900  .Z..G.........I.
+00001c70: 0000 0700 4754 696d 6553 0007 0049 4e54  ....GTimeS...INT
+00001c80: 5f34 5500 2100 4672 616d 6520 7374 6172  _4U.!.Frame star
+00001c90: 7420 7469 6d65 2069 6e20 4750 5320 5365  t time in GPS Se
+00001ca0: 636f 6e64 732e 0018 add0 ff56 0000 0000  conds......V....
+00001cb0: 0000 0001 024a 0000 0007 0047 5469 6d65  .....J.....GTime
+00001cc0: 4e00 0700 494e 545f 3455 0030 0046 7261  N...INT_4U.0.Fra
+00001cd0: 6d65 2073 7461 7274 2074 696d 6520 7265  me start time re
+00001ce0: 7369 6475 616c 2c20 696e 7465 6765 7220  sidual, integer 
+00001cf0: 6e61 6e6f 7365 636f 6e64 732e 0064 338f  nanoseconds..d3.
+00001d00: ba36 0000 0000 0000 0001 024b 0000 0007  .6.........K....
+00001d10: 0063 686b 5375 6d00 0700 494e 545f 3455  .chkSum...INT_4U
+00001d20: 0010 0053 7472 7563 7420 6368 6563 6b73  ...Struct checks
+00001d30: 756d 0022 ca11 6222 0000 0000 0000 0001  um."..b"........
+00001d40: 0700 0000 0000 0000 0000 0000 0000 0000  ................
+00001d50: 0000 0000 00c9 70fa 3b37 0000 0000 0000  ......p.;7......
+00001d60: 0001 0100 0000 0006 0046 7254 4f43 0013  .........FrTOC..
+00001d70: 0019 0053 696d 756c 6174 6564 2044 6174  ...Simulated Dat
+00001d80: 6120 5374 7275 6374 7572 6500 7c69 656b  a Structure.|iek
+00001d90: 4800 0000 0000 0000 0102 0000 0000 0700  H...............
+00001da0: 554c 6561 7053 0007 0049 4e54 5f32 5300  ULeapS...INT_2S.
+00001db0: 2200 4672 6f6d 2074 6865 2066 6972 7374  ".From the first
+00001dc0: 2046 7261 6d65 4820 696e 2074 6865 2066   FrameH in the f
+00001dd0: 696c 6500 0087 5256 4300 0000 0000 0000  ile...RVC.......
+00001de0: 0102 0100 0000 0700 6e46 7261 6d65 0007  ........nFrame..
+00001df0: 0049 4e54 5f34 5500 1d00 4e75 6d62 6572  .INT_4U...Number
+00001e00: 206f 6620 6672 616d 6573 2069 6e20 7468   of frames in th
+00001e10: 6520 6669 6c65 00cc 3d5f 7370 0000 0000  e file..=_sp....
+00001e20: 0000 0001 0202 0000 000c 0064 6174 6151  ...........dataQ
+00001e30: 7561 6c69 7479 000f 0049 4e54 5f34 555b  uality...INT_4U[
+00001e40: 6e46 7261 6d65 5d00 3d00 4172 7261 7920  nFrame].=.Array 
+00001e50: 6f66 2069 6e74 6567 6572 2051 4120 776f  of integer QA wo
+00001e60: 7264 7320 6672 6f6d 2065 6163 6820 4672  rds from each Fr
+00001e70: 616d 6548 2028 7369 7a65 206f 6620 6e46  ameH (size of nF
+00001e80: 7261 6d65 7329 0088 6738 c05f 0000 0000  rames)..g8._....
+00001e90: 0000 0001 0203 0000 0007 0047 5469 6d65  ...........GTime
+00001ea0: 5300 0f00 494e 545f 3455 5b6e 4672 616d  S...INT_4U[nFram
+00001eb0: 655d 0031 0041 7272 6179 206f 6620 696e  e].1.Array of in
+00001ec0: 7465 6765 7220 4750 5320 6672 6165 2074  teger GPS frae t
+00001ed0: 696d 6573 2028 7369 7a65 206f 6620 6e46  imes (size of nF
+00001ee0: 7261 6d65 7300 d5b2 6755 7600 0000 0000  rames...gUv.....
+00001ef0: 0000 0102 0400 0000 0700 4754 696d 654e  ..........GTimeN
+00001f00: 000f 0049 4e54 5f34 555b 6e46 7261 6d65  ...INT_4U[nFrame
+00001f10: 5d00 4800 4172 7261 7920 6f66 2069 6e74  ].H.Array of int
+00001f20: 6567 6572 2047 5053 2072 6573 6964 7561  eger GPS residua
+00001f30: 6c20 6e61 6e6f 7365 636f 6e64 7320 666f  l nanoseconds fo
+00001f40: 7220 7468 6520 6672 616d 6520 2873 697a  r the frame (siz
+00001f50: 6520 6f66 206e 4672 616d 6500 154d fabb  e of nFrame..M..
+00001f60: 6000 0000 0000 0000 0102 0500 0000 0300  `...............
+00001f70: 6474 000f 0052 4541 4c5f 385b 6e46 7261  dt...REAL_8[nFra
+00001f80: 6d65 5d00 3600 4172 7261 7920 6f66 2066  me].6.Array of f
+00001f90: 7261 6d65 2064 7572 6174 696f 6e73 2069  rame durations i
+00001fa0: 6e20 7365 636f 6e64 7328 2073 697a 6520  n seconds( size 
+00001fb0: 6f66 206e 4672 616d 6573 2900 0d06 b877  of nFrames)....w
+00001fc0: 5200 0000 0000 0000 0102 0600 0000 0500  R...............
+00001fd0: 7275 6e73 000f 0049 4e54 5f34 535b 6e46  runs...INT_4S[nF
+00001fe0: 7261 6d65 5d00 2600 4172 7261 7920 6f66  rame].&.Array of
+00001ff0: 2072 756e 206e 756d 6265 7273 2028 7369   run numbers (si
+00002000: 7a65 206f 6620 6e46 7261 6d65 2900 ca0b  ze of nFrame)...
+00002010: 9f5c 5500 0000 0000 0000 0102 0700 0000  .\U.............
+00002020: 0600 6672 616d 6500 0f00 494e 545f 3455  ..frame...INT_4U
+00002030: 5b6e 4672 616d 655d 0028 0041 7272 6179  [nFrame].(.Array
+00002040: 206f 6620 6672 616d 6520 6e75 6d62 6572   of frame number
+00002050: 7320 2873 697a 6520 6f66 206e 4672 616d  s (size of nFram
+00002060: 6529 0031 285d 2581 0000 0000 0000 0001  e).1(]%.........
+00002070: 0208 0000 000a 0070 6f73 6974 696f 6e48  .......positionH
+00002080: 000f 0049 4e54 5f38 555b 6e46 7261 6d65  ...INT_8U[nFrame
+00002090: 5d00 5000 4172 7261 7920 6f66 2046 7261  ].P.Array of Fra
+000020a0: 6d65 4820 706f 7369 7469 6f6e 732c 2069  meH positions, i
+000020b0: 6e20 6279 7465 732c 2066 726f 6d20 7468  n bytes, from th
+000020c0: 6520 6267 696e 6e69 6e67 206f 6620 6669  e bginning of fi
+000020d0: 6c65 2028 7369 7a65 206f 6620 6e46 7261  le (size of nFra
+000020e0: 6d65 2900 db18 22e8 8700 0000 0000 0000  me)...".........
+000020f0: 0102 0900 0000 0a00 6e46 6972 7374 4144  ........nFirstAD
+00002100: 4300 0f00 494e 545f 3855 5b6e 4672 616d  C...INT_8U[nFram
+00002110: 655d 0056 0041 7272 6179 206f 6620 6669  e].V.Array of fi
+00002120: 7273 7420 4672 4144 4344 6174 6120 706f  rst FrADCData po
+00002130: 7369 7469 6f6e 732c 2069 6e20 6279 7465  sitions, in byte
+00002140: 732c 2066 726f 6d20 6265 6769 6e6e 696e  s, from beginnin
+00002150: 6720 6f66 2066 696c 6520 2873 697a 6520  g of file (size 
+00002160: 6f66 206e 4672 616d 6529 00b7 d5cd 8b86  of nFrame)......
+00002170: 0000 0000 0000 0001 020a 0000 000a 006e  ...............n
+00002180: 4669 7273 7453 6572 000f 0049 4e54 5f38  FirstSer...INT_8
+00002190: 555b 6e46 7261 6d65 5d00 5500 4172 7261  U[nFrame].U.Arra
+000021a0: 7920 6f66 2066 6972 7374 2046 7253 6572  y of first FrSer
+000021b0: 4461 7461 2070 6f73 6974 696f 6e73 2069  Data positions i
+000021c0: 6e20 6279 7465 732c 2066 726f 6d20 6265  n bytes, from be
+000021d0: 6769 6e6e 696e 6720 6f66 2066 696c 6520  ginning of file 
+000021e0: 2873 697a 6520 6f66 206e 4672 616d 6529  (size of nFrame)
+000021f0: 00fa c761 6b87 0000 0000 0000 0001 020b  ...ak...........
+00002200: 0000 000c 006e 4669 7273 7454 6162 6c65  .....nFirstTable
+00002210: 000f 0049 4e54 5f38 555b 6e46 7261 6d65  ...INT_8U[nFrame
+00002220: 5d00 5400 4172 7261 7920 6f66 2066 6972  ].T.Array of fir
+00002230: 7374 2046 7254 6162 6c65 2070 6f73 6974  st FrTable posit
+00002240: 696f 6e73 2c20 696e 2062 7974 6573 2c20  ions, in bytes, 
+00002250: 6672 6f6d 2062 6567 696e 6e69 6e67 206f  from beginning o
+00002260: 6620 6669 6c65 2028 7369 7a65 206f 6620  f file (size of 
+00002270: 6e46 7261 6d65 2900 1016 52a6 8300 0000  nFrame)...R.....
+00002280: 0000 0000 0102 0c00 0000 0a00 6e46 6972  ............nFir
+00002290: 7374 4d73 6700 0f00 494e 545f 3855 5b6e  stMsg...INT_8U[n
+000022a0: 4672 616d 655d 0052 0041 7272 6179 206f  Frame].R.Array o
+000022b0: 6620 6669 7273 7420 4672 4d73 6720 706f  f first FrMsg po
+000022c0: 7369 7469 6f6e 732c 2069 6e20 6279 7465  sitions, in byte
+000022d0: 732c 2066 726f 6d20 6265 6769 6e6e 696e  s, from beginnin
+000022e0: 6720 6f66 2066 696c 6520 2873 697a 6520  g of file (size 
+000022f0: 6f66 206e 4672 616d 6529 00b9 e1c6 f949  of nFrame).....I
+00002300: 0000 0000 0000 0001 020d 0000 0004 006e  ...............n
+00002310: 5348 0007 0049 4e54 5f34 5500 2600 4e75  SH...INT_4U.&.Nu
+00002320: 6d62 6572 206f 6620 4672 5348 2073 7472  mber of FrSH str
+00002330: 7563 7475 7265 7320 696e 2074 6865 2066  uctures in the f
+00002340: 696c 6500 f46c 0bb0 4900 0000 0000 0000  ile..l..I.......
+00002350: 0102 0e00 0000 0500 5348 6964 000c 0049  ........SHid...I
+00002360: 4e54 5f32 555b 6e53 485d 0020 0041 7272  NT_2U[nSH]. .Arr
+00002370: 6179 206f 6620 4672 5348 2049 4473 2028  ay of FrSH IDs (
+00002380: 7369 7a65 206f 6620 6e53 4829 0010 5b23  size of nSH)..[#
+00002390: 074d 0000 0000 0000 0001 020f 0000 0007  .M..............
+000023a0: 0053 486e 616d 6500 0c00 5354 5249 4e47  .SHname...STRING
+000023b0: 5b6e 5348 5d00 2200 4172 7261 7920 6f66  [nSH].".Array of
+000023c0: 2046 7253 4820 6e61 6d65 7320 2873 697a   FrSH names (siz
+000023d0: 6520 6f66 206e 5348 2900 a664 b4df 5c00  e of nSH)..d..\.
+000023e0: 0000 0000 0000 0102 1000 0000 0a00 6e44  ..............nD
+000023f0: 6574 6563 746f 7200 0700 494e 545f 3455  etector...INT_4U
+00002400: 0033 004e 756d 6265 7220 6f66 2064 6973  .3.Number of dis
+00002410: 7469 6e63 7420 7479 7065 7320 6f66 2046  tinct types of F
+00002420: 7244 6574 6563 746f 7220 696e 2074 6865  rDetector in the
+00002430: 2066 696c 6500 fa46 0067 8100 0000 0000   file..F.g......
+00002440: 0000 0102 1100 0000 0d00 6e61 6d65 4465  ..........nameDe
+00002450: 7465 6374 6f72 0012 0053 5452 494e 475b  tector...STRING[
+00002460: 6e44 6574 6563 746f 725d 004a 0041 7272  nDetector].J.Arr
+00002470: 6179 206f 6620 4672 4465 7465 6374 6f72  ay of FrDetector
+00002480: 206e 616d 6573 2028 7369 7a65 206f 6620   names (size of 
+00002490: 6e44 6574 6563 746f 7229 2e20 5468 6579  nDetector). They
+000024a0: 2061 7070 6561 7220 616c 7068 6162 6574   appear alphabet
+000024b0: 6963 616c 6c79 0011 11d2 a589 0000 0000  ically..........
+000024c0: 0000 0001 0212 0000 0011 0070 6f73 6974  ...........posit
+000024d0: 696f 6e44 6574 6563 746f 7200 1200 494e  ionDetector...IN
+000024e0: 545f 3855 5b6e 4465 7465 6374 6f72 5d00  T_8U[nDetector].
+000024f0: 4e00 4172 7261 7920 6f66 2046 7244 6574  N.Array of FrDet
+00002500: 6563 746f 7220 706f 7369 7469 6f6e 7320  ector positions 
+00002510: 6672 6f6d 2074 6865 2062 6567 696e 6e69  from the beginni
+00002520: 6e67 206f 6620 6669 6c65 2028 7369 7a65  ng of file (size
+00002530: 206f 6620 6e44 6574 6563 746f 7229 2e00   of nDetector)..
+00002540: 8345 9ff0 5800 0000 0000 0000 0102 1300  .E..X...........
+00002550: 0000 0a00 6e53 7461 7454 7970 6500 0700  ....nStatType...
+00002560: 494e 545f 3455 002f 004e 756d 6265 7220  INT_4U./.Number 
+00002570: 6f66 2073 7461 7469 6320 6461 7461 2062  of static data b
+00002580: 6c6f 636b 2074 7970 6573 2069 6e20 7468  lock types in th
+00002590: 6520 6669 6c65 2e00 0f05 6246 6000 0000  e file....bF`...
+000025a0: 0000 0000 0102 1400 0000 0900 6e61 6d65  ............name
+000025b0: 5374 6174 0012 0053 5452 494e 475b 6e53  Stat...STRING[nS
+000025c0: 7461 7454 7970 655d 002d 0041 7272 6179  tatType].-.Array
+000025d0: 206f 6620 4672 5374 6174 4461 7461 206e   of FrStatData n
+000025e0: 616d 6520 2873 697a 6520 6f66 206e 5374  ame (size of nSt
+000025f0: 6174 5479 7065 2900 a3bf 4547 5d00 0000  atType)...EG]...
+00002600: 0000 0000 0102 1500 0000 0900 6465 7465  ............dete
+00002610: 6374 6f72 0012 0053 5452 494e 475b 6e53  ctor...STRING[nS
+00002620: 7461 7454 7970 655d 002a 0041 7272 6179  tatType].*.Array
+00002630: 206f 6620 4465 7465 6374 6f72 206e 616d   of Detector nam
+00002640: 6528 7369 7a65 206f 6620 6e53 7461 7454  e(size of nStatT
+00002650: 7970 6529 0041 b642 9d7b 0000 0000 0000  ype).A.B.{......
+00002660: 0001 0216 0000 000e 006e 5374 6174 496e  .........nStatIn
+00002670: 7374 616e 6365 0012 0049 4e54 5f34 555b  stance...INT_4U[
+00002680: 6e53 7461 7454 7970 655d 0043 0041 7272  nStatType].C.Arr
+00002690: 6179 206f 6620 6e75 6d62 6572 206f 6620  ay of number of 
+000026a0: 696e 7374 616e 6365 2066 6f72 2065 6163  instance for eac
+000026b0: 6820 4672 5374 6174 4461 7461 2873 697a  h FrStatData(siz
+000026c0: 6520 6f66 206e 5374 6174 5479 7065 2900  e of nStatType).
+000026d0: 66b8 774f 4b00 0000 0000 0000 0102 1700  f.wOK...........
+000026e0: 0000 0b00 6e54 6f74 616c 5374 6174 0007  ....nTotalStat..
+000026f0: 0049 4e54 5f34 5500 2100 5375 6d6d 6174  .INT_4U.!.Summat
+00002700: 696f 6e20 6f66 206e 5374 6174 496e 7374  ion of nStatInst
+00002710: 616e 6365 2061 7272 6179 0089 b4e7 f874  ance array.....t
+00002720: 0000 0000 0000 0001 0218 0000 0007 0074  ...............t
+00002730: 5374 6172 7400 1300 494e 545f 3455 5b6e  Start...INT_4U[n
+00002740: 546f 7461 6c53 7461 745d 0042 0041 7272  TotalStat].B.Arr
+00002750: 6179 206f 6620 4750 5320 696e 7465 6765  ay of GPS intege
+00002760: 7220 7374 6172 7420 7469 6d65 732c 2069  r start times, i
+00002770: 6e20 7365 636f 6e64 7320 2873 697a 6520  n seconds (size 
+00002780: 6f66 206e 546f 7461 6c53 7461 7429 001a  of nTotalStat)..
+00002790: 531d 0970 0000 0000 0000 0001 0219 0000  S..p............
+000027a0: 0005 0074 456e 6400 1300 494e 545f 3455  ...tEnd...INT_4U
+000027b0: 5b6e 546f 7461 6c53 7461 745d 0040 0041  [nTotalStat].@.A
+000027c0: 7272 6179 206f 6620 4750 5320 696e 7465  rray of GPS inte
+000027d0: 6765 7220 656e 6420 7469 6d65 732c 2069  ger end times, i
+000027e0: 6e20 7365 636f 6e64 7320 2873 697a 6520  n seconds (size 
+000027f0: 6f66 206e 546f 7461 6c53 7461 7429 0045  of nTotalStat).E
+00002800: 668b 4d5e 0000 0000 0000 0001 021a 0000  f.M^............
+00002810: 0008 0076 6572 7369 6f6e 0013 0049 4e54  ...version...INT
+00002820: 5f34 555b 6e54 6f74 616c 5374 6174 5d00  _4U[nTotalStat].
+00002830: 2b00 4172 7261 7920 6f66 2076 6572 7369  +.Array of versi
+00002840: 6f6e 2074 696d 6520 2873 697a 6520 6f66  on time (size of
+00002850: 206e 546f 7461 6c53 7461 7429 0093 e259   nTotalStat)...Y
+00002860: 1d82 0000 0000 0000 0001 021b 0000 000d  ................
+00002870: 0070 6f73 6974 696f 6e53 7461 7400 1300  .positionStat...
+00002880: 494e 545f 3855 5b6e 546f 7461 6c53 7461  INT_8U[nTotalSta
+00002890: 745d 004a 0041 7272 6179 206f 6620 4672  t].J.Array of Fr
+000028a0: 5374 6174 4461 7461 2070 6f73 6974 696f  StatData positio
+000028b0: 6e73 2066 726f 6d20 6265 6769 6e6e 696e  ns from beginnin
+000028c0: 6720 6f66 2066 696c 6520 2873 697a 6520  g of file (size 
+000028d0: 6f66 206e 546f 7461 6c53 7461 7429 002e  of nTotalStat)..
+000028e0: 51de 564e 0000 0000 0000 0001 021c 0000  Q.VN............
+000028f0: 0005 006e 4144 4300 0700 494e 545f 3455  ...nADC...INT_4U
+00002900: 002a 004e 756d 6265 7220 6f66 2075 6e69  .*.Number of uni
+00002910: 7175 6520 4672 4164 6344 6174 6120 6e61  que FrAdcData na
+00002920: 6d65 7320 696e 2066 696c 652e 0007 54ee  mes in file...T.
+00002930: e143 0000 0000 0000 0001 021d 0000 0005  .C..............
+00002940: 006e 616d 6500 0d00 5354 5249 4e47 5b6e  .name...STRING[n
+00002950: 4144 435d 0019 0041 7272 6179 206f 6620  ADC]...Array of 
+00002960: 4672 4164 6344 6174 6120 6e61 6d65 7300  FrAdcData names.
+00002970: 89b1 c3ad 4800 0000 0000 0000 0102 1e00  ....H...........
+00002980: 0000 0a00 6368 616e 6e65 6c49 4400 0d00  ....channelID...
+00002990: 494e 545f 3455 5b6e 4144 435d 0019 0041  INT_4U[nADC]...A
+000029a0: 7272 6179 206f 6620 4144 4320 6368 616e  rray of ADC chan
+000029b0: 6e65 6c20 4944 7300 251b 8f78 4400 0000  nel IDs.%..xD...
+000029c0: 0000 0000 0102 1f00 0000 0800 6772 6f75  ............grou
+000029d0: 7049 4400 0d00 494e 545f 3455 5b6e 4144  pID...INT_4U[nAD
+000029e0: 435d 0017 0041 7272 6179 206f 6620 4144  C]...Array of AD
+000029f0: 4320 6772 6f75 7020 4944 7300 ec33 7c9e  C group IDs..3|.
+00002a00: 9e00 0000 0000 0000 0102 2000 0000 0c00  .......... .....
+00002a10: 706f 7369 7469 6f6e 4144 4300 1500 494e  positionADC...IN
+00002a20: 545f 3855 5b6e 4144 435d 5b6e 4672 616d  T_8U[nADC][nFram
+00002a30: 655d 0065 0041 7272 6179 206f 6620 6c69  e].e.Array of li
+00002a40: 7374 7320 6f66 2046 7241 6463 4461 7461  sts of FrAdcData
+00002a50: 206f 6666 7365 7420 706f 7369 7469 6f6e   offset position
+00002a60: 732c 2069 6e20 6279 7465 732c 2066 726f  s, in bytes, fro
+00002a70: 6d20 6265 6769 6e6e 696e 6720 6f66 2066  m beginning of f
+00002a80: 696c 6520 2873 697a 6520 6f66 206e 4672  ile (size of nFr
+00002a90: 616d 652a 6e41 4443 2900 6d54 ccf2 5000  ame*nADC).mT..P.
+00002aa0: 0000 0000 0000 0102 2100 0000 0600 6e50  ........!.....nP
+00002ab0: 726f 6300 0700 494e 545f 3455 002b 004e  roc...INT_4U.+.N
+00002ac0: 756d 6265 7220 6f66 2075 6e69 7175 6520  umber of unique 
+00002ad0: 4672 5072 6f63 4461 7461 206e 616d 6573  FrProcData names
+00002ae0: 2069 6e20 6669 6c65 2e00 feef 7499 4900   in file....t.I.
+00002af0: 0000 0000 0000 0102 2200 0000 0900 6e61  ........".....na
+00002b00: 6d65 5072 6f63 000e 0053 5452 494e 475b  meProc...STRING[
+00002b10: 6e50 726f 635d 001a 0041 7272 6179 206f  nProc]...Array o
+00002b20: 6620 4672 5072 6f63 4461 7461 206e 616d  f FrProcData nam
+00002b30: 6573 0092 f0ec 64a2 0000 0000 0000 0001  es....d.........
+00002b40: 0223 0000 000d 0070 6f73 6974 696f 6e50  .#.....positionP
+00002b50: 726f 6300 1600 494e 545f 3855 5b6e 5072  roc...INT_8U[nPr
+00002b60: 6f63 5d5b 6e46 7261 6d65 5d00 6700 4172  oc][nFrame].g.Ar
+00002b70: 7261 7920 6f66 206c 6973 7473 206f 6620  ray of lists of 
+00002b80: 4672 5072 6f63 4461 7461 206f 6666 7365  FrProcData offse
+00002b90: 7420 706f 7369 7469 6f6e 732c 2069 6e20  t positions, in 
+00002ba0: 6279 7465 732c 2066 726f 6d20 6265 6769  bytes, from begi
+00002bb0: 6e6e 696e 6720 6f66 2066 696c 6520 2873  nning of file (s
+00002bc0: 697a 6520 6f66 206e 4672 616d 652a 6e50  ize of nFrame*nP
+00002bd0: 726f 6329 00f2 b9e4 a64e 0000 0000 0000  roc).....N......
+00002be0: 0001 0224 0000 0005 006e 5369 6d00 0700  ...$.....nSim...
+00002bf0: 494e 545f 3455 002a 004e 756d 6265 7220  INT_4U.*.Number 
+00002c00: 6f66 2075 6e69 7175 6520 4672 5369 6d44  of unique FrSimD
+00002c10: 6174 6120 6e61 6d65 7320 696e 2066 696c  ata names in fil
+00002c20: 652e 0008 01bc 3746 0000 0000 0000 0001  e.....7F........
+00002c30: 0225 0000 0008 006e 616d 6553 696d 000d  .%.....nameSim..
+00002c40: 0053 5452 494e 475b 6e53 696d 5d00 1900  .STRING[nSim]...
+00002c50: 4172 7261 7920 6f66 2046 7253 696d 4461  Array of FrSimDa
+00002c60: 7461 206e 616d 6573 00c4 a72b f69e 0000  ta names...+....
+00002c70: 0000 0000 0001 0226 0000 000c 0070 6f73  .......&.....pos
+00002c80: 6974 696f 6e53 696d 0015 0049 4e54 5f38  itionSim...INT_8
+00002c90: 555b 6e53 696d 5d5b 6e46 7261 6d65 5d00  U[nSim][nFrame].
+00002ca0: 6500 4172 7261 7920 6f66 206c 6973 7473  e.Array of lists
+00002cb0: 206f 6620 4672 5369 6d44 6174 6120 6f66   of FrSimData of
+00002cc0: 6673 6574 2070 6f73 6974 696f 6e73 2c20  fset positions, 
+00002cd0: 696e 2062 7974 6573 2c20 6672 6f6d 2062  in bytes, from b
+00002ce0: 6567 696e 6e69 6e67 206f 6620 6669 6c65  eginning of file
+00002cf0: 2028 7369 7a65 206f 6620 6e46 7261 6d65   (size of nFrame
+00002d00: 2a6e 5369 6d29 00d3 40ba c14e 0000 0000  *nSim)..@..N....
+00002d10: 0000 0001 0227 0000 0005 006e 5365 7200  .....'.....nSer.
+00002d20: 0700 494e 545f 3455 002a 004e 756d 6265  ..INT_4U.*.Numbe
+00002d30: 7220 6f66 2075 6e69 7175 6520 4672 5365  r of unique FrSe
+00002d40: 7244 6174 6120 6e61 6d65 7320 696e 2066  rData names in f
+00002d50: 696c 652e 000f 814d 9046 0000 0000 0000  ile....M.F......
+00002d60: 0001 0228 0000 0008 006e 616d 6553 6572  ...(.....nameSer
+00002d70: 000d 0053 5452 494e 475b 6e53 6572 5d00  ...STRING[nSer].
+00002d80: 1900 4172 7261 7920 6f66 2046 7253 6572  ..Array of FrSer
+00002d90: 4461 7461 206e 616d 6573 00bd 2d79 109e  Data names..-y..
+00002da0: 0000 0000 0000 0001 0229 0000 000c 0070  .........).....p
+00002db0: 6f73 6974 696f 6e53 6572 0015 0049 4e54  ositionSer...INT
+00002dc0: 5f38 555b 6e53 6572 5d5b 6e46 7261 6d65  _8U[nSer][nFrame
+00002dd0: 5d00 6500 4172 7261 7920 6f66 206c 6973  ].e.Array of lis
+00002de0: 7473 206f 6620 4672 5365 7244 6174 6120  ts of FrSerData 
+00002df0: 6f66 6673 6574 2070 6f73 6974 696f 6e73  offset positions
+00002e00: 2c20 696e 2062 7974 6573 2c20 6672 6f6d  , in bytes, from
+00002e10: 2062 6567 696e 6e69 6e67 206f 6620 6669   beginning of fi
+00002e20: 6c65 2028 7369 7a65 206f 6620 6e46 7261  le (size of nFra
+00002e30: 6d65 2a6e 5365 7229 001c 5003 fb52 0000  me*nSer)..P..R..
+00002e40: 0000 0000 0001 022a 0000 0009 006e 5375  .......*.....nSu
+00002e50: 6d6d 6172 7900 0700 494e 545f 3455 002a  mmary...INT_4U.*
+00002e60: 004e 756d 6265 7220 6f66 2075 6e69 7175  .Number of uniqu
+00002e70: 6520 4672 5375 6d6d 6172 7920 6e61 6d65  e FrSummary name
+00002e80: 7320 696e 2066 696c 652e 0034 77a5 e94b  s in file..4w..K
+00002e90: 0000 0000 0000 0001 022b 0000 0009 006e  .........+.....n
+00002ea0: 616d 6553 5375 6d00 1100 5354 5249 4e47  ameSSum...STRING
+00002eb0: 5b6e 5375 6d6d 6172 795d 0019 0041 7272  [nSummary]...Arr
+00002ec0: 6179 206f 6620 4672 5375 6d6d 6172 7920  ay of FrSummary 
+00002ed0: 6e61 6d65 7300 0684 574e a200 0000 0000  names...WN......
+00002ee0: 0000 0102 2c00 0000 0c00 706f 7369 7469  ....,.....positi
+00002ef0: 6f6e 5365 7200 1900 494e 545f 3855 5b6e  onSer...INT_8U[n
+00002f00: 5375 6d6d 6172 795d 5b6e 4672 616d 655d  Summary][nFrame]
+00002f10: 0065 0041 7272 6179 206f 6620 6c69 7374  .e.Array of list
+00002f20: 7320 6f66 2046 7253 756d 6d61 7279 206f  s of FrSummary o
+00002f30: 6666 7365 7420 706f 7369 7469 6f6e 732c  ffset positions,
+00002f40: 2069 6e20 6279 7465 732c 2066 726f 6d20   in bytes, from 
+00002f50: 6265 6769 6e6e 696e 6720 6f66 2066 696c  beginning of fil
+00002f60: 6520 2873 697a 6520 6f66 206e 4672 616d  e (size of nFram
+00002f70: 652a 6e53 6572 2900 c376 da95 4800 0000  e*nSer)..v..H...
+00002f80: 0000 0000 0102 2d00 0000 0b00 6e45 7665  ......-.....nEve
+00002f90: 6e74 5479 7065 0007 0049 4e54 5f34 5500  ntType...INT_4U.
+00002fa0: 1e00 4e75 6d62 6572 206f 6620 4672 4576  ..Number of FrEv
+00002fb0: 656e 7420 696e 2074 6865 2066 696c 6500  ent in the file.
+00002fc0: cb0b 34f7 4c00 0000 0000 0000 0102 2e00  ..4.L...........
+00002fd0: 0000 0a00 6e61 6d65 4576 656e 7400 1300  ....nameEvent...
+00002fe0: 5354 5249 4e47 5b6e 4576 656e 7454 7970  STRING[nEventTyp
+00002ff0: 655d 0017 0041 7272 6179 206f 6620 4672  e]...Array of Fr
+00003000: 4576 656e 7420 6e61 6d65 7300 8aec 7442  Event names...tB
+00003010: 7200 0000 0000 0000 0102 2f00 0000 0700  r........./.....
+00003020: 6e45 7665 6e74 0013 0049 4e54 5f34 555b  nEvent...INT_4U[
+00003030: 6e45 7665 6e74 5479 7065 5d00 4000 4e75  nEventType].@.Nu
+00003040: 6d62 6572 206f 6620 4672 4576 656e 7420  mber of FrEvent 
+00003050: 666f 7220 6561 6368 2074 7970 6520 6f66  for each type of
+00003060: 2046 7245 7665 6e74 2028 7369 7a65 206f   FrEvent (size o
+00003070: 6620 6e45 7665 6e74 5479 7065 2900 aebb  f nEventType)...
+00003080: 6fd3 4300 0000 0000 0000 0102 3000 0000  o.C.........0...
+00003090: 0c00 6e54 6f74 616c 4576 656e 7400 0700  ..nTotalEvent...
+000030a0: 494e 545f 3455 0018 0054 6f74 616c 206e  INT_4U...Total n
+000030b0: 756d 6265 7220 6f66 2046 7245 7665 6e74  umber of FrEvent
+000030c0: 0074 8af4 4a54 0000 0000 0000 0001 0231  .t..JT.........1
+000030d0: 0000 000c 0047 5469 6d65 5345 7665 6e74  .....GTimeSEvent
+000030e0: 0014 0049 4e54 5f34 555b 6e54 6f74 616c  ...INT_4U[nTotal
+000030f0: 4576 656e 745d 001c 0047 5053 2074 696d  Event]...GPS tim
+00003100: 6520 696e 2069 6e74 6567 6572 2073 6563  e in integer sec
+00003110: 6f6e 6473 0015 3513 2961 0000 0000 0000  onds..5.)a......
+00003120: 0001 0232 0000 000c 0047 5469 6d65 4e45  ...2.....GTimeNE
+00003130: 7665 6e74 0014 0049 4e54 5f34 555b 6e54  vent...INT_4U[nT
+00003140: 6f74 616c 4576 656e 745d 0029 0052 6573  otalEvent].).Res
+00003150: 6964 7561 6c20 4750 5320 7469 6d65 2069  idual GPS time i
+00003160: 6e20 696e 7465 6765 7220 6e61 6e6f 7365  n integer nanose
+00003170: 636f 6e64 7300 157d 335d 4b00 0000 0000  conds..}3]K.....
+00003180: 0000 0102 3300 0000 0f00 616d 706c 6974  ....3.....amplit
+00003190: 7564 6545 7665 6e74 0014 0052 4541 4c5f  udeEvent...REAL_
+000031a0: 345b 6e54 6f74 616c 4576 656e 745d 0010  4[nTotalEvent]..
+000031b0: 0045 7665 6e74 2061 6d70 6c69 7475 6465  .Event amplitude
+000031c0: 00c2 ba16 4177 0000 0000 0000 0001 0234  ....Aw.........4
+000031d0: 0000 000e 0070 6f73 6974 696f 6e45 7665  .....positionEve
+000031e0: 6e74 0014 0049 4e54 5f38 555b 6e54 6f74  nt...INT_8U[nTot
+000031f0: 616c 4576 656e 745d 003d 0041 7272 6179  alEvent].=.Array
+00003200: 206f 6620 4672 4576 656e 7420 706f 7369   of FrEvent posi
+00003210: 7469 6f6e 732c 2069 6e20 6279 7465 732c  tions, in bytes,
+00003220: 2066 726f 6d20 6265 6769 6e6e 696e 6720   from beginning 
+00003230: 6f66 2066 696c 6500 46be 4b47 4e00 0000  of file.F.KGN...
+00003240: 0000 0000 0102 3500 0000 0e00 6e53 696d  ......5.....nSim
+00003250: 4576 656e 7454 7970 6500 0700 494e 545f  EventType...INT_
+00003260: 3455 0021 004e 756d 6265 7220 6f66 2046  4U.!.Number of F
+00003270: 7253 696d 4576 656e 7420 696e 2074 6865  rSimEvent in the
+00003280: 2066 696c 6500 d601 de2b 5500 0000 0000   file....+U.....
+00003290: 0000 0102 3600 0000 0d00 6e61 6d65 5369  ....6.....nameSi
+000032a0: 6d45 7665 6e74 0016 0053 5452 494e 475b  mEvent...STRING[
+000032b0: 6e53 696d 4576 656e 7454 7970 655d 001a  nSimEventType]..
+000032c0: 0041 7272 6179 206f 6620 4672 5369 6d45  .Array of FrSimE
+000032d0: 7665 6e74 206e 616d 6573 00c3 e4da a081  vent names......
+000032e0: 0000 0000 0000 0001 0237 0000 000a 006e  .........7.....n
+000032f0: 5369 6d45 7665 6e74 0016 0049 4e54 5f34  SimEvent...INT_4
+00003300: 555b 6e53 696d 4576 656e 7454 7970 655d  U[nSimEventType]
+00003310: 0049 004e 756d 6265 7220 6f66 2046 7253  .I.Number of FrS
+00003320: 696d 4576 656e 7420 666f 7220 6561 6368  imEvent for each
+00003330: 2074 7970 6520 6f66 2046 7253 696d 4576   type of FrSimEv
+00003340: 656e 7420 2873 697a 6520 6f66 206e 5369  ent (size of nSi
+00003350: 6d45 7665 6e74 5479 7065 2900 4e11 c946  mEventType).N..F
+00003360: 4700 0000 0000 0000 0102 3800 0000 0d00  G.........8.....
+00003370: 6e54 6f74 616c 5345 7665 6e74 0007 0049  nTotalSEvent...I
+00003380: 4e54 5f34 5500 1b00 546f 7461 6c20 6e75  NT_4U...Total nu
+00003390: 6d62 6572 206f 6620 4672 5369 6d45 7665  mber of FrSimEve
+000033a0: 6e74 00de 86a5 7e53 0000 0000 0000 0001  nt....~S........
+000033b0: 0239 0000 000a 0047 5469 6d65 5353 696d  .9.....GTimeSSim
+000033c0: 0015 0049 4e54 5f34 555b 6e54 6f74 616c  ...INT_4U[nTotal
+000033d0: 5345 7665 6e74 5d00 1c00 4750 5320 7469  SEvent]...GPS ti
+000033e0: 6d65 2069 6e20 696e 7465 6765 7220 7365  me in integer se
+000033f0: 636f 6e64 7300 8b64 9181 6000 0000 0000  conds..d..`.....
+00003400: 0000 0102 3a00 0000 0a00 4754 696d 654e  ....:.....GTimeN
+00003410: 5369 6d00 1500 494e 545f 3455 5b6e 546f  Sim...INT_4U[nTo
+00003420: 7461 6c53 4576 656e 745d 0029 0052 6573  talSEvent].).Res
+00003430: 6964 7561 6c20 4750 5320 7469 6d65 2069  idual GPS time i
+00003440: 6e20 696e 7465 6765 7220 6e61 6e6f 7365  n integer nanose
+00003450: 636f 6e64 7300 6127 db26 5200 0000 0000  conds.a'.&R.....
+00003460: 0000 0102 3b00 0000 1200 616d 706c 6974  ....;.....amplit
+00003470: 7564 6553 696d 4576 656e 7400 1500 5245  udeSimEvent...RE
+00003480: 414c 5f34 5b6e 546f 7461 6c53 4576 656e  AL_4[nTotalSEven
+00003490: 745d 0013 0053 696d 4576 656e 7420 616d  t]...SimEvent am
+000034a0: 706c 6974 7564 6500 2410 90c2 7e00 0000  plitude.$...~...
+000034b0: 0000 0000 0102 3c00 0000 1100 706f 7369  ......<.....posi
+000034c0: 7469 6f6e 5369 6d45 7665 6e74 0015 0049  tionSimEvent...I
+000034d0: 4e54 5f38 555b 6e54 6f74 616c 5345 7665  NT_8U[nTotalSEve
+000034e0: 6e74 5d00 4000 4172 7261 7920 6f66 2046  nt].@.Array of F
+000034f0: 7253 696d 4576 656e 7420 706f 7369 7469  rSimEvent positi
+00003500: 6f6e 732c 2069 6e20 6279 7465 732c 2066  ons, in bytes, f
+00003510: 726f 6d20 6265 6769 6e6e 696e 6720 6f66  rom beginning of
+00003520: 2066 696c 6500 9f96 37f5 3600 0000 0000   file...7.6.....
+00003530: 0000 0102 3d00 0000 0700 6368 6b53 756d  ....=.....chkSum
+00003540: 0007 0049 4e54 5f34 5500 1000 5374 7275  ...INT_4U...Stru
+00003550: 6374 2063 6865 636b 7375 6d00 8e79 d77a  ct checksum..y.z
+00003560: 5001 0000 0000 0000 0113 0000 0000 2500  P.............%.
+00003570: 0100 0000 0000 0000 b881 8348 0000 0000  ...........H....
+00003580: 0000 0000 0000 1040 0000 0000 0000 0000  .......@........
+00003590: 6e09 0000 0000 0000 0000 0000 0000 0000  n...............
 000035a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000035b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000035c0: 0600 0000 0300 0500 0b00 1400 0700 1300  ................
-000035d0: 0700 4672 616d 6548 000b 0046 7244 6574  ..FrameH...FrDet
-000035e0: 6563 746f 7200 0b00 4672 5072 6f63 4461  ector...FrProcDa
-000035f0: 7461 0007 0046 7256 6563 7400 0d00 4672  ta...FrVect...Fr
-00003600: 456e 644f 6646 7261 6d65 0006 0046 7254  EndOfFrame...FrT
-00003610: 4f43 0001 0000 0007 004c 4c4f 5f34 6b00  OC.......LLO_4k.
-00003620: 020d 0000 0000 0000 0000 0000 0000 0000  ................
-00003630: 0000 0000 0300 0000 1100 4c31 3a44 4d54  ..........L1:DMT
-00003640: 2d44 515f 5645 4354 4f52 001a 004c 313a  -DQ_VECTOR...L1:
-00003650: 4744 532d 4341 4c49 425f 5354 4154 455f  GDS-CALIB_STATE_
-00003660: 5645 4354 4f52 0017 004c 313a 4944 512d  VECTOR...L1:IDQ-
-00003670: 4641 505f 4f56 4c5f 3332 5f32 3034 3800  FAP_OVL_32_2048.
-00003680: 0214 0000 0000 0000 1619 0000 0000 0000  ................
-00003690: 291a 0000 0000 0000 ffff ffff ffff ffff  )...............
-000036a0: ffff ffff 0000 0000 0000 0000 0000 0000  ................
-000036b0: 0000 0000 de12 5dba 3f00 0000 0000 0000  ......].?.......
-000036c0: 0101 0100 0000 0c00 4672 456e 644f 6646  ........FrEndOfF
-000036d0: 696c 6500 0600 1b00 456e 6420 6f66 2046  ile.....End of F
-000036e0: 696c 6520 4461 7461 2053 7472 7563 7475  ile Data Structu
-000036f0: 7265 00a8 da1b ec45 0000 0000 0000 0001  re.....E........
-00003700: 023e 0000 0008 006e 4672 616d 6573 0007  .>.....nFrames..
-00003710: 0049 4e54 5f34 5500 1e00 4e75 6d62 6572  .INT_4U...Number
-00003720: 206f 6620 6672 616d 6573 2069 6e20 7468   of frames in th
-00003730: 6973 2066 696c 6500 c01d f442 5f00 0000  is file....B_...
-00003740: 0000 0000 0102 3f00 0000 0700 6e42 7974  ......?.....nByt
-00003750: 6573 0007 0049 4e54 5f38 5500 3900 546f  es...INT_8U.9.To
-00003760: 7461 6c20 6e75 6d62 6572 206f 6620 6279  tal number of by
-00003770: 7465 7320 696e 2074 6869 7320 6669 6c65  tes in this file
-00003780: 2028 2030 2069 6620 4e4f 5420 636f 6d70   ( 0 if NOT comp
-00003790: 7574 6564 2029 0082 8d13 02a1 0000 0000  uted )..........
-000037a0: 0000 0001 0240 0000 0008 0073 6565 6b54  .....@.....seekT
-000037b0: 4f43 0007 0049 4e54 5f38 5500 7a00 4279  OC...INT_8U.z.By
-000037c0: 6573 2074 6f20 6261 636b 2075 7020 746f  es to back up to
-000037d0: 2074 6865 2062 6567 696e 6e69 6e67 206f   the beginning o
-000037e0: 6620 7468 6520 7461 626c 6520 6f66 2063  f the table of c
-000037f0: 6f6e 7465 6e74 7320 7374 7275 6374 7572  ontents structur
-00003800: 652e 2049 6620 7365 656b 544f 4320 3d3d  e. If seekTOC ==
-00003810: 2030 2c20 7468 656e 2074 6865 7265 2069   0, then there i
-00003820: 7320 6e6f 2054 4f43 2066 6f72 2074 6869  s no TOC for thi
-00003830: 7320 6669 6c65 2e00 c8d4 6535 4100 0000  s file....e5A...
-00003840: 0000 0000 0102 4100 0000 0f00 6368 6b53  ......A.....chkS
-00003850: 756d 4672 4865 6164 6572 0007 0049 4e54  umFrHeader...INT
-00003860: 5f34 5500 1300 4672 4865 6164 6572 2063  _4U...FrHeader c
-00003870: 6865 636b 7375 6d2e 0009 9135 933a 0000  hecksum....5.:..
-00003880: 0000 0000 0001 0242 0000 0007 0063 686b  .......B.....chk
-00003890: 5375 6d00 0700 494e 545f 3455 0014 0053  Sum...INT_4U...S
-000038a0: 7472 7563 7475 7265 2063 6865 636b 7375  tructure checksu
-000038b0: 6d2e 00d0 97d1 a839 0000 0000 0000 0001  m......9........
-000038c0: 0243 0000 000b 0063 686b 5375 6d46 696c  .C.....chkSumFil
-000038d0: 6500 0700 494e 545f 3455 000f 0046 696c  e...INT_4U...Fil
-000038e0: 6520 6368 6563 6b73 756d 2e00 16df ff60  e checksum.....`
-000038f0: 2e00 0000 0000 0000 0106 0000 0000 0100  ................
-00003900: 0000 1e39 0000 0000 0000 b603 0000 0000  ...9............
-00003910: 0000 bac1 b663 544f 306c ba4a a03b       .....cTO0l.J.;
+000035b0: 0000 0000 0000 0000 0600 0000 0300 0500  ................
+000035c0: 0b00 1400 0700 1300 0700 4672 616d 6548  ..........FrameH
+000035d0: 000b 0046 7244 6574 6563 746f 7200 0b00  ...FrDetector...
+000035e0: 4672 5072 6f63 4461 7461 0007 0046 7256  FrProcData...FrV
+000035f0: 6563 7400 0d00 4672 456e 644f 6646 7261  ect...FrEndOfFra
+00003600: 6d65 0006 0046 7254 4f43 0001 0000 0007  me...FrTOC......
+00003610: 004c 4c4f 5f34 6b00 020d 0000 0000 0000  .LLO_4k.........
+00003620: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00003630: 1100 4c31 3a44 4d54 2d44 515f 5645 4354  ..L1:DMT-DQ_VECT
+00003640: 4f52 001a 004c 313a 4744 532d 4341 4c49  OR...L1:GDS-CALI
+00003650: 425f 5354 4154 455f 5645 4354 4f52 0017  B_STATE_VECTOR..
+00003660: 004c 313a 4944 512d 4641 505f 4f56 4c5f  .L1:IDQ-FAP_OVL_
+00003670: 3332 5f32 3034 3800 0214 0000 0000 0000  32_2048.........
+00003680: 1619 0000 0000 0000 291a 0000 0000 0000  ........).......
+00003690: ffff ffff ffff ffff ffff ffff 0000 0000  ................
+000036a0: 0000 0000 0000 0000 0000 0000 5a2d 2ead  ............Z-..
+000036b0: 3f00 0000 0000 0000 0101 0100 0000 0c00  ?...............
+000036c0: 4672 456e 644f 6646 696c 6500 0600 1b00  FrEndOfFile.....
+000036d0: 456e 6420 6f66 2046 696c 6520 4461 7461  End of File Data
+000036e0: 2053 7472 7563 7475 7265 00a8 da1b ec45   Structure.....E
+000036f0: 0000 0000 0000 0001 023e 0000 0008 006e  .........>.....n
+00003700: 4672 616d 6573 0007 0049 4e54 5f34 5500  Frames...INT_4U.
+00003710: 1e00 4e75 6d62 6572 206f 6620 6672 616d  ..Number of fram
+00003720: 6573 2069 6e20 7468 6973 2066 696c 6500  es in this file.
+00003730: c01d f442 5f00 0000 0000 0000 0102 3f00  ...B_.........?.
+00003740: 0000 0700 6e42 7974 6573 0007 0049 4e54  ....nBytes...INT
+00003750: 5f38 5500 3900 546f 7461 6c20 6e75 6d62  _8U.9.Total numb
+00003760: 6572 206f 6620 6279 7465 7320 696e 2074  er of bytes in t
+00003770: 6869 7320 6669 6c65 2028 2030 2069 6620  his file ( 0 if 
+00003780: 4e4f 5420 636f 6d70 7574 6564 2029 0082  NOT computed )..
+00003790: 8d13 02a1 0000 0000 0000 0001 0240 0000  .............@..
+000037a0: 0008 0073 6565 6b54 4f43 0007 0049 4e54  ...seekTOC...INT
+000037b0: 5f38 5500 7a00 4279 6573 2074 6f20 6261  _8U.z.Byes to ba
+000037c0: 636b 2075 7020 746f 2074 6865 2062 6567  ck up to the beg
+000037d0: 696e 6e69 6e67 206f 6620 7468 6520 7461  inning of the ta
+000037e0: 626c 6520 6f66 2063 6f6e 7465 6e74 7320  ble of contents 
+000037f0: 7374 7275 6374 7572 652e 2049 6620 7365  structure. If se
+00003800: 656b 544f 4320 3d3d 2030 2c20 7468 656e  ekTOC == 0, then
+00003810: 2074 6865 7265 2069 7320 6e6f 2054 4f43   there is no TOC
+00003820: 2066 6f72 2074 6869 7320 6669 6c65 2e00   for this file..
+00003830: c8d4 6535 4100 0000 0000 0000 0102 4100  ..e5A.........A.
+00003840: 0000 0f00 6368 6b53 756d 4672 4865 6164  ....chkSumFrHead
+00003850: 6572 0007 0049 4e54 5f34 5500 1300 4672  er...INT_4U...Fr
+00003860: 4865 6164 6572 2063 6865 636b 7375 6d2e  Header checksum.
+00003870: 0009 9135 933a 0000 0000 0000 0001 0242  ...5.:.........B
+00003880: 0000 0007 0063 686b 5375 6d00 0700 494e  .....chkSum...IN
+00003890: 545f 3455 0014 0053 7472 7563 7475 7265  T_4U...Structure
+000038a0: 2063 6865 636b 7375 6d2e 00d0 97d1 a839   checksum......9
+000038b0: 0000 0000 0000 0001 0243 0000 000b 0063  .........C.....c
+000038c0: 686b 5375 6d46 696c 6500 0700 494e 545f  hkSumFile...INT_
+000038d0: 3455 000f 0046 696c 6520 6368 6563 6b73  4U...File checks
+000038e0: 756d 2e00 16df ff60 2e00 0000 0000 0000  um.....`........
+000038f0: 0106 0000 0000 0100 0000 1639 0000 0000  ...........9....
+00003900: 0000 b603 0000 0000 0000 bac1 b663 8668  .............c.h
+00003910: 785b bd0c 3ba0                           x[..;.
```

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/llhoft/omegascan/scanme.gwf` & `gwcelery-2.1.0/gwcelery/tests/data/llhoft/omegascan/scanme.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.1.0/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/lvalert_event_creation.json` & `gwcelery-2.1.0/gwcelery/tests/data/lvalert_event_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/lvalert_xmpp.xml` & `gwcelery-2.1.0/gwcelery/tests/data/lvalert_xmpp.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/mock_superevent_object.json` & `gwcelery-2.1.0/gwcelery/tests/data/mock_superevent_object.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite` & `gwcelery-2.1.0/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/psd.xml.gz` & `gwcelery-2.1.0/gwcelery/tests/data/psd.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/rrt_small_area.fits` & `gwcelery-2.1.0/gwcelery/tests/data/rrt_small_area.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/sample_events.json` & `gwcelery-2.1.0/gwcelery/tests/data/sample_events.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/samples.hdf5` & `gwcelery-2.1.0/gwcelery/tests/data/samples.hdf5`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/scaler_set_all.pickle` & `gwcelery-2.1.0/gwcelery/tests/data/scaler_set_all.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/snews_gcn.xml` & `gwcelery-2.1.0/gwcelery/tests/data/snews_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/snews_gcn_test.xml` & `gwcelery-2.1.0/gwcelery/tests/data/snews_gcn_test.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/superevents.json` & `gwcelery-2.1.0/gwcelery/tests/data/superevents.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/swift_grb_gcn.xml` & `gwcelery-2.1.0/gwcelery/tests/data/swift_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/data/test_classifier.pickle` & `gwcelery-2.1.0/gwcelery/tests/data/test_classifier.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/process.py` & `gwcelery-2.1.0/gwcelery/tests/process.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_sentry.py` & `gwcelery-2.1.0/gwcelery/tests/test_sentry.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_alerts.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_alerts.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_alerts_validate.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_alerts_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_bayestar.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_circulars.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_circulars.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,14 +29,29 @@
 
     # call create_emcoinc_circular
     circulars.create_emcoinc_circular(superevent_id)
     mock_compose_emcoinc_circular.assert_called_once_with(
         'S1234', client=gracedb.client)
 
 
+def test_create_medium_latency_circular(monkeypatch):
+    """Test that the compose medium latency circulars method is called with the
+    correct input parameters.
+    """
+    ext_event_id = 'E1234'
+    mock_compose_medium_latency_circular = Mock()
+    monkeypatch.setattr('ligo.followup_advocate.compose_grb_medium_latency',
+                        mock_compose_medium_latency_circular)
+
+    # call create_emcoinc_circular
+    circulars.create_medium_latency_circular(ext_event_id)
+    mock_compose_medium_latency_circular.assert_called_once_with(
+        'E1234', client=gracedb.client)
+
+
 @pytest.mark.parametrize(
      'update_types',
      [['sky_localization', 'em_bright', 'p_astro'],
       ['sky_localization', 'em_bright', 'p_astro', 'raven'],
       ['raven']])
 def test_create_update_circular(monkeypatch, update_types):
     """Test that the compose update circulars method is called with the
```

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_condor.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_detchar.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_detchar.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from io import BytesIO
 import logging
 from pathlib import Path
 from unittest.mock import call, patch
 
 from astropy.time import Time
+import celery
 from gwpy.timeseries import Bits
 import matplotlib.pyplot as plt
 import numpy as np
 import pytest
 
 from ..import app
 from ..import _version
@@ -30,20 +31,39 @@
 def ifo_h1(monkeypatch):
     monkeypatch.setitem(app.conf, 'llhoft_channels', {
         'H1:DMT-DQ_VECTOR': 'dmt_dq_vector_bits',
         'H1:GDS-CALIB_STATE_VECTOR': 'ligo_state_vector_bits'})
 
 
 @pytest.fixture
+def ifo_l1(monkeypatch):
+    monkeypatch.setitem(app.conf, 'llhoft_channels', {
+        'L1:DMT-DQ_VECTOR': 'dmt_dq_vector_bits',
+        'L1:GDS-CALIB_STATE_VECTOR': 'ligo_state_vector_bits'})
+
+
+@pytest.fixture
 def ifo_h1_idq(monkeypatch):
     monkeypatch.setitem(
         app.conf, 'idq_channels', ['H1:IDQ-FAP_OVL_32_2048'])
 
 
 @pytest.fixture
+def ifo_l1_idq(monkeypatch):
+    monkeypatch.setitem(
+        app.conf, 'idq_channels', ['L1:IDQ-FAP_OVL_32_2048'])
+
+
+@pytest.fixture
+def ifo_l1_idq_wrong_channel_name(monkeypatch):
+    monkeypatch.setitem(
+        app.conf, 'idq_channels', ['L1:IDQ-FAP_OVL_WRONG'])
+
+
+@pytest.fixture
 def gatedpipe(monkeypatch):
     monkeypatch.setitem(app.conf, 'uses_gatedhoft', {'gatepipe': True})
 
 
 @pytest.fixture
 def gatedpipe_prepost(monkeypatch):
     monkeypatch.setitem(
@@ -116,14 +136,25 @@
     channel = 'H1:IDQ-FAP_OVL_32_2048'
     start, end = 1216577976, 1216577980
     cache = detchar.create_cache('H1', start, end)
     assert detchar.check_idq(cache, channel, start, end) == (
         'H1:IDQ-FAP_OVL_32_2048', 1)
 
 
+def test_check_idq_wrong_channel_handled(caplog, llhoft_glob_pass):
+    """Test that iDQ checks looking at the wrong channel are handled."""
+    caplog.set_level(logging.INFO)
+    channel = 'H1:IDQ-FAP_OVL_WRONG'
+    start, end = 1216577976, 1216577980
+    cache = detchar.create_cache('H1', start, end)
+    detchar.check_idq(cache, channel, start, end)
+    messages = [record.message for record in caplog.records]
+    assert 'Failed to read from low-latency iDQ frame files' in messages  # noqa: E501
+
+
 @patch('time.strftime', return_value='00:00:00 UTC Mon 01 Jan 2000')
 @patch('socket.gethostname', return_value='test_host')
 @patch('getpass.getuser', return_value='test_user')
 def test_dqr_json(mock_time, mock_host, mock_user):
     state = "pass"
     summary = "72 and sunny!!"
     assert detchar.dqr_json(state, summary) == {
@@ -223,15 +254,15 @@
         call(
             None, None, 'S12345a',
             ('No HW injections found. '
              'Check looked within -1.5/+1.5 seconds of superevent. '),
             ['data_quality']),
         call(
             None, None, 'S12345a',
-            ('iDQ false alarm probabilities at both H1 and L1'
+            ('iDQ false alarm probabilities for active detectors'
              ' are good (above {} threshold). '
              'Minimum FAP is "H1:IDQ-FAP_OVL_32_2048": 1.0. '
              'Check looked within -1.5/+1.5 seconds of superevent. ').format(
                  app.conf['idq_fap_thresh']),
             ['data_quality']),
         call(
             '"dqrjson"', 'gwcelerydetcharcheckvectors-S12345a.json', 'S12345a',
@@ -245,14 +276,81 @@
         any_order=True)
 
 
 @patch('gwcelery.tasks.detchar.dqr_json', return_value='dqrjson')
 @patch('gwcelery.tasks.gracedb.upload.run')
 @patch('gwcelery.tasks.gracedb.remove_label')
 @patch('gwcelery.tasks.gracedb.create_label')
+def test_check_vectors_fails(
+        mock_create_label, mock_remove_label, mock_upload,
+        mock_json, llhoft_glob_fail, ifo_l1, ifo_l1_idq):
+    event = {'search': 'AllSky', 'instruments': 'L1', 'pipeline': 'oLIB'}
+    superevent_id = 'S12345a'
+    start, end = 1216577978, 1216577978.1
+    detchar.check_vectors(event, superevent_id, start, end)
+    calls = [
+        call(
+            None, None, 'S12345a',
+            ('Detector state for active instruments is bad.\n{}'
+             'Check looked within -1.5/+1.5 seconds of superevent. ').format(
+                 detchar.generate_table(
+                     'Data quality bits', [],
+                     ['L1:NO_OMC_DCPD_ADC_OVERFLOW',
+                      'L1:NO_DMT-ETMY_ESD_DAC_OVERFLOW',
+                      'L1:HOFT_OK', 'L1:OBSERVATION_INTENT'], [])),
+            ['data_quality']),
+        call(
+            None, None, 'S12345a',
+            ('Injection found.\n{}\n'
+             'Check looked within -1.5/+1.5 seconds of superevent. ').format(
+                 detchar.generate_table(
+                     'Injection bits', [],
+                     ['L1:NO_STOCH_HW_INJ', 'L1:NO_CBC_HW_INJ',
+                      'L1:NO_BURST_HW_INJ', 'L1:NO_DETCHAR_HW_INJ'], [])),
+            ['data_quality']),
+        call(
+            None, None, 'S12345a',
+            ('iDQ false alarm probability is low '
+             '(below {} threshold), '
+             'i.e., there could be a data quality issue: '
+             'minimum FAP is "L1:IDQ-FAP_OVL_32_2048": 0.0. '
+             'Check looked within -1.5/+1.5 seconds of superevent. ').format(
+                 app.conf['idq_fap_thresh']),
+            ['data_quality']),
+        call(
+            '"dqrjson"', 'gwcelerydetcharcheckvectors-S12345a.json', 'S12345a',
+            'DQR-compatible json generated from check_vectors results'),
+    ]
+    mock_upload.assert_has_calls(calls, any_order=True)
+    mock_create_label.assert_called_with('DQV', 'S12345a')
+    mock_remove_label.assert_called_with('DQOK', 'S12345a')
+
+
+@patch('gwcelery.tasks.gracedb.upload.run')
+@patch('celery.app.task.Task.request')
+@patch('gwcelery.tasks.detchar.check_vector', side_effect=ValueError)
+def test_check_vectors_retries_on_valueerror(
+        mock_check_vector, mock_request,
+        mock_upload, llhoft_glob_pass, ifo_h1, ifo_h1_idq):
+    # Mocking this retry https://docs.celeryq.dev/en/stable/_modules/celery/app/task.html#Task.retry  # noqa E501
+    event = {'search': 'AllSky', 'instruments': 'L1', 'pipeline': 'oLIB'}
+    superevent_id = 'S12345a'
+    start, end = 1216577978, 1216577978.1
+    mock_request.called_directly = False
+    mock_request.retries = 3
+    with pytest.raises(celery.exceptions.Retry) as retry_exc:
+        detchar.check_vectors.delay(event, superevent_id, start, end)
+    # after three retries, should still retry once in 5 seconds
+    assert retry_exc.value.when == 5
+
+
+@patch('gwcelery.tasks.detchar.dqr_json', return_value='dqrjson')
+@patch('gwcelery.tasks.gracedb.upload.run')
+@patch('gwcelery.tasks.gracedb.remove_label')
+@patch('gwcelery.tasks.gracedb.create_label')
 def test_gatedhoft_skips_dmtvec(mock_create_label, mock_remove_label,
                                 mock_upload, mock_json, llhoft_glob_pass,
                                 ifo_h1, ifo_h1_idq, gatedpipe,
                                 gatedpipe_prepost):
     event = {'search': 'AllSky', 'instruments': 'H1', 'pipeline': 'gatepipe'}
     superevent_id = 'S12345a'
     start, end = 1216577977, 1216577979
```

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_em_bright.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_em_bright.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_external_skymaps.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_external_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_external_triggers.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_external_triggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,15 +316,16 @@
              }
     external_triggers.handle_grb_igwn_alert(alert)
     mock_raven_pipeline.assert_called_once_with([{'superevent_id': 'S1234',
                                                   'preferred_event': 'G1234',
                                                   'preferred_event_data':
                                                       {'group': 'CBC'}}],
                                                 'E1212', alert['object'],
-                                                -5, 1, 'CBC')
+                                                -5, 1, 'CBC',
+                                                use_superevent_skymap=False)
     if pipeline != 'Swift':
         mock_create_combined_skymap.assert_called_once_with(
             'S1234', 'E1212', preferred_event='G1234')
     else:
         mock_create_combined_skymap.assert_not_called()
 
 
@@ -437,34 +438,100 @@
     else:
         mock_create_combined_skymap.assert_not_called()
     if 'S' in graceid:
         calls = [
             call(
                 [_mock_get_event('E1')],
                 graceid, event,
-                -1, 5, 'CBC'),
+                -1, 5, 'CBC',
+                use_superevent_skymap=True),
             call(
                 [_mock_get_event('E2')],
                 graceid, event,
-                -1, 5, 'CBC'),
+                -1, 5, 'CBC',
+                use_superevent_skymap=True),
             call(
                 [_mock_get_event('E3')],
                 graceid, event,
-                -1, 5, 'CBC')
+                -1, 5, 'CBC',
+                use_superevent_skymap=True)
         ]
     else:
         calls = [
             call(
                 [_mock_get_superevent('S1')],
                 graceid, event,
-                -5, 1, 'CBC')
+                -5, 1, 'CBC',
+                use_superevent_skymap=(graceid == 'E3'))
         ]
     mock_raven_pipeline.assert_has_calls(calls)
 
 
+@pytest.mark.parametrize(
+    "alert_type, comment,"
+    "expected_combined_skymap_calls, expected_pipeline_calls,"
+    "expected_result",
+    [
+        ("log",
+         "Updated superevent parameters: preferred_event: example", 1, 2,
+         True),
+        ("log",
+         "Some other comment", 0, 0, False),
+        ("other_type",
+         "Updated superevent parameters: preferred_event: example", 0, 0,
+         False),
+        ("log",
+         "Updated superevent parameters: different_param: example", 0, 0,
+         False)
+    ]
+)
+@patch('gwcelery.tasks.raven.raven_pipeline.run')
+@patch('gwcelery.tasks.external_skymaps.create_combined_skymap.run')
+@patch('gwcelery.tasks.gracedb.get_event', _mock_get_event)
+def test_preferred_event_coinc_far_calculation(
+        mock_create_combined_skymap,
+        mock_raven_pipeline,
+        alert_type,
+        comment,
+        expected_combined_skymap_calls,
+        expected_pipeline_calls,
+        expected_result):
+    alert = {
+        "alert_type": alert_type,
+        "uid": 'S1',
+        "object": {"labels": ["EM_COINC"], "superevent_id": 'S1',
+                   "em_events": ["E1", "E2"],
+                   "preferred_event": 'G1',
+                   "em_type": 'E1',
+                   "preferred_event_data": {"group": "CBC"}},
+        "data": {"comment": comment, "filename": ""}
+    }
+
+    external_triggers.handle_grb_igwn_alert(alert)
+
+    assert (mock_create_combined_skymap.call_count ==
+            expected_combined_skymap_calls)
+    assert mock_raven_pipeline.call_count == expected_pipeline_calls
+
+    if expected_result:
+        mock_create_combined_skymap.assert_called_with(
+            'S1', 'E1', preferred_event='G1')
+        mock_raven_pipeline.assert_has_calls(
+            [call(
+                [_mock_get_event('E1')],
+                'S1', alert['object'],
+                -1, 5, 'CBC',
+                use_superevent_skymap=False),
+             call(
+                 [_mock_get_event('E2')],
+                 'S1', alert['object'],
+                 -1, 5, 'CBC',
+                 use_superevent_skymap=False)])
+
+
 @pytest.mark.parametrize('labels',
                          [["EM_COINC", "SKYMAP_READY", "RAVEN_ALERT", "ADVOK"],
                           ["EM_COINC", "SKYMAP_READY", "ADVOK"]])
 @patch('gwcelery.tasks.gracedb.client')
 @patch('gwcelery.tasks.gracedb.get_event.run', return_value={
     'graceid': 'E1234', 'pipeline': 'Fermi'})
 @patch('gwcelery.tasks.gracedb.create_label.run')
```

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_first2years.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_first2years_external.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_first2years_external.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_gcn.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_gcn_validate.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_gcn_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_gracedb.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_igwn_alert.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_inference.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import configparser
+import glob
 from itertools import product
 import os
 import subprocess
 
 import json
 import pytest
 from unittest.mock import Mock
@@ -216,15 +217,16 @@
 
         path_to_settings = cmd[10]
         assert os.path.exists(path_to_settings)
         ans = {
             'summarypages_arguments': {'gracedb': event['graceid'],
                                        'no_ligo_skymap': True},
             'queue': 'Online_PE',
-            'accounting_user': 'soichiro.morisaki'
+            'accounting_user': 'soichiro.morisaki',
+            'enforce_signal_duration': False
         }
         if host != 'gracedb.ligo.org':
             ans['queue'] = 'Online_PE_MDC'
         if mode == 'production':
             ans.update(
                 {'sampler_kwargs': {'naccept': 60, 'nlive': 500,
                                     'npool': 24, 'sample': 'acceptance-walk'},
@@ -243,15 +245,16 @@
                 if 0.6 < mc < 1.465:
                     assert w == "IMRPhenomD"
                     ans['sampler_kwargs']['naccept'] = 10
                 elif mc < 11.033:
                     assert w == "IMRPhenomPv2"
                 else:
                     assert w == "IMRPhenomXPHM"
-                    ans['request_memory_generation'] = 16.0
+                    ans['request_memory_generation'] = 36.0
+                    ans['request_memory'] = 16.0
         elif mode == 'fast_test' and mc < 3.9:
             ans['request_memory_generation'] = 8.0
         with open(path_to_settings, 'r') as f:
             assert json.load(f) == ans
 
         with open(os.path.join(rundir, 'bilby_config.ini'), 'w') as f:
             f.write(ini)
@@ -406,29 +409,41 @@
             mock_setup_dag_for_rapidpe.assert_called_once()
     else:
         with pytest.raises(NotImplementedError):
             inference.dag_prepare_task(
                 rundir, event, sid, pipeline, frametype_dict).delay()
 
 
-@pytest.mark.parametrize('exc', [condor.JobAborted(1, 'test'),
-                                 condor.JobFailed(1, 'test'),
-                                 condor.JobRunning({'Cluster': 1234})])
-def test_job_error_notification(monkeypatch, tmp_path, exc):
+@pytest.mark.parametrize(
+    'exc,host',
+    product(
+        [condor.JobAborted(1, 'test'),
+         condor.JobFailed(1, 'test'),
+         condor.JobRunning({'Cluster': 1234})],
+        ['gracedb-playground.ligo.org', 'gracedb.ligo.org']
+    )
+)
+def test_job_error_notification(monkeypatch, tmp_path, exc, host):
+    monkeypatch.setitem(app.conf, 'gracedb_host', host)
     filenames = ['pe.log', 'pe.err', 'pe.out']
     for filename in filenames:
         with open(str(tmp_path / filename), 'w') as f:
             f.write('test')
     upload = Mock()
+    cleanup = Mock()
     monkeypatch.setattr('gwcelery.tasks.gracedb.upload.run', upload)
+    monkeypatch.setattr(
+        'gwcelery.tasks.inference._clean_up_bilby.run', cleanup
+    )
     monkeypatch.setattr('subprocess.run', Mock())
-
     inference.job_error_notification(
-        None, exc, 'test', 'S1234', str(tmp_path), 'lalinference')
+        None, exc, 'test', 'S1234', str(tmp_path), 'bilby')
     assert upload.call_count == len(filenames) + 1
+    if host != 'gracedb.ligo.org':
+        cleanup.assert_called_once()
 
 
 @pytest.mark.parametrize(
     'pipeline,host',
     product(
         ['lalinference', 'bilby_production', 'bilby_fast_test', 'rapidpe',
          'my_awesome_pipeline'],
@@ -437,21 +452,23 @@
 )
 def test_dag_finished(monkeypatch, tmp_path, pipeline, host):
     monkeypatch.setitem(app.conf, 'gracedb_host', host)
     sid = 'S1234'
     rundir = str(tmp_path / 'rundir')
     resultdir = str(tmp_path / 'rundir/result')
     sampledir = str(tmp_path / 'rundir/final_result')
+    datadir = str(tmp_path / 'rundir/data')
     pe_results_path = str(tmp_path / 'public_html/online_pe')
     monkeypatch.setitem(app.conf, 'pe_results_path', pe_results_path)
     pe_results_path = os.path.join(pe_results_path, sid, pipeline)
     os.makedirs(rundir)
     os.makedirs(resultdir)
     os.makedirs(sampledir)
     os.makedirs(pe_results_path)
+    os.makedirs(datadir)
 
     upload = Mock()
     create_label = Mock()
     monkeypatch.setattr('gwcelery.tasks.gracedb.upload.run', upload)
     monkeypatch.setattr('gwcelery.tasks.gracedb.create_label.run',
                         create_label)
 
@@ -518,27 +535,51 @@
                         "--redshift_method", "exact", "--evolve_spins_forwards"
                     ]
                 assert args == ans
 
             monkeypatch.setattr(
                 'gwcelery.tasks.condor.check_output.run', mock_check_output)
 
+            with open(
+                os.path.join(datadir, "test_generation_roq_weights.hdf5"),
+                "wb"
+            ) as f:
+                f.write(b'data')
+            with open(
+                os.path.join(datadir, "test_generation_data_dump.pickle"),
+                "wb"
+            ) as f:
+                f.write(b'data')
+        elif pipeline == "rapidpe":
+            summary_path = os.path.join(rundir, "summary")
+            os.makedirs(summary_path, exist_ok=True)
+            paths = [
+                os.path.join(summary_path, "p_astro.json"),
+                os.path.join(summary_path, "p_astro.png"),
+            ]
+
         else:
             paths = []
         for path in paths:
             with open(path, 'wb') as f:
                 f.write(b'result')
 
         inference.dag_finished(rundir, sid, pipeline, **kwargs)
 
         if pipeline == 'rapidpe':
-            upload.assert_called_once()
+            # +1 corresponds to summary page link
+            assert upload.call_count == len(paths) + 1
         elif pipeline == 'bilby':
             # +1 corresponds to pesummary link
             assert upload.call_count == len(paths) + 1
+            n = len(glob.glob(os.path.join(datadir, "*")))
+            if host == "gracedb.ligo.org":
+                assert n == 2
+            else:
+                assert n == 0
         else:
             assert upload.call_count == len(paths)
 
         if pipeline == 'bilby':
             create_label.assert_called_once()
         else:
             create_label.assert_not_called()
```

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_orchestrator.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_orchestrator.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_p_astro.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_raven.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_raven.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,35 +242,29 @@
         'M15', -1, 5, 'CBC'],
      [[{'superevent_id': 'S13', 'far': 1, 'preferred_event': 'G4'}],
         'E6', -60, 600, 'Burst']])
 @patch('gwcelery.tasks.raven.trigger_raven_alert.run')
 @patch('gwcelery.tasks.gracedb.get_labels', mock_get_labels)
 @patch('gwcelery.tasks.raven.calculate_coincidence_far.run',
        return_value=mock_coinc_far())
-@patch('gwcelery.tasks.gracedb.update_superevent')
 @patch('gwcelery.tasks.gracedb.create_label.run')
-@patch('gwcelery.tasks.external_skymaps.plot_overlap_integral.run')
 @patch('gwcelery.tasks.gracedb.get_superevent', mock_get_superevent)
-def test_raven_pipeline(mock_plot_overlap_integral,
-                        mock_create_label,
-                        mock_update_superevent,
+def test_raven_pipeline(mock_create_label,
                         mock_calculate_coincidence_far,
                         mock_trigger_raven_alert,
                         raven_search_results, graceid, tl, th, group):
     """This function tests that the RAVEN pipeline runs correctly for scenarios
     where RAVEN finds nothing, a coincidence is found but does not pass
     threshold, when a coincidence is found but does pass threshold, and when
     multiple events are found.
     """
     alert_object = {'preferred_event': 'G1', 'pipeline': 'Fermi',
                     'search': 'Supernova' if graceid == 'T4' else 'GRB',
                     'labels': [],
                     'superevent': None if graceid != 'E6' else 'S14'}
-    time_coinc_far = mock_coinc_far()['temporal_coinc_far']
-    space_coinc_far = mock_coinc_far()['spatiotemporal_coinc_far']
 
     for result in raven_search_results:
         result['labels'] = []
     if 'S' not in graceid:
         alert_object['group'] = 'External'
         if 'T' in graceid:
             alert_object['group'] = 'Test'
@@ -287,43 +281,30 @@
         for result in raven_search_results:
             result['superevent'] = None
     raven.raven_pipeline(raven_search_results, graceid, alert_object, tl, th,
                          group)
 
     coinc_calls = []
     label_calls = []
-    update_calls = []
-    plot_calls = []
     if not raven_search_results:
         mock_calculate_coincidence_far.assert_not_called()
         mock_create_label.assert_not_called()
         return
     if 'S' in graceid:
         for result in raven_search_results:
             label_calls.append(call('EM_COINC', result['graceid']))
-            coinc_calls.append(call(alert_object, result, tl, th))
+            coinc_calls.append(call(alert_object, result, tl, th,
+                                    use_superevent_skymap=None))
             label_calls.append(call('EM_COINC', graceid))
-            update_calls.append(
-                call(graceid, em_type=result['graceid'],
-                     time_coinc_far=time_coinc_far,
-                     space_coinc_far=space_coinc_far))
-            plot_calls.append(
-                call(mock_coinc_far(), alert_object, result))
     else:
         result = raven.preferred_superevent(raven_search_results)[0]
         label_calls.append(call('EM_COINC', result['superevent_id']))
-        coinc_calls.append(call(result, alert_object, tl, th))
+        coinc_calls.append(call(result, alert_object, tl, th,
+                                use_superevent_skymap=None))
         label_calls.append(call('EM_COINC', graceid))
-        update_calls.append(
-            call(raven_search_results[-1]['superevent_id'],
-                 em_type=graceid,
-                 time_coinc_far=time_coinc_far,
-                 space_coinc_far=space_coinc_far))
-        plot_calls.append(
-            call(mock_coinc_far(), result, alert_object))
 
     alert_calls = []
     if 'S' in graceid:
         for result in raven_search_results:
             alert_calls.append(call(mock_coinc_far(),
                                     alert_object, graceid, result, group))
     else:
@@ -331,23 +312,19 @@
             mock_coinc_far(),
             result, graceid, alert_object, group))
     if graceid != 'E6':
         mock_trigger_raven_alert.assert_has_calls(alert_calls, any_order=True)
 
         mock_calculate_coincidence_far.assert_has_calls(coinc_calls,
                                                         any_order=True)
-        mock_update_superevent.assert_has_calls(update_calls, any_order=True)
         mock_create_label.assert_has_calls(label_calls, any_order=True)
-        mock_plot_overlap_integral.assert_has_calls(plot_calls, any_order=True)
     else:
         mock_trigger_raven_alert.assert_not_called()
         mock_calculate_coincidence_far.assert_not_called()
-        mock_update_superevent.assert_not_called()
         mock_create_label.assert_not_called()
-        mock_plot_overlap_integral.assert_not_called()
 
 
 @pytest.mark.parametrize(
     'raven_search_results, testnum',
     [[[{'superevent_id': 'S10', 'far': 1, 'preferred_event': 'G1'}], 1],
      [[{'superevent_id': 'S11', 'far': 1, 'preferred_event': 'G2'},
        {'superevent_id': 'S12', 'far': .001, 'preferred_event': 'G3'}], 2],
@@ -583,14 +560,18 @@
     elif graceid == "MS1111":
         return {"temporal_coinc_far": 1e-09,
                 "spatiotemporal_coinc_far": 1e-10}
     else:
         return {}
 
 
+def _return_coinc_far_dict(coinc_far_dict, *args):
+    return coinc_far_dict
+
+
 @pytest.mark.parametrize(
     'graceid,result_id,group,expected_result',
     [['S1234', 'E1', 'Burst', False],
      ['S2468', 'E1', 'CBC', False],
      ['S2468', 'E5', 'CBC', False],
      ['S2468', 'E2', 'CBC', False],
      ['S2345', 'E3', 'Burst', True],
@@ -601,41 +582,53 @@
      ['E1', 'S2468', 'CBC', False],
      ['E2', 'S5678', 'CBC', False],
      ['E3', 'S8642', 'Burst', False],
      ['E3', 'S9876', 'Burst', True],
      ['T4', 'TS1111', 'CBC', False],
      ['E5', 'S5678', 'CBC', False]])
 @patch('gwcelery.tasks.gracedb.get_labels', side_effect=_mock_get_labels)
-@patch('gwcelery.tasks.gracedb.update_superevent')
+@patch('gwcelery.tasks.gracedb.upload.run')
+@patch('gwcelery.tasks.raven.update_coinc_far.run',
+       side_effect=_return_coinc_far_dict)
+@patch('gwcelery.tasks.external_skymaps.plot_overlap_integral.run')
 @patch('gwcelery.tasks.gracedb.create_label.run')
-def test_trigger_raven_alert(mock_create_label, mock_update_superevent,
+def test_trigger_raven_alert(mock_create_label, mock_plot_overlap_integral,
+                             mock_update_coinc_far, mock_upload,
                              mock_get_labels,
                              graceid, result_id, group, expected_result):
     if 'S' in graceid:
         superevent_id = graceid
         ext_id = result_id
     else:
         superevent_id = result_id
         ext_id = graceid
     superevent = _mock_get_event(superevent_id)
+    superevent['labels'] = []
     coinc_far_json = _mock_get_coinc_far(superevent_id)
     ext_event = _mock_get_event(ext_id)
     preferred_id = superevent['preferred_event']
     raven.trigger_raven_alert(coinc_far_json, superevent,
                               graceid, ext_event, group)
 
     if expected_result:
         label_calls = [call('RAVEN_ALERT', superevent_id),
                        call('HIGH_PROFILE', superevent_id),
                        call('RAVEN_ALERT', ext_id),
                        call('RAVEN_ALERT', preferred_id)]
         mock_create_label.assert_has_calls(label_calls)
+        superevent['labels'] += 'RAVEN_ALERT'
     else:
         mock_create_label.assert_not_called()
 
+    mock_update_coinc_far.assert_called_with(
+        coinc_far_json, superevent, ext_event)
+    mock_plot_overlap_integral.assert_called_with(
+        coinc_far_json, superevent, ext_event)
+    mock_upload.assert_called()
+
 
 @pytest.mark.parametrize(
     'se_id,ext_id,expected_result',
     [['S2468', 'E5', True],
      ['S2468', 'E1', True],
      ['S2468', 'E2', False],
      ['S2468', 'M6', True],
```

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_rrt_utils.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_rrt_utils.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_skymaps.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tasks_superevents.py` & `gwcelery-2.1.0/gwcelery/tests/test_tasks_superevents.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,17 @@
     'labels,label,search,alert_type',
     [[['EMBRIGHT_READY', 'PASTRO_READY'], 'EMBRIGHT_READY', 'AllSky',
       'label_added'],
      [['SKYMAP_READY', 'EMBRIGHT_READY', 'PASTRO_READY'], 'SKYMAP_READY',
       'AllSky', 'label_added'],
      [['EMBRIGHT_READY'], 'EMBRIGHT_READY', 'EarlyWarning',
       'label_added'],  # Less-significant EW events are not processed
-     [['EMBRIGHT_READY'], 'EMBRIGHT_READY', 'EarlyWarning', 'new']]
+     [['EMBRIGHT_READY'], 'EMBRIGHT_READY', 'EarlyWarning', 'new'],
+     [[''], '', 'SSM', 'new'],
+     [['PASTRO_READY'], '', 'SSM', 'label_added']]
 )
 def test_process_called(labels, label, search, alert_type):
     """Test whether the :meth:`superevents.process` is called
     new type IGWN alerts, and label additions that complete the event.
     """
     payload = {
         "alert_type": alert_type,
@@ -324,15 +326,16 @@
             "pipeline": "pipeline",
             "search": search,
             "labels": labels
         }
     }
     with patch('gwcelery.tasks.superevents.process.run') as process:
         superevents.handle(payload)
-        if search == superevents.EARLY_WARNING_SEARCH_NAME:
+        if search == superevents.EARLY_WARNING_SEARCH_NAME or \
+                search == superevents.SUBSOLAR_SEARCH_NAME:
             process.assert_not_called()
         elif superevents.is_complete(payload['object']):
             process.assert_called()
         else:
             process.assert_not_called()
```

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tempfile.py` & `gwcelery-2.1.0/gwcelery/tests/test_tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tools_condor.py` & `gwcelery-2.1.0/gwcelery/tests/test_tools_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tools_condor_submit_helper.py` & `gwcelery-2.1.0/gwcelery/tests/test_tools_condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tools_flask.py` & `gwcelery-2.1.0/gwcelery/tests/test_tools_flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_tools_nagios.py` & `gwcelery-2.1.0/gwcelery/tests/test_tools_nagios.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 @pytest.fixture
 def celery_worker_parameters():
     return dict(
         perform_ping_check=False,
         queues=['celery', 'exttrig', 'kafka', 'multiprocessing', 'openmp',
-                'superevent', 'voevent']
+                'superevent', 'voevent', 'skynet']
     )
 
 
 def test_nagios(capsys, monkeypatch, request, socket_enabled, starter,
                 tmp_path):
     mock_igwn_alert_client = Mock()
     mock_hop_stream_object = Mock()
```

### Comparing `gwcelery-2.0.6/gwcelery/tests/test_views.py` & `gwcelery-2.1.0/gwcelery/tests/test_views.py`

 * *Files 3% similar despite different names*

```diff
@@ -338,14 +338,36 @@
         'raven': raven})
 
     assert HTTP_STATUS_CODES[response.status_code] == 'OK'
     mock_create_circular.assert_called_once_with(
         'MS190208a', update_types=answer)
 
 
+@patch('gwcelery.tasks.circulars.create_medium_latency_circular',
+       return_value='')
+def test_send_medium_latency_gcn_circular_post(mock_create_circular,
+                                               client):
+    """Test send_medium_latency_gcn_circular endpoint with complete form
+    data."""
+    response = client.post(url_for('create_medium_latency_gcn_circular'),
+                           data={'ext_event_id': 'E12345'})
+
+    assert HTTP_STATUS_CODES[response.status_code] == 'OK'
+    mock_create_circular.assert_called_once_with('E12345')
+
+
+def test_send_medium_latency_gcn_circular_post_no_data(client):
+    """Test send_medium_latency_gcn_circular endpoint with no form
+    data."""
+    response = client.post(url_for('create_medium_latency_gcn_circular'))
+    assert HTTP_STATUS_CODES[response.status_code] == 'Found'
+    assert get_flashed_messages() == [
+        'No circular created. Please fill in external event ID']
+
+
 def test_typeahead_superevent_id(client, monkeypatch):
     """Test typeahead filtering for superevent_id."""
     mock_superevents = Mock(return_value=(
         {
             'superevent_id': (
                 datetime.date(2019, 2, 1) + datetime.timedelta(i)
             ).strftime('MS%y%m%da')
```

### Comparing `gwcelery-2.0.6/gwcelery/tools/condor.py` & `gwcelery-2.1.0/gwcelery/tools/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tools/condor_submit_helper.py` & `gwcelery-2.1.0/gwcelery/tools/condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tools/flask.py` & `gwcelery-2.1.0/gwcelery/tools/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/tools/nagios.py` & `gwcelery-2.1.0/gwcelery/tools/nagios.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/util/cmdline.py` & `gwcelery-2.1.0/gwcelery/util/cmdline.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/util/resources.py` & `gwcelery-2.1.0/gwcelery/util/resources.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/util/tempfile.py` & `gwcelery-2.1.0/gwcelery/util/tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/views.py` & `gwcelery-2.1.0/gwcelery/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,15 +251,15 @@
         except HTTPError as e:
             flash(f'No change performed. GraceDB query for {superevent_id} '
                   f'returned error code {e.response.status_code}.', 'danger')
             return redirect(url_for('index'))
         (
             gracedb.upload.s(
                 None, None, superevent_id,
-                'User {} queued a preferred event change to {}.'
+                celery_app.conf['views_manual_preferred_event_log_message']
                 .format(request.remote_user or '(unknown)', event_id),
                 tags=['em_follow'])
             |
             gracedb.update_superevent.si(
                 superevent_id, preferred_event=event_id)
             |
             _construct_igwn_alert_and_send_prelim_alert.si(
@@ -373,14 +373,29 @@
         ).delay()
         flash('Queued update alert for {}.'.format(superevent_id), 'success')
     else:
         flash('No alert sent. Please fill in all fields.', 'danger')
     return redirect(url_for('index'))
 
 
+@app.route('/create_medium_latency_gcn_circular', methods=['POST'])
+def create_medium_latency_gcn_circular():
+    """Handle submission of medium_latency GCN Circular form."""
+    ext_event_id = request.form.get('ext_event_id')
+    if ext_event_id:
+        response = make_response(circulars.create_medium_latency_circular(
+            ext_event_id))
+        response.headers["content-type"] = "text/plain"
+        return response
+    else:
+        flash('No circular created. Please fill in external event ID',
+              'danger')
+    return redirect(url_for('index'))
+
+
 @app.route('/create_update_gcn_circular', methods=['POST'])
 def create_update_gcn_circular():
     """Handle submission of GCN Circular form."""
     keys = ['sky_localization', 'em_bright', 'p_astro', 'raven']
     superevent_id = request.form.get('superevent_id')
     updates = [key for key in keys if request.form.get(key)]
     if superevent_id and updates:
```

### Comparing `gwcelery-2.0.6/gwcelery/voevent/bootsteps.py` & `gwcelery-2.1.0/gwcelery/voevent/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/voevent/logging.py` & `gwcelery-2.1.0/gwcelery/voevent/logging.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/voevent/signals.py` & `gwcelery-2.1.0/gwcelery/voevent/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/voevent/subscriber.py` & `gwcelery-2.1.0/gwcelery/voevent/subscriber.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/gwcelery/voevent/util.py` & `gwcelery-2.1.0/gwcelery/voevent/util.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.6/pyproject.toml` & `gwcelery-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwcelery"
-version = "2.0.6"
+version = "2.1.0"
 description = "Low-latency pipeline for annotating IGWN events"
 readme = "README.rst"
 authors = [
     "Deep Chatterjee <deep.chatterjee@ligo.org>",
     "Cody Messick <cody.messick@ligo.org>",
     "Geoffrey Mo <geoffrey.mo@ligo.org>",
     "Leo Singer <leo.singer@ligo.org>"
@@ -49,53 +49,54 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://git.ligo.org/emfollow/gwcelery/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
 adc-streaming = ">=2.3.0"  # https://github.com/astronomy-commons/adc-streaming/pull/62
 astropy = ">=4.3.1"  # https://github.com/astropy/astropy/issues/11879
-bilby = ">=2.1.0"
-bilby_pipe = ">=1.0.10"
+bilby = ">=2.1.1"
+bilby_pipe = "==1.0.10"
 celery = {version = ">=5.1", extras = ["redis"]}
 ciecplib = {version = "*", extras = ["kerberos"]}  # for renew-cert.sh
 click = ">=7"
 comet = "*"
 confluent-kafka = "^1.9.2"
 dnspython = "*"  # silence "DNS: dnspython not found. Can not use SRV lookup." warning from SleekXMPP
 flask = ">=2.2"
 flask-caching = "*"
 gracedb-sdk = ">=0.2.0"  # https://git.ligo.org/emfollow/gracedb-sdk/-/merge_requests/7
 gwdatafind = ">=1.1.1"
 gwpy = ">=2.0.1"  # https://github.com/gwpy/gwpy/issues/1277
+GWSkyNet = ">=2.3.0" # https://git.ligo.org/computing/sccb/-/issues/1153
 healpy = "*"
 hop-client = ">=0.7.0"  # https://github.com/scimma/hop-client/pull/176
 igwn-alert = ">=0.2.2"
 igwn-gwalert-schema = "^1.0.0"
 imapclient = "*"
 importlib-metadata = { version = "*"}
 jinja2 = ">=2.11.2"  # https://github.com/pallets/jinja/issues/1168
 lalsuite = ">=6.82"  # https://git.ligo.org/lscsoft/lalsuite/-/issues/414
-ligo-followup-advocate = ">=1.2.1"
+ligo-followup-advocate = ">=1.2.2"
 ligo-gracedb = ">=2.7.5"  # https://git.ligo.org/lscsoft/gracedb-client/-/issues/28
-ligo-raven = ">=3.1"
+ligo-raven = ">=3.2"
 ligo-segments = "*"
 "ligo.em-bright" = ">=1.1.2"  # https://git.ligo.org/computing/sccb/-/issues/1166
 "ligo.skymap" = ">=1.0.4"  # https://git.ligo.org/lscsoft/ligo.skymap/-/merge_requests/299
 lscsoft-glue = "*"
 lxml = "*"
 matplotlib = "<3.7"  # Matplotlib changed an axes behaviour which breaks some of our plotting scripts. When gwpy has a new release, we can unpin this.
 numba = ">=0.56"  # Poetry update chooses an old version of numba and its deps that break the python3.9 and 3.10 build tests if this is not specified; dependence on numba comes from rift. Version chosen because it adds python 3.10 support. This requirement can be dropped here if RIFT adds it https://git.ligo.org/rapidpe-rift/rift/-/issues/24
 numpy = "*"
 p_astro = ">=1.0.1"  # https://git.ligo.org/lscsoft/p-astro/-/merge_requests/40
 pesummary = ">=1.0.0"  # https://git.ligo.org/computing/sccb/-/issues/1182
 pygcn = ">=1.0.1"
 python-ligo-lw = "^1.8.3"
 pyxdg = "*"
-rapid-pe = ">=0.0.6"  # https://git.ligo.org/computing/sccb/-/issues/1154
-rapidpe-rift-pipe = ">=0.0.12"  # https://git.ligo.org/computing/sccb/-/issues/1155
+rapid-pe = ">=0.1.0,<0.2.0"  # https://git.ligo.org/computing/sccb/-/issues/1154
+rapidpe-rift-pipe = ">=0.3.0"  # https://git.ligo.org/computing/sccb/-/issues/1214
 redis = "!=4.5.2,!=4.5.3"  # https://git.ligo.org/emfollow/gwcelery/-/issues/556
 RIFT = ">=0.0.15.7"
 scipy = "<1.10"  # https://github.com/astropy/astropy/issues/14230
 safe-netrc = "*"
 sentry-sdk = {version = "*", extras = ["flask", "tornado"]}
 service-identity = "*"  # We don't actually use this package, but it silences some annoying warnings from twistd.
 voeventlib = ">=1.2"
```

### Comparing `gwcelery-2.0.6/PKG-INFO` & `gwcelery-2.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: gwcelery
-Version: 2.0.6
+Version: 2.1.0
 Summary: Low-latency pipeline for annotating IGWN events
 Home-page: https://git.ligo.org/emfollow/gwcelery
 License: GPL-2.0+
 Author: Deep Chatterjee
 Author-email: deep.chatterjee@ligo.org
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: doc
 Provides-Extra: test
+Requires-Dist: GWSkyNet (>=2.3.0)
 Requires-Dist: RIFT (>=0.0.15.7)
 Requires-Dist: adc-streaming (>=2.3.0)
 Requires-Dist: astropy (>=4.3.1)
-Requires-Dist: bilby (>=2.1.0)
-Requires-Dist: bilby_pipe (>=1.0.10)
+Requires-Dist: bilby (>=2.1.1)
+Requires-Dist: bilby_pipe (==1.0.10)
 Requires-Dist: celery[redis] (>=5.1)
 Requires-Dist: ciecplib[kerberos]
 Requires-Dist: click (>=7)
 Requires-Dist: comet
 Requires-Dist: confluent-kafka (>=1.9.2,<2.0.0)
 Requires-Dist: dnspython
 Requires-Dist: fastavro (>=1.6.1,<2.0.0) ; extra == "test"
@@ -44,17 +42,17 @@
 Requires-Dist: hop-client (>=0.7.0)
 Requires-Dist: igwn-alert (>=0.2.2)
 Requires-Dist: igwn-gwalert-schema (>=1.0.0,<2.0.0)
 Requires-Dist: imapclient
 Requires-Dist: importlib-metadata
 Requires-Dist: jinja2 (>=2.11.2)
 Requires-Dist: lalsuite (>=6.82)
-Requires-Dist: ligo-followup-advocate (>=1.2.1)
+Requires-Dist: ligo-followup-advocate (>=1.2.2)
 Requires-Dist: ligo-gracedb (>=2.7.5)
-Requires-Dist: ligo-raven (>=3.1)
+Requires-Dist: ligo-raven (>=3.2)
 Requires-Dist: ligo-rrt-chat (>=0.1.1)
 Requires-Dist: ligo-segments
 Requires-Dist: ligo.em-bright (>=1.1.2)
 Requires-Dist: ligo.skymap (>=1.0.4)
 Requires-Dist: lscsoft-glue
 Requires-Dist: lxml
 Requires-Dist: matplotlib (<3.7)
@@ -66,16 +64,16 @@
 Requires-Dist: pygcn (>=1.0.1)
 Requires-Dist: pytest-celery ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-flask ; extra == "test"
 Requires-Dist: pytest-socket ; extra == "test"
 Requires-Dist: python-ligo-lw (>=1.8.3,<2.0.0)
 Requires-Dist: pyxdg
-Requires-Dist: rapid-pe (>=0.0.6)
-Requires-Dist: rapidpe-rift-pipe (>=0.0.12)
+Requires-Dist: rapid-pe (>=0.1.0,<0.2.0)
+Requires-Dist: rapidpe-rift-pipe (>=0.3.0)
 Requires-Dist: redis (!=4.5.2,!=4.5.3)
 Requires-Dist: safe-netrc
 Requires-Dist: scipy (<1.10)
 Requires-Dist: sentry-sdk[flask,tornado]
 Requires-Dist: service-identity
 Requires-Dist: sphinx (>=4.0,<=5.3.0) ; extra == "doc"
 Requires-Dist: voeventlib (>=1.2)
```

