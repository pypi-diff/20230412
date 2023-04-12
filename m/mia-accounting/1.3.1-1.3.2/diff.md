# Comparing `tmp/mia-accounting-1.3.1.tar.gz` & `tmp/mia-accounting-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia-accounting-1.3.1.tar", last modified: Tue Apr 11 14:32:42 2023, max compression
+gzip compressed data, was "mia-accounting-1.3.2.tar", last modified: Wed Apr 12 10:01:53 2023, max compression
```

## Comparing `mia-accounting-1.3.1.tar` & `mia-accounting-1.3.2.tar`

### file list

```diff
@@ -1,305 +1,310 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.088098 mia-accounting-1.3.1/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.3.1/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.3.1/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-11 14:32:42.084098 mia-accounting-1.3.1/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     5871 2023-04-11 13:56:49.000000 mia-accounting-1.3.1/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.956100 mia-accounting-1.3.1/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.3.1/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.3.1/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.956100 mia-accounting-1.3.1/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.956100 mia-accounting-1.3.1/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.3.1/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.956100 mia-accounting-1.3.1/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.3.1/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-10 16:05:21.000000 mia-accounting-1.3.1/docs/source/accounting.account.rst
--rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-10 16:05:21.000000 mia-accounting-1.3.1/docs/source/accounting.base_account.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.currency.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.journal_entry.forms.rst
--rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.journal_entry.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.journal_entry.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.option.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.report.period.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2043 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.report.reports.rst
--rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.report.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1775 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.report.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1332 2023-04-10 16:05:21.000000 mia-accounting-1.3.1/docs/source/accounting.rst
--rw-r--r--   0 imacat    (1000) users      (100)      615 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.unmatched_offset.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2756 2023-04-10 16:05:22.000000 mia-accounting-1.3.1/docs/source/accounting.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-11 14:30:58.000000 mia-accounting-1.3.1/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.3.1/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.3.1/docs/source/history.rst
--rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.3.1/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     3615 2023-04-11 13:56:49.000000 mia-accounting-1.3.1/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.3.1/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-11 14:30:59.000000 mia-accounting-1.3.1/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-11 14:32:42.088098 mia-accounting-1.3.1/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.952100 mia-accounting-1.3.1/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.956100 mia-accounting-1.3.1/src/accounting/
--rw-r--r--   0 imacat    (1000) users      (100)     3065 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/__init__.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.960100 mia-accounting-1.3.1/src/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.3.1/src/accounting/account/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.3.1/src/accounting/account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.960100 mia-accounting-1.3.1/src/accounting/base_account/
--rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/base_account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/base_account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/base_account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.3.1/src/accounting/base_account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.3.1/src/accounting/base_account/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/commands.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.960100 mia-accounting-1.3.1/src/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/currency/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2212 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/src/accounting/currency/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/currency/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.3.1/src/accounting/currency/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/currency/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.3.1/src/accounting/currency/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.960100 mia-accounting-1.3.1/src/accounting/data/
--rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.3.1/src/accounting/data/base_accounts.csv
--rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.3.1/src/accounting/data/currencies.csv
--rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.3.1/src/accounting/forms.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.960100 mia-accounting-1.3.1/src/accounting/journal_entry/
--rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/journal_entry/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3345 2023-04-07 07:30:13.000000 mia-accounting-1.3.1/src/accounting/journal_entry/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.964100 mia-accounting-1.3.1/src/accounting/journal_entry/forms/
--rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.3.1/src/accounting/journal_entry/forms/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    11055 2023-04-08 10:12:54.000000 mia-accounting-1.3.1/src/accounting/journal_entry/forms/currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.3.1/src/accounting/journal_entry/forms/journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    19508 2023-04-07 16:44:13.000000 mia-accounting-1.3.1/src/accounting/journal_entry/forms/line_item.py
--rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/journal_entry/forms/reorder.py
--rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.3.1/src/accounting/journal_entry/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.964100 mia-accounting-1.3.1/src/accounting/journal_entry/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.3.1/src/accounting/journal_entry/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1729 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/journal_entry/utils/account_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    12821 2023-04-04 09:21:31.000000 mia-accounting-1.3.1/src/accounting/journal_entry/utils/description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/journal_entry/utils/operators.py
--rw-r--r--   0 imacat    (1000) users      (100)     3787 2023-04-08 10:12:55.000000 mia-accounting-1.3.1/src/accounting/journal_entry/utils/original_line_items.py
--rw-r--r--   0 imacat    (1000) users      (100)     9472 2023-04-09 02:08:22.000000 mia-accounting-1.3.1/src/accounting/journal_entry/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.3.1/src/accounting/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    31691 2023-04-08 10:12:57.000000 mia-accounting-1.3.1/src/accounting/models.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.964100 mia-accounting-1.3.1/src/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/option/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.3.1/src/accounting/option/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.3.1/src/accounting/option/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.964100 mia-accounting-1.3.1/src/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.3.1/src/accounting/report/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.3.1/src/accounting/report/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.964100 mia-accounting-1.3.1/src/accounting/report/period/
--rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.3.1/src/accounting/report/period/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/report/period/chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/report/period/description.py
--rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.3.1/src/accounting/report/period/month_end.py
--rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.3.1/src/accounting/report/period/parser.py
--rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.3.1/src/accounting/report/period/period.py
--rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/report/period/shortcuts.py
--rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/report/period/specification.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.968100 mia-accounting-1.3.1/src/accounting/report/reports/
--rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.3.1/src/accounting/report/reports/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.3.1/src/accounting/report/reports/balance_sheet.py
--rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/report/reports/income_expenses.py
--rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.3.1/src/accounting/report/reports/income_statement.py
--rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.3.1/src/accounting/report/reports/journal.py
--rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.3.1/src/accounting/report/reports/ledger.py
--rw-r--r--   0 imacat    (1000) users      (100)     8819 2023-04-09 13:02:35.000000 mia-accounting-1.3.1/src/accounting/report/reports/search.py
--rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.3.1/src/accounting/report/reports/trial_balance.py
--rw-r--r--   0 imacat    (1000) users      (100)     6975 2023-04-08 16:39:45.000000 mia-accounting-1.3.1/src/accounting/report/reports/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4555 2023-04-08 10:12:55.000000 mia-accounting-1.3.1/src/accounting/report/reports/unapplied_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.3.1/src/accounting/report/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.968100 mia-accounting-1.3.1/src/accounting/report/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/report/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/report/utils/base_page_params.py
--rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.3.1/src/accounting/report/utils/base_report.py
--rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-09 04:04:18.000000 mia-accounting-1.3.1/src/accounting/report/utils/csv_export.py
--rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.3.1/src/accounting/report/utils/option_link.py
--rw-r--r--   0 imacat    (1000) users      (100)     6925 2023-04-08 10:12:55.000000 mia-accounting-1.3.1/src/accounting/report/utils/report_chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     1305 2023-04-08 03:26:33.000000 mia-accounting-1.3.1/src/accounting/report/utils/report_type.py
--rw-r--r--   0 imacat    (1000) users      (100)     2740 2023-04-08 10:12:55.000000 mia-accounting-1.3.1/src/accounting/report/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4477 2023-04-09 02:08:22.000000 mia-accounting-1.3.1/src/accounting/report/utils/urls.py
--rw-r--r--   0 imacat    (1000) users      (100)    10434 2023-04-09 02:08:22.000000 mia-accounting-1.3.1/src/accounting/report/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.952100 mia-accounting-1.3.1/src/accounting/static/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.968100 mia-accounting-1.3.1/src/accounting/static/css/
--rw-r--r--   0 imacat    (1000) users      (100)    13001 2023-04-08 16:39:45.000000 mia-accounting-1.3.1/src/accounting/static/css/style.css
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.968100 mia-accounting-1.3.1/src/accounting/static/js/
--rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/account-form.js
--rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/account-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/currency-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    38778 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/description-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/drag-and-drop-reorder.js
--rw-r--r--   0 imacat    (1000) users      (100)     9092 2023-04-07 04:32:27.000000 mia-accounting-1.3.1/src/accounting/static/js/journal-entry-account-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    32504 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/journal-entry-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    19866 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/journal-entry-line-item-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/journal-entry-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/material-fab-speed-dial.js
--rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/option-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    11640 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/original-line-item-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.3.1/src/accounting/static/js/period-chooser.js
--rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.3.1/src/accounting/template_filters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/template_globals.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.952100 mia-accounting-1.3.1/src/accounting/templates/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.968100 mia-accounting-1.3.1/src/accounting/templates/accounting/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/account/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/account/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/account/include/
--rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/account/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/account/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/base-account/
--rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/base-account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/base-account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/base.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/currency/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/currency/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/currency/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/currency/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/currency/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/currency/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3103 2023-04-10 23:49:07.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/include/nav.html
--rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/include/pagination.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/
--rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.972100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3373 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)    14459 2023-04-05 01:08:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3131 2023-04-07 06:56:44.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
--rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
--rw-r--r--   0 imacat    (1000) users      (100)     6161 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
--rw-r--r--   0 imacat    (1000) users      (100)     3490 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/
--rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/
--rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/option/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/option/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
--rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/form-recurring-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.976100 mia-accounting-1.3.1/src/accounting/templates/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     5065 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/balance-sheet.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.980100 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
--rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/balance-sheet-section.html
--rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/period-chooser.html
--rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/search-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     5572 2023-04-04 23:56:52.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/toolbar-buttons.html
--rw-r--r--   0 imacat    (1000) users      (100)     4623 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/income-expenses.html
--rw-r--r--   0 imacat    (1000) users      (100)     4242 2023-04-04 10:04:12.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/income-statement.html
--rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/journal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4745 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/ledger.html
--rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/search.html
--rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-04 10:04:10.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/trial-balance.html
--rw-r--r--   0 imacat    (1000) users      (100)     2201 2023-04-08 10:12:55.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/unapplied-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     4086 2023-04-08 16:39:45.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/report/unapplied.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.980100 mia-accounting-1.3.1/src/accounting/templates/accounting/unmatched-offset/
--rw-r--r--   0 imacat    (1000) users      (100)     1212 2023-04-08 16:38:54.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/unmatched-offset/dashboard.html
--rw-r--r--   0 imacat    (1000) users      (100)     4668 2023-04-08 10:12:57.000000 mia-accounting-1.3.1/src/accounting/templates/accounting/unmatched-offset/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.996100 mia-accounting-1.3.1/src/accounting/translations/
--rw-r--r--   0 imacat    (1000) users      (100)    47460 2023-04-08 17:41:05.000000 mia-accounting-1.3.1/src/accounting/translations/accounting.pot
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.3.1/src/accounting/translations/babel.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.952100 mia-accounting-1.3.1/src/accounting/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.020099 mia-accounting-1.3.1/src/accounting/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.952100 mia-accounting-1.3.1/src/accounting/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.064098 mia-accounting-1.3.1/src/accounting/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.064098 mia-accounting-1.3.1/src/accounting/unmatched_offset/
--rw-r--r--   0 imacat    (1000) users      (100)     1032 2023-04-08 10:12:57.000000 mia-accounting-1.3.1/src/accounting/unmatched_offset/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-08 10:12:57.000000 mia-accounting-1.3.1/src/accounting/unmatched_offset/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     3178 2023-04-08 16:39:45.000000 mia-accounting-1.3.1/src/accounting/unmatched_offset/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.068098 mia-accounting-1.3.1/src/accounting/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.3.1/src/accounting/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/utils/cast.py
--rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/utils/current_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/utils/flash_errors.py
--rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.3.1/src/accounting/utils/journal_entry_types.py
--rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/src/accounting/utils/next_uri.py
--rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.3.1/src/accounting/utils/offset_alias.py
--rw-r--r--   0 imacat    (1000) users      (100)     5198 2023-04-08 16:39:45.000000 mia-accounting-1.3.1/src/accounting/utils/offset_matcher.py
--rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.3.1/src/accounting/utils/options.py
--rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.3.1/src/accounting/utils/pagination.py
--rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.3.1/src/accounting/utils/permission.py
--rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/utils/query.py
--rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/utils/random_id.py
--rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.3.1/src/accounting/utils/strip_text.py
--rw-r--r--   0 imacat    (1000) users      (100)     3080 2023-04-08 10:12:56.000000 mia-accounting-1.3.1/src/accounting/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.3.1/src/accounting/utils/user.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.068098 mia-accounting-1.3.1/src/mia_accounting.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-11 14:32:41.000000 mia-accounting-1.3.1/src/mia_accounting.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)    11392 2023-04-11 14:32:41.000000 mia-accounting-1.3.1/src/mia_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-11 14:32:41.000000 mia-accounting-1.3.1/src/mia_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-11 14:32:41.000000 mia-accounting-1.3.1/src/mia_accounting.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-11 14:32:41.000000 mia-accounting-1.3.1/src/mia_accounting.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.072098 mia-accounting-1.3.1/tests/
--rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-04 09:21:35.000000 mia-accounting-1.3.1/tests/babel-utils-test-site.py
--rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-04 09:21:32.000000 mia-accounting-1.3.1/tests/babel-utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    32736 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_base_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_commands.py
--rw-r--r--   0 imacat    (1000) users      (100)    23824 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    15999 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)   103461 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    38268 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    15935 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    15398 2023-04-11 00:28:47.000000 mia-accounting-1.3.1/tests/test_report.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.072098 mia-accounting-1.3.1/tests/test_site/
--rw-r--r--   0 imacat    (1000) users      (100)     4456 2023-04-11 14:03:11.000000 mia-accounting-1.3.1/tests/test_site/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3073 2023-04-11 14:24:08.000000 mia-accounting-1.3.1/tests/test_site/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.3.1/tests/test_site/locale.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.072098 mia-accounting-1.3.1/tests/test_site/static/
--rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.3.1/tests/test_site/static/favicon.svg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.072098 mia-accounting-1.3.1/tests/test_site/templates/
--rw-r--r--   0 imacat    (1000) users      (100)     6015 2023-04-05 18:00:22.000000 mia-accounting-1.3.1/tests/test_site/templates/base.html
--rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.3.1/tests/test_site/templates/home.html
--rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.3.1/tests/test_site/templates/login.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.072098 mia-accounting-1.3.1/tests/test_site/translations/
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.3.1/tests/test_site/translations/babel.cfg
--rw-r--r--   0 imacat    (1000) users      (100)     1837 2023-04-11 14:18:30.000000 mia-accounting-1.3.1/tests/test_site/translations/messages.pot
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.952100 mia-accounting-1.3.1/tests/test_site/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.084098 mia-accounting-1.3.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     1486 2023-04-11 14:18:32.000000 mia-accounting-1.3.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     2369 2023-04-11 14:18:32.000000 mia-accounting-1.3.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:41.952100 mia-accounting-1.3.1/tests/test_site/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-11 14:32:42.084098 mia-accounting-1.3.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     1486 2023-04-11 14:18:32.000000 mia-accounting-1.3.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     2369 2023-04-11 14:27:31.000000 mia-accounting-1.3.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
--rw-r--r--   0 imacat    (1000) users      (100)    28229 2023-04-10 15:59:48.000000 mia-accounting-1.3.1/tests/test_unmatched_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.3.1/tests/test_utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    14555 2023-04-11 14:26:58.000000 mia-accounting-1.3.1/tests/testlib.py
--rw-r--r--   0 imacat    (1000) users      (100)    16670 2023-04-09 03:46:55.000000 mia-accounting-1.3.1/tests/testlib_journal_entry.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.3.2/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.3.2/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     5871 2023-04-11 13:56:49.000000 mia-accounting-1.3.2/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.207196 mia-accounting-1.3.2/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.3.2/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.3.2/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.207196 mia-accounting-1.3.2/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.207196 mia-accounting-1.3.2/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.3.2/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.207196 mia-accounting-1.3.2/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.3.2/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-10 16:05:21.000000 mia-accounting-1.3.2/docs/source/accounting.account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-10 16:05:21.000000 mia-accounting-1.3.2/docs/source/accounting.base_account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.currency.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.journal_entry.forms.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.journal_entry.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.journal_entry.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.option.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.report.period.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2043 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.report.reports.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.report.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1775 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.report.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1332 2023-04-10 16:05:21.000000 mia-accounting-1.3.2/docs/source/accounting.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      615 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.unmatched_offset.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2756 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-12 09:53:44.000000 mia-accounting-1.3.2/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.3.2/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.3.2/docs/source/history.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.3.2/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     3615 2023-04-11 13:56:49.000000 mia-accounting-1.3.2/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.3.2/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-12 09:53:44.000000 mia-accounting-1.3.2/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.203196 mia-accounting-1.3.2/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.211195 mia-accounting-1.3.2/src/accounting/
+-rw-r--r--   0 imacat    (1000) users      (100)     3065 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/__init__.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.211195 mia-accounting-1.3.2/src/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.3.2/src/accounting/account/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.3.2/src/accounting/account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.211195 mia-accounting-1.3.2/src/accounting/base_account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/base_account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/base_account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/base_account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.3.2/src/accounting/base_account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.3.2/src/accounting/base_account/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/commands.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.211195 mia-accounting-1.3.2/src/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/currency/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2212 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/currency/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/currency/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.3.2/src/accounting/currency/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/currency/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.3.2/src/accounting/currency/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.211195 mia-accounting-1.3.2/src/accounting/data/
+-rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.3.2/src/accounting/data/base_accounts.csv
+-rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.3.2/src/accounting/data/currencies.csv
+-rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.3.2/src/accounting/forms.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.211195 mia-accounting-1.3.2/src/accounting/journal_entry/
+-rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/journal_entry/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3283 2023-04-11 16:41:29.000000 mia-accounting-1.3.2/src/accounting/journal_entry/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.215195 mia-accounting-1.3.2/src/accounting/journal_entry/forms/
+-rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.3.2/src/accounting/journal_entry/forms/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11055 2023-04-08 10:12:54.000000 mia-accounting-1.3.2/src/accounting/journal_entry/forms/currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.3.2/src/accounting/journal_entry/forms/journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    19508 2023-04-07 16:44:13.000000 mia-accounting-1.3.2/src/accounting/journal_entry/forms/line_item.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/journal_entry/forms/reorder.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.3.2/src/accounting/journal_entry/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.215195 mia-accounting-1.3.2/src/accounting/journal_entry/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.3.2/src/accounting/journal_entry/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1729 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/journal_entry/utils/account_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12821 2023-04-04 09:21:31.000000 mia-accounting-1.3.2/src/accounting/journal_entry/utils/description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/journal_entry/utils/operators.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3787 2023-04-08 10:12:55.000000 mia-accounting-1.3.2/src/accounting/journal_entry/utils/original_line_items.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9472 2023-04-09 02:08:22.000000 mia-accounting-1.3.2/src/accounting/journal_entry/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.3.2/src/accounting/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    31691 2023-04-08 10:12:57.000000 mia-accounting-1.3.2/src/accounting/models.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.215195 mia-accounting-1.3.2/src/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/option/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.3.2/src/accounting/option/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.3.2/src/accounting/option/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.215195 mia-accounting-1.3.2/src/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.3.2/src/accounting/report/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.3.2/src/accounting/report/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.215195 mia-accounting-1.3.2/src/accounting/report/period/
+-rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.3.2/src/accounting/report/period/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/report/period/chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/report/period/description.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.3.2/src/accounting/report/period/month_end.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.3.2/src/accounting/report/period/parser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.3.2/src/accounting/report/period/period.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/report/period/shortcuts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/report/period/specification.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.219195 mia-accounting-1.3.2/src/accounting/report/reports/
+-rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.3.2/src/accounting/report/reports/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.3.2/src/accounting/report/reports/balance_sheet.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/report/reports/income_expenses.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.3.2/src/accounting/report/reports/income_statement.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.3.2/src/accounting/report/reports/journal.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.3.2/src/accounting/report/reports/ledger.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8819 2023-04-09 13:02:35.000000 mia-accounting-1.3.2/src/accounting/report/reports/search.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.3.2/src/accounting/report/reports/trial_balance.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6975 2023-04-08 16:39:45.000000 mia-accounting-1.3.2/src/accounting/report/reports/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4555 2023-04-08 10:12:55.000000 mia-accounting-1.3.2/src/accounting/report/reports/unapplied_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.3.2/src/accounting/report/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.219195 mia-accounting-1.3.2/src/accounting/report/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/report/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/report/utils/base_page_params.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.3.2/src/accounting/report/utils/base_report.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-09 04:04:18.000000 mia-accounting-1.3.2/src/accounting/report/utils/csv_export.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.3.2/src/accounting/report/utils/option_link.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6925 2023-04-08 10:12:55.000000 mia-accounting-1.3.2/src/accounting/report/utils/report_chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1305 2023-04-08 03:26:33.000000 mia-accounting-1.3.2/src/accounting/report/utils/report_type.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2740 2023-04-08 10:12:55.000000 mia-accounting-1.3.2/src/accounting/report/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4477 2023-04-09 02:08:22.000000 mia-accounting-1.3.2/src/accounting/report/utils/urls.py
+-rw-r--r--   0 imacat    (1000) users      (100)    10434 2023-04-09 02:08:22.000000 mia-accounting-1.3.2/src/accounting/report/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.203196 mia-accounting-1.3.2/src/accounting/static/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.219195 mia-accounting-1.3.2/src/accounting/static/css/
+-rw-r--r--   0 imacat    (1000) users      (100)    13001 2023-04-08 16:39:45.000000 mia-accounting-1.3.2/src/accounting/static/css/style.css
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.219195 mia-accounting-1.3.2/src/accounting/static/js/
+-rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/account-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/account-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/currency-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    38778 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/description-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/drag-and-drop-reorder.js
+-rw-r--r--   0 imacat    (1000) users      (100)     9092 2023-04-07 04:32:27.000000 mia-accounting-1.3.2/src/accounting/static/js/journal-entry-account-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    32504 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/journal-entry-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    19866 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/journal-entry-line-item-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/journal-entry-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/material-fab-speed-dial.js
+-rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/option-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    11640 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/original-line-item-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/period-chooser.js
+-rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.3.2/src/accounting/template_filters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/template_globals.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.203196 mia-accounting-1.3.2/src/accounting/templates/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.219195 mia-accounting-1.3.2/src/accounting/templates/accounting/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/account/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/account/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/account/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/account/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/account/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/base-account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/base-account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/base-account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/base.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/currency/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/currency/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/currency/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/currency/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/currency/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/currency/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3103 2023-04-10 23:49:07.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/include/nav.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/include/pagination.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/
+-rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.227195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3373 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)    14459 2023-04-05 01:08:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3131 2023-04-07 06:56:44.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6161 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3490 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.227195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/
+-rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.227195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.227195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/
+-rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.227195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.227195 mia-accounting-1.3.2/src/accounting/templates/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/option/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/option/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.227195 mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/form-recurring-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.231195 mia-accounting-1.3.2/src/accounting/templates/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     5065 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/balance-sheet.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.231195 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/balance-sheet-section.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/period-chooser.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/search-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     5572 2023-04-04 23:56:52.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/toolbar-buttons.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4623 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/income-expenses.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4242 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/income-statement.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/journal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4745 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/ledger.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/search.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/trial-balance.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2201 2023-04-08 10:12:55.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/unapplied-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4086 2023-04-08 16:39:45.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/unapplied.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.231195 mia-accounting-1.3.2/src/accounting/templates/accounting/unmatched-offset/
+-rw-r--r--   0 imacat    (1000) users      (100)     1212 2023-04-08 16:38:54.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/unmatched-offset/dashboard.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4668 2023-04-08 10:12:57.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/unmatched-offset/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.231195 mia-accounting-1.3.2/src/accounting/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)    47460 2023-04-08 17:41:05.000000 mia-accounting-1.3.2/src/accounting/translations/accounting.pot
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.3.2/src/accounting/translations/babel.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.203196 mia-accounting-1.3.2/src/accounting/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.231195 mia-accounting-1.3.2/src/accounting/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.2/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.2/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.203196 mia-accounting-1.3.2/src/accounting/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.231195 mia-accounting-1.3.2/src/accounting/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.2/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.2/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.231195 mia-accounting-1.3.2/src/accounting/unmatched_offset/
+-rw-r--r--   0 imacat    (1000) users      (100)     1032 2023-04-08 10:12:57.000000 mia-accounting-1.3.2/src/accounting/unmatched_offset/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-08 10:12:57.000000 mia-accounting-1.3.2/src/accounting/unmatched_offset/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3178 2023-04-08 16:39:45.000000 mia-accounting-1.3.2/src/accounting/unmatched_offset/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.235195 mia-accounting-1.3.2/src/accounting/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.3.2/src/accounting/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/utils/cast.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/utils/current_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/utils/flash_errors.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.3.2/src/accounting/utils/journal_entry_types.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/utils/next_uri.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.3.2/src/accounting/utils/offset_alias.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5198 2023-04-08 16:39:45.000000 mia-accounting-1.3.2/src/accounting/utils/offset_matcher.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.3.2/src/accounting/utils/options.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.3.2/src/accounting/utils/pagination.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.3.2/src/accounting/utils/permission.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/utils/query.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/utils/random_id.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.3.2/src/accounting/utils/strip_text.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3080 2023-04-08 10:12:56.000000 mia-accounting-1.3.2/src/accounting/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/utils/user.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.235195 mia-accounting-1.3.2/src/mia_accounting.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-12 10:01:53.000000 mia-accounting-1.3.2/src/mia_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)    11508 2023-04-12 10:01:53.000000 mia-accounting-1.3.2/src/mia_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-12 10:01:53.000000 mia-accounting-1.3.2/src/mia_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-12 10:01:53.000000 mia-accounting-1.3.2/src/mia_accounting.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-12 10:01:53.000000 mia-accounting-1.3.2/src/mia_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.3.2/tests/babel-utils-test-site.py
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.3.2/tests/babel-utils.py
+-rwxr-xr-x   0 imacat    (1000) users      (100)    11020 2023-04-12 09:13:03.000000 mia-accounting-1.3.2/tests/make-sample.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32736 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/tests/test_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/tests/test_base_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/tests/test_commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)    23824 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/tests/test_currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15999 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/tests/test_description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)   103461 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/tests/test_journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    38264 2023-04-12 04:25:38.000000 mia-accounting-1.3.2/tests/test_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15935 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/tests/test_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15371 2023-04-12 04:25:38.000000 mia-accounting-1.3.2/tests/test_report.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/test_site/
+-rw-r--r--   0 imacat    (1000) users      (100)     4505 2023-04-11 16:31:36.000000 mia-accounting-1.3.2/tests/test_site/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3073 2023-04-11 14:24:08.000000 mia-accounting-1.3.2/tests/test_site/auth.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/test_site/data/
+-rw-r--r--   0 imacat    (1000) users      (100)   121813 2023-04-12 09:21:52.000000 mia-accounting-1.3.2/tests/test_site/data/sample.json
+-rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.3.2/tests/test_site/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4888 2023-04-12 09:59:37.000000 mia-accounting-1.3.2/tests/test_site/reset.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/test_site/static/
+-rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.3.2/tests/test_site/static/favicon.svg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/test_site/templates/
+-rw-r--r--   0 imacat    (1000) users      (100)     6435 2023-04-12 09:40:17.000000 mia-accounting-1.3.2/tests/test_site/templates/base.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.3.2/tests/test_site/templates/home.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.3.2/tests/test_site/templates/login.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 09:48:47.000000 mia-accounting-1.3.2/tests/test_site/templates/reset.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/test_site/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.3.2/tests/test_site/translations/babel.cfg
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.3.2/tests/test_site/translations/messages.pot
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.203196 mia-accounting-1.3.2/tests/test_site/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/test_site/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.3.2/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.3.2/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.203196 mia-accounting-1.3.2/tests/test_site/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/test_site/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.3.2/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.3.2/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
+-rw-r--r--   0 imacat    (1000) users      (100)    27871 2023-04-12 04:25:38.000000 mia-accounting-1.3.2/tests/test_unmatched_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.3.2/tests/test_utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18890 2023-04-12 09:21:46.000000 mia-accounting-1.3.2/tests/testlib.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16670 2023-04-09 03:46:55.000000 mia-accounting-1.3.2/tests/testlib_journal_entry.py
```

### Comparing `mia-accounting-1.3.1/LICENSE` & `mia-accounting-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/MANIFEST.in` & `mia-accounting-1.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/PKG-INFO` & `mia-accounting-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
 Keywords: mia,accounting,flask
