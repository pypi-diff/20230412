# Comparing `tmp/evase-analysis-1.0.8.4.tar.gz` & `tmp/evase-analysis-1.0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evase-analysis-1.0.8.4.tar", last modified: Mon Apr 10 20:18:01 2023, max compression
+gzip compressed data, was "evase-analysis-1.0.8.5.tar", last modified: Wed Apr 12 20:35:14 2023, max compression
```

## Comparing `evase-analysis-1.0.8.4.tar` & `evase-analysis-1.0.8.5.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.534396 evase-analysis-1.0.8.4/
--rw-rw-rw-   0        0        0     7073 2023-04-10 20:18:01.534396 evase-analysis-1.0.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     6230 2023-04-04 20:11:33.000000 evase-analysis-1.0.8.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.466239 evase-analysis-1.0.8.4/docs/
--rw-rw-rw-   0        0        0     1166 2023-04-10 18:09:48.000000 evase-analysis-1.0.8.4/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.467240 evase-analysis-1.0.8.4/evase/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/evase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.471239 evase-analysis-1.0.8.4/evase/depanalyze/
--rw-rw-rw-   0        0        0        0 2023-04-10 01:10:48.000000 evase-analysis-1.0.8.4/evase/depanalyze/__init__.py
--rw-rw-rw-   0        0        0     9152 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.4/evase/depanalyze/codetraversalnode.py
--rw-rw-rw-   0        0        0    12059 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.4/evase/depanalyze/importresolver.py
--rw-rw-rw-   0        0        0     3829 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.4/evase/depanalyze/scoperesolver.py
--rw-rw-rw-   0        0        0    15873 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.4/evase/depanalyze/searching.py
--rw-rw-rw-   0        0        0     1450 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.4/evase/depanalyze/surfacedetector.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.471745 evase-analysis-1.0.8.4/evase/exceptions/
--rw-rw-rw-   0        0        0        0 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.4/evase/exceptions/__init__.py
--rw-rw-rw-   0        0        0      626 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.4/evase/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.473758 evase-analysis-1.0.8.4/evase/sql_injection/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/evase/sql_injection/__init__.py
--rw-rw-rw-   0        0        0     4242 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/evase/sql_injection/injectionutil.py
--rw-rw-rw-   0        0        0     6537 2023-04-06 19:27:17.000000 evase-analysis-1.0.8.4/evase/sql_injection/injectionvisitor.py
--rw-rw-rw-   0        0        0    10947 2023-04-06 19:27:17.000000 evase-analysis-1.0.8.4/evase/sql_injection/vulnerabletraversal.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.475758 evase-analysis-1.0.8.4/evase/structures/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/evase/structures/__init__.py
--rw-rw-rw-   0        0        0    14911 2023-04-10 20:13:56.000000 evase-analysis-1.0.8.4/evase/structures/analysisperformer.py
--rw-rw-rw-   0        0        0     5410 2023-04-10 18:09:51.000000 evase-analysis-1.0.8.4/evase/structures/modulestructure.py
--rw-rw-rw-   0        0        0     6608 2023-04-10 18:09:51.000000 evase-analysis-1.0.8.4/evase/structures/projectstructure.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.477758 evase-analysis-1.0.8.4/evase/util/
--rw-rw-rw-   0        0        0        0 2023-03-30 01:19:57.000000 evase-analysis-1.0.8.4/evase/util/__init__.py
--rw-rw-rw-   0        0        0     3012 2023-04-06 19:27:17.000000 evase-analysis-1.0.8.4/evase/util/fileutil.py
--rw-rw-rw-   0        0        0     1411 2023-04-06 19:27:20.000000 evase-analysis-1.0.8.4/evase/util/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.492798 evase-analysis-1.0.8.4/evase_analysis.egg-info/
--rw-rw-rw-   0        0        0     7073 2023-04-10 20:18:01.000000 evase-analysis-1.0.8.4/evase_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2685 2023-04-10 20:18:01.000000 evase-analysis-1.0.8.4/evase_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 20:18:01.000000 evase-analysis-1.0.8.4/evase_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-10 20:18:01.000000 evase-analysis-1.0.8.4/evase_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-10 20:18:01.000000 evase-analysis-1.0.8.4/evase_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1345 2023-04-10 20:15:15.000000 evase-analysis-1.0.8.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 20:18:01.534396 evase-analysis-1.0.8.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.513347 evase-analysis-1.0.8.4/tests/
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.518356 evase-analysis-1.0.8.4/tests/resources/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.463231 evase-analysis-1.0.8.4/tests/resources/demo/
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.521860 evase-analysis-1.0.8.4/tests/resources/demo/backend/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/demo/backend/__init__.py
--rw-rw-rw-   0        0        0     1108 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/demo/backend/app.py
--rw-rw-rw-   0        0        0     1098 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/demo/backend/vul.py
--rw-rw-rw-   0        0        0     1140 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/demo/backend/vul_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.462231 evase-analysis-1.0.8.4/tests/resources/demo2/
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.520355 evase-analysis-1.0.8.4/tests/resources/demo2/demonstration/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/demo2/demonstration/__init__.py
--rw-rw-rw-   0        0        0      185 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/demo2/demonstration/api.py
--rw-rw-rw-   0        0        0      183 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/demo2/demonstration/controller.py
--rw-rw-rw-   0        0        0      458 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/demo2/demonstration/model.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.522869 evase-analysis-1.0.8.4/tests/resources/prjstructtest/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/prjstructtest/__init__.py
--rw-rw-rw-   0        0        0      290 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/prjstructtest/runner.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.523877 evase-analysis-1.0.8.4/tests/resources/prjstructtest/test/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/prjstructtest/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.524875 evase-analysis-1.0.8.4/tests/resources/prjstructtest/util/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/prjstructtest/util/__init__.py
--rw-rw-rw-   0        0        0      163 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/prjstructtest/util/helper.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.525876 evase-analysis-1.0.8.4/tests/resources/prjstructtest/util/moreutil/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/prjstructtest/util/moreutil/__init__.py
--rw-rw-rw-   0        0        0       79 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/prjstructtest/util/moreutil/helper2.py
--rw-rw-rw-   0        0        0      306 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/screstest.py
--rw-rw-rw-   0        0        0      108 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_safe1.py
--rw-rw-rw-   0        0        0      150 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_safe2.py
--rw-rw-rw-   0        0        0      128 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_vul1.py
--rw-rw-rw-   0        0        0      122 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_vul2.py
--rw-rw-rw-   0        0        0      130 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_vul3.py
--rw-rw-rw-   0        0        0      122 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_vul4.py
--rw-rw-rw-   0        0        0      535 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_vul5.py
--rw-rw-rw-   0        0        0     5135 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/sql_injection_vul6.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.527876 evase-analysis-1.0.8.4/tests/resources/type_demo/
--rw-rw-rw-   0        0        0      911 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/type_demo/app.py
--rw-rw-rw-   0        0        0      280 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/type_demo/create_db.py
--rw-rw-rw-   0        0        0      759 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/type_demo/user_db_handler.py
--rw-rw-rw-   0        0        0      700 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/type_demo/vul.py
--rw-rw-rw-   0        0        0      732 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.4/tests/resources/type_demo/vul_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.464237 evase-analysis-1.0.8.4/tests/resources/webgoat/
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.532391 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/
--rw-rw-rw-   0        0        0     1534 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/__init__.py
--rw-rw-rw-   0        0        0     2063 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/actions.py
--rw-rw-rw-   0        0        0     1633 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/auth.py
--rw-rw-rw-   0        0        0      232 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/status.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:18:01.533390 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/templates/
--rw-rw-rw-   0        0        0       89 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/templates/__init__.py
--rw-rw-rw-   0        0        0       32 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/templates/hello.py
--rw-rw-rw-   0        0        0       77 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/templates/helper.py
--rw-rw-rw-   0        0        0      850 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/ui.py
--rw-rw-rw-   0        0        0     1488 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/users.py
--rw-rw-rw-   0        0        0     2172 2023-04-10 20:14:52.000000 evase-analysis-1.0.8.4/tests/test_analysisperformer.py
--rw-rw-rw-   0        0        0     2593 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.4/tests/test_fileutil.py
--rw-rw-rw-   0        0        0     1618 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.4/tests/test_projectstructure.py
--rw-rw-rw-   0        0        0     1639 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.4/tests/test_scoperesolver.py
--rw-rw-rw-   0        0        0     1714 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.4/tests/testutil.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.609722 evase-analysis-1.0.8.5/
+-rw-rw-rw-   0        0        0     7073 2023-04-12 20:35:14.608723 evase-analysis-1.0.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6230 2023-04-04 20:11:33.000000 evase-analysis-1.0.8.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.302145 evase-analysis-1.0.8.5/docs/
+-rw-rw-rw-   0        0        0     1166 2023-04-10 18:09:48.000000 evase-analysis-1.0.8.5/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.303154 evase-analysis-1.0.8.5/evase/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/evase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.335716 evase-analysis-1.0.8.5/evase/depanalyze/
+-rw-rw-rw-   0        0        0        0 2023-04-10 01:10:48.000000 evase-analysis-1.0.8.5/evase/depanalyze/__init__.py
+-rw-rw-rw-   0        0        0     9152 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.5/evase/depanalyze/codetraversalnode.py
+-rw-rw-rw-   0        0        0    12059 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.5/evase/depanalyze/importresolver.py
+-rw-rw-rw-   0        0        0     3829 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.5/evase/depanalyze/scoperesolver.py
+-rw-rw-rw-   0        0        0    15873 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.5/evase/depanalyze/searching.py
+-rw-rw-rw-   0        0        0     1450 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.5/evase/depanalyze/surfacedetector.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.340714 evase-analysis-1.0.8.5/evase/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-04-04 19:22:58.000000 evase-analysis-1.0.8.5/evase/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-04-12 03:31:02.000000 evase-analysis-1.0.8.5/evase/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.360745 evase-analysis-1.0.8.5/evase/sql_injection/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/evase/sql_injection/__init__.py
+-rw-rw-rw-   0        0        0     4499 2023-04-11 23:23:28.000000 evase-analysis-1.0.8.5/evase/sql_injection/injectionutil.py
+-rw-rw-rw-   0        0        0     6537 2023-04-06 19:27:17.000000 evase-analysis-1.0.8.5/evase/sql_injection/injectionvisitor.py
+-rw-rw-rw-   0        0        0    10947 2023-04-06 19:27:17.000000 evase-analysis-1.0.8.5/evase/sql_injection/vulnerabletraversal.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.379783 evase-analysis-1.0.8.5/evase/structures/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/evase/structures/__init__.py
+-rw-rw-rw-   0        0        0    14911 2023-04-10 20:13:56.000000 evase-analysis-1.0.8.5/evase/structures/analysisperformer.py
+-rw-rw-rw-   0        0        0     5410 2023-04-10 18:09:51.000000 evase-analysis-1.0.8.5/evase/structures/modulestructure.py
+-rw-rw-rw-   0        0        0     6608 2023-04-10 18:09:51.000000 evase-analysis-1.0.8.5/evase/structures/projectstructure.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.392300 evase-analysis-1.0.8.5/evase/util/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:19:57.000000 evase-analysis-1.0.8.5/evase/util/__init__.py
+-rw-rw-rw-   0        0        0     3012 2023-04-06 19:27:17.000000 evase-analysis-1.0.8.5/evase/util/fileutil.py
+-rw-rw-rw-   0        0        0     1411 2023-04-06 19:27:20.000000 evase-analysis-1.0.8.5/evase/util/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.407346 evase-analysis-1.0.8.5/evase_analysis.egg-info/
+-rw-rw-rw-   0        0        0     7073 2023-04-12 20:35:14.000000 evase-analysis-1.0.8.5/evase_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2685 2023-04-12 20:35:14.000000 evase-analysis-1.0.8.5/evase_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 20:35:14.000000 evase-analysis-1.0.8.5/evase_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-12 20:35:14.000000 evase-analysis-1.0.8.5/evase_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-04-12 20:35:14.000000 evase-analysis-1.0.8.5/evase_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1345 2023-04-11 23:23:48.000000 evase-analysis-1.0.8.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 20:35:14.609722 evase-analysis-1.0.8.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.434403 evase-analysis-1.0.8.5/tests/
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.487012 evase-analysis-1.0.8.5/tests/resources/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.292625 evase-analysis-1.0.8.5/tests/resources/demo/
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.519556 evase-analysis-1.0.8.5/tests/resources/demo/backend/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/demo/backend/__init__.py
+-rw-rw-rw-   0        0        0     1108 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.5/tests/resources/demo/backend/app.py
+-rw-rw-rw-   0        0        0     1098 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/demo/backend/vul.py
+-rw-rw-rw-   0        0        0     1140 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.5/tests/resources/demo/backend/vul_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.292625 evase-analysis-1.0.8.5/tests/resources/demo2/
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.502030 evase-analysis-1.0.8.5/tests/resources/demo2/demonstration/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/demo2/demonstration/__init__.py
+-rw-rw-rw-   0        0        0      185 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/demo2/demonstration/api.py
+-rw-rw-rw-   0        0        0      183 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/demo2/demonstration/controller.py
+-rw-rw-rw-   0        0        0      458 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/demo2/demonstration/model.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.526588 evase-analysis-1.0.8.5/tests/resources/prjstructtest/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/prjstructtest/__init__.py
+-rw-rw-rw-   0        0        0      290 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/prjstructtest/runner.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.526588 evase-analysis-1.0.8.5/tests/resources/prjstructtest/test/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/prjstructtest/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.532097 evase-analysis-1.0.8.5/tests/resources/prjstructtest/util/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/prjstructtest/util/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/prjstructtest/util/helper.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.537110 evase-analysis-1.0.8.5/tests/resources/prjstructtest/util/moreutil/
+-rw-rw-rw-   0        0        0        0 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/prjstructtest/util/moreutil/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/prjstructtest/util/moreutil/helper2.py
+-rw-rw-rw-   0        0        0      306 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/screstest.py
+-rw-rw-rw-   0        0        0      108 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/sql_injection_safe1.py
+-rw-rw-rw-   0        0        0      150 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/sql_injection_safe2.py
+-rw-rw-rw-   0        0        0      128 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/sql_injection_vul1.py
+-rw-rw-rw-   0        0        0      122 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/sql_injection_vul2.py
+-rw-rw-rw-   0        0        0      130 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/sql_injection_vul3.py
+-rw-rw-rw-   0        0        0      122 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/sql_injection_vul4.py
+-rw-rw-rw-   0        0        0      535 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/sql_injection_vul5.py
+-rw-rw-rw-   0        0        0     5135 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/sql_injection_vul6.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.562142 evase-analysis-1.0.8.5/tests/resources/type_demo/
+-rw-rw-rw-   0        0        0      911 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/type_demo/app.py
+-rw-rw-rw-   0        0        0      280 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/type_demo/create_db.py
+-rw-rw-rw-   0        0        0      759 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/type_demo/user_db_handler.py
+-rw-rw-rw-   0        0        0      700 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/type_demo/vul.py
+-rw-rw-rw-   0        0        0      732 2023-03-27 20:42:02.000000 evase-analysis-1.0.8.5/tests/resources/type_demo/vul_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.294638 evase-analysis-1.0.8.5/tests/resources/webgoat/
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.595210 evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/
+-rw-rw-rw-   0        0        0     1534 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/__init__.py
+-rw-rw-rw-   0        0        0     2063 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/actions.py
+-rw-rw-rw-   0        0        0     1633 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/auth.py
+-rw-rw-rw-   0        0        0      232 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/status.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:35:14.607722 evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/templates/
+-rw-rw-rw-   0        0        0       89 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/templates/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/templates/hello.py
+-rw-rw-rw-   0        0        0       77 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/templates/helper.py
+-rw-rw-rw-   0        0        0      850 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/ui.py
+-rw-rw-rw-   0        0        0     1488 2023-03-30 01:20:00.000000 evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/users.py
+-rw-rw-rw-   0        0        0     2172 2023-04-10 20:14:52.000000 evase-analysis-1.0.8.5/tests/test_analysisperformer.py
+-rw-rw-rw-   0        0        0     2593 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.5/tests/test_fileutil.py
+-rw-rw-rw-   0        0        0     1618 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.5/tests/test_projectstructure.py
+-rw-rw-rw-   0        0        0     1639 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.5/tests/test_scoperesolver.py
+-rw-rw-rw-   0        0        0     1714 2023-04-04 20:06:40.000000 evase-analysis-1.0.8.5/tests/testutil.py
```

### Comparing `evase-analysis-1.0.8.4/PKG-INFO` & `evase-analysis-1.0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evase-analysis
-Version: 1.0.8.4
+Version: 1.0.8.5
 Summary: A Python package with tools for the detection of SQL injection vulnerabilities in projects.
 Author-email: Tony Abou Zeidan <tony.azp25@gmail.com>, Anthony Dooley <anthonydooley@cmail.carleton.ca>, Ethan Chase <e281828c@gmail.com>, Shaopeng Liu <shaopengliu@cmail.carleton.ca>, Jason Jaskolka <jason.jaskolka@carleton.ca>
 Maintainer-email: Tony Abou Zeidan <tony.azp25@gmail.com>, Anthony Dooley <anthonydooley@cmail.carleton.ca>, Ethan Chase <e281828c@gmail.com>, Shaopeng Liu <shaopengliu@cmail.carleton.ca>, Jason Jaskolka <jason.jaskolka@carleton.ca>
 Keywords: attack,security,SQL,injection
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `evase-analysis-1.0.8.4/README.md` & `evase-analysis-1.0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/docs/conf.py` & `evase-analysis-1.0.8.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/evase/depanalyze/codetraversalnode.py` & `evase-analysis-1.0.8.5/evase/depanalyze/codetraversalnode.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/evase/depanalyze/importresolver.py` & `evase-analysis-1.0.8.5/evase/depanalyze/importresolver.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/evase/depanalyze/scoperesolver.py` & `evase-analysis-1.0.8.5/evase/depanalyze/scoperesolver.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/evase/depanalyze/searching.py` & `evase-analysis-1.0.8.5/evase/depanalyze/searching.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/evase/depanalyze/surfacedetector.py` & `evase-analysis-1.0.8.5/evase/depanalyze/surfacedetector.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/evase/exceptions/exceptions.py` & `evase-analysis-1.0.8.5/evase/exceptions/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from pathlib import Path
 from typing import Union
 
 
-
-
-
 class EvasePathException(Exception):
 
     def __init__(self, path: Union[str, Path], message: str = None):
         """
         Custom exception to display cases where Evase fails due to processing files incorrectly
         or where paths are passed incorrectly.
```