```

### Comparing `mia-accounting-1.3.1/README.rst` & `mia-accounting-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/Makefile` & `mia-accounting-1.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/make.bat` & `mia-accounting-1.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/accounting.account.rst` & `mia-accounting-1.3.2/docs/source/accounting.account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/accounting.base_account.rst` & `mia-accounting-1.3.2/docs/source/accounting.base_account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/accounting.currency.rst` & `mia-accounting-1.3.2/docs/source/accounting.currency.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/accounting.journal_entry.forms.rst` & `mia-accounting-1.3.2/docs/source/accounting.journal_entry.forms.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/accounting.journal_entry.rst` & `mia-accounting-1.3.2/docs/source/accounting.journal_entry.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/accounting.journal_entry.utils.rst` & `mia-accounting-1.3.2/docs/source/accounting.journal_entry.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/accounting.option.rst` & `mia-accounting-1.3.2/docs/source/accounting.option.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/accounting.report.period.rst` & `mia-accounting-1.3.2/docs/source/accounting.report.period.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/accounting.report.reports.rst` & `mia-accounting-1.3.2/docs/source/accounting.report.reports.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/accounting.report.rst` & `mia-accounting-1.3.2/docs/source/accounting.report.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/accounting.report.utils.rst` & `mia-accounting-1.3.2/docs/source/accounting.report.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/accounting.rst` & `mia-accounting-1.3.2/docs/source/accounting.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/accounting.unmatched_offset.rst` & `mia-accounting-1.3.2/docs/source/accounting.unmatched_offset.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/accounting.utils.rst` & `mia-accounting-1.3.2/docs/source/accounting.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/conf.py` & `mia-accounting-1.3.2/docs/source/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Mia! Accounting'
 copyright = '2023, imacat'
 author = 'imacat'