### Comparing `evase-analysis-1.0.8.4/evase/sql_injection/injectionutil.py` & `evase-analysis-1.0.8.5/evase/sql_injection/injectionutil.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     # base case 1, stop when the parameter has an ID
     if hasattr(node, "id"):
         args.add(node.id)
     elif isinstance(node, ast.Call):
         if isinstance(node.func, ast.Attribute):
             if node.func.attr == "replace" and len(node.args) == 2 and node.args[0].value == ";" and not node.args[
-                                                                                         1].value == ";":
+                                                                                                             1].value == ";":
                 return args
 
         # resolveCall(node)
     elif hasattr(node, "elts"):
         for subarg in node.elts:
             for subsubarg in get_all_vars(subarg):
                 args.add(subsubarg)
@@ -73,15 +73,14 @@
             args.add(r_subarg)
 
     elif isinstance(node, ast.JoinedStr):
         for value in node.values:
             for subarg in get_all_vars(value):
                 args.add(subarg)
 
-
     elif isinstance(node, ast.FormattedValue):
         for subargs in get_all_vars(node.value):
             args.add(subargs)
 
     elif hasattr(node, "args"):
         args.add(node)
         # for arg in node.args:
@@ -91,15 +90,15 @@
     elif hasattr(node, "value"):
         for subarg in get_all_vars(node.value):
             args.add(subarg)
 
     return args
 
 