-release = '1.3.1'
+release = '1.3.2'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc']
 
 templates_path = ['_templates']
```

### Comparing `mia-accounting-1.3.1/docs/source/examples.rst` & `mia-accounting-1.3.2/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/history.rst` & `mia-accounting-1.3.2/docs/source/history.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/docs/source/intro.rst` & `mia-accounting-1.3.2/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/pyproject.toml` & `mia-accounting-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 [project]
 name = "mia-accounting"
-version = "1.3.1"
+version = "1.3.2"
 description = "A Flask accounting module."
 readme = "README.rst"
 requires-python = ">=3.11"
 authors = [
     {name = "imacat", email = "imacat@mail.imacat.idv.tw"},
 ]
 keywords = ["mia", "accounting", "flask"]
```

### Comparing `mia-accounting-1.3.1/src/accounting/__init__.py` & `mia-accounting-1.3.2/src/accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/account/__init__.py` & `mia-accounting-1.3.2/src/accounting/account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/account/commands.py` & `mia-accounting-1.3.2/src/accounting/account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/account/converters.py` & `mia-accounting-1.3.2/src/accounting/account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/account/forms.py` & `mia-accounting-1.3.2/src/accounting/account/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/account/queries.py` & `mia-accounting-1.3.2/src/accounting/account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/account/views.py` & `mia-accounting-1.3.2/src/accounting/account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/base_account/__init__.py` & `mia-accounting-1.3.2/src/accounting/base_account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/base_account/commands.py` & `mia-accounting-1.3.2/src/accounting/base_account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/base_account/converters.py` & `mia-accounting-1.3.2/src/accounting/base_account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/base_account/queries.py` & `mia-accounting-1.3.2/src/accounting/base_account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/base_account/views.py` & `mia-accounting-1.3.2/src/accounting/base_account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/commands.py` & `mia-accounting-1.3.2/src/accounting/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/currency/__init__.py` & `mia-accounting-1.3.2/src/accounting/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/currency/commands.py` & `mia-accounting-1.3.2/src/accounting/currency/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/currency/converters.py` & `mia-accounting-1.3.2/src/accounting/currency/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/currency/forms.py` & `mia-accounting-1.3.2/src/accounting/currency/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/currency/queries.py` & `mia-accounting-1.3.2/src/accounting/currency/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/currency/views.py` & `mia-accounting-1.3.2/src/accounting/currency/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/data/base_accounts.csv` & `mia-accounting-1.3.2/src/accounting/data/base_accounts.csv`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/forms.py` & `mia-accounting-1.3.2/src/accounting/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/journal_entry/__init__.py` & `mia-accounting-1.3.2/src/accounting/journal_entry/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/journal_entry/converters.py` & `mia-accounting-1.3.2/src/accounting/journal_entry/converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,18 @@
 #  limitations under the License.
 """The path converters for the journal entry management.
 
 """
 from datetime import date
 
 from flask import abort
-from sqlalchemy.orm import selectinload
 from werkzeug.routing import BaseConverter
 
 from accounting import db
-from accounting.models import JournalEntry, JournalEntryLineItem
+from accounting.models import JournalEntry
 from accounting.utils.journal_entry_types import JournalEntryType
 
 
 class JournalEntryConverter(BaseConverter):
     """The journal entry converter to convert the journal entry ID from and to
     the corresponding journal entry in the routes."""
```

### Comparing `mia-accounting-1.3.1/src/accounting/journal_entry/forms/__init__.py` & `mia-accounting-1.3.2/src/accounting/journal_entry/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/journal_entry/forms/currency.py` & `mia-accounting-1.3.2/src/accounting/journal_entry/forms/currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/journal_entry/forms/journal_entry.py` & `mia-accounting-1.3.2/src/accounting/journal_entry/forms/journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/journal_entry/forms/line_item.py` & `mia-accounting-1.3.2/src/accounting/journal_entry/forms/line_item.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/journal_entry/forms/reorder.py` & `mia-accounting-1.3.2/src/accounting/journal_entry/forms/reorder.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/journal_entry/template_filters.py` & `mia-accounting-1.3.2/src/accounting/journal_entry/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/journal_entry/utils/__init__.py` & `mia-accounting-1.3.2/src/accounting/journal_entry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/journal_entry/utils/account_option.py` & `mia-accounting-1.3.2/src/accounting/journal_entry/utils/account_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/journal_entry/utils/description_editor.py` & `mia-accounting-1.3.2/src/accounting/journal_entry/utils/description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/journal_entry/utils/operators.py` & `mia-accounting-1.3.2/src/accounting/journal_entry/utils/operators.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/journal_entry/utils/original_line_items.py` & `mia-accounting-1.3.2/src/accounting/journal_entry/utils/original_line_items.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/journal_entry/views.py` & `mia-accounting-1.3.2/src/accounting/journal_entry/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/locale.py` & `mia-accounting-1.3.2/src/accounting/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/models.py` & `mia-accounting-1.3.2/src/accounting/models.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/option/__init__.py` & `mia-accounting-1.3.2/src/accounting/option/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/option/forms.py` & `mia-accounting-1.3.2/src/accounting/option/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/option/views.py` & `mia-accounting-1.3.2/src/accounting/option/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/__init__.py` & `mia-accounting-1.3.2/src/accounting/report/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/converters.py` & `mia-accounting-1.3.2/src/accounting/report/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/period/__init__.py` & `mia-accounting-1.3.2/src/accounting/report/period/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/period/chooser.py` & `mia-accounting-1.3.2/src/accounting/report/period/chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/period/description.py` & `mia-accounting-1.3.2/src/accounting/report/period/description.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/period/month_end.py` & `mia-accounting-1.3.2/src/accounting/report/period/month_end.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/period/parser.py` & `mia-accounting-1.3.2/src/accounting/report/period/parser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/period/period.py` & `mia-accounting-1.3.2/src/accounting/report/period/period.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/period/shortcuts.py` & `mia-accounting-1.3.2/src/accounting/report/period/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/period/specification.py` & `mia-accounting-1.3.2/src/accounting/report/period/specification.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/reports/__init__.py` & `mia-accounting-1.3.2/src/accounting/report/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/reports/balance_sheet.py` & `mia-accounting-1.3.2/src/accounting/report/reports/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/reports/income_expenses.py` & `mia-accounting-1.3.2/src/accounting/report/reports/income_expenses.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/reports/income_statement.py` & `mia-accounting-1.3.2/src/accounting/report/reports/income_statement.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/reports/journal.py` & `mia-accounting-1.3.2/src/accounting/report/reports/journal.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/reports/ledger.py` & `mia-accounting-1.3.2/src/accounting/report/reports/ledger.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/reports/search.py` & `mia-accounting-1.3.2/src/accounting/report/reports/search.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/reports/trial_balance.py` & `mia-accounting-1.3.2/src/accounting/report/reports/trial_balance.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/reports/unapplied.py` & `mia-accounting-1.3.2/src/accounting/report/reports/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/reports/unapplied_accounts.py` & `mia-accounting-1.3.2/src/accounting/report/reports/unapplied_accounts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/template_filters.py` & `mia-accounting-1.3.2/src/accounting/report/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/utils/__init__.py` & `mia-accounting-1.3.2/src/accounting/report/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/utils/base_page_params.py` & `mia-accounting-1.3.2/src/accounting/report/utils/base_page_params.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/utils/base_report.py` & `mia-accounting-1.3.2/src/accounting/report/utils/base_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/utils/csv_export.py` & `mia-accounting-1.3.2/src/accounting/report/utils/csv_export.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/utils/option_link.py` & `mia-accounting-1.3.2/src/accounting/report/utils/option_link.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/utils/report_chooser.py` & `mia-accounting-1.3.2/src/accounting/report/utils/report_chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/utils/report_type.py` & `mia-accounting-1.3.2/src/accounting/report/utils/report_type.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/utils/unapplied.py` & `mia-accounting-1.3.2/src/accounting/report/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/utils/urls.py` & `mia-accounting-1.3.2/src/accounting/report/utils/urls.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/report/views.py` & `mia-accounting-1.3.2/src/accounting/report/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/static/css/style.css` & `mia-accounting-1.3.2/src/accounting/static/css/style.css`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/static/js/account-form.js` & `mia-accounting-1.3.2/src/accounting/static/js/account-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/static/js/account-order.js` & `mia-accounting-1.3.2/src/accounting/static/js/account-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/static/js/currency-form.js` & `mia-accounting-1.3.2/src/accounting/static/js/currency-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/static/js/description-editor.js` & `mia-accounting-1.3.2/src/accounting/static/js/description-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/static/js/drag-and-drop-reorder.js` & `mia-accounting-1.3.2/src/accounting/static/js/drag-and-drop-reorder.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/static/js/journal-entry-account-selector.js` & `mia-accounting-1.3.2/src/accounting/static/js/journal-entry-account-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/static/js/journal-entry-form.js` & `mia-accounting-1.3.2/src/accounting/static/js/journal-entry-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/static/js/journal-entry-line-item-editor.js` & `mia-accounting-1.3.2/src/accounting/static/js/journal-entry-line-item-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/static/js/journal-entry-order.js` & `mia-accounting-1.3.2/src/accounting/static/js/journal-entry-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/static/js/material-fab-speed-dial.js` & `mia-accounting-1.3.2/src/accounting/static/js/material-fab-speed-dial.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/static/js/option-form.js` & `mia-accounting-1.3.2/src/accounting/static/js/option-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/static/js/original-line-item-selector.js` & `mia-accounting-1.3.2/src/accounting/static/js/original-line-item-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/static/js/period-chooser.js` & `mia-accounting-1.3.2/src/accounting/static/js/period-chooser.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/template_filters.py` & `mia-accounting-1.3.2/src/accounting/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/template_globals.py` & `mia-accounting-1.3.2/src/accounting/template_globals.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/account/create.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/account/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/account/detail.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/account/edit.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/account/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/account/include/form.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/account/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/account/list.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/account/order.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/account/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/base-account/detail.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/base-account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/base-account/list.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/base-account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/base.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/currency/create.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/currency/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/currency/detail.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/currency/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/currency/edit.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/currency/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/currency/include/form.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/currency/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/currency/list.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/currency/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/include/nav.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/include/nav.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/include/pagination.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/include/pagination.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/create.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/detail.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/edit.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/detail.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form-currency.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form-line-item.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form-line-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/form.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/order.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/create.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/detail.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/edit.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/receipt/include/form.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/create.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/detail.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/edit.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/journal-entry/transfer/include/form.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/option/detail.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/option/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/option/form.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/option/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/form-recurring-item.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/form-recurring-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/balance-sheet.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/balance-sheet.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/balance-sheet-section.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/balance-sheet-section.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/ledger-row-desktop.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/ledger-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/ledger-row-mobile.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/ledger-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/period-chooser.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/period-chooser.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/search-modal.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/search-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/include/toolbar-buttons.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/toolbar-buttons.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/income-expenses.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/income-expenses.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/income-statement.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/income-statement.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/journal.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/journal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/ledger.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/ledger.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/search.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/search.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/trial-balance.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/trial-balance.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/unapplied-accounts.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/unapplied-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/report/unapplied.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/report/unapplied.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/unmatched-offset/dashboard.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/unmatched-offset/dashboard.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/templates/accounting/unmatched-offset/list.html` & `mia-accounting-1.3.2/src/accounting/templates/accounting/unmatched-offset/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/translations/accounting.pot` & `mia-accounting-1.3.2/src/accounting/translations/accounting.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo` & `mia-accounting-1.3.2/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po` & `mia-accounting-1.3.2/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo` & `mia-accounting-1.3.2/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po` & `mia-accounting-1.3.2/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/unmatched_offset/__init__.py` & `mia-accounting-1.3.2/src/accounting/unmatched_offset/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/unmatched_offset/queries.py` & `mia-accounting-1.3.2/src/accounting/unmatched_offset/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/unmatched_offset/views.py` & `mia-accounting-1.3.2/src/accounting/unmatched_offset/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/__init__.py` & `mia-accounting-1.3.2/src/accounting/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/cast.py` & `mia-accounting-1.3.2/src/accounting/utils/cast.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/current_account.py` & `mia-accounting-1.3.2/src/accounting/utils/current_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/flash_errors.py` & `mia-accounting-1.3.2/src/accounting/utils/flash_errors.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/journal_entry_types.py` & `mia-accounting-1.3.2/src/accounting/utils/journal_entry_types.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/next_uri.py` & `mia-accounting-1.3.2/src/accounting/utils/next_uri.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/offset_alias.py` & `mia-accounting-1.3.2/src/accounting/utils/offset_alias.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/offset_matcher.py` & `mia-accounting-1.3.2/src/accounting/utils/offset_matcher.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/options.py` & `mia-accounting-1.3.2/src/accounting/utils/options.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/pagination.py` & `mia-accounting-1.3.2/src/accounting/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/permission.py` & `mia-accounting-1.3.2/src/accounting/utils/permission.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/query.py` & `mia-accounting-1.3.2/src/accounting/utils/query.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/random_id.py` & `mia-accounting-1.3.2/src/accounting/utils/random_id.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/strip_text.py` & `mia-accounting-1.3.2/src/accounting/utils/strip_text.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/unapplied.py` & `mia-accounting-1.3.2/src/accounting/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/accounting/utils/user.py` & `mia-accounting-1.3.2/src/accounting/utils/user.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/src/mia_accounting.egg-info/PKG-INFO` & `mia-accounting-1.3.2/src/mia_accounting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
 Keywords: mia,accounting,flask