-def get_all_target_values(node: ast.Assign) -> list:
+def get_all_target_values(node: ast.Assign) -> tuple:
     """
     Gets the variables used in the assignment of each target.
 
     :param node: The assignment node
     :return: The list of values for each target, empty set signifies no variables
     """
     val_lst = []  # collect all variables mentioned for each assignment
@@ -110,15 +109,23 @@
             val_lst.append(set())
     except AttributeError:
         val_lst.append(get_all_vars(node.value))
 
     return val_lst, 0
 
 
-def get_inner_scope_assignments(index, assignments):
+def get_inner_scope_assignments(index, assignments) -> tuple:
+    """
+    Helper function for the obtaining of the assignment nodes in an inner scope.
+
+    :param index: Indexer
+    :param assignments: Previous assignment nodes
+    :return: New indexer, and new assignments
+    """
+
     stack = ["end" + assignments[index]]
     index += 1
     inner_assignments = [[]]
     assignment_ind = 0
 
     while len(stack) != 0 and index < len(assignments):
```

### Comparing `evase-analysis-1.0.8.4/evase/sql_injection/injectionvisitor.py` & `evase-analysis-1.0.8.5/evase/sql_injection/injectionvisitor.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/evase/sql_injection/vulnerabletraversal.py` & `evase-analysis-1.0.8.5/evase/sql_injection/vulnerabletraversal.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/evase/structures/analysisperformer.py` & `evase-analysis-1.0.8.5/evase/structures/analysisperformer.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/evase/structures/modulestructure.py` & `evase-analysis-1.0.8.5/evase/structures/modulestructure.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/evase/structures/projectstructure.py` & `evase-analysis-1.0.8.5/evase/structures/projectstructure.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/evase/util/fileutil.py` & `evase-analysis-1.0.8.5/evase/util/fileutil.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/evase/util/logger.py` & `evase-analysis-1.0.8.5/evase/util/logger.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/evase_analysis.egg-info/PKG-INFO` & `evase-analysis-1.0.8.5/evase_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evase-analysis
-Version: 1.0.8.4
+Version: 1.0.8.5
 Summary: A Python package with tools for the detection of SQL injection vulnerabilities in projects.
 Author-email: Tony Abou Zeidan <tony.azp25@gmail.com>, Anthony Dooley <anthonydooley@cmail.carleton.ca>, Ethan Chase <e281828c@gmail.com>, Shaopeng Liu <shaopengliu@cmail.carleton.ca>, Jason Jaskolka <jason.jaskolka@carleton.ca>
 Maintainer-email: Tony Abou Zeidan <tony.azp25@gmail.com>, Anthony Dooley <anthonydooley@cmail.carleton.ca>, Ethan Chase <e281828c@gmail.com>, Shaopeng Liu <shaopengliu@cmail.carleton.ca>, Jason Jaskolka <jason.jaskolka@carleton.ca>
 Keywords: attack,security,SQL,injection
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `evase-analysis-1.0.8.4/evase_analysis.egg-info/SOURCES.txt` & `evase-analysis-1.0.8.5/evase_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/pyproject.toml` & `evase-analysis-1.0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     {name = "Shaopeng Liu", email="shaopengliu@cmail.carleton.ca"},
     {name = "Jason Jaskolka", email="jason.jaskolka@carleton.ca"}
 ]
 description = "A Python package with tools for the detection of SQL injection vulnerabilities in projects."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["attack", "security", "SQL", "injection"]
-version="1.0.8.4"
+version="1.0.8.5"
 classifiers=[
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3"
 ]
 dependencies = [
     'Flask~=2.2.2',
     'Jinja2~=3.1.2',
```