```

### Comparing `mia-accounting-1.3.1/src/mia_accounting.egg-info/SOURCES.txt` & `mia-accounting-1.3.2/src/mia_accounting.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,15 @@
 src/mia_accounting.egg-info/PKG-INFO
 src/mia_accounting.egg-info/SOURCES.txt
 src/mia_accounting.egg-info/dependency_links.txt
 src/mia_accounting.egg-info/requires.txt
 src/mia_accounting.egg-info/top_level.txt
 tests/babel-utils-test-site.py
 tests/babel-utils.py
+tests/make-sample.py
 tests/test_account.py
 tests/test_base_account.py
 tests/test_commands.py
 tests/test_currency.py
 tests/test_description_editor.py
 tests/test_journal_entry.py
 tests/test_offset.py
@@ -227,17 +228,20 @@
 tests/test_unmatched_offset.py
 tests/test_utils.py
 tests/testlib.py
 tests/testlib_journal_entry.py
 tests/test_site/__init__.py
 tests/test_site/auth.py
 tests/test_site/locale.py
+tests/test_site/reset.py
+tests/test_site/data/sample.json
 tests/test_site/static/favicon.svg
 tests/test_site/templates/base.html
 tests/test_site/templates/home.html
 tests/test_site/templates/login.html
+tests/test_site/templates/reset.html
 tests/test_site/translations/babel.cfg
 tests/test_site/translations/messages.pot
 tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
 tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
 tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
 tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
```

### Comparing `mia-accounting-1.3.1/tests/babel-utils-test-site.py` & `mia-accounting-1.3.2/tests/babel-utils-test-site.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,9 +125,9 @@
         f.seek(0)
         f.write(content)
 
 
 main.add_command(babel_extract)
 main.add_command(babel_compile)
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `mia-accounting-1.3.1/tests/babel-utils.py` & `mia-accounting-1.3.2/tests/babel-utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,9 +125,9 @@
         f.seek(0)
         f.write(content)
 
 
 main.add_command(babel_extract)
 main.add_command(babel_compile)
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `mia-accounting-1.3.1/tests/test_account.py` & `mia-accounting-1.3.2/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/tests/test_base_account.py` & `mia-accounting-1.3.2/tests/test_base_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/tests/test_commands.py` & `mia-accounting-1.3.2/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/tests/test_currency.py` & `mia-accounting-1.3.2/tests/test_currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/tests/test_description_editor.py` & `mia-accounting-1.3.2/tests/test_description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/tests/test_journal_entry.py` & `mia-accounting-1.3.2/tests/test_journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/tests/test_offset.py` & `mia-accounting-1.3.2/tests/test_offset.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 
         with self.app.app_context():
             from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
 
         self.client, self.csrf_token = get_client(self.app, "editor")
-        self.data: OffsetTestData = OffsetTestData(
-            self.app, self.client, self.csrf_token)
+        self.data: OffsetTestData = OffsetTestData(self.app, "editor")
+        self.data.populate()
 
     def test_add_receivable_offset(self) -> None:
         """Tests to add the receivable offset.
 
         :return: None.
         """
         from accounting.models import Account, JournalEntry
```

### Comparing `mia-accounting-1.3.1/tests/test_option.py` & `mia-accounting-1.3.2/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/tests/test_report.py` & `mia-accounting-1.3.2/tests/test_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
         """
         client, csrf_token = get_client(self.app, "nobody")
-        ReportTestData(self.app, self.client, self.csrf_token)
+        ReportTestData(self.app, "editor").populate()
         response: httpx.Response
 
         response = client.get(PREFIX)
         self.assertEqual(response.status_code, 403)
 
         response = client.get(f"{PREFIX}?as=csv")
         self.assertEqual(response.status_code, 403)
@@ -126,15 +126,15 @@
 
     def test_viewer(self) -> None:
         """Test the permission as viewer.
 
         :return: None.
         """
         client, csrf_token = get_client(self.app, "viewer")
-        ReportTestData(self.app, self.client, self.csrf_token)
+        ReportTestData(self.app, "editor").populate()
         response: httpx.Response
 
         response = client.get(PREFIX)
         self.assertEqual(response.status_code, 200)
 
         response = client.get(f"{PREFIX}?as=csv")
         self.assertEqual(response.status_code, 200)
@@ -211,15 +211,15 @@
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
     def test_editor(self) -> None:
         """Test the permission as editor.
 
         :return: None.
         """
-        ReportTestData(self.app, self.client, self.csrf_token)
+        ReportTestData(self.app, "editor").populate()
         response: httpx.Response
 
         response = self.client.get(PREFIX)
         self.assertEqual(response.status_code, 200)
 
         response = self.client.get(f"{PREFIX}?as=csv")
         self.assertEqual(response.status_code, 200)
```

### Comparing `mia-accounting-1.3.1/tests/test_site/__init__.py` & `mia-accounting-1.3.2/tests/test_site/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,17 @@
 
     from . import locale
     locale.init_app(app)
 
     from . import auth
     auth.init_app(app)
 
+    from . import reset
+    reset.init_app(app)
+
     class UserUtilities(accounting.UserUtilityInterface[auth.User]):
 
         def can_view(self) -> bool:
             return auth.current_user() is not None \
                 and auth.current_user().username in ["viewer", "editor",
                                                      "admin"]
```

### Comparing `mia-accounting-1.3.1/tests/test_site/auth.py` & `mia-accounting-1.3.2/tests/test_site/auth.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/tests/test_site/locale.py` & `mia-accounting-1.3.2/tests/test_site/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/tests/test_site/static/favicon.svg` & `mia-accounting-1.3.2/tests/test_site/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/tests/test_site/templates/base.html` & `mia-accounting-1.3.2/tests/test_site/templates/base.html`

 * *Files 6% similar despite different names*

```diff
@@ -68,14 +68,22 @@
                   <input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
                   <button class="btn dropdown-item" type="submit">
                     <i class="fa-solid fa-right-from-bracket"></i>
                     {{ _("Log Out") }}
                   </button>
                 </form>
               </li>
+              {% if current_user().username == "admin" %}
+                <li>
+                  <a class="dropdown-item {% if request.endpoint and request.endpoint.startswith("reset.") %} active {% endif %}" href="{{ url_for("reset.reset-page") }}">
+                    <i class="fa-solid fa-rotate-right"></i>
+                    {{ _("Reset") }}
+                  </a>
+                </li>
+              {% endif %}
             </ul>
           </li>
         {% else %}
           <li class="nav-item">
             <a class="nav-link" href="{{ url_for("auth.login") }}">
               <i class="fa-solid fa-right-to-bracket"></i>
               {{ _("Log In") }}
```

#### html2text {}

```diff
@@ -21,14 +21,18 @@
 , filename="favicon.svg") }}">
 home") }}">  {{ _("Home") }}
 
     * {% include "accounting/include/nav.html" %}
     * {% if current_user() is not none %}
     *   {{ current_user().username }}
           o logout") }}" method="post">    {{ _("Log Out") }}
+{% if current_user().username == "admin" %}
+") %} active {% endif %}" href="{{ url_for("reset.reset-page") }}">  {{ _
+("Reset") }}
+{% endif %}
 {% else %}
 login") }}">  {{ _("Log In") }}
 {% endif %}
 
 set-locale") }}" method="post">
     * {% for locale_code, locale_name in get_all_linguas().items() %}
     *  {{ locale_name }}
```

### Comparing `mia-accounting-1.3.1/tests/test_site/templates/home.html` & `mia-accounting-1.3.2/tests/test_site/templates/home.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/tests/test_site/templates/login.html` & `mia-accounting-1.3.2/tests/test_site/templates/login.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/tests/test_site/translations/messages.pot` & `mia-accounting-1.3.2/tests/test_site/translations/messages.pot`

 * *Files 21% similar despite different names*

```diff
@@ -4,41 +4,53 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-11 22:18+0800\n"
+"POT-Creation-Date: 2023-04-12 17:59+0800\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
+#: tests/test_site/reset.py:55
+msgid "The sample data are emptied and reset successfully."
+msgstr ""
+
+#: tests/test_site/reset.py:68
+msgid "The database is emptied successfully."
+msgstr ""
+
 #: tests/test_site/templates/base.html:23
 msgid "en"
 msgstr ""
 
 #: tests/test_site/templates/base.html:46
 msgid "Home"
 msgstr ""
 
 #: tests/test_site/templates/base.html:71
 msgid "Log Out"
 msgstr ""
 
-#: tests/test_site/templates/base.html:81
+#: tests/test_site/templates/base.html:79
+msgid "Reset"
+msgstr ""
+
+#: tests/test_site/templates/base.html:89
 #: tests/test_site/templates/login.html:24
 msgid "Log In"
 msgstr ""
 
-#: tests/test_site/templates/base.html:122
+#: tests/test_site/templates/base.html:130
 msgid "Error:"
 msgstr ""
 
 #: tests/test_site/templates/home.html:24
 msgid "Mia! Accounting Live Demonstration"
 msgstr ""
 
@@ -68,7 +80,31 @@
 msgid "Administrator"
 msgstr ""
 
 #: tests/test_site/templates/login.html:36
 msgid "Nobody"
 msgstr ""
 
+#: tests/test_site/templates/reset.html:24
+msgid "Reset Database"
+msgstr ""
+
+#: tests/test_site/templates/reset.html:28
+msgid ""
+"Warning: All the current accounting data will be deleted.  This cannot be"
+" undone.  Please backup your database first."
+msgstr ""
+
+#: tests/test_site/templates/reset.html:30
+msgid ""
+"Database reset is provided by the live demonstration.  This is not part "
+"of the Mia! Accounting project."
+msgstr ""
+
+#: tests/test_site/templates/reset.html:37
+msgid "Empty the Database"
+msgstr ""
+
+#: tests/test_site/templates/reset.html:45
+msgid "Empty and reset the Sample Data"
+msgstr ""
+
```

### Comparing `mia-accounting-1.3.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo` & `mia-accounting-1.3.2/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,28 +1,39 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: mia-accounting-test-site 1.0.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-11 22:18+0800\n"
-"PO-Revision-Date: 2023-04-11 22:18+0800\n"
+"POT-Creation-Date: 2023-04-12 17:59+0800\n"
+"PO-Revision-Date: 2023-04-12 18:00+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hans\n"
 "Language-Team: zh_Hans <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "Administrator"
 msgstr "管理者"
 
+msgid ""
+"Database reset is provided by the live demonstration.  This is not part of "
+"the Mia! Accounting project."
+msgstr "数据库重设是示范站的功能，不是 Mia! Accounting 的功能。"
+
 msgid "Editor"
 msgstr "记帐者"
 
+msgid "Empty and reset the Sample Data"
+msgstr "清空并重设范例数据"
+
+msgid "Empty the Database"
+msgstr "清空数据库"
+
 msgid "Error:"
 msgstr "错误："
 
 msgid "Home"
 msgstr "首页"
 
 msgid "Log In"
@@ -33,25 +44,42 @@
 
 msgid "Mia! Accounting Live Demonstration"
 msgstr "Mia! Accounting 示范站"
 
 msgid "Nobody"
 msgstr "没有权限者"
 
+msgid "Reset"
+msgstr "重设"
+
+msgid "Reset Database"
+msgstr "数据库重设"
+
+msgid "The database is emptied successfully."
+msgstr "数据库已清空。"
+
+msgid "The sample data are emptied and reset successfully."
+msgstr "范例数据已清空重设。"
+
 msgid ""
 "This is the live demonstration of the Mia! Accounting project.  Please <a "
 "href=\"/login?next=%%2Faccounting\">log in</a> to continue."
 msgstr ""
 "这是 Mia! Accounting 项目的示范站。请先<a href=\"/login?next=%"
 "%2Faccounting\">登录</a>。"
 
 msgid "Viewer"
 msgstr "读报表者"
 
 msgid ""
+"Warning: All the current accounting data will be deleted.  This cannot be "
+"undone.  Please backup your database first."
+msgstr "警告：现有数据会全部删除，无法复原。请先备份您的数据。"
+
+msgid ""
 "You may also want to check the <a href=\"https://mia-accounting.readthedocs."
 "io\">full documentation</a> and the <a href=\"https://github.com/imacat/mia-"
 "accounting\">Github repository</a>."
 msgstr ""
 "详情请参阅<a href=\"https://mia-accounting.readthedocs.io\">完整说明文档</a>"
 "与<a href=\"https://github.com/imacat/mia-accounting\">Github 项目库</a>。"
```

### Comparing `mia-accounting-1.3.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po` & `mia-accounting-1.3.2/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files 25% similar despite different names*

```diff
@@ -5,75 +5,111 @@
 # project.
 # imacat <imacat@mail.imacat.idv.tw>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: mia-accounting-test-site 1.0.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-11 22:18+0800\n"
-"PO-Revision-Date: 2023-04-11 22:18+0800\n"
+"POT-Creation-Date: 2023-04-12 17:59+0800\n"
+"PO-Revision-Date: 2023-04-12 18:00+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
-"Language: zh_Hans\n"
-"Language-Team: zh_Hans <imacat@mail.imacat.idv.tw>\n"
+"Language: zh_Hant\n"
+"Language-Team: zh_Hant <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
+#: tests/test_site/reset.py:55
+msgid "The sample data are emptied and reset successfully."
+msgstr "範例資料已清空重設。"
+
+#: tests/test_site/reset.py:68
+msgid "The database is emptied successfully."
+msgstr "資料庫已清空。"
+
 #: tests/test_site/templates/base.html:23
 msgid "en"
-msgstr "zh-Hans"
+msgstr "zh-Hant"
 
 #: tests/test_site/templates/base.html:46
 msgid "Home"
-msgstr "首页"
+msgstr "首頁"
 
 #: tests/test_site/templates/base.html:71
 msgid "Log Out"
-msgstr "注销"
+msgstr "登出"
+
+#: tests/test_site/templates/base.html:79
+msgid "Reset"
+msgstr "重設"
 
-#: tests/test_site/templates/base.html:81
+#: tests/test_site/templates/base.html:89
 #: tests/test_site/templates/login.html:24
 msgid "Log In"
-msgstr "登录"
+msgstr "登入"
 
-#: tests/test_site/templates/base.html:122
+#: tests/test_site/templates/base.html:130
 msgid "Error:"
-msgstr "错误："
+msgstr "錯誤："
 
 #: tests/test_site/templates/home.html:24
 msgid "Mia! Accounting Live Demonstration"
-msgstr "Mia! Accounting 示范站"
+msgstr "Mia! Accounting 示範站"
 
 #: tests/test_site/templates/home.html:28
 #, python-format
 msgid ""
 "This is the live demonstration of the Mia! Accounting project.  Please <a"
 " href=\"/login?next=%%2Faccounting\">log in</a> to continue."
-msgstr "这是 Mia! Accounting 项目的示范站。请先<a href=\"/login?next=%%2Faccounting\">登录</a>。"
+msgstr "這是 Mia! Accounting 專案的示範站。請先<a href=\"/login?next=%%2Faccounting\">登入</a>。"
 
 #: tests/test_site/templates/home.html:30
 msgid ""
 "You may also want to check the <a href=\"https://mia-"
 "accounting.readthedocs.io\">full documentation</a> and the <a "
 "href=\"https://github.com/imacat/mia-accounting\">Github repository</a>."
 msgstr ""
-"详情请参阅<a href=\"https://mia-accounting.readthedocs.io\">完整说明文档</a>与<a "
-"href=\"https://github.com/imacat/mia-accounting\">Github 项目库</a>。"
+"詳情請參閱<a href=\"https://mia-accounting.readthedocs.io\">完整說明文件</a>與<a "
+"href=\"https://github.com/imacat/mia-accounting\">Github 專案庫</a>。"
 
 #: tests/test_site/templates/login.html:33
 msgid "Viewer"
-msgstr "读报表者"
+msgstr "讀報表者"
 
 #: tests/test_site/templates/login.html:34
 msgid "Editor"
-msgstr "记帐者"
+msgstr "記帳者"
 
 #: tests/test_site/templates/login.html:35
 msgid "Administrator"
 msgstr "管理者"
 
 #: tests/test_site/templates/login.html:36
 msgid "Nobody"
-msgstr "没有权限者"
+msgstr "沒有權限者"
+
+#: tests/test_site/templates/reset.html:24
+msgid "Reset Database"
+msgstr "資料庫重設"
+
+#: tests/test_site/templates/reset.html:28
+msgid ""
+"Warning: All the current accounting data will be deleted.  This cannot be"
+" undone.  Please backup your database first."
+msgstr "警告：現有資料會全部刪除，無法復原。請先備份您的資料。"
+
+#: tests/test_site/templates/reset.html:30
+msgid ""
+"Database reset is provided by the live demonstration.  This is not part "
+"of the Mia! Accounting project."
+msgstr "資料庫重設是示範站的功能，不是 Mia! Accounting 的功能。"
+
+#: tests/test_site/templates/reset.html:37
+msgid "Empty the Database"
+msgstr "清空資料庫"
+
+#: tests/test_site/templates/reset.html:45
+msgid "Empty and reset the Sample Data"
+msgstr "清空並重設範例資料"
```

### Comparing `mia-accounting-1.3.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo` & `mia-accounting-1.3.2/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,28 +1,39 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: mia-accounting-test-site 1.0.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-11 22:18+0800\n"
-"PO-Revision-Date: 2023-04-11 22:18+0800\n"
+"POT-Creation-Date: 2023-04-12 17:59+0800\n"
+"PO-Revision-Date: 2023-04-12 18:00+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hant\n"
 "Language-Team: zh_Hant <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "Administrator"
 msgstr "管理者"
 
+msgid ""
+"Database reset is provided by the live demonstration.  This is not part of "
+"the Mia! Accounting project."
+msgstr "資料庫重設是示範站的功能，不是 Mia! Accounting 的功能。"
+
 msgid "Editor"
 msgstr "記帳者"
 
+msgid "Empty and reset the Sample Data"
+msgstr "清空並重設範例資料"
+
+msgid "Empty the Database"
+msgstr "清空資料庫"
+
 msgid "Error:"
 msgstr "錯誤："
 
 msgid "Home"
 msgstr "首頁"
 
 msgid "Log In"
@@ -33,25 +44,42 @@
 
 msgid "Mia! Accounting Live Demonstration"
 msgstr "Mia! Accounting 示範站"
 
 msgid "Nobody"
 msgstr "沒有權限者"
 
+msgid "Reset"
+msgstr "重設"
+
+msgid "Reset Database"
+msgstr "資料庫重設"
+
+msgid "The database is emptied successfully."
+msgstr "資料庫已清空。"
+
+msgid "The sample data are emptied and reset successfully."
+msgstr "範例資料已清空重設。"
+
 msgid ""
 "This is the live demonstration of the Mia! Accounting project.  Please <a "
 "href=\"/login?next=%%2Faccounting\">log in</a> to continue."
 msgstr ""
 "這是 Mia! Accounting 專案的示範站。請先<a href=\"/login?next=%"
 "%2Faccounting\">登入</a>。"
 
 msgid "Viewer"
 msgstr "讀報表者"
 
 msgid ""
+"Warning: All the current accounting data will be deleted.  This cannot be "
+"undone.  Please backup your database first."
+msgstr "警告：現有資料會全部刪除，無法復原。請先備份您的資料。"
+
+msgid ""
 "You may also want to check the <a href=\"https://mia-accounting.readthedocs."
 "io\">full documentation</a> and the <a href=\"https://github.com/imacat/mia-"
 "accounting\">Github repository</a>."
 msgstr ""
 "詳情請參閱<a href=\"https://mia-accounting.readthedocs.io\">完整說明文件</a>"
 "與<a href=\"https://github.com/imacat/mia-accounting\">Github 專案庫</a>。"
```

### Comparing `mia-accounting-1.3.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po` & `mia-accounting-1.3.2/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files 25% similar despite different names*

```diff
@@ -5,75 +5,111 @@
 # project.
 # imacat <imacat@mail.imacat.idv.tw>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: mia-accounting-test-site 1.0.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-11 22:18+0800\n"
-"PO-Revision-Date: 2023-04-11 22:18+0800\n"
+"POT-Creation-Date: 2023-04-12 17:59+0800\n"
+"PO-Revision-Date: 2023-04-12 18:00+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
-"Language: zh_Hant\n"
-"Language-Team: zh_Hant <imacat@mail.imacat.idv.tw>\n"
+"Language: zh_Hans\n"
+"Language-Team: zh_Hans <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
+#: tests/test_site/reset.py:55
+msgid "The sample data are emptied and reset successfully."
+msgstr "范例数据已清空重设。"
+
+#: tests/test_site/reset.py:68
+msgid "The database is emptied successfully."
+msgstr "数据库已清空。"
+
 #: tests/test_site/templates/base.html:23
 msgid "en"
-msgstr "zh-Hant"
+msgstr "zh-Hans"
 
 #: tests/test_site/templates/base.html:46
 msgid "Home"
-msgstr "首頁"
+msgstr "首页"
 
 #: tests/test_site/templates/base.html:71
 msgid "Log Out"
-msgstr "登出"
+msgstr "注销"
+
+#: tests/test_site/templates/base.html:79
+msgid "Reset"
+msgstr "重设"
 
-#: tests/test_site/templates/base.html:81
+#: tests/test_site/templates/base.html:89
 #: tests/test_site/templates/login.html:24
 msgid "Log In"
-msgstr "登入"
+msgstr "登录"
 
-#: tests/test_site/templates/base.html:122
+#: tests/test_site/templates/base.html:130
 msgid "Error:"
-msgstr "錯誤："
+msgstr "错误："
 
 #: tests/test_site/templates/home.html:24
 msgid "Mia! Accounting Live Demonstration"
-msgstr "Mia! Accounting 示範站"
+msgstr "Mia! Accounting 示范站"
 
 #: tests/test_site/templates/home.html:28
 #, python-format
 msgid ""
 "This is the live demonstration of the Mia! Accounting project.  Please <a"
 " href=\"/login?next=%%2Faccounting\">log in</a> to continue."
-msgstr "這是 Mia! Accounting 專案的示範站。請先<a href=\"/login?next=%%2Faccounting\">登入</a>。"
+msgstr "这是 Mia! Accounting 项目的示范站。请先<a href=\"/login?next=%%2Faccounting\">登录</a>。"
 
 #: tests/test_site/templates/home.html:30
 msgid ""
 "You may also want to check the <a href=\"https://mia-"
 "accounting.readthedocs.io\">full documentation</a> and the <a "
 "href=\"https://github.com/imacat/mia-accounting\">Github repository</a>."
 msgstr ""
-"詳情請參閱<a href=\"https://mia-accounting.readthedocs.io\">完整說明文件</a>與<a "
-"href=\"https://github.com/imacat/mia-accounting\">Github 專案庫</a>。"
+"详情请参阅<a href=\"https://mia-accounting.readthedocs.io\">完整说明文档</a>与<a "
+"href=\"https://github.com/imacat/mia-accounting\">Github 项目库</a>。"
 
 #: tests/test_site/templates/login.html:33
 msgid "Viewer"
-msgstr "讀報表者"
+msgstr "读报表者"
 
 #: tests/test_site/templates/login.html:34
 msgid "Editor"
-msgstr "記帳者"
+msgstr "记帐者"
 
 #: tests/test_site/templates/login.html:35
 msgid "Administrator"
 msgstr "管理者"
 
 #: tests/test_site/templates/login.html:36
 msgid "Nobody"
-msgstr "沒有權限者"
+msgstr "没有权限者"
+
+#: tests/test_site/templates/reset.html:24
+msgid "Reset Database"
+msgstr "数据库重设"
+
+#: tests/test_site/templates/reset.html:28
+msgid ""
+"Warning: All the current accounting data will be deleted.  This cannot be"
+" undone.  Please backup your database first."
+msgstr "警告：现有数据会全部删除，无法复原。请先备份您的数据。"
+
+#: tests/test_site/templates/reset.html:30
+msgid ""
+"Database reset is provided by the live demonstration.  This is not part "
+"of the Mia! Accounting project."
+msgstr "数据库重设是示范站的功能，不是 Mia! Accounting 的功能。"
+
+#: tests/test_site/templates/reset.html:37
+msgid "Empty the Database"
+msgstr "清空数据库"
+
+#: tests/test_site/templates/reset.html:45
+msgid "Empty and reset the Sample Data"
+msgstr "清空并重设范例数据"
```

### Comparing `mia-accounting-1.3.1/tests/test_unmatched_offset.py` & `mia-accounting-1.3.2/tests/test_unmatched_offset.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
         """
         client, csrf_token = get_client(self.app, "nobody")