### Comparing `evase-analysis-1.0.8.4/tests/resources/demo/backend/app.py` & `evase-analysis-1.0.8.5/tests/resources/demo/backend/app.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/resources/demo/backend/vul.py` & `evase-analysis-1.0.8.5/tests/resources/demo/backend/vul.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/resources/demo/backend/vul_wrapper.py` & `evase-analysis-1.0.8.5/tests/resources/demo/backend/vul_wrapper.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/resources/sql_injection_vul5.py` & `evase-analysis-1.0.8.5/tests/resources/sql_injection_vul5.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/resources/sql_injection_vul6.py` & `evase-analysis-1.0.8.5/tests/resources/sql_injection_vul6.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/resources/type_demo/app.py` & `evase-analysis-1.0.8.5/tests/resources/type_demo/app.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/resources/type_demo/user_db_handler.py` & `evase-analysis-1.0.8.5/tests/resources/type_demo/user_db_handler.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/resources/type_demo/vul.py` & `evase-analysis-1.0.8.5/tests/resources/type_demo/vul.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/resources/type_demo/vul_wrapper.py` & `evase-analysis-1.0.8.5/tests/resources/type_demo/vul_wrapper.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/__init__.py` & `evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/__init__.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/actions.py` & `evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/actions.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/auth.py` & `evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/auth.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/ui.py` & `evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/ui.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/resources/webgoat/flask_webgoat/users.py` & `evase-analysis-1.0.8.5/tests/resources/webgoat/flask_webgoat/users.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/test_analysisperformer.py` & `evase-analysis-1.0.8.5/tests/test_analysisperformer.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/test_fileutil.py` & `evase-analysis-1.0.8.5/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/test_projectstructure.py` & `evase-analysis-1.0.8.5/tests/test_projectstructure.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/test_scoperesolver.py` & `evase-analysis-1.0.8.5/tests/test_scoperesolver.py`

 * *Files identical despite different names*

### Comparing `evase-analysis-1.0.8.4/tests/testutil.py` & `evase-analysis-1.0.8.5/tests/testutil.py`

 * *Files identical despite different names*