-        DifferentTestData(self.app, self.client, self.csrf_token)
+        DifferentTestData(self.app, "nobody").populate()
         response: httpx.Response
 
         response = client.get(PREFIX)
         self.assertEqual(response.status_code, 403)
 
         response = client.get(f"{PREFIX}/{Accounts.PAYABLE}")
         self.assertEqual(response.status_code, 403)
@@ -69,15 +69,15 @@
 
     def test_viewer(self) -> None:
         """Test the permission as viewer.
 
         :return: None.
         """
         client, csrf_token = get_client(self.app, "viewer")
-        DifferentTestData(self.app, self.client, self.csrf_token)
+        DifferentTestData(self.app, "viewer").populate()
         response: httpx.Response
 
         response = client.get(PREFIX)
         self.assertEqual(response.status_code, 403)
 
         response = client.get(f"{PREFIX}/{Accounts.PAYABLE}")
         self.assertEqual(response.status_code, 403)
@@ -87,15 +87,15 @@
         self.assertEqual(response.status_code, 403)
 
     def test_editor(self) -> None:
         """Test the permission as editor.
 
         :return: None.
         """
-        DifferentTestData(self.app, self.client, self.csrf_token)
+        DifferentTestData(self.app, "editor").populate()
         response: httpx.Response
 
         response = self.client.get(PREFIX)
         self.assertEqual(response.status_code, 200)
 
         response = self.client.get(f"{PREFIX}/{Accounts.PAYABLE}")
         self.assertEqual(response.status_code, 200)
@@ -128,16 +128,16 @@
     def test_different(self) -> None:
         """Tests to match against different descriptions and amounts.
 
         :return: None.
         """
         from accounting.models import Account, JournalEntryLineItem
         from accounting.utils.offset_matcher import OffsetMatcher
-        data: DifferentTestData \
-            = DifferentTestData(self.app, self.client, self.csrf_token)
+        data: DifferentTestData = DifferentTestData(self.app, "editor")
+        data.populate()
         account: Account | None
         line_item: JournalEntryLineItem | None
         matcher: OffsetMatcher
         list_uri: str
         match_uri: str
         response: httpx.Response
 
@@ -244,16 +244,16 @@
     def test_same(self) -> None:
         """Tests to match against same descriptions and amounts.
 
         :return: None.
         """
         from accounting.models import Account, JournalEntryLineItem
         from accounting.utils.offset_matcher import OffsetMatcher
-        data: SameTestData \
-            = SameTestData(self.app, self.client, self.csrf_token)
+        data: SameTestData = SameTestData(self.app, "editor")
+        data.populate()
         account: Account | None
         line_item: JournalEntryLineItem | None
         matcher: OffsetMatcher
         list_uri: str
         match_uri: str
         response: httpx.Response
 
@@ -479,22 +479,20 @@
             10, [JournalEntryCurrencyData(
                 "USD", [self.l_p_of2d, self.l_p_of3d, self.l_p_of4d],
                 [self.l_p_of2c, self.l_p_of3c, self.l_p_of4c])])
         self.j_p_of3: JournalEntryData = JournalEntryData(
             5, [JournalEntryCurrencyData(
                 "USD", [self.l_p_of5d], [self.l_p_of5c])])
 
-        self._set_need_offset({Accounts.RECEIVABLE, Accounts.PAYABLE}, False)
         self._add_journal_entry(self.j_r_of1)
         self._add_journal_entry(self.j_r_of2)
         self._add_journal_entry(self.j_r_of3)
         self._add_journal_entry(self.j_p_of1)
         self._add_journal_entry(self.j_p_of2)
         self._add_journal_entry(self.j_p_of3)
-        self._set_need_offset({Accounts.RECEIVABLE, Accounts.PAYABLE}, True)
 
 
 class SameTestData(BaseTestData):
     """The test data with same descriptions and amounts."""
 
     def _init_data(self) -> None:
         # Receivable original line items
@@ -521,16 +519,14 @@
         self.l_p_or4d, self.l_p_or4c = self._add_simple_journal_entry(
             30, "USD", "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
         self.l_p_or5d, self.l_p_or5c = self._add_simple_journal_entry(
             20, "USD", "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
         self.l_p_or6d, self.l_p_or6c = self._add_simple_journal_entry(
             10, "USD", "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
 
-        self._set_need_offset({Accounts.RECEIVABLE, Accounts.PAYABLE}, False)
-
         # Receivable offset items
         self.l_r_of1d, self.l_r_of1c = self._add_simple_journal_entry(
             65, "USD", "Noodles", "100", Accounts.CASH, Accounts.RECEIVABLE)
         self.l_r_of2d, self.l_r_of2c = self._add_simple_journal_entry(
             35, "USD", "Noodles", "100", Accounts.CASH, Accounts.RECEIVABLE)
         self.l_r_of3d, self.l_r_of3c = self._couple(
             "Noodles", "100", Accounts.CASH, Accounts.RECEIVABLE)
@@ -559,10 +555,9 @@
         self.l_p_of4d, self.l_p_of4c = self._add_simple_journal_entry(
             35, "USD", "Steak", "120", Accounts.PAYABLE, Accounts.CASH)
         self.l_p_of5d, self.l_p_of5c = self._add_simple_journal_entry(
             35, "USD", "Steak", "120", Accounts.PAYABLE, Accounts.CASH)
         self.l_p_of6d, self.l_p_of6c = self._add_simple_journal_entry(
             15, "USD", "Steak", "120", Accounts.PAYABLE, Accounts.CASH)
 
-        self._set_need_offset({Accounts.RECEIVABLE, Accounts.PAYABLE}, True)
         self._add_journal_entry(j_r_of3)
         self._add_journal_entry(j_p_of3)
```

### Comparing `mia-accounting-1.3.1/tests/test_utils.py` & `mia-accounting-1.3.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.1/tests/testlib.py` & `mia-accounting-1.3.2/tests/testlib.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,39 +15,44 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The common test libraries.
 
 """
 from __future__ import annotations
 
+import json
 import re
 import typing as t
 from abc import ABC, abstractmethod
 from datetime import date, timedelta
+from secrets import randbelow
 
-from _decimal import Decimal
+from decimal import Decimal
+import sqlalchemy as sa
 
 import httpx
 from flask import Flask, render_template_string
 
 from test_site import create_app, db
+from test_site.auth import User
 
 TEST_SERVER: str = "https://testserver"
 """The test server URI."""
 NEXT_URI: str = "/_next"
 """The next URI."""
 
 
 class Accounts:
     """The shortcuts to the common accounts."""
     CASH: str = "1111-001"
     PETTY_CASH: str = "1112-001"
     BANK: str = "1113-001"
     NOTES_RECEIVABLE: str = "1131-001"
     RECEIVABLE: str = "1141-001"
+    MACHINERY: str = "1441-001"
     PREPAID: str = "1258-001"
     NOTES_PAYABLE: str = "2131-001"
     PAYABLE: str = "2141-001"
     SALES: str = "4111-001"
     SERVICE: str = "4611-001"
     AGENCY: str = "4711-001"
     RENT_EXPENSE: str = "6252-001"
@@ -159,30 +164,30 @@
     assert m is not None
     return int(m.group(1))
 
 
 class JournalEntryLineItemData:
     """The journal entry line item data."""
 
-    def __init__(self, account: str, description: str, amount: str,
+    def __init__(self, account: str, description: str | None, amount: str,
                  original_line_item: JournalEntryLineItemData | None = None):
         """Constructs the journal entry line item data.
 
         :param account: The account code.
         :param description: The description.
         :param amount: The amount.
         :param original_line_item: The original journal entry line item.
         """
         self.journal_entry: JournalEntryData | None = None
         self.id: int = -1
         self.no: int = -1
         self.original_line_item: JournalEntryLineItemData | None \
             = original_line_item
         self.account: str = account
-        self.description: str = description
+        self.description: str | None = description
         self.amount: Decimal = Decimal(amount)
 
     def form(self, prefix: str, debit_credit: str, index: int,
              is_update: bool) -> dict[str, str]:
         """Returns the line item as form data.
 
         :param prefix: The prefix of the form fields.
@@ -290,33 +295,92 @@
             form["note"] = self.note
         return form
 
 
 class BaseTestData(ABC):
     """The base test data."""
 
-    def __init__(self, app: Flask, client: httpx.Client, csrf_token: str):
+    def __init__(self, app: Flask, username: str):
         """Constructs the test data.
 
         :param app: The Flask application.
-        :param client: The client.
-        :param csrf_token: The CSRF token.
+        :param username: The username.
         """
-        self.app: Flask = app
-        self.client: httpx.Client = client
-        self.csrf_token: str = csrf_token
-        self._init_data()
+        self.__app: Flask = app
+        with self.__app.app_context():
+            current_user: User | None = User.query\
+                .filter(User.username == username).first()
+            assert current_user is not None
+            self.__current_user_id: int = current_user.id
+            self.__journal_entries: list[dict[str, t.Any]] = []
+            self.__line_items: list[dict[str, t.Any]] = []
+            self._init_data()
 
     @abstractmethod
     def _init_data(self) -> None:
         """Initializes the test data.
 
         :return: None
         """
 
+    def populate(self) -> None:
+        """Populates the data into the database.
+
+        :return: None
+        """
+        from accounting.models import JournalEntry, JournalEntryLineItem
+        with self.__app.app_context():
+            db.session.execute(sa.insert(JournalEntry), self.__journal_entries)
+            db.session.execute(sa.insert(JournalEntryLineItem),
+                               self.__line_items)
+            db.session.commit()
+
+    def json(self) -> str:
+        """Returns the data as JSON.
+
+        :return: The JSON string.
+        """
+        from accounting.models import Account
+        today: date = date.today()
+
+        def filter_journal_entry(data: dict[str, t.Any]) -> list[t.Any]:
+            """Filters the journal entry data for JSON encoding.
+
+            :param data: The journal entry data.
+            :return: The journal entry data for JSON encoding.
+            """
+            data = data.copy()
+            data["date"] = (today - data["date"]).days
+            del data["created_by_id"]
+            del data["updated_by_id"]
+            return [data[x] for x in ["id", "date", "no", "note"]]
+
+        def filter_line_item(data: dict[str, t.Any]) -> list[t.Any]:
+            """Filters the journal entry line item data for JSON encoding.
+
+            :param data: The journal entry line item data.
+            :return: The journal entry line item data for JSON encoding.
+            """
+            data = data.copy()
+            with self.__app.app_context():
+                data["account_id"] \
+                    = db.session.get(Account, data["account_id"]).code
+            data["amount"] = str(data["amount"])
+            if "original_line_item_id" not in data:
+                data["original_line_item_id"] = None
+            return [data[x] for x in ["id", "journal_entry_id",
+                                      "original_line_item_id", "is_debit",
+                                      "no", "account_id", "currency_code",
+                                      "description", "amount"]]
+
+        return json.dumps(
+            [[filter_journal_entry(x) for x in self.__journal_entries],
+             [filter_line_item(x) for x in self.__line_items]],
+            ensure_ascii=False, separators=(",", ":"))
+
     @staticmethod
     def _couple(description: str, amount: str, debit: str, credit: str) \
             -> tuple[JournalEntryLineItemData, JournalEntryLineItemData]:
         """Returns a couple of debit-credit line items.
 
         :param description: The description.
         :param amount: The amount.
@@ -329,34 +393,90 @@
 
     def _add_journal_entry(self, journal_entry_data: JournalEntryData) -> None:
         """Adds a journal entry.
 
         :param journal_entry_data: The journal entry data.
         :return: None.
         """
-        from accounting.models import JournalEntry
-        store_uri: str = "/accounting/journal-entries/store/transfer"
+        from accounting.models import Account
+        existing_j_id: set[int] = {x["id"] for x in self.__journal_entries}
+        existing_l_id: set[int] = {x["id"] for x in self.__line_items}
+        journal_entry_data.id = self.__new_id(existing_j_id)
+        j_date: date = date.today() - timedelta(days=journal_entry_data.days)
+        self.__journal_entries.append(
+            {"id": journal_entry_data.id,
+             "date": j_date,
+             "no": self.__next_j_no(j_date),
+             "note": journal_entry_data.note,
+             "created_by_id": self.__current_user_id,
+             "updated_by_id": self.__current_user_id})
+        debit_no: int = 0
+        credit_no: int = 0
+        for currency in journal_entry_data.currencies:
+            for line_item in currency.debit:
+                account: Account | None \
+                    = Account.find_by_code(line_item.account)
+                assert account is not None
+                debit_no = debit_no + 1
+                line_item.id = self.__new_id(existing_l_id)
+                data: dict[str, t.Any] \
+                    = {"id": line_item.id,
+                       "journal_entry_id": journal_entry_data.id,
+                       "is_debit": True,
+                       "no": debit_no,
+                       "account_id": account.id,
+                       "currency_code": currency.code,
+                       "description": line_item.description,
+                       "amount": line_item.amount}
+                if line_item.original_line_item is not None:
+                    data["original_line_item_id"] \
+                        = line_item.original_line_item.id
+                self.__line_items.append(data)
+            for line_item in currency.credit:
+                account: Account | None \
+                    = Account.find_by_code(line_item.account)
+                assert account is not None
+                credit_no = credit_no + 1
+                line_item.id = self.__new_id(existing_l_id)
+                data: dict[str, t.Any] \
+                    = {"id": line_item.id,
+                       "journal_entry_id": journal_entry_data.id,
+                       "is_debit": False,
+                       "no": credit_no,
+                       "account_id": account.id,
+                       "currency_code": currency.code,
+                       "description": line_item.description,
+                       "amount": line_item.amount}
+                if line_item.original_line_item is not None:
+                    data["original_line_item_id"] \
+                        = line_item.original_line_item.id
+                self.__line_items.append(data)
+
+    @staticmethod
+    def __new_id(existing_id: set[int]) -> int:
+        """Generates and returns a new random unique ID.
 
-        response: httpx.Response = self.client.post(
-            store_uri, data=journal_entry_data.new_form(self.csrf_token))
-        assert response.status_code == 302
-        journal_entry_id: int \
-            = match_journal_entry_detail(response.headers["Location"])
-        journal_entry_data.id = journal_entry_id
-        with self.app.app_context():
-            journal_entry: JournalEntry | None \
-                = db.session.get(JournalEntry, journal_entry_id)
-            assert journal_entry is not None
-            for i in range(len(journal_entry.currencies)):
-                for j in range(len(journal_entry.currencies[i].debit)):
-                    journal_entry_data.currencies[i].debit[j].id \
-                        = journal_entry.currencies[i].debit[j].id
-                for j in range(len(journal_entry.currencies[i].credit)):
-                    journal_entry_data.currencies[i].credit[j].id \
-                        = journal_entry.currencies[i].credit[j].id
+        :param existing_id: The existing ID.
+        :return: The newly-generated random unique ID.
+        """
+        while True:
+            obj_id: int = 100000000 + randbelow(900000000)
+            if obj_id not in existing_id:
+                existing_id.add(obj_id)
+                return obj_id
+
+    def __next_j_no(self, j_date: date) -> int:
+        """Returns the next journal entry number in a day.
+
+        :param j_date: The journal entry date.
+        :return: The next journal entry number.
+        """
+        existing: set[int] = {x["no"] for x in self.__journal_entries
+                              if x["date"] == j_date}
+        return 1 if len(existing) == 0 else max(existing) + 1
 
     def _add_simple_journal_entry(
             self, days: int, currency: str, description: str, amount: str,
             debit: str, credit: str) \
             -> tuple[JournalEntryLineItemData, JournalEntryLineItemData]:
         """Adds a simple journal entry.
 
@@ -370,24 +490,7 @@
         """
         debit_item, credit_item = self._couple(
             description, amount, debit, credit)
         self._add_journal_entry(JournalEntryData(
             days, [JournalEntryCurrencyData(
                 currency, [debit_item], [credit_item])]))
         return debit_item, credit_item
-
-    def _set_need_offset(self, account_codes: set[str],
-                         is_need_offset: bool) -> None:
-        """Sets whether the line items in some accounts need offset.
-
-        :param account_codes: The account codes.
-        :param is_need_offset: True if the line items in the accounts need
-            offset, or False otherwise.
-        :return:
-        """
-        from accounting.models import Account
-        with self.app.app_context():
-            for code in account_codes:
-                account: Account | None = Account.find_by_code(code)
-                assert account is not None
-                account.is_need_offset = is_need_offset
-            db.session.commit()
```

### Comparing `mia-accounting-1.3.1/tests/testlib_journal_entry.py` & `mia-accounting-1.3.2/tests/testlib_journal_entry.py`

 * *Files identical despite different names*

