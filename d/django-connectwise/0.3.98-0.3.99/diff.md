# Comparing `tmp/django-connectwise-0.3.98.tar.gz` & `tmp/django-connectwise-0.3.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-connectwise-0.3.98.tar", last modified: Fri Aug  7 00:18:28 2020, max compression
+gzip compressed data, was "dist/django-connectwise-0.3.99.tar", last modified: Mon Aug 10 22:35:23 2020, max compression
```

## Comparing `django-connectwise-0.3.98.tar` & `django-connectwise-0.3.99.tar`

### file list

```diff
@@ -1,356 +1,356 @@
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/
--rw-rw-r--   0 sam       (1000) sam       (1000)     1796 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/setup.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/djconnectwise/
--rw-rw-r--   0 sam       (1000) sam       (1000)     5315 2019-12-31 19:19:26.000000 django-connectwise-0.3.98/djconnectwise/callbacks.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     4629 2020-01-01 00:28:18.000000 django-connectwise-0.3.98/djconnectwise/views.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      222 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/apps.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/djconnectwise/migrations/
--rw-rw-r--   0 sam       (1000) sam       (1000)      509 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0075_auto_20180910_1629.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      278 2019-07-18 17:49:22.000000 django-connectwise-0.3.98/djconnectwise/migrations/0093_merge_20190716_1459.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1312 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0062_auto_20180606_1117.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      461 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0042_auto_20171115_1131.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      889 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0031_auto_20170607_2234.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1001 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0025_opportunitypriority.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      427 2020-05-29 19:42:56.000000 django-connectwise-0.3.98/djconnectwise/migrations/0115_agreement_agreement_status.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1172 2019-07-31 17:43:16.000000 django-connectwise-0.3.98/djconnectwise/migrations/0107_auto_20190729_1352.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      300 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0051_merge.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      618 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0007_auto_20170311_1415.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      519 2019-07-18 17:49:22.000000 django-connectwise-0.3.98/djconnectwise/migrations/0094_connectwiseboard_work_role.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1000 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0024_opportunitystage.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      283 2019-07-12 16:30:47.000000 django-connectwise-0.3.98/djconnectwise/migrations/0089_merge_20190711_1100.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      275 2019-07-22 15:39:58.000000 django-connectwise-0.3.98/djconnectwise/migrations/0097_merge_20190718_1325.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      549 2019-12-31 19:19:26.000000 django-connectwise-0.3.98/djconnectwise/migrations/0111_auto_20191204_0838.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    15323 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0001_initial.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1174 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0013_auto_20170403_1203.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      283 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0063_merge_20180611_0905.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      768 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0041_auto_20171030_1047.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      502 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0059_auto_20180518_0811.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      496 2019-07-22 15:39:58.000000 django-connectwise-0.3.98/djconnectwise/migrations/0101_agreement_company.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      367 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0010_remove_project_project_href.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1947 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0050_timeentry.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      283 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0086_merge_20190507_1402.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      621 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0056_auto_20180504_0744.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2653 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0077_item_subtype_type.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      530 2020-02-06 18:50:46.000000 django-connectwise-0.3.98/djconnectwise/migrations/0113_auto_20200204_1054.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2749 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0025_opportunity.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      496 2019-07-12 16:30:47.000000 django-connectwise-0.3.98/djconnectwise/migrations/0088_auto_20190710_0953.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      438 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0015_auto_20170404_1504.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      584 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0012_auto_20170320_1057.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2239 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0065_auto_20180809_1124.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      335 2019-07-16 19:46:55.000000 django-connectwise-0.3.98/djconnectwise/migrations/0092_remove_ticket_work_type.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      722 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0018_auto_20170505_1531.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1045 2019-07-18 17:49:22.000000 django-connectwise-0.3.98/djconnectwise/migrations/0091_workrole.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      477 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0014_company_status.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      425 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0011_company_deleted_flag.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      540 2020-05-29 19:42:56.000000 django-connectwise-0.3.98/djconnectwise/migrations/0116_auto_20200522_1107.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      453 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0016_auto_20170404_1504.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      389 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0078_auto_20181203_1017.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      426 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0047_syncjob_sync_type.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      576 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0017_auto_20170504_2054.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)      684 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0080_auto_20181210_0930.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      556 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0089_merge_20190711_1100.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      791 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0014_company_status.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1181 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0071_auto_20180822_1300.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      722 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0111_auto_20191204_0838.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      914 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0041_auto_20171030_1047.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      704 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0010_remove_project_project_href.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      843 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0044_auto_20171222_1700.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      878 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0099_timeentry_agreement.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      935 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0106_auto_20190722_1524.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      729 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0033_auto_20170616_1251.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1684 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0050_servicenote.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1172 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0050_auto_20180417_1620.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1184 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0091_workrole.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      694 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0060_auto_20180605_0840.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      598 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0092_remove_ticket_work_type.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      741 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0027_auto_20170605_1534.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      768 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0046_auto_20180104_1504.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1473 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0114_auto_20200219_1515.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      754 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0015_auto_20170404_1504.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1601 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0096_agreement.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1362 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0062_auto_20180606_1117.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      903 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0031_auto_20170607_2234.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      816 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0012_auto_20170320_1057.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      632 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0020_merge.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      838 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0082_auto_20190125_1109.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      820 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0090_auto_20190711_1114.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1977 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0050_timeentry.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      945 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0045_auto_20171222_1725.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1143 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0061_auto_20180607_1210.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      899 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0085_auto_20190506_1028.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      795 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0102_auto_20190719_1058.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      890 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0056_auto_20180504_0744.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      718 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0038_auto_20170920_1138.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      733 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0112_syncjob_synchronizer_class.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      872 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0009_member_license_class.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      719 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0042_auto_20171115_1131.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      943 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0039_auto_20170925_1418.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      729 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0002_auto_20170223_2143.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      596 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0086_merge_20190507_1402.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1747 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0077_item_subtype_type.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1585 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0064_auto_20180808_1214.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      841 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0048_project_manager.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      650 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0029_merge.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      833 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0113_auto_20200204_1054.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      741 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0054_auto_20180501_1009.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      750 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0034_auto_20170727_1243.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      591 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0083_delete_callbackentry.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      596 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0063_merge_20180611_0905.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      556 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0068_merge_20180814_1104.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1028 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0037_auto_20170920_0959.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      870 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0058_auto_20180516_1052.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      835 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0075_auto_20180910_1629.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1624 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0103_activitystatus_activitytype.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      945 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0084_auto_20190404_1532.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1114 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0069_auto_20180815_1116.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1284 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0051_opportunitynote.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      791 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0074_auto_20180827_1241.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1362 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0023_auto_20170605_0705.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1174 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0024_opportunitystage.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     2012 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0065_auto_20180809_1124.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1196 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0025_opportunitypriority.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1996 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0108_projectphase.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      576 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0093_merge_20190716_1459.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      735 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0011_company_deleted_flag.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1532 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0035_activity.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1302 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0043_projectstatus.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1056 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0117_auto_20200609_1514.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      761 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0006_auto_20170303_1242.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      648 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0061_auto_20180605_1208.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      803 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0110_project_company.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      766 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0081_auto_20181220_0917.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1334 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0022_opportunitystatus.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      670 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0067_auto_20180813_1355.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      983 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0040_auto_20170926_2145.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      940 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0018_auto_20170505_1531.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      906 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0066_auto_20180814_1046.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      848 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0091_worktype_bill_time.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      790 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0016_auto_20170404_1504.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      897 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0007_auto_20170311_1415.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1116 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0079_auto_20181203_1606.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      789 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0093_auto_20190716_1630.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      737 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0003_auto_20170223_2233.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     7746 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0001_initial.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      831 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0088_auto_20190710_0953.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      606 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0072_remove_callbackentry_member.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      754 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0008_project_status_name.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      851 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0109_ticket_phase.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1423 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0076_auto_20180925_1618.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1070 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0029_auto_20170607_1147.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1595 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0087_auto_20190709_0836.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1418 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0066_slapriority.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      793 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0017_auto_20170504_2054.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1693 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0120_auto_20200721_1617.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1766 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0073_auto_20180824_1446.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      744 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0055_auto_20180501_1022.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      805 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0059_auto_20180518_0811.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      951 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0070_mycompanyother.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      612 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0096_merge_20190718_1102.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      930 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0105_auto_20190722_1444.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      740 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0020_ticket_customer_updated.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      821 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0100_auto_20190718_1417.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      682 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0028_remove_company_company_alias.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      792 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0019_syncjob_entity_name.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      701 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0118_auto_20200623_1016.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      800 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0019_ticket_owner.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      652 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0026_merge.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      700 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0104_auto_20190722_1232.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      178 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     2315 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0025_opportunity.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      840 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0095_connectwiseboard_work_type.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1264 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0107_auto_20190729_1352.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      756 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0004_auto_20170224_1853.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1122 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0087_auto_20190705_1015.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      747 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0119_auto_20200624_1028.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1268 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0013_auto_20170403_1203.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      751 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0057_auto_20180511_1440.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      970 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0032_auto_20170616_1144.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      616 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0052_merge.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      608 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0021_merge.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      713 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0115_agreement_agreement_status.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      745 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0047_syncjob_sync_type.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      827 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0085_auto_20190430_1004.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      909 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0098_auto_20190718_1406.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      617 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0053_merge.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      939 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0005_auto_20170225_0101.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      638 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0051_merge.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      854 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0094_connectwiseboard_work_role.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1404 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0049_auto_20180205_1122.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     2332 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0036_auto_20170823_1417.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      559 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0097_merge_20190718_1325.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      800 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0101_agreement_company.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      670 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0078_auto_20181203_1017.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      630 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0028_merge.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      756 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0116_auto_20200522_1107.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      610 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0030_merge.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1659 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0071_auto_20180822_1300.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      611 2019-07-18 21:27:40.000000 django-connectwise-0.3.98/djconnectwise/migrations/0093_auto_20190716_1630.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      654 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0070_mycompanyother.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1170 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0043_projectstatus.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      307 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0026_merge.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      890 2020-06-16 00:09:59.000000 django-connectwise-0.3.98/djconnectwise/migrations/0117_auto_20200609_1514.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      752 2019-07-23 22:38:23.000000 django-connectwise-0.3.98/djconnectwise/migrations/0105_auto_20190722_1444.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1067 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0079_auto_20181203_1606.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      306 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0029_merge.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      697 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0074_auto_20180827_1241.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1261 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0022_opportunitystatus.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      503 2019-09-11 15:54:41.000000 django-connectwise-0.3.98/djconnectwise/migrations/0110_project_company.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      293 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0053_merge.py
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1688 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0050_servicenote.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      509 2019-07-16 17:10:11.000000 django-connectwise-0.3.98/djconnectwise/migrations/0091_worktype_bill_time.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      417 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0054_auto_20180501_1009.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1731 2020-07-23 20:30:50.000000 django-connectwise-0.3.98/djconnectwise/migrations/0120_auto_20200721_1617.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      903 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0085_auto_20190506_1028.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      471 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0081_auto_20181220_0917.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      296 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0030_merge.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      861 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0045_auto_20171222_1725.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      747 2019-07-23 22:38:23.000000 django-connectwise-0.3.98/djconnectwise/migrations/0106_auto_20190722_1524.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      424 2020-06-23 19:37:28.000000 django-connectwise-0.3.98/djconnectwise/migrations/0118_auto_20200623_1016.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      576 2020-07-14 17:17:58.000000 django-connectwise-0.3.98/djconnectwise/migrations/0119_auto_20200624_1028.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      289 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0052_merge.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      422 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0057_auto_20180511_1440.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      581 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0044_auto_20171222_1700.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      526 2019-07-18 17:49:22.000000 django-connectwise-0.3.98/djconnectwise/migrations/0095_connectwiseboard_work_type.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1586 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0076_auto_20180925_1618.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1351 2020-03-04 17:33:45.000000 django-connectwise-0.3.98/djconnectwise/migrations/0114_auto_20200219_1515.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1089 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0051_opportunitynote.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1085 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0084_auto_20190404_1532.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      832 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0069_auto_20180815_1116.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      653 2019-07-22 15:39:58.000000 django-connectwise-0.3.98/djconnectwise/migrations/0098_auto_20190718_1406.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1217 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0029_auto_20170607_1147.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1232 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0023_auto_20170605_0705.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      502 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0048_project_manager.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      413 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0020_ticket_customer_updated.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1507 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0035_activity.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      574 2019-07-22 15:39:58.000000 django-connectwise-0.3.98/djconnectwise/migrations/0102_auto_20190719_1058.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      571 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0032_auto_20170616_1144.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      437 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0046_auto_20180104_1504.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1061 2019-07-12 16:30:47.000000 django-connectwise-0.3.98/djconnectwise/migrations/0087_auto_20190705_1015.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3313 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0036_auto_20170823_1417.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      301 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0021_merge.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      339 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0072_remove_callbackentry_member.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      420 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0034_auto_20170727_1243.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1469 2019-07-22 15:39:58.000000 django-connectwise-0.3.98/djconnectwise/migrations/0096_agreement.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1234 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0049_auto_20180205_1122.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1730 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0073_auto_20180824_1446.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      404 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0033_auto_20170616_1251.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      492 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0067_auto_20180813_1355.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      427 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0055_auto_20180501_1022.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      291 2019-07-18 21:27:40.000000 django-connectwise-0.3.98/djconnectwise/migrations/0096_merge_20190718_1102.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      535 2019-08-21 20:37:19.000000 django-connectwise-0.3.98/djconnectwise/migrations/0109_ticket_phase.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      515 2019-07-22 15:39:58.000000 django-connectwise-0.3.98/djconnectwise/migrations/0100_auto_20190718_1417.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      513 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0082_auto_20190125_1109.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      409 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0060_auto_20180605_0840.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2178 2019-07-23 22:38:23.000000 django-connectwise-0.3.98/djconnectwise/migrations/0103_activitystatus_activitytype.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      461 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0019_syncjob_entity_name.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      304 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0020_merge.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      554 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0066_auto_20180814_1046.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      306 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0083_delete_callbackentry.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      366 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0028_remove_company_company_alias.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2112 2019-08-21 20:37:19.000000 django-connectwise-0.3.98/djconnectwise/migrations/0108_projectphase.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      424 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0027_auto_20170605_1534.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      436 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0008_project_status_name.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1591 2019-07-12 16:30:47.000000 django-connectwise-0.3.98/djconnectwise/migrations/0087_auto_20190709_0836.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      507 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0009_member_license_class.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      740 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0085_auto_20190430_1004.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      428 2020-01-01 00:28:18.000000 django-connectwise-0.3.98/djconnectwise/migrations/0112_syncjob_synchronizer_class.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1000 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0050_auto_20180417_1620.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1377 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0066_slapriority.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      514 2019-07-12 16:30:47.000000 django-connectwise-0.3.98/djconnectwise/migrations/0090_auto_20190711_1114.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      411 2019-07-23 22:38:23.000000 django-connectwise-0.3.98/djconnectwise/migrations/0104_auto_20190722_1232.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      412 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0002_auto_20170223_2143.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      829 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0037_auto_20170920_0959.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1271 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0061_auto_20180607_1210.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      468 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0019_ticket_owner.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      444 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0006_auto_20170303_1242.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      915 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0039_auto_20170925_1418.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      283 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0068_merge_20180814_1104.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      439 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0004_auto_20170224_1853.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      732 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0005_auto_20170225_0101.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      385 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0061_auto_20180605_1208.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1509 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0064_auto_20180808_1214.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      921 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0040_auto_20170926_2145.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      404 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0080_auto_20181210_0930.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      296 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0028_merge.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      561 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0058_auto_20180516_1052.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      413 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0038_auto_20170920_1138.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      546 2019-07-22 15:39:58.000000 django-connectwise-0.3.98/djconnectwise/migrations/0099_timeentry_agreement.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      409 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/migrations/0003_auto_20170223_2233.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/djconnectwise/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)      408 2020-08-07 00:18:12.000000 django-connectwise-0.3.98/djconnectwise/__pycache__/urls.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    61336 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/__pycache__/models.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     4242 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/__pycache__/views.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      896 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/__pycache__/signals.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    34782 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/__pycache__/api.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     4323 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/__pycache__/callbacks.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     3535 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/__pycache__/utils.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      590 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/__pycache__/apps.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      427 2020-08-07 00:17:58.000000 django-connectwise-0.3.98/djconnectwise/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    73561 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/__pycache__/sync.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    65367 2020-07-23 20:30:50.000000 django-connectwise-0.3.98/djconnectwise/models.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      213 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/urls.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      294 2020-08-07 00:17:44.000000 django-connectwise-0.3.98/djconnectwise/__init__.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/djconnectwise/tests/
--rw-rw-r--   0 sam       (1000) sam       (1000)    49462 2020-07-23 20:30:50.000000 django-connectwise-0.3.98/djconnectwise/tests/fixtures.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    30559 2019-12-31 19:19:26.000000 django-connectwise-0.3.98/djconnectwise/tests/test_api.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3846 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/tests/AnonymousMember.png
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/djconnectwise/tests/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)     1093 2020-08-07 00:18:11.000000 django-connectwise-0.3.98/djconnectwise/tests/__pycache__/mommy_recipes.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      342 2020-08-07 00:18:12.000000 django-connectwise-0.3.98/djconnectwise/tests/__pycache__/urls.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    19229 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/tests/__pycache__/test_models.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    23930 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/tests/__pycache__/test_commands.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     2570 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/tests/__pycache__/test_utils.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    10868 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/tests/__pycache__/fixture_utils.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    30065 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/tests/__pycache__/fixtures.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    72919 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/tests/__pycache__/test_sync.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     3572 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/tests/__pycache__/test_callback.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    15539 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/tests/__pycache__/mocks.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     7221 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/tests/__pycache__/test_views.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      173 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/tests/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    31955 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/tests/__pycache__/test_api.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     2168 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/tests/test_utils.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    21972 2020-07-23 20:30:50.000000 django-connectwise-0.3.98/djconnectwise/tests/test_commands.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      161 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/tests/urls.py
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/tests/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    14171 2020-07-23 20:30:50.000000 django-connectwise-0.3.98/djconnectwise/tests/mocks.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    76499 2020-07-23 20:30:50.000000 django-connectwise-0.3.98/djconnectwise/tests/test_sync.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     4598 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/tests/test_callback.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      731 2019-07-23 22:38:23.000000 django-connectwise-0.3.98/djconnectwise/tests/mommy_recipes.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     8161 2020-07-23 20:30:50.000000 django-connectwise-0.3.98/djconnectwise/tests/fixture_utils.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     6856 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/tests/test_views.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    21909 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/tests/test_models.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    11081 2020-07-23 20:30:50.000000 django-connectwise-0.3.98/djconnectwise/admin.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    86153 2020-08-07 00:17:44.000000 django-connectwise-0.3.98/djconnectwise/sync.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1078 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/signals.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/djconnectwise/management/
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/djconnectwise/management/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)      178 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/management/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/management/__init__.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/djconnectwise/management/commands/
--rw-rw-r--   0 sam       (1000) sam       (1000)      559 2020-06-23 19:37:28.000000 django-connectwise-0.3.98/djconnectwise/management/commands/list_users.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/djconnectwise/management/commands/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)      904 2020-08-07 00:18:09.000000 django-connectwise-0.3.98/djconnectwise/management/commands/__pycache__/list_users.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     6226 2020-08-07 00:18:09.000000 django-connectwise-0.3.98/djconnectwise/management/commands/__pycache__/cwsync.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      187 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/djconnectwise/management/commands/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      460 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/management/commands/callbacks_deleted.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1639 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/management/commands/cwclearoldsyncjobs.py
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/management/commands/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     7297 2020-07-23 20:30:50.000000 django-connectwise-0.3.98/djconnectwise/management/commands/cwsync.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      619 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/management/commands/list_callbacks.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1067 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/management/commands/updateslaexpiretimes.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      466 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/djconnectwise/management/commands/callbacks_registered.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2996 2020-03-05 16:56:09.000000 django-connectwise-0.3.98/djconnectwise/utils.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    42645 2020-07-23 20:30:50.000000 django-connectwise-0.3.98/djconnectwise/api.py
--rw-rw-r--   0 sam       (1000) sam       (1000)       38 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/setup.cfg
--rw-rw-r--   0 sam       (1000) sam       (1000)     4928 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/PKG-INFO
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/django_connectwise.egg-info/
--rw-rw-r--   0 sam       (1000) sam       (1000)    20068 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/django_connectwise.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/django_connectwise.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)     4928 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/django_connectwise.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)       99 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/django_connectwise.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       14 2020-08-07 00:18:28.000000 django-connectwise-0.3.98/django_connectwise.egg-info/top_level.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2020-08-07 00:17:59.000000 django-connectwise-0.3.98/django_connectwise.egg-info/not-zip-safe
--rw-rw-r--   0 sam       (1000) sam       (1000)     3080 2019-08-21 20:37:19.000000 django-connectwise-0.3.98/README.md
--rw-rw-r--   0 sam       (1000) sam       (1000)       85 2019-07-05 20:18:44.000000 django-connectwise-0.3.98/MANIFEST.in
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1796 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/setup.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)       85 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/MANIFEST.in
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     3080 2019-08-21 22:56:20.000000 django-connectwise-0.3.99/README.md
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/djconnectwise/
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     4629 2020-01-06 20:58:00.000000 django-connectwise-0.3.99/djconnectwise/views.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     2996 2020-03-05 01:06:07.000000 django-connectwise-0.3.99/djconnectwise/utils.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    86153 2020-08-10 22:31:22.000000 django-connectwise-0.3.99/djconnectwise/sync.py
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/djconnectwise/migrations/
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      921 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0040_auto_20170926_2145.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1377 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0066_slapriority.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      584 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0012_auto_20170320_1057.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      509 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0075_auto_20180910_1629.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      492 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0067_auto_20180813_1355.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      300 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0051_merge.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      477 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0014_company_status.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      903 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0085_auto_20190506_1028.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      732 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0005_auto_20170225_0101.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1089 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0051_opportunitynote.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      278 2019-07-18 18:57:10.000000 django-connectwise-0.3.99/djconnectwise/migrations/0093_merge_20190716_1459.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1000 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0050_auto_20180417_1620.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      574 2019-08-14 17:00:26.000000 django-connectwise-0.3.99/djconnectwise/migrations/0102_auto_20190719_1058.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      424 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0027_auto_20170605_1534.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)     1731 2020-08-10 22:31:22.000000 django-connectwise-0.3.99/djconnectwise/migrations/0120_auto_20200721_1617.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      611 2019-07-18 20:22:29.000000 django-connectwise-0.3.99/djconnectwise/migrations/0093_auto_20190716_1630.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      502 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0059_auto_20180518_0811.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      507 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0009_member_license_class.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     2749 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0025_opportunity.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      890 2020-06-10 22:14:42.000000 django-connectwise-0.3.99/djconnectwise/migrations/0117_auto_20200609_1514.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      306 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0029_merge.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1085 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0084_auto_20190404_1532.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      576 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0017_auto_20170504_2054.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      540 2020-05-22 23:31:25.000000 django-connectwise-0.3.99/djconnectwise/migrations/0116_auto_20200522_1107.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      291 2019-07-18 20:22:29.000000 django-connectwise-0.3.99/djconnectwise/migrations/0096_merge_20190718_1102.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      740 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0085_auto_20190430_1004.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      509 2019-07-16 21:55:55.000000 django-connectwise-0.3.99/djconnectwise/migrations/0091_worktype_bill_time.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      513 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0082_auto_20190125_1109.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1001 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0025_opportunitypriority.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      413 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0020_ticket_customer_updated.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      554 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0066_auto_20180814_1046.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1688 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0050_servicenote.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     2178 2019-08-14 17:00:26.000000 django-connectwise-0.3.99/djconnectwise/migrations/0103_activitystatus_activitytype.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      409 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0003_auto_20170223_2233.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      304 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0020_merge.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1659 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0071_auto_20180822_1300.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      367 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0010_remove_project_project_href.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      453 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0016_auto_20170404_1504.py
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      624 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0104_auto_20190722_1232.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      821 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0056_auto_20180504_0744.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1417 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0064_auto_20180808_1214.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      840 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0039_auto_20170925_1418.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      701 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0102_auto_20190719_1058.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      666 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0020_ticket_customer_updated.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      910 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0037_auto_20170920_0959.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      555 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0028_merge.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      681 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0047_syncjob_sync_type.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1481 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0073_auto_20180824_1446.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      514 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0063_merge_20180611_0905.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      821 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0105_auto_20190722_1444.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      874 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0040_auto_20170926_2145.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      167 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      798 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0066_auto_20180814_1046.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      764 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0095_connectwiseboard_work_type.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      658 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0038_auto_20170920_1138.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      666 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0034_auto_20170727_1243.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      514 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0068_merge_20180814_1104.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1412 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0096_agreement.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      741 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0091_worktype_bill_time.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1129 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0013_auto_20170403_1203.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      732 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0088_auto_20190710_0953.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      649 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0033_auto_20170616_1251.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      948 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0117_auto_20200609_1514.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1254 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0049_auto_20180205_1122.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      609 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0067_auto_20180813_1355.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1452 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0077_item_subtype_type.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      737 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0012_auto_20170320_1057.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      832 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0098_auto_20190718_1406.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      728 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0101_agreement_company.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      527 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0083_delete_callbackentry.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      821 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0084_auto_20190404_1532.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      757 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0109_ticket_phase.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      563 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0020_merge.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1431 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0087_auto_20190709_0836.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      636 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0042_auto_20171115_1131.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      685 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0074_auto_20180827_1241.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      939 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0071_auto_20180822_1300.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      717 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0085_auto_20190430_1004.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      509 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0093_merge_20190716_1459.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      971 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0069_auto_20180815_1116.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      640 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0111_auto_20191204_0838.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      707 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0019_ticket_owner.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      801 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0007_auto_20170311_1415.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      628 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0010_remove_project_project_href.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      790 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0058_auto_20180516_1052.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1236 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0062_auto_20180606_1117.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      560 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0021_merge.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      739 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0075_auto_20180910_1629.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      626 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0060_auto_20180605_0840.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      847 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0041_auto_20171030_1047.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      566 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0026_merge.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      702 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0016_auto_20170404_1504.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      552 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0053_merge.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     2019 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0036_auto_20170823_1417.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      718 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0017_auto_20170504_2054.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      649 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0115_agreement_agreement_status.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1393 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0035_activity.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      839 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0070_mycompanyother.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      962 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0079_auto_20181203_1606.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      686 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0008_project_status_name.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1276 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0066_slapriority.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      757 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0113_auto_20200204_1054.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      773 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0044_auto_20171222_1700.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      746 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0082_auto_20190125_1109.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1052 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0050_auto_20180417_1620.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      979 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0087_auto_20190705_1015.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      842 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0032_auto_20170616_1144.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      555 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0030_merge.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1722 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0050_timeentry.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      773 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0009_member_license_class.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      558 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0072_remove_callbackentry_member.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      624 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0080_auto_20181210_0930.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1079 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0025_opportunitypriority.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      718 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0014_company_status.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      745 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0048_project_manager.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      756 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0085_auto_20190506_1028.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      671 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0057_auto_20180511_1440.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     5994 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0001_initial.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      688 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0004_auto_20170224_1853.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     2050 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0025_opportunity.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1167 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0051_opportunitynote.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      757 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0094_connectwiseboard_work_role.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      704 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0019_syncjob_entity_name.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      815 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0045_auto_20171222_1725.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1202 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0022_opportunitystatus.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      666 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0119_auto_20200624_1028.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      677 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0054_auto_20180501_1009.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      727 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0110_project_company.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      703 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0116_auto_20200522_1107.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      687 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0055_auto_20180501_1022.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      744 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0090_auto_20190711_1114.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      848 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0005_auto_20170225_0101.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      514 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0089_merge_20190711_1100.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      550 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0092_remove_ticket_work_type.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      602 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0061_auto_20180605_1208.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      700 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0093_auto_20190716_1630.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      674 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0081_auto_20181220_0917.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1402 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0103_activitystatus_activitytype.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1003 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0061_auto_20180607_1210.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1107 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0107_auto_20190729_1352.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      660 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0002_auto_20170223_2143.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      565 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0029_merge.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      637 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0118_auto_20200623_1016.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      548 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0052_merge.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      854 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0018_auto_20170505_1531.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1322 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0114_auto_20200219_1515.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1254 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0076_auto_20180925_1618.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      733 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0059_auto_20180518_0811.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      559 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0051_merge.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1501 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0050_servicenote.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      745 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0100_auto_20190718_1417.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      693 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0006_auto_20170303_1242.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      826 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0106_auto_20190722_1524.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1254 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0023_auto_20170605_0705.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      522 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0096_merge_20190718_1102.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      671 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0003_auto_20170223_2233.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      649 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0112_syncjob_synchronizer_class.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      628 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0028_remove_company_company_alias.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      673 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0027_auto_20170605_1534.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)     1497 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0120_auto_20200721_1617.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1075 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0024_opportunitystage.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1756 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0108_projectphase.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      685 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0046_auto_20180104_1504.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1064 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0091_workrole.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      675 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0011_company_deleted_flag.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1168 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0043_projectstatus.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      778 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0099_timeentry_agreement.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      795 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0031_auto_20170607_2234.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      690 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0015_auto_20170404_1504.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      933 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0029_auto_20170607_1147.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      506 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0097_merge_20190718_1325.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      514 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0086_merge_20190507_1402.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1729 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0065_auto_20180809_1124.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      599 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0078_auto_20181203_1017.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      546 2019-08-14 17:00:26.000000 django-connectwise-0.3.99/djconnectwise/migrations/0099_timeentry_agreement.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      301 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0021_merge.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      389 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0078_auto_20181203_1017.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1312 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0062_auto_20180606_1117.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      752 2019-08-14 17:00:26.000000 django-connectwise-0.3.99/djconnectwise/migrations/0105_auto_20190722_1444.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      422 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0057_auto_20180511_1440.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     2653 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0077_item_subtype_type.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      654 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0070_mycompanyother.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      296 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0028_merge.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      915 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0039_auto_20170925_1418.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1045 2019-07-18 18:57:10.000000 django-connectwise-0.3.99/djconnectwise/migrations/0091_workrole.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      561 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0058_auto_20180516_1052.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1507 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0035_activity.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      861 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0045_auto_20171222_1725.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     2112 2019-08-21 22:56:27.000000 django-connectwise-0.3.99/djconnectwise/migrations/0108_projectphase.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1061 2019-07-10 20:32:12.000000 django-connectwise-0.3.99/djconnectwise/migrations/0087_auto_20190705_1015.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      549 2019-12-04 23:58:20.000000 django-connectwise-0.3.99/djconnectwise/migrations/0111_auto_20191204_0838.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      436 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0008_project_status_name.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      428 2020-01-06 20:58:00.000000 django-connectwise-0.3.99/djconnectwise/migrations/0112_syncjob_synchronizer_class.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      515 2019-08-14 17:00:26.000000 django-connectwise-0.3.99/djconnectwise/migrations/0100_auto_20190718_1417.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      768 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0041_auto_20171030_1047.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      581 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0044_auto_20171222_1700.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      444 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0006_auto_20170303_1242.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      283 2019-07-12 16:47:16.000000 django-connectwise-0.3.99/djconnectwise/migrations/0089_merge_20190711_1100.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1271 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0061_auto_20180607_1210.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      722 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0018_auto_20170505_1531.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      412 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0002_auto_20170223_2143.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      526 2019-07-18 18:57:10.000000 django-connectwise-0.3.99/djconnectwise/migrations/0095_connectwiseboard_work_type.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      461 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0019_syncjob_entity_name.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      426 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0047_syncjob_sync_type.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1947 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0050_timeentry.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1469 2019-08-14 17:00:26.000000 django-connectwise-0.3.99/djconnectwise/migrations/0096_agreement.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      425 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0011_company_deleted_flag.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      275 2019-08-14 17:00:26.000000 django-connectwise-0.3.99/djconnectwise/migrations/0097_merge_20190718_1325.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      503 2019-09-10 17:58:50.000000 django-connectwise-0.3.99/djconnectwise/migrations/0110_project_company.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      471 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0081_auto_20181220_0917.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      439 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0004_auto_20170224_1853.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      571 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0032_auto_20170616_1144.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      296 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0030_merge.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      829 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0037_auto_20170920_0959.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1591 2019-07-12 16:47:16.000000 django-connectwise-0.3.99/djconnectwise/migrations/0087_auto_20190709_0836.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1174 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0013_auto_20170403_1203.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      496 2019-08-14 17:00:26.000000 django-connectwise-0.3.99/djconnectwise/migrations/0101_agreement_company.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      289 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0052_merge.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      420 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0034_auto_20170727_1243.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      307 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0026_merge.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      438 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0015_auto_20170404_1504.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      411 2019-08-14 17:00:26.000000 django-connectwise-0.3.99/djconnectwise/migrations/0104_auto_20190722_1232.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1000 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0024_opportunitystage.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      404 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0033_auto_20170616_1251.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      283 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0068_merge_20180814_1104.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      427 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0055_auto_20180501_1022.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1234 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0049_auto_20180205_1122.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1730 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0073_auto_20180824_1446.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     2239 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0065_auto_20180809_1124.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      427 2020-04-16 20:15:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0115_agreement_agreement_status.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1351 2020-02-20 17:46:44.000000 django-connectwise-0.3.99/djconnectwise/migrations/0114_auto_20200219_1515.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     3313 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0036_auto_20170823_1417.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      409 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0060_auto_20180605_0840.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      366 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0028_remove_company_company_alias.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      385 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0061_auto_20180605_1208.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1170 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0043_projectstatus.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1172 2019-08-14 17:00:26.000000 django-connectwise-0.3.99/djconnectwise/migrations/0107_auto_20190729_1352.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      437 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0046_auto_20180104_1504.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      697 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0074_auto_20180827_1241.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1261 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0022_opportunitystatus.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      519 2019-07-18 18:57:10.000000 django-connectwise-0.3.99/djconnectwise/migrations/0094_connectwiseboard_work_role.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)    15323 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0001_initial.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      339 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0072_remove_callbackentry_member.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      424 2020-06-26 00:25:43.000000 django-connectwise-0.3.99/djconnectwise/migrations/0118_auto_20200623_1016.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      653 2019-08-14 17:00:26.000000 django-connectwise-0.3.99/djconnectwise/migrations/0098_auto_20190718_1406.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      461 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0042_auto_20171115_1131.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      576 2020-06-26 00:25:43.000000 django-connectwise-0.3.99/djconnectwise/migrations/0119_auto_20200624_1028.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1586 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0076_auto_20180925_1618.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      618 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0007_auto_20170311_1415.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      404 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0080_auto_20181210_0930.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)        0 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/__init__.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      621 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0056_auto_20180504_0744.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      502 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0048_project_manager.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      468 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0019_ticket_owner.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      283 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0086_merge_20190507_1402.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1509 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0064_auto_20180808_1214.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1067 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0079_auto_20181203_1606.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      417 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0054_auto_20180501_1009.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1217 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0029_auto_20170607_1147.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1232 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0023_auto_20170605_0705.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      335 2019-07-16 21:55:55.000000 django-connectwise-0.3.99/djconnectwise/migrations/0092_remove_ticket_work_type.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      535 2019-08-21 22:56:27.000000 django-connectwise-0.3.99/djconnectwise/migrations/0109_ticket_phase.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      306 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0083_delete_callbackentry.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      413 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0038_auto_20170920_1138.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      283 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0063_merge_20180611_0905.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      530 2020-02-05 17:45:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0113_auto_20200204_1054.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      889 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0031_auto_20170607_2234.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      747 2019-08-14 17:00:26.000000 django-connectwise-0.3.99/djconnectwise/migrations/0106_auto_20190722_1524.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      496 2019-07-11 17:48:16.000000 django-connectwise-0.3.99/djconnectwise/migrations/0088_auto_20190710_0953.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      293 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0053_merge.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      832 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/migrations/0069_auto_20180815_1116.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      514 2019-07-12 16:47:16.000000 django-connectwise-0.3.99/djconnectwise/migrations/0090_auto_20190711_1114.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1078 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/signals.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      222 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/apps.py
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/djconnectwise/__pycache__/
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     3899 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/__pycache__/views.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    32411 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/__pycache__/api.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      387 2020-08-10 22:34:48.000000 django-connectwise-0.3.99/djconnectwise/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     3969 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/__pycache__/callbacks.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      555 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/__pycache__/apps.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    55403 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/__pycache__/models.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      813 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/__pycache__/signals.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     3268 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/__pycache__/utils.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      372 2020-08-10 22:35:03.000000 django-connectwise-0.3.99/djconnectwise/__pycache__/urls.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    67806 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/__pycache__/sync.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    11081 2020-08-10 22:31:22.000000 django-connectwise-0.3.99/djconnectwise/admin.py
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/djconnectwise/management/
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/djconnectwise/management/__pycache__/
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      167 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/management/__pycache__/__init__.cpython-36.pyc
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/djconnectwise/management/commands/
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      466 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/management/commands/callbacks_registered.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1639 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/management/commands/cwclearoldsyncjobs.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      460 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/management/commands/callbacks_deleted.py
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/djconnectwise/management/commands/__pycache__/
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      176 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/management/commands/__pycache__/__init__.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)     5682 2020-08-10 22:35:00.000000 django-connectwise-0.3.99/djconnectwise/management/commands/__pycache__/cwsync.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      841 2020-08-10 22:34:59.000000 django-connectwise-0.3.99/djconnectwise/management/commands/__pycache__/list_users.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      559 2020-06-26 00:25:43.000000 django-connectwise-0.3.99/djconnectwise/management/commands/list_users.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)     7297 2020-08-10 22:31:22.000000 django-connectwise-0.3.99/djconnectwise/management/commands/cwsync.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1067 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/management/commands/updateslaexpiretimes.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      619 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/management/commands/list_callbacks.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)        0 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/management/commands/__init__.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)        0 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/management/__init__.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      213 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/urls.py
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/djconnectwise/tests/
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     3846 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/tests/AnonymousMember.png
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     4598 2019-12-18 00:37:11.000000 django-connectwise-0.3.99/djconnectwise/tests/test_callback.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    49462 2020-08-10 22:31:22.000000 django-connectwise-0.3.99/djconnectwise/tests/fixtures.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    14171 2020-08-10 22:31:22.000000 django-connectwise-0.3.99/djconnectwise/tests/mocks.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    76499 2020-08-10 22:31:22.000000 django-connectwise-0.3.99/djconnectwise/tests/test_sync.py
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/djconnectwise/tests/__pycache__/
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     2406 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/tests/__pycache__/test_utils.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     3200 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/tests/__pycache__/test_callback.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      162 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/tests/__pycache__/__init__.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    14887 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/tests/__pycache__/mocks.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     6665 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/tests/__pycache__/test_views.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    10239 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/tests/__pycache__/fixture_utils.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    22277 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/tests/__pycache__/test_commands.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)    29453 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/tests/__pycache__/test_api.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    27366 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/tests/__pycache__/fixtures.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1005 2020-08-10 22:35:02.000000 django-connectwise-0.3.99/djconnectwise/tests/__pycache__/mommy_recipes.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      317 2020-08-10 22:35:03.000000 django-connectwise-0.3.99/djconnectwise/tests/__pycache__/urls.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    67328 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/tests/__pycache__/test_sync.cpython-36.pyc
+-rw-r--r--   0 cameron   (1000) cameron   (1000)    17242 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/djconnectwise/tests/__pycache__/test_models.cpython-36.pyc
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    21972 2020-08-10 22:31:22.000000 django-connectwise-0.3.99/djconnectwise/tests/test_commands.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)     8161 2020-08-10 22:31:22.000000 django-connectwise-0.3.99/djconnectwise/tests/fixture_utils.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      161 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/tests/urls.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     6856 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/tests/test_views.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     2168 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/tests/test_utils.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)        0 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/tests/__init__.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)    21909 2019-05-14 16:25:52.000000 django-connectwise-0.3.99/djconnectwise/tests/test_models.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)    30559 2019-12-04 23:58:20.000000 django-connectwise-0.3.99/djconnectwise/tests/test_api.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)      731 2019-08-14 17:00:26.000000 django-connectwise-0.3.99/djconnectwise/tests/mommy_recipes.py
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     5315 2019-12-20 18:42:10.000000 django-connectwise-0.3.99/djconnectwise/callbacks.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    65814 2020-08-10 22:33:20.000000 django-connectwise-0.3.99/djconnectwise/models.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      294 2020-08-10 22:33:20.000000 django-connectwise-0.3.99/djconnectwise/__init__.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    42645 2020-08-10 22:31:22.000000 django-connectwise-0.3.99/djconnectwise/api.py
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/django_connectwise.egg-info/
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)        1 2020-08-10 22:34:49.000000 django-connectwise-0.3.99/django_connectwise.egg-info/not-zip-safe
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)        1 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/django_connectwise.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)       99 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/django_connectwise.egg-info/requires.txt
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)     4928 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/django_connectwise.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)       14 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/django_connectwise.egg-info/top_level.txt
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)    20068 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/django_connectwise.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)     4928 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/PKG-INFO
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)       38 2020-08-10 22:35:23.000000 django-connectwise-0.3.99/setup.cfg
```

### Comparing `django-connectwise-0.3.98/setup.py` & `django-connectwise-0.3.99/setup.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/callbacks.py` & `django-connectwise-0.3.99/djconnectwise/callbacks.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/views.py` & `django-connectwise-0.3.99/djconnectwise/views.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0062_auto_20180606_1117.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0062_auto_20180606_1117.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0031_auto_20170607_2234.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0031_auto_20170607_2234.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0025_opportunitypriority.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0025_opportunitypriority.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0107_auto_20190729_1352.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0107_auto_20190729_1352.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0007_auto_20170311_1415.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0007_auto_20170311_1415.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0094_connectwiseboard_work_role.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0094_connectwiseboard_work_role.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0024_opportunitystage.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0024_opportunitystage.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0111_auto_20191204_0838.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0111_auto_20191204_0838.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0001_initial.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0013_auto_20170403_1203.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0013_auto_20170403_1203.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0041_auto_20171030_1047.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0041_auto_20171030_1047.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0050_timeentry.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0050_timeentry.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0056_auto_20180504_0744.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0056_auto_20180504_0744.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0077_item_subtype_type.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0077_item_subtype_type.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0113_auto_20200204_1054.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0113_auto_20200204_1054.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0025_opportunity.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0025_opportunity.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0012_auto_20170320_1057.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0012_auto_20170320_1057.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0065_auto_20180809_1124.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0065_auto_20180809_1124.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0018_auto_20170505_1531.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0018_auto_20170505_1531.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0091_workrole.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0091_workrole.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0116_auto_20200522_1107.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0116_auto_20200522_1107.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0017_auto_20170504_2054.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0017_auto_20170504_2054.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0080_auto_20181210_0930.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0081_auto_20181220_0917.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-00000000: 160d 0d0a a4b0 1f5d 9401 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c d701 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3300 0000 6400 0064 0100 6c00 006d  .s3...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 4764 0200  ..Z..m..Z...Gd..
-00000040: 6403 0084 0000 6403 0065 0100 6a03 0083  d.....d..e..j...
-00000050: 0300 5a03 0064 0400 5329 05e9 0000 0000  ..Z..d..S)......
-00000060: 2902 da0a 6d69 6772 6174 696f 6e73 da06  )...migrations..
-00000070: 6d6f 6465 6c73 6300 0000 0000 0000 0000  modelsc.........
-00000080: 0000 000b 0000 0040 0000 0073 4c00 0000  .......@...sL...
-00000090: 6500 005a 0100 6400 005a 0200 640d 0067  e..Z..d..Z..d..g
-000000a0: 0100 5a03 0065 0400 6a05 0064 0300 6404  ..Z..e..j..d..d.
-000000b0: 0064 0500 6406 0064 0700 6506 006a 0700  .d..d..d..e..j..
-000000c0: 6408 0064 0900 640a 0064 0b00 8300 0283  d..d..d..d......
-000000d0: 0003 6701 005a 0800 640c 0053 290e da09  ..g..Z..d..S)...
-000000e0: 4d69 6772 6174 696f 6eda 0d64 6a63 6f6e  Migration..djcon
-000000f0: 6e65 6374 7769 7365 da17 3030 3739 5f61  nectwise..0079_a
-00000100: 7574 6f5f 3230 3138 3132 3033 5f31 3630  uto_20181203_160
-00000110: 36da 0a6d 6f64 656c 5f6e 616d 65da 066d  6..model_name..m
-00000120: 656d 6265 72da 046e 616d 65da 096c 6173  ember..name..las
-00000130: 745f 6e61 6d65 da05 6669 656c 64da 0a6d  t_name..field..m
-00000140: 6178 5f6c 656e 6774 68e9 1e00 0000 da04  ax_length.......
-00000150: 6e75 6c6c 544e 2902 7a0d 646a 636f 6e6e  nullTN).z.djconn
-00000160: 6563 7477 6973 6572 0600 0000 2909 da08  ectwiser....)...
-00000170: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000180: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000190: 5f5f da0c 6465 7065 6e64 656e 6369 6573  __..dependencies
-000001a0: 7202 0000 00da 0a41 6c74 6572 4669 656c  r......AlterFiel
-000001b0: 6472 0300 0000 da09 4368 6172 4669 656c  dr......CharFiel
-000001c0: 64da 0a6f 7065 7261 7469 6f6e 73a9 0072  d..operations..r
-000001d0: 1600 0000 7216 0000 00fa 6e2f 686f 6d65  ....r.....n/home
-000001e0: 2f73 616d 2f67 6974 2f4b 616e 6261 6e2f  /sam/git/Kanban/
-000001f0: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
-00000200: 7365 2f64 6a61 6e67 6f2d 636f 6e6e 6563  se/django-connec
-00000210: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
-00000220: 6973 652f 6d69 6772 6174 696f 6e73 2f30  ise/migrations/0
-00000230: 3038 305f 6175 746f 5f32 3031 3831 3231  080_auto_2018121
-00000240: 305f 3039 3330 2e70 7972 0400 0000 0600  0_0930.pyr......
-00000250: 0000 730a 0000 000c 0309 0409 0106 0106  ..s.............
-00000260: 0172 0400 0000 4e29 04da 0964 6a61 6e67  .r....N)...djang
-00000270: 6f2e 6462 7202 0000 0072 0300 0000 7204  o.dbr....r....r.
-00000280: 0000 0072 1600 0000 7216 0000 0072 1600  ...r....r....r..
-00000290: 0000 7217 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000002a0: 3e03 0000 0073 0200 0000 1603            >....s......
+00000020: 0073 2600 0000 6400 6401 6c00 6d01 5a01  .s&...d.d.l.m.Z.
+00000030: 6d02 5a02 0100 4700 6402 6403 8400 6403  m.Z...G.d.d...d.
+00000040: 6501 6a03 8303 5a03 6404 5300 2905 e900  e.j...Z.d.S.)...
+00000050: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
+00000060: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000070: 0000 0000 0000 0a00 0000 4000 0000 7334  ..........@...s4
+00000080: 0000 0065 005a 0164 005a 0264 0b67 015a  ...e.Z.d.Z.d.g.Z
+00000090: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000a0: 0664 0764 0564 0664 088d 0564 098d 0367  .d.d.d.d...d...g
+000000b0: 015a 0864 0a53 0029 0cda 094d 6967 7261  .Z.d.S.)...Migra
+000000c0: 7469 6f6e da0d 646a 636f 6e6e 6563 7477  tion..djconnectw
+000000d0: 6973 65da 1730 3038 305f 6175 746f 5f32  ise..0080_auto_2
+000000e0: 3031 3831 3231 305f 3039 3330 da06 6d65  0181210_0930..me
+000000f0: 6d62 6572 da06 6176 6174 6172 547a 0d4d  mber..avatarTz.M
+00000100: 656d 6265 7220 4176 6174 6172 e9fa 0000  ember Avatar....
+00000110: 0029 05da 0562 6c61 6e6b da09 6865 6c70  .)...blank..help
+00000120: 5f74 6578 74da 0a6d 6178 5f6c 656e 6774  _text..max_lengt
+00000130: 68da 046e 756c 6cda 0c76 6572 626f 7365  h..null..verbose
+00000140: 5f6e 616d 6529 03da 0a6d 6f64 656c 5f6e  _name)...model_n
+00000150: 616d 65da 046e 616d 65da 0566 6965 6c64  ame..name..field
+00000160: 4e29 0272 0500 0000 7206 0000 0029 09da  N).r....r....)..
+00000170: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000180: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000190: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
+000001a0: 7372 0200 0000 da0a 416c 7465 7246 6965  sr......AlterFie
+000001b0: 6c64 7203 0000 00da 0943 6861 7246 6965  ldr......CharFie
+000001c0: 6c64 da0a 6f70 6572 6174 696f 6e73 a900  ld..operations..
+000001d0: 7219 0000 0072 1900 0000 fa63 2f68 6f6d  r....r.....c/hom
+000001e0: 652f 6361 6d65 726f 6e2f 4465 762f 6b61  e/cameron/Dev/ka
+000001f0: 6e62 616e 2d64 6576 2f64 6a61 6e67 6f2d  nban-dev/django-
+00000200: 636f 6e6e 6563 7477 6973 652f 646a 636f  connectwise/djco
+00000210: 6e6e 6563 7477 6973 652f 6d69 6772 6174  nnectwise/migrat
+00000220: 696f 6e73 2f30 3038 315f 6175 746f 5f32  ions/0081_auto_2
+00000230: 3031 3831 3232 305f 3039 3137 2e70 7972  0181220_0917.pyr
+00000240: 0400 0000 0600 0000 730a 0000 0008 0306  ........s.......
+00000250: 0404 0102 0102 0172 0400 0000 4e29 04da  .......r....N)..
+00000260: 0964 6a61 6e67 6f2e 6462 7202 0000 0072  .django.dbr....r
+00000270: 0300 0000 7204 0000 0072 1900 0000 7219  ....r....r....r.
+00000280: 0000 0072 1900 0000 721a 0000 00da 083c  ...r....r......<
+00000290: 6d6f 6475 6c65 3e03 0000 0073 0200 0000  module>....s....
+000002a0: 1003                                     ..
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0089_merge_20190711_1100.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0083_delete_callbackentry.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-00000000: 160d 0d0a b7b5 285d 1b01 0000 e300 0000  ......(]........
+00000000: 330d 0d0a 10ec da5c 3201 0000 e300 0000  3......\2.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
-00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
-00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
-00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
-00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
-00000070: 0000 0000 0003 0000 0040 0000 0073 2200  .........@...s".
-00000080: 0000 6500 005a 0100 6400 005a 0200 6405  ..e..Z..d..Z..d.
-00000090: 0064 0600 6702 005a 0300 6700 005a 0400  .d..g..Z..g..Z..
-000000a0: 6404 0053 2907 da09 4d69 6772 6174 696f  d..S)...Migratio
-000000b0: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
-000000c0: da17 3030 3838 5f61 7574 6f5f 3230 3139  ..0088_auto_2019
-000000d0: 3037 3130 5f30 3935 33da 1730 3038 375f  0710_0953..0087_
-000000e0: 6175 746f 5f32 3031 3930 3730 395f 3038  auto_20190709_08
-000000f0: 3336 4e29 02fa 0d64 6a63 6f6e 6e65 6374  36N)...djconnect
-00000100: 7769 7365 7205 0000 0029 0272 0700 0000  wiser....).r....
-00000110: 7206 0000 0029 05da 085f 5f6e 616d 655f  r....)...__name_
-00000120: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000130: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
-00000140: 656e 6465 6e63 6965 73da 0a6f 7065 7261  endencies..opera
-00000150: 7469 6f6e 73a9 0072 0d00 0000 720d 0000  tions..r....r...
-00000160: 00fa 6f2f 686f 6d65 2f73 616d 2f67 6974  ..o/home/sam/git
-00000170: 2f4b 616e 6261 6e2f 646a 616e 676f 2d63  /Kanban/django-c
-00000180: 6f6e 6e65 6374 7769 7365 2f64 6a61 6e67  onnectwise/djang
-00000190: 6f2d 636f 6e6e 6563 7477 6973 652f 646a  o-connectwise/dj
-000001a0: 636f 6e6e 6563 7477 6973 652f 6d69 6772  connectwise/migr
-000001b0: 6174 696f 6e73 2f30 3038 395f 6d65 7267  ations/0089_merg
-000001c0: 655f 3230 3139 3037 3131 5f31 3130 302e  e_20190711_1100.
-000001d0: 7079 7203 0000 0006 0000 0073 0600 0000  pyr........s....
-000001e0: 0c03 0301 0903 7203 0000 004e 2903 da09  ......r....N)...
-000001f0: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
-00000200: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
-00000210: 0000 720e 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000220: 3e03 0000 0073 0200 0000 1003            >....s......
+00000020: 0073 2200 0000 6400 6401 6c00 6d01 5a01  .s"...d.d.l.m.Z.
+00000030: 0100 4700 6402 6403 8400 6403 6501 6a02  ..G.d.d...d.e.j.
+00000040: 8303 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
+00000050: 01da 0a6d 6967 7261 7469 6f6e 7363 0000  ...migrationsc..
+00000060: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+00000070: 0000 7320 0000 0065 005a 0164 005a 0264  ..s ...e.Z.d.Z.d
+00000080: 0667 015a 0365 046a 0564 0364 048d 0167  .g.Z.e.j.d.d...g
+00000090: 015a 0664 0553 0029 07da 094d 6967 7261  .Z.d.S.)...Migra
+000000a0: 7469 6f6e da0d 646a 636f 6e6e 6563 7477  tion..djconnectw
+000000b0: 6973 65da 1730 3038 325f 6175 746f 5f32  ise..0082_auto_2
+000000c0: 3031 3930 3132 355f 3131 3039 5a0d 4361  0190125_1109Z.Ca
+000000d0: 6c6c 4261 636b 456e 7472 7929 01da 046e  llBackEntry)...n
+000000e0: 616d 654e 2902 7204 0000 0072 0500 0000  ameN).r....r....
+000000f0: 2907 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000100: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000110: 6e61 6d65 5f5f da0c 6465 7065 6e64 656e  name__..dependen
+00000120: 6369 6573 7202 0000 00da 0b44 656c 6574  ciesr......Delet
+00000130: 654d 6f64 656c da0a 6f70 6572 6174 696f  eModel..operatio
+00000140: 6e73 a900 720d 0000 0072 0d00 0000 fa65  ns..r....r.....e
+00000150: 2f68 6f6d 652f 6361 6d65 726f 6e2f 4465  /home/cameron/De
+00000160: 762f 6b61 6e62 616e 2d64 6576 2f64 6a61  v/kanban-dev/dja
+00000170: 6e67 6f2d 636f 6e6e 6563 7477 6973 652f  ngo-connectwise/
+00000180: 646a 636f 6e6e 6563 7477 6973 652f 6d69  djconnectwise/mi
+00000190: 6772 6174 696f 6e73 2f30 3038 335f 6465  grations/0083_de
+000001a0: 6c65 7465 5f63 616c 6c62 6163 6b65 6e74  lete_callbackent
+000001b0: 7279 2e70 7972 0300 0000 0600 0000 7306  ry.pyr........s.
+000001c0: 0000 0008 0306 0404 0172 0300 0000 4e29  .........r....N)
+000001d0: 03da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
+000001e0: 0072 0300 0000 720d 0000 0072 0d00 0000  .r....r....r....
+000001f0: 720d 0000 0072 0e00 0000 da08 3c6d 6f64  r....r......<mod
+00000200: 756c 653e 0300 0000 7302 0000 000c 03    ule>....s......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0014_company_status.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0028_remove_company_company_alias.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,40 @@
-00000000: 160d 0d0a a4b0 1f5d dd01 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c 6e01 0000 e300 0000  3......\n.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 000f 0000 0040 0000 0073  ...........@...s
-000000b0: 5b00 0000 6500 005a 0100 6400 005a 0200  [...e..Z..d..Z..
-000000c0: 640f 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 6408 0064 0900 640a 0064 0900  .j..d..d..d..d..
-000000f0: 640b 0064 0c00 640d 0065 0600 6a08 0083  d..d..d..e..j...
-00000100: 0004 8300 0367 0100 5a09 0064 0e00 5329  .....g..Z..d..S)
-00000110: 10da 094d 6967 7261 7469 6f6e da0d 646a  ...Migration..dj
-00000120: 636f 6e6e 6563 7477 6973 65da 1730 3031  connectwise..001
-00000130: 335f 6175 746f 5f32 3031 3730 3430 335f  3_auto_20170403_
-00000140: 3132 3033 da0a 6d6f 6465 6c5f 6e61 6d65  1203..model_name
-00000150: da07 636f 6d70 616e 79da 046e 616d 65da  ..company..name.
-00000160: 0673 7461 7475 73da 0566 6965 6c64 da05  .status..field..
-00000170: 626c 616e 6b54 da04 6e75 6c6c da02 746f  blankT..null..to
-00000180: 7a1b 646a 636f 6e6e 6563 7477 6973 652e  z.djconnectwise.
-00000190: 436f 6d70 616e 7953 7461 7475 73da 096f  CompanyStatus..o
-000001a0: 6e5f 6465 6c65 7465 4e29 027a 0d64 6a63  n_deleteN).z.djc
-000001b0: 6f6e 6e65 6374 7769 7365 7207 0000 0029  onnectwiser....)
-000001c0: 0ada 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000001d0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000001e0: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
-000001f0: 6965 7372 0300 0000 da08 4164 6446 6965  iesr......AddFie
-00000200: 6c64 7204 0000 00da 0a46 6f72 6569 676e  ldr......Foreign
-00000210: 4b65 79da 0853 4554 5f4e 554c 4cda 0a6f  Key..SET_NULL..o
-00000220: 7065 7261 7469 6f6e 73a9 0072 1900 0000  perations..r....
-00000230: 7219 0000 00fa 6a2f 686f 6d65 2f73 616d  r.....j/home/sam
-00000240: 2f67 6974 2f4b 616e 6261 6e2f 646a 616e  /git/Kanban/djan
-00000250: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
-00000260: 6a61 6e67 6f2d 636f 6e6e 6563 7477 6973  jango-connectwis
-00000270: 652f 646a 636f 6e6e 6563 7477 6973 652f  e/djconnectwise/
-00000280: 6d69 6772 6174 696f 6e73 2f30 3031 345f  migrations/0014_
-00000290: 636f 6d70 616e 795f 7374 6174 7573 2e70  company_status.p
-000002a0: 7972 0500 0000 0700 0000 730a 0000 000c  yr........s.....
-000002b0: 0309 0409 0106 0106 0172 0500 0000 4e29  .........r....N)
-000002c0: 06da 0a5f 5f66 7574 7572 655f 5f72 0200  ...__future__r..
-000002d0: 0000 da09 646a 616e 676f 2e64 6272 0300  ....django.dbr..
-000002e0: 0000 7204 0000 0072 0500 0000 7219 0000  ..r....r....r...
-000002f0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00000300: da08 3c6d 6f64 756c 653e 0200 0000 7304  ..<module>....s.
-00000310: 0000 0010 0216 03                        .......
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0400 0000 4000 0000 7322  ..........@...s"
+000000a0: 0000 0065 005a 0164 005a 0264 0767 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0464 058d 0267 015a  .e.j.d.d.d...g.Z
+000000c0: 0664 0653 0029 08da 094d 6967 7261 7469  .d.S.)...Migrati
+000000d0: 6f6e da0d 646a 636f 6e6e 6563 7477 6973  on..djconnectwis
+000000e0: 65da 1730 3032 375f 6175 746f 5f32 3031  e..0027_auto_201
+000000f0: 3730 3630 355f 3135 3334 da07 636f 6d70  70605_1534..comp
+00000100: 616e 79da 0d63 6f6d 7061 6e79 5f61 6c69  any..company_ali
+00000110: 6173 2902 da0a 6d6f 6465 6c5f 6e61 6d65  as)...model_name
+00000120: da04 6e61 6d65 4e29 0272 0600 0000 7207  ..nameN).r....r.
+00000130: 0000 0029 07da 085f 5f6e 616d 655f 5fda  ...)...__name__.
+00000140: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000150: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
+00000160: 6465 6e63 6965 7372 0300 0000 da0b 5265  denciesr......Re
+00000170: 6d6f 7665 4669 656c 64da 0a6f 7065 7261  moveField..opera
+00000180: 7469 6f6e 73a9 0072 1200 0000 7212 0000  tions..r....r...
+00000190: 00fa 6d2f 686f 6d65 2f63 616d 6572 6f6e  ..m/home/cameron
+000001a0: 2f44 6576 2f6b 616e 6261 6e2d 6465 762f  /Dev/kanban-dev/
+000001b0: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
+000001c0: 7365 2f64 6a63 6f6e 6e65 6374 7769 7365  se/djconnectwise
+000001d0: 2f6d 6967 7261 7469 6f6e 732f 3030 3238  /migrations/0028
+000001e0: 5f72 656d 6f76 655f 636f 6d70 616e 795f  _remove_company_
+000001f0: 636f 6d70 616e 795f 616c 6961 732e 7079  company_alias.py
+00000200: 7205 0000 0007 0000 0073 0800 0000 0803  r........s......
+00000210: 0604 0401 0201 7205 0000 004e 2906 da0a  ......r....N)...
+00000220: 5f5f 6675 7475 7265 5f5f 7202 0000 00da  __future__r.....
+00000230: 0964 6a61 6e67 6f2e 6462 7203 0000 0072  .django.dbr....r
+00000240: 0400 0000 7205 0000 0072 1200 0000 7212  ....r....r....r.
+00000250: 0000 0072 1200 0000 7213 0000 00da 083c  ...r....r......<
+00000260: 6d6f 6475 6c65 3e02 0000 0073 0400 0000  module>....s....
+00000270: 0c02 1003                                ....
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0111_auto_20191204_0838.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0072_remove_callbackentry_member.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-00000000: 160d 0d0a 3e9f 0b5e 2502 0000 e300 0000  ....>..^%.......
+00000000: 330d 0d0a 10ec da5c 5301 0000 e300 0000  3......\S.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
-00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
-00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
-00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
-00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
-00000070: 0000 0000 0008 0000 0040 0000 0073 5500  .........@...sU.
-00000080: 0000 6500 005a 0100 6400 005a 0200 640c  ..e..Z..d..Z..d.
-00000090: 0067 0100 5a03 0065 0400 6a05 0064 0300  .g..Z..e..j..d..
-000000a0: 6404 0064 0500 6406 0064 0700 6408 0083  d..d..d..d..d...
-000000b0: 0003 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0900 6407 0064 0a00 8300 0367 0200  .d..d..d.....g..
-000000d0: 5a06 0064 0b00 5329 0dda 094d 6967 7261  Z..d..S)...Migra
-000000e0: 7469 6f6e da0d 646a 636f 6e6e 6563 7477  tion..djconnectw
-000000f0: 6973 65da 1430 3131 305f 7072 6f6a 6563  ise..0110_projec
-00000100: 745f 636f 6d70 616e 79da 0a6d 6f64 656c  t_company..model
-00000110: 5f6e 616d 65da 0d73 6368 6564 756c 6565  _name..schedulee
-00000120: 6e74 7279 da08 6f6c 645f 6e61 6d65 da11  ntry..old_name..
-00000130: 6578 7065 6374 6564 5f64 6174 655f 656e  expected_date_en
-00000140: 64da 086e 6577 5f6e 616d 65da 0864 6174  d..new_name..dat
-00000150: 655f 656e 64da 1365 7870 6563 7465 645f  e_end..expected_
-00000160: 6461 7465 5f73 7461 7274 da0a 6461 7465  date_start..date
-00000170: 5f73 7461 7274 4e29 027a 0d64 6a63 6f6e  _startN).z.djcon
-00000180: 6e65 6374 7769 7365 7a14 3031 3130 5f70  nectwisez.0110_p
-00000190: 726f 6a65 6374 5f63 6f6d 7061 6e79 2907  roject_company).
-000001a0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000001b0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000001c0: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
-000001d0: 6573 7202 0000 00da 0b52 656e 616d 6546  esr......RenameF
-000001e0: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
-000001f0: a900 7214 0000 0072 1400 0000 fa6e 2f68  ..r....r.....n/h
-00000200: 6f6d 652f 7361 6d2f 6769 742f 4b61 6e62  ome/sam/git/Kanb
-00000210: 616e 2f64 6a61 6e67 6f2d 636f 6e6e 6563  an/django-connec
-00000220: 7477 6973 652f 646a 616e 676f 2d63 6f6e  twise/django-con
-00000230: 6e65 6374 7769 7365 2f64 6a63 6f6e 6e65  nectwise/djconne
-00000240: 6374 7769 7365 2f6d 6967 7261 7469 6f6e  ctwise/migration
-00000250: 732f 3031 3131 5f61 7574 6f5f 3230 3139  s/0111_auto_2019
-00000260: 3132 3034 5f30 3833 382e 7079 7203 0000  1204_0838.pyr...
-00000270: 0006 0000 0073 1200 0000 0c03 0904 0901  .....s..........
-00000280: 0601 0601 0602 0901 0601 0601 7203 0000  ............r...
-00000290: 004e 2903 da09 646a 616e 676f 2e64 6272  .N)...django.dbr
-000002a0: 0200 0000 7203 0000 0072 1400 0000 7214  ....r....r....r.
-000002b0: 0000 0072 1400 0000 7215 0000 00da 083c  ...r....r......<
-000002c0: 6d6f 6475 6c65 3e03 0000 0073 0200 0000  module>....s....
-000002d0: 1003                                     ..
+00000020: 0073 2200 0000 6400 6401 6c00 6d01 5a01  .s"...d.d.l.m.Z.
+00000030: 0100 4700 6402 6403 8400 6403 6501 6a02  ..G.d.d...d.e.j.
+00000040: 8303 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
+00000050: 01da 0a6d 6967 7261 7469 6f6e 7363 0000  ...migrationsc..
+00000060: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+00000070: 0000 7322 0000 0065 005a 0164 005a 0264  ..s"...e.Z.d.Z.d
+00000080: 0767 015a 0365 046a 0564 0364 0464 058d  .g.Z.e.j.d.d.d..
+00000090: 0267 015a 0664 0653 0029 08da 094d 6967  .g.Z.d.S.)...Mig
+000000a0: 7261 7469 6f6e da0d 646a 636f 6e6e 6563  ration..djconnec
+000000b0: 7477 6973 65da 1730 3037 315f 6175 746f  twise..0071_auto
+000000c0: 5f32 3031 3830 3832 325f 3133 3030 da0d  _20180822_1300..
+000000d0: 6361 6c6c 6261 636b 656e 7472 79da 066d  callbackentry..m
+000000e0: 656d 6265 7229 02da 0a6d 6f64 656c 5f6e  ember)...model_n
+000000f0: 616d 65da 046e 616d 654e 2902 7204 0000  ame..nameN).r...
+00000100: 0072 0500 0000 2907 da08 5f5f 6e61 6d65  .r....)...__name
+00000110: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000120: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
+00000130: 7065 6e64 656e 6369 6573 7202 0000 00da  pendenciesr.....
+00000140: 0b52 656d 6f76 6546 6965 6c64 da0a 6f70  .RemoveField..op
+00000150: 6572 6174 696f 6e73 a900 7210 0000 0072  erations..r....r
+00000160: 1000 0000 fa6c 2f68 6f6d 652f 6361 6d65  .....l/home/came
+00000170: 726f 6e2f 4465 762f 6b61 6e62 616e 2d64  ron/Dev/kanban-d
+00000180: 6576 2f64 6a61 6e67 6f2d 636f 6e6e 6563  ev/django-connec
+00000190: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
+000001a0: 6973 652f 6d69 6772 6174 696f 6e73 2f30  ise/migrations/0
+000001b0: 3037 325f 7265 6d6f 7665 5f63 616c 6c62  072_remove_callb
+000001c0: 6163 6b65 6e74 7279 5f6d 656d 6265 722e  ackentry_member.
+000001d0: 7079 7203 0000 0006 0000 0073 0800 0000  pyr........s....
+000001e0: 0803 0604 0401 0201 7203 0000 004e 2903  ........r....N).
+000001f0: da09 646a 616e 676f 2e64 6272 0200 0000  ..django.dbr....
+00000200: 7203 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
+00000210: 1000 0000 7211 0000 00da 083c 6d6f 6475  ....r......<modu
+00000220: 6c65 3e03 0000 0073 0200 0000 0c03       le>....s......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0041_auto_20171030_1047.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0046_auto_20180104_1504.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,43 @@
-00000000: 160d 0d0a a4b0 1f5d 0003 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c b501 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 000a 0000 0040 0000 0073  ...........@...s
-000000b0: 7c00 0000 6500 005a 0100 6400 005a 0200  |...e..Z..d..Z..
-000000c0: 6410 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6408  ..d..d..d..d..d.
-000000e0: 0064 0900 6902 0083 0002 6504 006a 0500  .d..i.....e..j..
-000000f0: 6403 0064 0a00 6405 0064 0600 640b 0069  d..d..d..d..d..i
-00000100: 0100 8300 0265 0400 6a05 0064 0300 640c  .....e..j..d..d.
-00000110: 0064 0500 640d 0064 1100 6406 0064 0e00  .d..d..d..d..d..
-00000120: 6902 0083 0002 6703 005a 0600 640f 0053  i.....g..Z..d..S
-00000130: 2912 da09 4d69 6772 6174 696f 6eda 0d64  )...Migration..d
-00000140: 6a63 6f6e 6e65 6374 7769 7365 da17 3030  jconnectwise..00
-00000150: 3430 5f61 7574 6f5f 3230 3137 3039 3236  40_auto_20170926
-00000160: 5f32 3134 35da 046e 616d 655a 0d63 616c  _2145..nameZ.cal
-00000170: 6c62 6163 6b65 6e74 7279 da07 6f70 7469  lbackentry..opti
-00000180: 6f6e 73da 1376 6572 626f 7365 5f6e 616d  ons..verbose_nam
-00000190: 655f 706c 7572 616c 7a10 4361 6c6c 6261  e_pluralz.Callba
-000001a0: 636b 2065 6e74 7269 6573 da0c 7665 7262  ck entries..verb
-000001b0: 6f73 655f 6e61 6d65 7a0e 4361 6c6c 6261  ose_namez.Callba
-000001c0: 636b 2065 6e74 7279 5a0d 636f 6d70 616e  ck entryZ.compan
-000001d0: 7973 7461 7475 737a 1043 6f6d 7061 6e79  ystatusz.Company
-000001e0: 2073 7461 7475 7365 735a 136f 7070 6f72   statusesZ.oppor
-000001f0: 7475 6e69 7479 7072 696f 7269 7479 da08  tunitypriority..
-00000200: 6f72 6465 7269 6e67 7a16 6f70 706f 7274  orderingz.opport
-00000210: 756e 6974 7920 7072 696f 7269 7469 6573  unity priorities
-00000220: 4e29 027a 0d64 6a63 6f6e 6e65 6374 7769  N).z.djconnectwi
-00000230: 7365 7207 0000 0029 0172 0800 0000 2907  ser....).r....).
-00000240: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000250: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000260: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
-00000270: 6573 7203 0000 00da 1141 6c74 6572 4d6f  esr......AlterMo
-00000280: 6465 6c4f 7074 696f 6e73 da0a 6f70 6572  delOptions..oper
-00000290: 6174 696f 6e73 a900 7213 0000 0072 1300  ations..r....r..
-000002a0: 0000 fa6e 2f68 6f6d 652f 7361 6d2f 6769  ...n/home/sam/gi
-000002b0: 742f 4b61 6e62 616e 2f64 6a61 6e67 6f2d  t/Kanban/django-
-000002c0: 636f 6e6e 6563 7477 6973 652f 646a 616e  connectwise/djan
-000002d0: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
-000002e0: 6a63 6f6e 6e65 6374 7769 7365 2f6d 6967  jconnectwise/mig
-000002f0: 7261 7469 6f6e 732f 3030 3431 5f61 7574  rations/0041_aut
-00000300: 6f5f 3230 3137 3130 3330 5f31 3034 372e  o_20171030_1047.
-00000310: 7079 7205 0000 0007 0000 0073 1400 0000  pyr........s....
-00000320: 0c03 0904 0901 0601 1202 0901 0601 0c02  ................
-00000330: 0901 0601 7205 0000 004e 2906 da0a 5f5f  ....r....N)...__
-00000340: 6675 7475 7265 5f5f 7202 0000 00da 0964  future__r......d
-00000350: 6a61 6e67 6f2e 6462 7203 0000 0072 0400  jango.dbr....r..
-00000360: 0000 7205 0000 0072 1300 0000 7213 0000  ..r....r....r...
-00000370: 0072 1300 0000 7214 0000 00da 083c 6d6f  .r....r......<mo
-00000380: 6475 6c65 3e02 0000 0073 0400 0000 1002  dule>....s......
-00000390: 1603                                     ..
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0800 0000 4000 0000 7330  ..........@...s0
+000000a0: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000c0: 0664 0564 078d 0364 088d 0367 015a 0864  .d.d...d...g.Z.d
+000000d0: 0953 0029 0bda 094d 6967 7261 7469 6f6e  .S.)...Migration
+000000e0: da0d 646a 636f 6e6e 6563 7477 6973 65da  ..djconnectwise.
+000000f0: 1730 3034 355f 6175 746f 5f32 3031 3731  .0045_auto_20171
+00000100: 3232 325f 3137 3235 da0d 7363 6865 6475  222_1725..schedu
+00000110: 6c65 656e 7472 79da 046e 616d 6554 e9fa  leentry..nameT..
+00000120: 0000 0029 03da 046e 756c 6cda 0a6d 6178  ...)...null..max
+00000130: 5f6c 656e 6774 68da 0562 6c61 6e6b 2903  _length..blank).
+00000140: da0a 6d6f 6465 6c5f 6e61 6d65 7209 0000  ..model_namer...
+00000150: 00da 0566 6965 6c64 4e29 0272 0600 0000  ...fieldN).r....
+00000160: 7207 0000 0029 09da 085f 5f6e 616d 655f  r....)...__name_
+00000170: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000180: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
+00000190: 656e 6465 6e63 6965 7372 0300 0000 da0a  endenciesr......
+000001a0: 416c 7465 7246 6965 6c64 7204 0000 00da  AlterFieldr.....
+000001b0: 0943 6861 7246 6965 6c64 da0a 6f70 6572  .CharField..oper
+000001c0: 6174 696f 6e73 a900 7217 0000 0072 1700  ations..r....r..
+000001d0: 0000 fa63 2f68 6f6d 652f 6361 6d65 726f  ...c/home/camero
+000001e0: 6e2f 4465 762f 6b61 6e62 616e 2d64 6576  n/Dev/kanban-dev
+000001f0: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
+00000200: 6973 652f 646a 636f 6e6e 6563 7477 6973  ise/djconnectwis
+00000210: 652f 6d69 6772 6174 696f 6e73 2f30 3034  e/migrations/004
+00000220: 365f 6175 746f 5f32 3031 3830 3130 345f  6_auto_20180104_
+00000230: 3135 3034 2e70 7972 0500 0000 0700 0000  1504.pyr........
+00000240: 730a 0000 0008 0306 0404 0102 0102 0172  s..............r
+00000250: 0500 0000 4e29 06da 0a5f 5f66 7574 7572  ....N)...__futur
+00000260: 655f 5f72 0200 0000 da09 646a 616e 676f  e__r......django
+00000270: 2e64 6272 0300 0000 7204 0000 0072 0500  .dbr....r....r..
+00000280: 0000 7217 0000 0072 1700 0000 7217 0000  ..r....r....r...
+00000290: 0072 1800 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000002a0: 0200 0000 7304 0000 000c 0210 03         ....s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0010_remove_project_project_href.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0016_auto_20170404_1504.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-00000000: 160d 0d0a a4b0 1f5d 6f01 0000 e300 0000  .......]o.......
+00000000: 330d 0d0a 10ec da5c c501 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0005 0000 0040 0000 0073  ...........@...s
-000000b0: 3400 0000 6500 005a 0100 6400 005a 0200  4...e..Z..d..Z..
-000000c0: 6408 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0083 0002 6701  ..d..d..d.....g.
-000000e0: 005a 0600 6407 0053 2909 da09 4d69 6772  .Z..d..S)...Migr
-000000f0: 6174 696f 6eda 0d64 6a63 6f6e 6e65 6374  ation..djconnect
-00000100: 7769 7365 da19 3030 3039 5f6d 656d 6265  wise..0009_membe
-00000110: 725f 6c69 6365 6e73 655f 636c 6173 73da  r_license_class.
-00000120: 0a6d 6f64 656c 5f6e 616d 65da 0770 726f  .model_name..pro
-00000130: 6a65 6374 da04 6e61 6d65 da0c 7072 6f6a  ject..name..proj
-00000140: 6563 745f 6872 6566 4e29 027a 0d64 6a63  ect_hrefN).z.djc
-00000150: 6f6e 6e65 6374 7769 7365 7a19 3030 3039  onnectwisez.0009
-00000160: 5f6d 656d 6265 725f 6c69 6365 6e73 655f  _member_license_
-00000170: 636c 6173 7329 07da 085f 5f6e 616d 655f  class)...__name_
-00000180: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000190: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
-000001a0: 656e 6465 6e63 6965 7372 0300 0000 da0b  endenciesr......
-000001b0: 5265 6d6f 7665 4669 656c 64da 0a6f 7065  RemoveField..ope
-000001c0: 7261 7469 6f6e 73a9 0072 1200 0000 7212  rations..r....r.
-000001d0: 0000 00fa 772f 686f 6d65 2f73 616d 2f67  ....w/home/sam/g
-000001e0: 6974 2f4b 616e 6261 6e2f 646a 616e 676f  it/Kanban/django
-000001f0: 2d63 6f6e 6e65 6374 7769 7365 2f64 6a61  -connectwise/dja
-00000200: 6e67 6f2d 636f 6e6e 6563 7477 6973 652f  ngo-connectwise/
-00000210: 646a 636f 6e6e 6563 7477 6973 652f 6d69  djconnectwise/mi
-00000220: 6772 6174 696f 6e73 2f30 3031 305f 7265  grations/0010_re
-00000230: 6d6f 7665 5f70 726f 6a65 6374 5f70 726f  move_project_pro
-00000240: 6a65 6374 5f68 7265 662e 7079 7205 0000  ject_href.pyr...
-00000250: 0007 0000 0073 0800 0000 0c03 0904 0901  .....s..........
-00000260: 0601 7205 0000 004e 2906 da0a 5f5f 6675  ..r....N)...__fu
-00000270: 7475 7265 5f5f 7202 0000 00da 0964 6a61  ture__r......dja
-00000280: 6e67 6f2e 6462 7203 0000 0072 0400 0000  ngo.dbr....r....
-00000290: 7205 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-000002a0: 1200 0000 7213 0000 00da 083c 6d6f 6475  ....r......<modu
-000002b0: 6c65 3e02 0000 0073 0400 0000 1002 1603  le>....s........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0800 0000 4000 0000 7330  ..........@...s0
+000000a0: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000c0: 0664 0664 078d 0364 088d 0367 015a 0864  .d.d...d...g.Z.d
+000000d0: 0953 0029 0bda 094d 6967 7261 7469 6f6e  .S.)...Migration
+000000e0: da0d 646a 636f 6e6e 6563 7477 6973 65da  ..djconnectwise.
+000000f0: 1730 3031 355f 6175 746f 5f32 3031 3730  .0015_auto_20170
+00000100: 3430 345f 3135 3034 da0d 636f 6d70 616e  404_1504..compan
+00000110: 7973 7461 7475 73da 146e 6f74 6966 6963  ystatus..notific
+00000120: 6174 696f 6e5f 6d65 7373 6167 6569 f401  ation_messagei..
+00000130: 0000 5429 03da 0a6d 6178 5f6c 656e 6774  ..T)...max_lengt
+00000140: 68da 046e 756c 6cda 0562 6c61 6e6b 2903  h..null..blank).
+00000150: da0a 6d6f 6465 6c5f 6e61 6d65 da04 6e61  ..model_name..na
+00000160: 6d65 da05 6669 656c 644e 2902 7206 0000  me..fieldN).r...
+00000170: 0072 0700 0000 2909 da08 5f5f 6e61 6d65  .r....)...__name
+00000180: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000190: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
+000001a0: 7065 6e64 656e 6369 6573 7203 0000 00da  pendenciesr.....
+000001b0: 0a41 6c74 6572 4669 656c 6472 0400 0000  .AlterFieldr....
+000001c0: da09 4368 6172 4669 656c 64da 0a6f 7065  ..CharField..ope
+000001d0: 7261 7469 6f6e 73a9 0072 1700 0000 7217  rations..r....r.
+000001e0: 0000 00fa 632f 686f 6d65 2f63 616d 6572  ....c/home/camer
+000001f0: 6f6e 2f44 6576 2f6b 616e 6261 6e2d 6465  on/Dev/kanban-de
+00000200: 762f 646a 616e 676f 2d63 6f6e 6e65 6374  v/django-connect
+00000210: 7769 7365 2f64 6a63 6f6e 6e65 6374 7769  wise/djconnectwi
+00000220: 7365 2f6d 6967 7261 7469 6f6e 732f 3030  se/migrations/00
+00000230: 3136 5f61 7574 6f5f 3230 3137 3034 3034  16_auto_20170404
+00000240: 5f31 3530 342e 7079 7205 0000 0007 0000  _1504.pyr.......
+00000250: 0073 0a00 0000 0803 0604 0401 0201 0201  .s..............
+00000260: 7205 0000 004e 2906 da0a 5f5f 6675 7475  r....N)...__futu
+00000270: 7265 5f5f 7202 0000 00da 0964 6a61 6e67  re__r......djang
+00000280: 6f2e 6462 7203 0000 0072 0400 0000 7205  o.dbr....r....r.
+00000290: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
+000002a0: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000002b0: 3e02 0000 0073 0400 0000 0c02 1003       >....s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0044_auto_20171222_1700.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0018_auto_20170505_1531.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-00000000: 160d 0d0a a4b0 1f5d 4502 0000 e300 0000  .......]E.......
+00000000: 330d 0d0a 10ec da5c d202 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0010 0000 0040 0000 0073  ...........@...s
-000000b0: 7000 0000 6500 005a 0100 6400 005a 0200  p...e..Z..d..Z..
-000000c0: 6410 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0083 0002 6504  ..d..d..d.....e.
-000000e0: 006a 0600 6403 0064 0400 6405 0064 0700  .j..d..d..d..d..
-000000f0: 6408 0065 0700 6a08 0064 0900 640a 0064  d..e..j..d..d..d
-00000100: 0b00 640c 0064 0d00 640c 0064 0e00 6507  ..d..d..d..d..e.
-00000110: 006a 0900 8300 0483 0003 6702 005a 0a00  .j........g..Z..
-00000120: 640f 0053 2911 da09 4d69 6772 6174 696f  d..S)...Migratio
-00000130: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
-00000140: da12 3030 3433 5f70 726f 6a65 6374 7374  ..0043_projectst
-00000150: 6174 7573 da0a 6d6f 6465 6c5f 6e61 6d65  atus..model_name
-00000160: da07 7072 6f6a 6563 74da 046e 616d 65da  ..project..name.
-00000170: 0b73 7461 7475 735f 6e61 6d65 da06 7374  .status_name..st
-00000180: 6174 7573 da05 6669 656c 64da 0274 6f7a  atus..field..toz
-00000190: 1b64 6a63 6f6e 6e65 6374 7769 7365 2e50  .djconnectwise.P
-000001a0: 726f 6a65 6374 5374 6174 7573 da05 626c  rojectStatus..bl
-000001b0: 616e 6b54 da04 6e75 6c6c da09 6f6e 5f64  ankT..null..on_d
-000001c0: 656c 6574 654e 2902 7a0d 646a 636f 6e6e  eleteN).z.djconn
-000001d0: 6563 7477 6973 6572 0700 0000 290b da08  ectwiser....)...
-000001e0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000001f0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000200: 5f5f da0c 6465 7065 6e64 656e 6369 6573  __..dependencies
-00000210: 7203 0000 00da 0b52 656d 6f76 6546 6965  r......RemoveFie
-00000220: 6c64 da08 4164 6446 6965 6c64 7204 0000  ld..AddFieldr...
-00000230: 00da 0a46 6f72 6569 676e 4b65 79da 0853  ...ForeignKey..S
-00000240: 4554 5f4e 554c 4cda 0a6f 7065 7261 7469  ET_NULL..operati
-00000250: 6f6e 73a9 0072 1b00 0000 721b 0000 00fa  ons..r....r.....
-00000260: 6e2f 686f 6d65 2f73 616d 2f67 6974 2f4b  n/home/sam/git/K
-00000270: 616e 6261 6e2f 646a 616e 676f 2d63 6f6e  anban/django-con
-00000280: 6e65 6374 7769 7365 2f64 6a61 6e67 6f2d  nectwise/django-
-00000290: 636f 6e6e 6563 7477 6973 652f 646a 636f  connectwise/djco
-000002a0: 6e6e 6563 7477 6973 652f 6d69 6772 6174  nnectwise/migrat
-000002b0: 696f 6e73 2f30 3034 345f 6175 746f 5f32  ions/0044_auto_2
-000002c0: 3031 3731 3232 325f 3137 3030 2e70 7972  0171222_1700.pyr
-000002d0: 0500 0000 0700 0000 7310 0000 000c 0309  ........s.......
-000002e0: 0409 0106 0106 0209 0106 0106 0172 0500  .............r..
-000002f0: 0000 4e29 06da 0a5f 5f66 7574 7572 655f  ..N)...__future_
-00000300: 5f72 0200 0000 da09 646a 616e 676f 2e64  _r......django.d
-00000310: 6272 0300 0000 7204 0000 0072 0500 0000  br....r....r....
-00000320: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
-00000330: 1c00 0000 da08 3c6d 6f64 756c 653e 0200  ......<module>..
-00000340: 0000 7304 0000 0010 0216 03              ..s........
+00000020: 0073 3a00 0000 6400 6401 6c00 6d01 5a01  .s:...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 6400 6403 6c05 5a06 4700 6404 6405  ..d.d.l.Z.G.d.d.
+00000050: 8400 6405 6503 6a07 8303 5a07 6403 5300  ..d.e.j...Z.d.S.
+00000060: 2906 e900 0000 0029 01da 1075 6e69 636f  )......)...unico
+00000070: 6465 5f6c 6974 6572 616c 7329 02da 0a6d  de_literals)...m
+00000080: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000090: 734e 6300 0000 0000 0000 0000 0000 0008  sNc.............
+000000a0: 0000 0040 0000 0073 4e00 0000 6500 5a01  ...@...sN...e.Z.
+000000b0: 6400 5a02 640b 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000c0: 6404 6506 6a07 6a08 6a09 6405 6404 6406  d.e.j.j.j.d.d.d.
+000000d0: 8d02 6407 8d03 6504 6a05 6403 6408 6506  ..d...e.j.d.d.e.
+000000e0: 6a07 6a08 6a0a 6408 6405 6409 8d02 6407  j.j.j.d.d.d...d.
+000000f0: 8d03 6702 5a0b 640a 5300 290c da09 4d69  ..g.Z.d.S.)...Mi
+00000100: 6772 6174 696f 6eda 0d64 6a63 6f6e 6e65  gration..djconne
+00000110: 6374 7769 7365 da17 3030 3137 5f61 7574  ctwise..0017_aut
+00000120: 6f5f 3230 3137 3035 3034 5f32 3035 34da  o_20170504_2054.
+00000130: 066d 656d 6265 72da 0763 7265 6174 6564  .member..created
+00000140: 5429 02da 0c61 7574 6f5f 6e6f 775f 6164  T)...auto_now_ad
+00000150: 64da 0c76 6572 626f 7365 5f6e 616d 6529  d..verbose_name)
+00000160: 03da 0a6d 6f64 656c 5f6e 616d 65da 046e  ...model_name..n
+00000170: 616d 65da 0566 6965 6c64 da08 6d6f 6469  ame..field..modi
+00000180: 6669 6564 2902 720b 0000 00da 0861 7574  fied).r......aut
+00000190: 6f5f 6e6f 774e 2902 7206 0000 0072 0700  o_nowN).r....r..
+000001a0: 0000 290c da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+000001b0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000001c0: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
+000001d0: 656e 6369 6573 7203 0000 00da 0a41 6c74  enciesr......Alt
+000001e0: 6572 4669 656c 64da 1164 6a61 6e67 6f5f  erField..django_
+000001f0: 6578 7465 6e73 696f 6e73 da02 6462 da06  extensions..db..
+00000200: 6669 656c 6473 da15 4372 6561 7469 6f6e  fields..Creation
+00000210: 4461 7465 5469 6d65 4669 656c 64da 194d  DateTimeField..M
+00000220: 6f64 6966 6963 6174 696f 6e44 6174 6554  odificationDateT
+00000230: 696d 6546 6965 6c64 da0a 6f70 6572 6174  imeField..operat
+00000240: 696f 6e73 a900 721c 0000 0072 1c00 0000  ions..r....r....
+00000250: fa63 2f68 6f6d 652f 6361 6d65 726f 6e2f  .c/home/cameron/
+00000260: 4465 762f 6b61 6e62 616e 2d64 6576 2f64  Dev/kanban-dev/d
+00000270: 6a61 6e67 6f2d 636f 6e6e 6563 7477 6973  jango-connectwis
+00000280: 652f 646a 636f 6e6e 6563 7477 6973 652f  e/djconnectwise/
+00000290: 6d69 6772 6174 696f 6e73 2f30 3031 385f  migrations/0018_
+000002a0: 6175 746f 5f32 3031 3730 3530 355f 3135  auto_20170505_15
+000002b0: 3331 2e70 7972 0500 0000 0800 0000 7312  31.pyr........s.
+000002c0: 0000 0008 0306 0404 0102 0102 0114 0204  ................
+000002d0: 0102 0102 0172 0500 0000 2908 da0a 5f5f  .....r....)...__
+000002e0: 6675 7475 7265 5f5f 7202 0000 00da 0964  future__r......d
+000002f0: 6a61 6e67 6f2e 6462 7203 0000 0072 0400  jango.dbr....r..
+00000300: 0000 da1b 646a 616e 676f 5f65 7874 656e  ....django_exten
+00000310: 7369 6f6e 732e 6462 2e66 6965 6c64 7372  sions.db.fieldsr
+00000320: 1600 0000 7205 0000 0072 1c00 0000 721c  ....r....r....r.
+00000330: 0000 0072 1c00 0000 721d 0000 00da 083c  ...r....r......<
+00000340: 6d6f 6475 6c65 3e02 0000 0073 0600 0000  module>....s....
+00000350: 0c02 1001 0803                           ......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0099_timeentry_agreement.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0059_auto_20180518_0811.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,46 @@
-00000000: 160d 0d0a ced8 355d 2202 0000 e300 0000  ......5]".......
+00000000: 330d 0d0a 10ec da5c f601 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 1100 0000 4000 0000 736a 0000 0065 0000  ....@...sj...e..
-000000a0: 5a01 0064 0000 5a02 0064 1100 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6407 0065 0600 6a07 0064 0800  .d..d..e..j..d..
-000000d0: 6409 0064 0a00 6409 0064 0b00 6508 006a  d..d..d..d..e..j
-000000e0: 0900 6a06 006a 0a00 6a0b 0064 0c00 640d  ..j..j..j..d..d.
-000000f0: 0064 0e00 640f 0083 0005 8300 0367 0100  .d..d........g..
-00000100: 5a0c 0064 1000 5329 12da 094d 6967 7261  Z..d..S)...Migra
-00000110: 7469 6f6e da0d 646a 636f 6e6e 6563 7477  tion..djconnectw
-00000120: 6973 65da 1730 3039 385f 6175 746f 5f32  ise..0098_auto_2
-00000130: 3031 3930 3731 385f 3134 3036 da0a 6d6f  0190718_1406..mo
-00000140: 6465 6c5f 6e61 6d65 da09 7469 6d65 656e  del_name..timeen
-00000150: 7472 79da 046e 616d 65da 0961 6772 6565  try..name..agree
-00000160: 6d65 6e74 da05 6669 656c 64da 0562 6c61  ment..field..bla
-00000170: 6e6b 54da 046e 756c 6cda 096f 6e5f 6465  nkT..null..on_de
-00000180: 6c65 7465 da0c 7265 6c61 7465 645f 6e61  lete..related_na
-00000190: 6d65 da11 6167 7265 656d 656e 745f 7469  me..agreement_ti
-000001a0: 636b 6574 73da 0274 6f7a 1764 6a63 6f6e  ckets..toz.djcon
-000001b0: 6e65 6374 7769 7365 2e41 6772 6565 6d65  nectwise.Agreeme
-000001c0: 6e74 4e29 027a 0d64 6a63 6f6e 6e65 6374  ntN).z.djconnect
-000001d0: 7769 7365 7a17 3030 3938 5f61 7574 6f5f  wisez.0098_auto_
-000001e0: 3230 3139 3037 3138 5f31 3430 3629 0dda  20190718_1406)..
-000001f0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000200: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000210: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
-00000220: 7372 0200 0000 da08 4164 6446 6965 6c64  sr......AddField
-00000230: 7203 0000 00da 0a46 6f72 6569 676e 4b65  r......ForeignKe
-00000240: 79da 0664 6a61 6e67 6fda 0264 62da 0864  y..django..db..d
-00000250: 656c 6574 696f 6eda 0853 4554 5f4e 554c  eletion..SET_NUL
-00000260: 4cda 0a6f 7065 7261 7469 6f6e 73a9 0072  L..operations..r
-00000270: 1d00 0000 721d 0000 00fa 6f2f 686f 6d65  ....r.....o/home
-00000280: 2f73 616d 2f67 6974 2f4b 616e 6261 6e2f  /sam/git/Kanban/
-00000290: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
-000002a0: 7365 2f64 6a61 6e67 6f2d 636f 6e6e 6563  se/django-connec
-000002b0: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
-000002c0: 6973 652f 6d69 6772 6174 696f 6e73 2f30  ise/migrations/0
-000002d0: 3039 395f 7469 6d65 656e 7472 795f 6167  099_timeentry_ag
-000002e0: 7265 656d 656e 742e 7079 7204 0000 0007  reement.pyr.....
-000002f0: 0000 0073 0a00 0000 0c03 0904 0901 0601  ...s............
-00000300: 0601 7204 0000 0029 06da 0964 6a61 6e67  ..r....)...djang
-00000310: 6f2e 6462 7202 0000 0072 0300 0000 da19  o.dbr....r......
-00000320: 646a 616e 676f 2e64 622e 6d6f 6465 6c73  django.db.models
-00000330: 2e64 656c 6574 696f 6e72 1800 0000 7204  .deletionr....r.
-00000340: 0000 0072 1d00 0000 721d 0000 0072 1d00  ...r....r....r..
-00000350: 0000 721e 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000360: 3e03 0000 0073 0400 0000 1601 0c03       >....s........
+00000020: 0073 2e00 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 4700  m.Z...d.d.l.Z.G.
+00000040: 6403 6404 8400 6404 6501 6a05 8303 5a05  d.d...d.e.j...Z.
+00000050: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 734e 6300 0000 0000 0000 0000 0000 0008  sNc.............
+00000080: 0000 0040 0000 0073 3800 0000 6500 5a01  ...@...s8...e.Z.
+00000090: 6400 5a02 640a 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000a0: 6404 6506 6a07 6405 6508 6a09 6a06 6a0a  d.e.j.d.e.j.j.j.
+000000b0: 6a0b 6406 6407 8d03 6408 8d03 6701 5a0c  j.d.d...d...g.Z.
+000000c0: 6409 5300 290b da09 4d69 6772 6174 696f  d.S.)...Migratio
+000000d0: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
+000000e0: da17 3030 3538 5f61 7574 6f5f 3230 3138  ..0058_auto_2018
+000000f0: 3035 3136 5f31 3035 32da 0d63 616c 6c62  0516_1052..callb
+00000100: 6163 6b65 6e74 7279 da06 6d65 6d62 6572  ackentry..member
+00000110: 547a 1464 6a63 6f6e 6e65 6374 7769 7365  Tz.djconnectwise
+00000120: 2e4d 656d 6265 7229 03da 046e 756c 6cda  .Member)...null.
+00000130: 096f 6e5f 6465 6c65 7465 da02 746f 2903  .on_delete..to).
+00000140: da0a 6d6f 6465 6c5f 6e61 6d65 da04 6e61  ..model_name..na
+00000150: 6d65 da05 6669 656c 644e 2902 7205 0000  me..fieldN).r...
+00000160: 0072 0600 0000 290d da08 5f5f 6e61 6d65  .r....)...__name
+00000170: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000180: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
+00000190: 7065 6e64 656e 6369 6573 7202 0000 00da  pendenciesr.....
+000001a0: 0a41 6c74 6572 4669 656c 6472 0300 0000  .AlterFieldr....
+000001b0: da0a 466f 7265 6967 6e4b 6579 da06 646a  ..ForeignKey..dj
+000001c0: 616e 676f da02 6462 da08 6465 6c65 7469  ango..db..deleti
+000001d0: 6f6e da08 5345 545f 4e55 4c4c da0a 6f70  on..SET_NULL..op
+000001e0: 6572 6174 696f 6e73 a900 721a 0000 0072  erations..r....r
+000001f0: 1a00 0000 fa63 2f68 6f6d 652f 6361 6d65  .....c/home/came
+00000200: 726f 6e2f 4465 762f 6b61 6e62 616e 2d64  ron/Dev/kanban-d
+00000210: 6576 2f64 6a61 6e67 6f2d 636f 6e6e 6563  ev/django-connec
+00000220: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
+00000230: 6973 652f 6d69 6772 6174 696f 6e73 2f30  ise/migrations/0
+00000240: 3035 395f 6175 746f 5f32 3031 3830 3531  059_auto_2018051
+00000250: 385f 3038 3131 2e70 7972 0400 0000 0700  8_0811.pyr......
+00000260: 0000 730a 0000 0008 0306 0404 0102 0102  ..s.............
+00000270: 0172 0400 0000 2906 da09 646a 616e 676f  .r....)...django
+00000280: 2e64 6272 0200 0000 7203 0000 00da 1964  .dbr....r......d
+00000290: 6a61 6e67 6f2e 6462 2e6d 6f64 656c 732e  jango.db.models.
+000002a0: 6465 6c65 7469 6f6e 7215 0000 0072 0400  deletionr....r..
+000002b0: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+000002c0: 0072 1b00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000002d0: 0300 0000 7304 0000 0010 0108 03         ....s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0033_auto_20170616_1251.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0033_auto_20170616_1251.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,41 @@
-00000000: 160d 0d0a a4b0 1f5d 9401 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c 9401 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0007 0000 0040 0000 0073  ...........@...s
-000000b0: 4000 0000 6500 005a 0100 6400 005a 0200  @...e..Z..d..Z..
-000000c0: 6409 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 8300 0083 0003 6701 005a 0800  .j........g..Z..
-000000f0: 6408 0053 290a da09 4d69 6772 6174 696f  d..S)...Migratio
-00000100: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
-00000110: da17 3030 3332 5f61 7574 6f5f 3230 3137  ..0032_auto_2017
-00000120: 3036 3136 5f31 3134 34da 0a6d 6f64 656c  0616_1144..model
-00000130: 5f6e 616d 65da 0773 796e 636a 6f62 da04  _name..syncjob..
-00000140: 6e61 6d65 da0a 7374 6172 745f 7469 6d65  name..start_time
-00000150: da05 6669 656c 644e 2902 7a0d 646a 636f  ..fieldN).z.djco
-00000160: 6e6e 6563 7477 6973 657a 1730 3033 325f  nnectwisez.0032_
-00000170: 6175 746f 5f32 3031 3730 3631 365f 3131  auto_20170616_11
-00000180: 3434 2909 da08 5f5f 6e61 6d65 5f5f da0a  44)...__name__..
-00000190: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000001a0: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
-000001b0: 656e 6369 6573 7203 0000 00da 0a41 6c74  enciesr......Alt
-000001c0: 6572 4669 656c 6472 0400 0000 da0d 4461  erFieldr......Da
-000001d0: 7465 5469 6d65 4669 656c 64da 0a6f 7065  teTimeField..ope
-000001e0: 7261 7469 6f6e 73a9 0072 1400 0000 7214  rations..r....r.
-000001f0: 0000 00fa 6e2f 686f 6d65 2f73 616d 2f67  ....n/home/sam/g
-00000200: 6974 2f4b 616e 6261 6e2f 646a 616e 676f  it/Kanban/django
-00000210: 2d63 6f6e 6e65 6374 7769 7365 2f64 6a61  -connectwise/dja
-00000220: 6e67 6f2d 636f 6e6e 6563 7477 6973 652f  ngo-connectwise/
-00000230: 646a 636f 6e6e 6563 7477 6973 652f 6d69  djconnectwise/mi
-00000240: 6772 6174 696f 6e73 2f30 3033 335f 6175  grations/0033_au
-00000250: 746f 5f32 3031 3730 3631 365f 3132 3531  to_20170616_1251
-00000260: 2e70 7972 0500 0000 0700 0000 730a 0000  .pyr........s...
-00000270: 000c 0309 0409 0106 0106 0172 0500 0000  ...........r....
-00000280: 4e29 06da 0a5f 5f66 7574 7572 655f 5f72  N)...__future__r
-00000290: 0200 0000 da09 646a 616e 676f 2e64 6272  ......django.dbr
-000002a0: 0300 0000 7204 0000 0072 0500 0000 7214  ....r....r....r.
-000002b0: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-000002c0: 0000 da08 3c6d 6f64 756c 653e 0200 0000  ....<module>....
-000002d0: 7304 0000 0010 0216 03                   s........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0500 0000 4000 0000 7328  ..........@...s(
+000000a0: 0000 0065 005a 0164 005a 0264 0767 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0783 0064  .e.j.d.d.e.j...d
+000000c0: 058d 0367 015a 0864 0653 0029 08da 094d  ...g.Z.d.S.)...M
+000000d0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
+000000e0: 6563 7477 6973 65da 1730 3033 325f 6175  ectwise..0032_au
+000000f0: 746f 5f32 3031 3730 3631 365f 3131 3434  to_20170616_1144
+00000100: 5a07 7379 6e63 6a6f 62da 0a73 7461 7274  Z.syncjob..start
+00000110: 5f74 696d 6529 03da 0a6d 6f64 656c 5f6e  _time)...model_n
+00000120: 616d 65da 046e 616d 65da 0566 6965 6c64  ame..name..field
+00000130: 4e29 0272 0600 0000 7207 0000 0029 09da  N).r....r....)..
+00000140: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000150: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000160: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
+00000170: 7372 0300 0000 da0a 416c 7465 7246 6965  sr......AlterFie
+00000180: 6c64 7204 0000 00da 0d44 6174 6554 696d  ldr......DateTim
+00000190: 6546 6965 6c64 da0a 6f70 6572 6174 696f  eField..operatio
+000001a0: 6e73 a900 7213 0000 0072 1300 0000 fa63  ns..r....r.....c
+000001b0: 2f68 6f6d 652f 6361 6d65 726f 6e2f 4465  /home/cameron/De
+000001c0: 762f 6b61 6e62 616e 2d64 6576 2f64 6a61  v/kanban-dev/dja
+000001d0: 6e67 6f2d 636f 6e6e 6563 7477 6973 652f  ngo-connectwise/
+000001e0: 646a 636f 6e6e 6563 7477 6973 652f 6d69  djconnectwise/mi
+000001f0: 6772 6174 696f 6e73 2f30 3033 335f 6175  grations/0033_au
+00000200: 746f 5f32 3031 3730 3631 365f 3132 3531  to_20170616_1251
+00000210: 2e70 7972 0500 0000 0700 0000 730a 0000  .pyr........s...
+00000220: 0008 0306 0404 0102 0102 0172 0500 0000  ...........r....
+00000230: 4e29 06da 0a5f 5f66 7574 7572 655f 5f72  N)...__future__r
+00000240: 0200 0000 da09 646a 616e 676f 2e64 6272  ......django.dbr
+00000250: 0300 0000 7204 0000 0072 0500 0000 7213  ....r....r....r.
+00000260: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+00000270: 0000 da08 3c6d 6f64 756c 653e 0200 0000  ....<module>....
+00000280: 7304 0000 000c 0210 03                   s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0091_workrole.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0066_slapriority.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,80 @@
-00000000: 160d 0d0a 22b1 305d 1504 0000 e300 0000  ....".0]........
+00000000: 330d 0d0a 10ec da5c 6105 0000 e300 0000  3......\a.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 0e00 0000 4000 0000 73df 0000 0065 0000  ....@...s....e..
-000000a0: 5a01 0064 0000 5a02 0064 1d00 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6506 006a 0700 6407 0064 0800  .d..e..j..d..d..
-000000d0: 6409 0064 0800 640a 0064 0b00 640c 0064  d..d..d..d..d..d
-000000e0: 0d00 8300 0466 0200 640e 0065 0800 6a09  .....f..d..e..j.
-000000f0: 006a 0a00 6a0b 0064 0f00 6408 0064 0c00  .j..j..d..d..d..
-00000100: 640e 0083 0002 6602 0064 1000 6508 006a  d.....f..d..e..j
-00000110: 0900 6a0a 006a 0c00 6411 0064 0800 640c  ..j..j..d..d..d.
-00000120: 0064 1000 8300 0266 0200 6403 0065 0600  .d.....f..d..e..
-00000130: 6a0d 0064 1200 6413 0083 0001 6602 0064  j..d..d.....f..d
-00000140: 1400 6506 006a 0e00 6415 0064 0b00 8300  ..e..j..d..d....
-00000150: 0166 0200 6705 0064 1600 6417 0064 1e00  .f..g..d..d..d..
-00000160: 641a 0064 1000 641b 0064 0b00 6903 0083  d..d..d..d..i...
-00000170: 0003 6701 005a 0f00 641c 0053 291f da09  ..g..Z..d..S)...
-00000180: 4d69 6772 6174 696f 6eda 0d64 6a63 6f6e  Migration..djcon
-00000190: 6e65 6374 7769 7365 da17 3030 3930 5f61  nectwise..0090_a
-000001a0: 7574 6f5f 3230 3139 3037 3131 5f31 3131  uto_20190711_111
-000001b0: 34da 046e 616d 65da 0857 6f72 6b52 6f6c  4..name..WorkRol
-000001c0: 65da 0666 6965 6c64 73da 0269 64da 0c61  e..fields..id..a
-000001d0: 7574 6f5f 6372 6561 7465 6454 da0b 7072  uto_createdT..pr
-000001e0: 696d 6172 795f 6b65 79da 0973 6572 6961  imary_key..seria
-000001f0: 6c69 7a65 46da 0c76 6572 626f 7365 5f6e  lizeF..verbose_n
-00000200: 616d 65da 0249 44da 0763 7265 6174 6564  ame..ID..created
-00000210: da0c 6175 746f 5f6e 6f77 5f61 6464 da08  ..auto_now_add..
-00000220: 6d6f 6469 6669 6564 da08 6175 746f 5f6e  modified..auto_n
-00000230: 6f77 da0a 6d61 785f 6c65 6e67 7468 e932  ow..max_length.2
-00000240: 0000 00da 0d69 6e61 6374 6976 655f 666c  .....inactive_fl
-00000250: 6167 da07 6465 6661 756c 74da 076f 7074  ag..default..opt
-00000260: 696f 6e73 da08 6f72 6465 7269 6e67 fa09  ions..ordering..
-00000270: 2d6d 6f64 6966 6965 64fa 082d 6372 6561  -modified..-crea
-00000280: 7465 64da 0d67 6574 5f6c 6174 6573 745f  ted..get_latest_
-00000290: 6279 da08 6162 7374 7261 6374 4e29 027a  by..abstractN).z
-000002a0: 0d64 6a63 6f6e 6e65 6374 7769 7365 7a17  .djconnectwisez.
-000002b0: 3030 3930 5f61 7574 6f5f 3230 3139 3037  0090_auto_201907
-000002c0: 3131 5f31 3131 3429 0272 1a00 0000 721b  11_1114).r....r.
-000002d0: 0000 0029 10da 085f 5f6e 616d 655f 5fda  ...)...__name__.
-000002e0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000002f0: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
-00000300: 6465 6e63 6965 7372 0200 0000 da0b 4372  denciesr......Cr
-00000310: 6561 7465 4d6f 6465 6c72 0300 0000 da09  eateModelr......
-00000320: 4175 746f 4669 656c 64da 1164 6a61 6e67  AutoField..djang
-00000330: 6f5f 6578 7465 6e73 696f 6e73 da02 6462  o_extensions..db
-00000340: 7209 0000 00da 1543 7265 6174 696f 6e44  r......CreationD
-00000350: 6174 6554 696d 6546 6965 6c64 da19 4d6f  ateTimeField..Mo
-00000360: 6469 6669 6361 7469 6f6e 4461 7465 5469  dificationDateTi
-00000370: 6d65 4669 656c 64da 0943 6861 7246 6965  meField..CharFie
-00000380: 6c64 da0c 426f 6f6c 6561 6e46 6965 6c64  ld..BooleanField
-00000390: da0a 6f70 6572 6174 696f 6e73 a900 722b  ..operations..r+
-000003a0: 0000 0072 2b00 0000 fa64 2f68 6f6d 652f  ...r+....d/home/
-000003b0: 7361 6d2f 6769 742f 4b61 6e62 616e 2f64  sam/git/Kanban/d
-000003c0: 6a61 6e67 6f2d 636f 6e6e 6563 7477 6973  jango-connectwis
-000003d0: 652f 646a 616e 676f 2d63 6f6e 6e65 6374  e/django-connect
-000003e0: 7769 7365 2f64 6a63 6f6e 6e65 6374 7769  wise/djconnectwi
-000003f0: 7365 2f6d 6967 7261 7469 6f6e 732f 3030  se/migrations/00
-00000400: 3931 5f77 6f72 6b72 6f6c 652e 7079 7204  91_workrole.pyr.
-00000410: 0000 0007 0000 0073 1600 0000 0c03 0904  .......s........
-00000420: 0901 0602 2701 2101 2101 1501 1b03 0601  ....'.!.!.......
-00000430: 0601 7204 0000 0029 06da 0964 6a61 6e67  ..r....)...djang
-00000440: 6f2e 6462 7202 0000 0072 0300 0000 da1b  o.dbr....r......
-00000450: 646a 616e 676f 5f65 7874 656e 7369 6f6e  django_extension
-00000460: 732e 6462 2e66 6965 6c64 7372 2400 0000  s.db.fieldsr$...
-00000470: 7204 0000 0072 2b00 0000 722b 0000 0072  r....r+...r+...r
-00000480: 2b00 0000 722c 0000 00da 083c 6d6f 6475  +...r,.....<modu
-00000490: 6c65 3e03 0000 0073 0400 0000 1601 0c03  le>....s........
+00000020: 0073 3600 0000 6400 6401 6c00 6d01 5a01  .s6...d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 6400  m.Z...d.d.l.Z.d.
+00000040: 6402 6c05 5a06 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
+00000050: 6501 6a07 8303 5a07 6402 5300 2905 e900  e.j...Z.d.S.)...
+00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
+00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
+00000080: 0000 0000 0000 000e 0000 0040 0000 0073  ...........@...s
+00000090: b600 0000 6500 5a01 6400 5a02 641a 6701  ....e.Z.d.Z.d.g.
+000000a0: 5a03 6504 6a05 6403 6404 6506 6a07 6405  Z.e.j.d.d.e.j.d.
+000000b0: 6405 6406 6407 6408 8d04 6602 6409 6508  d.d.d.d...f.d.e.
+000000c0: 6a09 6a0a 6a0b 6405 6409 640a 8d02 6602  j.j.j.d.d.d...f.
+000000d0: 640b 6508 6a09 6a0a 6a0c 6405 640b 640c  d.e.j.j.j.d.d.d.
+000000e0: 8d02 6602 640d 6506 6a0d 8300 6602 640e  ..f.d.e.j...f.d.
+000000f0: 6506 6a0d 8300 6602 640f 6506 6a0d 8300  e.j...f.d.e.j...
+00000100: 6602 6410 6506 6a0e 650f 6a09 6a06 6a10  f.d.e.j.e.j.j.j.
+00000110: 6a11 6411 6412 8d02 6602 6413 6506 6a0e  j.d.d...f.d.e.j.
+00000120: 650f 6a09 6a06 6a10 6a11 6414 6412 8d02  e.j.j.j.j.d.d...
+00000130: 6602 6708 641b 640b 6406 6417 9c03 6418  f.g.d.d.d.d...d.
+00000140: 8d03 6701 5a12 6419 5300 291c da09 4d69  ..g.Z.d.S.)...Mi
+00000150: 6772 6174 696f 6eda 0d64 6a63 6f6e 6e65  gration..djconne
+00000160: 6374 7769 7365 da17 3030 3635 5f61 7574  ctwise..0065_aut
+00000170: 6f5f 3230 3138 3038 3039 5f31 3132 34da  o_20180809_1124.
+00000180: 0b53 6c61 5072 696f 7269 7479 da02 6964  .SlaPriority..id
+00000190: 5446 da02 4944 2904 da0c 6175 746f 5f63  TF..ID)...auto_c
+000001a0: 7265 6174 6564 da0b 7072 696d 6172 795f  reated..primary_
+000001b0: 6b65 79da 0973 6572 6961 6c69 7a65 da0c  key..serialize..
+000001c0: 7665 7262 6f73 655f 6e61 6d65 da07 6372  verbose_name..cr
+000001d0: 6561 7465 6429 02da 0c61 7574 6f5f 6e6f  eated)...auto_no
+000001e0: 775f 6164 6472 0d00 0000 da08 6d6f 6469  w_addr......modi
+000001f0: 6669 6564 2902 da08 6175 746f 5f6e 6f77  fied)...auto_now
+00000200: 720d 0000 00da 0d72 6573 706f 6e64 5f68  r......respond_h
+00000210: 6f75 7273 da0b 706c 616e 5f77 6974 6869  ours..plan_withi
+00000220: 6eda 1072 6573 6f6c 7574 696f 6e5f 686f  n..resolution_ho
+00000230: 7572 73da 0870 7269 6f72 6974 797a 1c64  urs..priorityz.d
+00000240: 6a63 6f6e 6e65 6374 7769 7365 2e54 6963  jconnectwise.Tic
+00000250: 6b65 7450 7269 6f72 6974 7929 02da 096f  ketPriority)...o
+00000260: 6e5f 6465 6c65 7465 da02 746f da03 736c  n_delete..to..sl
+00000270: 617a 1164 6a63 6f6e 6e65 6374 7769 7365  az.djconnectwise
+00000280: 2e53 6c61 fa09 2d6d 6f64 6966 6965 64fa  .Sla..-modified.
+00000290: 082d 6372 6561 7465 6429 03da 086f 7264  .-created)...ord
+000002a0: 6572 696e 67da 0d67 6574 5f6c 6174 6573  ering..get_lates
+000002b0: 745f 6279 da08 6162 7374 7261 6374 2903  t_by..abstract).
+000002c0: da04 6e61 6d65 da06 6669 656c 6473 da07  ..name..fields..
+000002d0: 6f70 7469 6f6e 734e 2902 7205 0000 0072  optionsN).r....r
+000002e0: 0600 0000 2902 7219 0000 0072 1a00 0000  ....).r....r....
+000002f0: 2913 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000300: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000310: 6e61 6d65 5f5f da0c 6465 7065 6e64 656e  name__..dependen
+00000320: 6369 6573 7202 0000 00da 0b43 7265 6174  ciesr......Creat
+00000330: 654d 6f64 656c 7203 0000 00da 0941 7574  eModelr......Aut
+00000340: 6f46 6965 6c64 da11 646a 616e 676f 5f65  oField..django_e
+00000350: 7874 656e 7369 6f6e 73da 0264 6272 1f00  xtensions..dbr..
+00000360: 0000 da15 4372 6561 7469 6f6e 4461 7465  ....CreationDate
+00000370: 5469 6d65 4669 656c 64da 194d 6f64 6966  TimeField..Modif
+00000380: 6963 6174 696f 6e44 6174 6554 696d 6546  icationDateTimeF
+00000390: 6965 6c64 da0f 4269 6749 6e74 6567 6572  ield..BigInteger
+000003a0: 4669 656c 64da 0a46 6f72 6569 676e 4b65  Field..ForeignKe
+000003b0: 79da 0664 6a61 6e67 6fda 0864 656c 6574  y..django..delet
+000003c0: 696f 6eda 0743 4153 4341 4445 da0a 6f70  ion..CASCADE..op
+000003d0: 6572 6174 696f 6e73 a900 7231 0000 0072  erations..r1...r
+000003e0: 3100 0000 fa5c 2f68 6f6d 652f 6361 6d65  1....\/home/came
+000003f0: 726f 6e2f 4465 762f 6b61 6e62 616e 2d64  ron/Dev/kanban-d
+00000400: 6576 2f64 6a61 6e67 6f2d 636f 6e6e 6563  ev/django-connec
+00000410: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
+00000420: 6973 652f 6d69 6772 6174 696f 6e73 2f30  ise/migrations/0
+00000430: 3036 365f 736c 6170 7269 6f72 6974 792e  066_slapriority.
+00000440: 7079 7204 0000 0008 0000 0073 1c00 0000  pyr........s....
+00000450: 0803 0604 0401 0202 1401 1401 1401 0a01  ................
+00000460: 0a01 0a01 1801 1a03 0201 0201 7204 0000  ............r...
+00000470: 0029 08da 0964 6a61 6e67 6f2e 6462 7202  .)...django.dbr.
+00000480: 0000 0072 0300 0000 da19 646a 616e 676f  ...r......django
+00000490: 2e64 622e 6d6f 6465 6c73 2e64 656c 6574  .db.models.delet
+000004a0: 696f 6e72 2d00 0000 da1b 646a 616e 676f  ionr-.....django
+000004b0: 5f65 7874 656e 7369 6f6e 732e 6462 2e66  _extensions.db.f
+000004c0: 6965 6c64 7372 2700 0000 7204 0000 0072  ieldsr'...r....r
+000004d0: 3100 0000 7231 0000 0072 3100 0000 7232  1...r1...r1...r2
+000004e0: 0000 00da 083c 6d6f 6475 6c65 3e03 0000  .....<module>...
+000004f0: 0073 0600 0000 1001 0801 0803            .s..........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0027_auto_20170605_1534.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0012_auto_20170320_1057.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-00000000: 160d 0d0a a4b0 1f5d a801 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c 4802 0000 e300 0000  3......\H.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 000d 0000 0040 0000 0073  ...........@...s
-000000b0: 5200 0000 6500 005a 0100 6400 005a 0200  R...e..Z..d..Z..
-000000c0: 640e 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 6408 0064 0900 640a 0064 0b00  .j..d..d..d..d..
-000000f0: 640c 0064 0b00 8300 0383 0003 6701 005a  d..d........g..Z
-00000100: 0800 640d 0053 290f da09 4d69 6772 6174  ..d..S)...Migrat
-00000110: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-00000120: 7365 da0a 3030 3236 5f6d 6572 6765 da0a  se..0026_merge..
-00000130: 6d6f 6465 6c5f 6e61 6d65 da0b 6f70 706f  model_name..oppo
-00000140: 7274 756e 6974 79da 046e 616d 65da 0673  rtunity..name..s
-00000150: 6f75 7263 65da 0566 6965 6c64 da0a 6d61  ource..field..ma
-00000160: 785f 6c65 6e67 7468 e964 0000 00da 0562  x_length.d.....b
-00000170: 6c61 6e6b 54da 046e 756c 6c4e 2902 7a0d  lankT..nullN).z.
-00000180: 646a 636f 6e6e 6563 7477 6973 6572 0700  djconnectwiser..
-00000190: 0000 2909 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
-000001a0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000001b0: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
-000001c0: 656e 6369 6573 7203 0000 00da 0a41 6c74  enciesr......Alt
-000001d0: 6572 4669 656c 6472 0400 0000 da09 4368  erFieldr......Ch
-000001e0: 6172 4669 656c 64da 0a6f 7065 7261 7469  arField..operati
-000001f0: 6f6e 73a9 0072 1800 0000 7218 0000 00fa  ons..r....r.....
-00000200: 6e2f 686f 6d65 2f73 616d 2f67 6974 2f4b  n/home/sam/git/K
-00000210: 616e 6261 6e2f 646a 616e 676f 2d63 6f6e  anban/django-con
-00000220: 6e65 6374 7769 7365 2f64 6a61 6e67 6f2d  nectwise/django-
-00000230: 636f 6e6e 6563 7477 6973 652f 646a 636f  connectwise/djco
-00000240: 6e6e 6563 7477 6973 652f 6d69 6772 6174  nnectwise/migrat
-00000250: 696f 6e73 2f30 3032 375f 6175 746f 5f32  ions/0027_auto_2
-00000260: 3031 3730 3630 355f 3135 3334 2e70 7972  0170605_1534.pyr
-00000270: 0500 0000 0700 0000 730a 0000 000c 0309  ........s.......
-00000280: 0409 0106 0106 0172 0500 0000 4e29 06da  .......r....N)..
-00000290: 0a5f 5f66 7574 7572 655f 5f72 0200 0000  .__future__r....
-000002a0: da09 646a 616e 676f 2e64 6272 0300 0000  ..django.dbr....
-000002b0: 7204 0000 0072 0500 0000 7218 0000 0072  r....r....r....r
-000002c0: 1800 0000 7218 0000 0072 1900 0000 da08  ....r....r......
-000002d0: 3c6d 6f64 756c 653e 0200 0000 7304 0000  <module>....s...
-000002e0: 0010 0216 03                             .....
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0800 0000 4000 0000 7340  ..........@...s@
+000000a0: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0783 0064  .e.j.d.d.e.j...d
+000000c0: 058d 0365 046a 0564 0364 0665 066a 0864  ...e.j.d.d.e.j.d
+000000d0: 0764 0764 088d 0264 058d 0367 025a 0964  .d.d...d...g.Z.d
+000000e0: 0953 0029 0bda 094d 6967 7261 7469 6f6e  .S.)...Migration
+000000f0: da0d 646a 636f 6e6e 6563 7477 6973 65da  ..djconnectwise.
+00000100: 1930 3031 315f 636f 6d70 616e 795f 6465  .0011_company_de
+00000110: 6c65 7465 645f 666c 6167 da06 7469 636b  leted_flag..tick
+00000120: 6574 da10 6861 735f 6368 696c 645f 7469  et..has_child_ti
+00000130: 636b 6574 2903 da0a 6d6f 6465 6c5f 6e61  cket)...model_na
+00000140: 6d65 da04 6e61 6d65 da05 6669 656c 64da  me..name..field.
+00000150: 1070 6172 656e 745f 7469 636b 6574 5f69  .parent_ticket_i
+00000160: 6454 2902 da05 626c 616e 6bda 046e 756c  dT)...blank..nul
+00000170: 6c4e 2902 7206 0000 0072 0700 0000 290a  lN).r....r....).
+00000180: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000190: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+000001a0: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
+000001b0: 6573 7203 0000 00da 0841 6464 4669 656c  esr......AddFiel
+000001c0: 6472 0400 0000 da10 4e75 6c6c 426f 6f6c  dr......NullBool
+000001d0: 6561 6e46 6965 6c64 da0c 496e 7465 6765  eanField..Intege
+000001e0: 7246 6965 6c64 da0a 6f70 6572 6174 696f  rField..operatio
+000001f0: 6e73 a900 7218 0000 0072 1800 0000 fa63  ns..r....r.....c
+00000200: 2f68 6f6d 652f 6361 6d65 726f 6e2f 4465  /home/cameron/De
+00000210: 762f 6b61 6e62 616e 2d64 6576 2f64 6a61  v/kanban-dev/dja
+00000220: 6e67 6f2d 636f 6e6e 6563 7477 6973 652f  ngo-connectwise/
+00000230: 646a 636f 6e6e 6563 7477 6973 652f 6d69  djconnectwise/mi
+00000240: 6772 6174 696f 6e73 2f30 3031 325f 6175  grations/0012_au
+00000250: 746f 5f32 3031 3730 3332 305f 3130 3537  to_20170320_1057
+00000260: 2e70 7972 0500 0000 0700 0000 7312 0000  .pyr........s...
+00000270: 0008 0306 0404 0102 0102 010a 0204 0102  ................
+00000280: 0102 0172 0500 0000 4e29 06da 0a5f 5f66  ...r....N)...__f
+00000290: 7574 7572 655f 5f72 0200 0000 da09 646a  uture__r......dj
+000002a0: 616e 676f 2e64 6272 0300 0000 7204 0000  ango.dbr....r...
+000002b0: 0072 0500 0000 7218 0000 0072 1800 0000  .r....r....r....
+000002c0: 7218 0000 0072 1900 0000 da08 3c6d 6f64  r....r......<mod
+000002d0: 756c 653e 0200 0000 7304 0000 000c 0210  ule>....s.......
+000002e0: 03                                       .
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0046_auto_20180104_1504.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0027_auto_20170605_1534.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,43 @@
-00000000: 160d 0d0a a4b0 1f5d b501 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c a801 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 000d 0000 0040 0000 0073  ...........@...s
-000000b0: 5200 0000 6500 005a 0100 6400 005a 0200  R...e..Z..d..Z..
-000000c0: 640d 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6405 0064 0600 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 6407 0064 0800 6409 0064 0a00  .j..d..d..d..d..
-000000f0: 640b 0064 0800 8300 0383 0003 6701 005a  d..d........g..Z
-00000100: 0800 640c 0053 290e da09 4d69 6772 6174  ..d..S)...Migrat
-00000110: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-00000120: 7365 da17 3030 3435 5f61 7574 6f5f 3230  se..0045_auto_20
-00000130: 3137 3132 3232 5f31 3732 35da 0a6d 6f64  171222_1725..mod
-00000140: 656c 5f6e 616d 65da 0d73 6368 6564 756c  el_name..schedul
-00000150: 6565 6e74 7279 da04 6e61 6d65 da05 6669  eentry..name..fi
-00000160: 656c 64da 046e 756c 6c54 da0a 6d61 785f  eld..nullT..max_
-00000170: 6c65 6e67 7468 e9fa 0000 00da 0562 6c61  length.......bla
-00000180: 6e6b 4e29 027a 0d64 6a63 6f6e 6e65 6374  nkN).z.djconnect
-00000190: 7769 7365 7a17 3030 3435 5f61 7574 6f5f  wisez.0045_auto_
-000001a0: 3230 3137 3132 3232 5f31 3732 3529 09da  20171222_1725)..
-000001b0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000001c0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000001d0: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
-000001e0: 7372 0300 0000 da0a 416c 7465 7246 6965  sr......AlterFie
-000001f0: 6c64 7204 0000 00da 0943 6861 7246 6965  ldr......CharFie
-00000200: 6c64 da0a 6f70 6572 6174 696f 6e73 a900  ld..operations..
-00000210: 7217 0000 0072 1700 0000 fa6e 2f68 6f6d  r....r.....n/hom
-00000220: 652f 7361 6d2f 6769 742f 4b61 6e62 616e  e/sam/git/Kanban
-00000230: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
-00000240: 6973 652f 646a 616e 676f 2d63 6f6e 6e65  ise/django-conne
-00000250: 6374 7769 7365 2f64 6a63 6f6e 6e65 6374  ctwise/djconnect
-00000260: 7769 7365 2f6d 6967 7261 7469 6f6e 732f  wise/migrations/
-00000270: 3030 3436 5f61 7574 6f5f 3230 3138 3031  0046_auto_201801
-00000280: 3034 5f31 3530 342e 7079 7205 0000 0007  04_1504.pyr.....
-00000290: 0000 0073 0a00 0000 0c03 0904 0901 0601  ...s............
-000002a0: 0601 7205 0000 004e 2906 da0a 5f5f 6675  ..r....N)...__fu
-000002b0: 7475 7265 5f5f 7202 0000 00da 0964 6a61  ture__r......dja
-000002c0: 6e67 6f2e 6462 7203 0000 0072 0400 0000  ngo.dbr....r....
-000002d0: 7205 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
-000002e0: 1700 0000 7218 0000 00da 083c 6d6f 6475  ....r......<modu
-000002f0: 6c65 3e02 0000 0073 0400 0000 1002 1603  le>....s........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0800 0000 4000 0000 7330  ..........@...s0
+000000a0: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000c0: 0664 0664 078d 0364 088d 0367 015a 0864  .d.d...d...g.Z.d
+000000d0: 0953 0029 0bda 094d 6967 7261 7469 6f6e  .S.)...Migration
+000000e0: da0d 646a 636f 6e6e 6563 7477 6973 65da  ..djconnectwise.
+000000f0: 0a30 3032 365f 6d65 7267 65da 0b6f 7070  .0026_merge..opp
+00000100: 6f72 7475 6e69 7479 da06 736f 7572 6365  ortunity..source
+00000110: e964 0000 0054 2903 da0a 6d61 785f 6c65  .d...T)...max_le
+00000120: 6e67 7468 da05 626c 616e 6bda 046e 756c  ngth..blank..nul
+00000130: 6c29 03da 0a6d 6f64 656c 5f6e 616d 65da  l)...model_name.
+00000140: 046e 616d 65da 0566 6965 6c64 4e29 0272  .name..fieldN).r
+00000150: 0600 0000 7207 0000 0029 09da 085f 5f6e  ....r....)...__n
+00000160: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000170: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000180: 0c64 6570 656e 6465 6e63 6965 7372 0300  .dependenciesr..
+00000190: 0000 da0a 416c 7465 7246 6965 6c64 7204  ....AlterFieldr.
+000001a0: 0000 00da 0943 6861 7246 6965 6c64 da0a  .....CharField..
+000001b0: 6f70 6572 6174 696f 6e73 a900 7218 0000  operations..r...
+000001c0: 0072 1800 0000 fa63 2f68 6f6d 652f 6361  .r.....c/home/ca
+000001d0: 6d65 726f 6e2f 4465 762f 6b61 6e62 616e  meron/Dev/kanban
+000001e0: 2d64 6576 2f64 6a61 6e67 6f2d 636f 6e6e  -dev/django-conn
+000001f0: 6563 7477 6973 652f 646a 636f 6e6e 6563  ectwise/djconnec
+00000200: 7477 6973 652f 6d69 6772 6174 696f 6e73  twise/migrations
+00000210: 2f30 3032 375f 6175 746f 5f32 3031 3730  /0027_auto_20170
+00000220: 3630 355f 3135 3334 2e70 7972 0500 0000  605_1534.pyr....
+00000230: 0700 0000 730a 0000 0008 0306 0404 0102  ....s...........
+00000240: 0102 0172 0500 0000 4e29 06da 0a5f 5f66  ...r....N)...__f
+00000250: 7574 7572 655f 5f72 0200 0000 da09 646a  uture__r......dj
+00000260: 616e 676f 2e64 6272 0300 0000 7204 0000  ango.dbr....r...
+00000270: 0072 0500 0000 7218 0000 0072 1800 0000  .r....r....r....
+00000280: 7218 0000 0072 1900 0000 da08 3c6d 6f64  r....r......<mod
+00000290: 756c 653e 0200 0000 7304 0000 000c 0210  ule>....s.......
+000002a0: 03                                       .
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0015_auto_20170404_1504.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0015_auto_20170404_1504.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,44 @@
-00000000: 160d 0d0a a4b0 1f5d b601 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c b601 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 000b 0000 0040 0000 0073  ...........@...s
-000000b0: 4c00 0000 6500 005a 0100 6400 005a 0200  L...e..Z..d..Z..
-000000c0: 640d 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 6408 0064 0900 640a 0064 0b00  .j..d..d..d..d..
-000000f0: 8300 0283 0003 6701 005a 0800 640c 0053  ......g..Z..d..S
-00000100: 290e da09 4d69 6772 6174 696f 6eda 0d64  )...Migration..d
-00000110: 6a63 6f6e 6e65 6374 7769 7365 da13 3030  jconnectwise..00
-00000120: 3134 5f63 6f6d 7061 6e79 5f73 7461 7475  14_company_statu
-00000130: 73da 0a6d 6f64 656c 5f6e 616d 65da 0d63  s..model_name..c
-00000140: 6f6d 7061 6e79 7374 6174 7573 da04 6e61  ompanystatus..na
-00000150: 6d65 da14 6e6f 7469 6669 6361 7469 6f6e  me..notification
-00000160: 5f6d 6573 7361 6765 da05 6669 656c 64da  _message..field.
-00000170: 0a6d 6178 5f6c 656e 6774 6869 f401 0000  .max_lengthi....
-00000180: da05 626c 616e 6b54 4e29 027a 0d64 6a63  ..blankTN).z.djc
-00000190: 6f6e 6e65 6374 7769 7365 7207 0000 0029  onnectwiser....)
-000001a0: 09da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000001b0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000001c0: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
-000001d0: 6965 7372 0300 0000 da0a 416c 7465 7246  iesr......AlterF
-000001e0: 6965 6c64 7204 0000 00da 0943 6861 7246  ieldr......CharF
-000001f0: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
-00000200: a900 7216 0000 0072 1600 0000 fa6e 2f68  ..r....r.....n/h
-00000210: 6f6d 652f 7361 6d2f 6769 742f 4b61 6e62  ome/sam/git/Kanb
-00000220: 616e 2f64 6a61 6e67 6f2d 636f 6e6e 6563  an/django-connec
-00000230: 7477 6973 652f 646a 616e 676f 2d63 6f6e  twise/django-con
-00000240: 6e65 6374 7769 7365 2f64 6a63 6f6e 6e65  nectwise/djconne
-00000250: 6374 7769 7365 2f6d 6967 7261 7469 6f6e  ctwise/migration
-00000260: 732f 3030 3135 5f61 7574 6f5f 3230 3137  s/0015_auto_2017
-00000270: 3034 3034 5f31 3530 342e 7079 7205 0000  0404_1504.pyr...
-00000280: 0007 0000 0073 0a00 0000 0c03 0904 0901  .....s..........
-00000290: 0601 0601 7205 0000 004e 2906 da0a 5f5f  ....r....N)...__
-000002a0: 6675 7475 7265 5f5f 7202 0000 00da 0964  future__r......d
-000002b0: 6a61 6e67 6f2e 6462 7203 0000 0072 0400  jango.dbr....r..
-000002c0: 0000 7205 0000 0072 1600 0000 7216 0000  ..r....r....r...
-000002d0: 0072 1600 0000 7217 0000 00da 083c 6d6f  .r....r......<mo
-000002e0: 6475 6c65 3e02 0000 0073 0400 0000 1002  dule>....s......
-000002f0: 1603                                     ..
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0700 0000 4000 0000 732e  ..........@...s.
+000000a0: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000c0: 0664 078d 0264 088d 0367 015a 0864 0953  .d...d...g.Z.d.S
+000000d0: 0029 0bda 094d 6967 7261 7469 6f6e da0d  .)...Migration..
+000000e0: 646a 636f 6e6e 6563 7477 6973 65da 1330  djconnectwise..0
+000000f0: 3031 345f 636f 6d70 616e 795f 7374 6174  014_company_stat
+00000100: 7573 da0d 636f 6d70 616e 7973 7461 7475  us..companystatu
+00000110: 73da 146e 6f74 6966 6963 6174 696f 6e5f  s..notification_
+00000120: 6d65 7373 6167 6569 f401 0000 5429 02da  messagei....T)..
+00000130: 0a6d 6178 5f6c 656e 6774 68da 0562 6c61  .max_length..bla
+00000140: 6e6b 2903 da0a 6d6f 6465 6c5f 6e61 6d65  nk)...model_name
+00000150: da04 6e61 6d65 da05 6669 656c 644e 2902  ..name..fieldN).
+00000160: 7206 0000 0072 0700 0000 2909 da08 5f5f  r....r....)...__
+00000170: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000180: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000190: da0c 6465 7065 6e64 656e 6369 6573 7203  ..dependenciesr.
+000001a0: 0000 00da 0a41 6c74 6572 4669 656c 6472  .....AlterFieldr
+000001b0: 0400 0000 da09 4368 6172 4669 656c 64da  ......CharField.
+000001c0: 0a6f 7065 7261 7469 6f6e 73a9 0072 1600  .operations..r..
+000001d0: 0000 7216 0000 00fa 632f 686f 6d65 2f63  ..r.....c/home/c
+000001e0: 616d 6572 6f6e 2f44 6576 2f6b 616e 6261  ameron/Dev/kanba
+000001f0: 6e2d 6465 762f 646a 616e 676f 2d63 6f6e  n-dev/django-con
+00000200: 6e65 6374 7769 7365 2f64 6a63 6f6e 6e65  nectwise/djconne
+00000210: 6374 7769 7365 2f6d 6967 7261 7469 6f6e  ctwise/migration
+00000220: 732f 3030 3135 5f61 7574 6f5f 3230 3137  s/0015_auto_2017
+00000230: 3034 3034 5f31 3530 342e 7079 7205 0000  0404_1504.pyr...
+00000240: 0007 0000 0073 0a00 0000 0803 0604 0401  .....s..........
+00000250: 0201 0201 7205 0000 004e 2906 da0a 5f5f  ....r....N)...__
+00000260: 6675 7475 7265 5f5f 7202 0000 00da 0964  future__r......d
+00000270: 6a61 6e67 6f2e 6462 7203 0000 0072 0400  jango.dbr....r..
+00000280: 0000 7205 0000 0072 1600 0000 7216 0000  ..r....r....r...
+00000290: 0072 1600 0000 7217 0000 00da 083c 6d6f  .r....r......<mo
+000002a0: 6475 6c65 3e02 0000 0073 0400 0000 0c02  dule>....s......
+000002b0: 1003                                     ..
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0096_agreement.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0096_agreement.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,101 +1,89 @@
-00000000: 160d 0d0a ced8 355d bd05 0000 e300 0000  ......5]........
+00000000: 330d 0d0a 2a3e 545d bd05 0000 e300 0000  3...*>T]........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4b00 0000 6400 0064 0100 6c00 006d  .sK...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 6400 0064 0200 6c05  ..l..Z..d..d..l.
-00000050: 005a 0600 4764 0300 6404 0084 0000 6404  .Z..Gd..d.....d.
-00000060: 0065 0100 6a07 0083 0300 5a07 0064 0200  .e..j.....Z..d..
-00000070: 5329 05e9 0000 0000 2902 da0a 6d69 6772  S)......)...migr
-00000080: 6174 696f 6e73 da06 6d6f 6465 6c73 4e63  ations..modelsNc
-00000090: 0000 0000 0000 0000 0000 0000 1200 0000  ................
-000000a0: 4000 0000 7354 0100 0065 0000 5a01 0064  @...sT...e..Z..d
-000000b0: 0000 5a02 0064 2b00 6701 005a 0300 6504  ..Z..d+.g..Z..e.
-000000c0: 006a 0500 6403 0064 0400 6405 0064 0600  .j..d..d..d..d..
-000000d0: 6506 006a 0700 6407 0064 0800 6409 0064  e..j..d..d..d..d
-000000e0: 0800 640a 0064 0b00 640c 0064 0d00 8300  ..d..d..d..d....
-000000f0: 0466 0200 640e 0065 0800 6a09 006a 0a00  .f..d..e..j..j..
-00000100: 6a0b 0064 0f00 6408 0064 0c00 640e 0083  j..d..d..d..d...
-00000110: 0002 6602 0064 1000 6508 006a 0900 6a0a  ..f..d..e..j..j.
-00000120: 006a 0c00 6411 0064 0800 640c 0064 1000  .j..d..d..d..d..
-00000130: 8300 0266 0200 6403 0065 0600 6a0d 0064  ...f..d..e..j..d
-00000140: 1200 6413 0083 0001 6602 0064 1400 6506  ..d.....f..d..e.
-00000150: 006a 0d00 6415 0064 0800 6416 0064 2c00  .j..d..d..d..d,.
-00000160: 642d 0064 2e00 6703 0064 1200 641c 0064  d-.d..g..d..d..d
-00000170: 1d00 6408 0083 0004 6602 0064 1e00 6506  ..d.....f..d..e.
-00000180: 006a 0e00 641d 0064 0800 641f 0065 0f00  .j..d..d..d..e..
-00000190: 6a09 006a 0600 6a10 006a 1100 6420 0064  j..j..j..j..d .d
-000001a0: 2100 8300 0366 0200 6422 0065 0600 6a0e  !....f..d".e..j.
-000001b0: 0064 1d00 6408 0064 1f00 650f 006a 0900  .d..d..d..e..j..
-000001c0: 6a06 006a 1000 6a11 0064 2000 6423 0083  j..j..j..d .d#..
-000001d0: 0003 6602 0067 0700 6424 0064 2500 642f  ..f..g..d$.d%.d/
-000001e0: 0064 2800 6410 0064 2900 640b 0069 0300  .d(.d..d).d..i..
-000001f0: 8300 0367 0100 5a12 0064 2a00 5329 30da  ...g..Z..d*.S)0.
-00000200: 094d 6967 7261 7469 6f6e da0d 646a 636f  .Migration..djco
-00000210: 6e6e 6563 7477 6973 65da 1f30 3039 355f  nnectwise..0095_
-00000220: 636f 6e6e 6563 7477 6973 6562 6f61 7264  connectwiseboard
-00000230: 5f77 6f72 6b5f 7479 7065 da04 6e61 6d65  _work_type..name
-00000240: da09 4167 7265 656d 656e 74da 0666 6965  ..Agreement..fie
-00000250: 6c64 73da 0269 64da 0c61 7574 6f5f 6372  lds..id..auto_cr
-00000260: 6561 7465 6454 da0b 7072 696d 6172 795f  eatedT..primary_
-00000270: 6b65 79da 0973 6572 6961 6c69 7a65 46da  key..serializeF.
-00000280: 0c76 6572 626f 7365 5f6e 616d 65da 0249  .verbose_name..I
-00000290: 44da 0763 7265 6174 6564 da0c 6175 746f  D..created..auto
-000002a0: 5f6e 6f77 5f61 6464 da08 6d6f 6469 6669  _now_add..modifi
-000002b0: 6564 da08 6175 746f 5f6e 6f77 da0a 6d61  ed..auto_now..ma
-000002c0: 785f 6c65 6e67 7468 e964 0000 00da 0962  x_length.d.....b
-000002d0: 696c 6c5f 7469 6d65 da05 626c 616e 6bda  ill_time..blank.
-000002e0: 0763 686f 6963 6573 da08 4269 6c6c 6162  .choices..Billab
-000002f0: 6c65 da09 446f 4e6f 7442 696c 6cfa 0b44  le..DoNotBill..D
-00000300: 6f20 4e6f 7420 4269 6c6c da08 4e6f 4368  o Not Bill..NoCh
-00000310: 6172 6765 fa09 4e6f 2043 6861 7267 65e9  arge..No Charge.
-00000320: 3200 0000 da04 6e75 6c6c da09 776f 726b  2.....null..work
-00000330: 5f72 6f6c 65da 096f 6e5f 6465 6c65 7465  _role..on_delete
-00000340: da02 746f 7a16 646a 636f 6e6e 6563 7477  ..toz.djconnectw
-00000350: 6973 652e 576f 726b 526f 6c65 da09 776f  ise.WorkRole..wo
-00000360: 726b 5f74 7970 657a 1664 6a63 6f6e 6e65  rk_typez.djconne
-00000370: 6374 7769 7365 2e57 6f72 6b54 7970 65da  ctwise.WorkType.
-00000380: 076f 7074 696f 6e73 da08 6f72 6465 7269  .options..orderi
-00000390: 6e67 fa09 2d6d 6f64 6966 6965 64fa 082d  ng..-modified..-
-000003a0: 6372 6561 7465 64da 0d67 6574 5f6c 6174  created..get_lat
-000003b0: 6573 745f 6279 da08 6162 7374 7261 6374  est_by..abstract
-000003c0: 4e29 027a 0d64 6a63 6f6e 6e65 6374 7769  N).z.djconnectwi
-000003d0: 7365 7a1f 3030 3935 5f63 6f6e 6e65 6374  sez.0095_connect
-000003e0: 7769 7365 626f 6172 645f 776f 726b 5f74  wiseboard_work_t
-000003f0: 7970 6529 02fa 0842 696c 6c61 626c 6572  ype)...Billabler
-00000400: 2a00 0000 2902 7a09 446f 4e6f 7442 696c  *...).z.DoNotBil
-00000410: 6c72 1b00 0000 2902 7a08 4e6f 4368 6172  lr....).z.NoChar
-00000420: 6765 721d 0000 0029 0272 2600 0000 7227  ger....).r&...r'
-00000430: 0000 0029 13da 085f 5f6e 616d 655f 5fda  ...)...__name__.
-00000440: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000450: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
-00000460: 6465 6e63 6965 7372 0200 0000 da0b 4372  denciesr......Cr
-00000470: 6561 7465 4d6f 6465 6c72 0300 0000 da09  eateModelr......
-00000480: 4175 746f 4669 656c 64da 1164 6a61 6e67  AutoField..djang
-00000490: 6f5f 6578 7465 6e73 696f 6e73 da02 6462  o_extensions..db
-000004a0: 7209 0000 00da 1543 7265 6174 696f 6e44  r......CreationD
-000004b0: 6174 6554 696d 6546 6965 6c64 da19 4d6f  ateTimeField..Mo
-000004c0: 6469 6669 6361 7469 6f6e 4461 7465 5469  dificationDateTi
-000004d0: 6d65 4669 656c 64da 0943 6861 7246 6965  meField..CharFie
-000004e0: 6c64 da0a 466f 7265 6967 6e4b 6579 da06  ld..ForeignKey..
-000004f0: 646a 616e 676f da08 6465 6c65 7469 6f6e  django..deletion
-00000500: da08 5345 545f 4e55 4c4c da0a 6f70 6572  ..SET_NULL..oper
-00000510: 6174 696f 6e73 a900 723b 0000 0072 3b00  ations..r;...r;.
-00000520: 0000 fa65 2f68 6f6d 652f 7361 6d2f 6769  ...e/home/sam/gi
-00000530: 742f 4b61 6e62 616e 2f64 6a61 6e67 6f2d  t/Kanban/django-
-00000540: 636f 6e6e 6563 7477 6973 652f 646a 616e  connectwise/djan
-00000550: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
-00000560: 6a63 6f6e 6e65 6374 7769 7365 2f6d 6967  jconnectwise/mig
-00000570: 7261 7469 6f6e 732f 3030 3936 5f61 6772  rations/0096_agr
-00000580: 6565 6d65 6e74 2e70 7972 0400 0000 0800  eement.pyr......
-00000590: 0000 731a 0000 000c 0309 0409 0106 0227  ..s............'
-000005a0: 0121 0121 0115 0130 012d 0133 0306 0106  .!.!...0.-.3....
-000005b0: 0172 0400 0000 2908 da09 646a 616e 676f  .r....)...django
-000005c0: 2e64 6272 0200 0000 7203 0000 00da 1964  .dbr....r......d
-000005d0: 6a61 6e67 6f2e 6462 2e6d 6f64 656c 732e  jango.db.models.
-000005e0: 6465 6c65 7469 6f6e 7237 0000 00da 1b64  deletionr7.....d
-000005f0: 6a61 6e67 6f5f 6578 7465 6e73 696f 6e73  jango_extensions
-00000600: 2e64 622e 6669 656c 6473 7231 0000 0072  .db.fieldsr1...r
-00000610: 0400 0000 723b 0000 0072 3b00 0000 723b  ....r;...r;...r;
-00000620: 0000 0072 3c00 0000 da08 3c6d 6f64 756c  ...r<.....<modul
-00000630: 653e 0300 0000 7306 0000 0016 010c 010c  e>....s.........
-00000640: 03                                       .
+00000020: 0073 3600 0000 6400 6401 6c00 6d01 5a01  .s6...d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 6400  m.Z...d.d.l.Z.d.
+00000040: 6402 6c05 5a06 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
+00000050: 6501 6a07 8303 5a07 6402 5300 2905 e900  e.j...Z.d.S.)...
+00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
+00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
+00000080: 0000 0000 0000 000e 0000 0040 0000 0073  ...........@...s
+00000090: c400 0000 6500 5a01 6400 5a02 6422 6701  ....e.Z.d.Z.d"g.
+000000a0: 5a03 6504 6a05 6403 6404 6506 6a07 6405  Z.e.j.d.d.e.j.d.
+000000b0: 6405 6406 6407 6408 8d04 6602 6409 6508  d.d.d.d...f.d.e.
+000000c0: 6a09 6a0a 6a0b 6405 6409 640a 8d02 6602  j.j.j.d.d.d...f.
+000000d0: 640b 6508 6a09 6a0a 6a0c 6405 640b 640c  d.e.j.j.j.d.d.d.
+000000e0: 8d02 6602 640d 6506 6a0d 640e 640f 8d01  ..f.d.e.j.d.d...
+000000f0: 6602 6410 6506 6a0d 6405 6423 6424 6425  f.d.e.j.d.d#d$d%
+00000100: 6703 6416 6405 6417 8d04 6602 6418 6506  g.d.d.d...f.d.e.
+00000110: 6a0e 6405 650f 6a09 6a06 6a10 6a11 6419  j.d.e.j.j.j.j.d.
+00000120: 641a 8d03 6602 641b 6506 6a0e 6405 650f  d...f.d.e.j.d.e.
+00000130: 6a09 6a06 6a10 6a11 641c 641a 8d03 6602  j.j.j.j.d.d...f.
+00000140: 6707 6426 640b 6406 641f 9c03 6420 8d03  g.d&d.d.d...d ..
+00000150: 6701 5a12 6421 5300 2927 da09 4d69 6772  g.Z.d!S.)'..Migr
+00000160: 6174 696f 6eda 0d64 6a63 6f6e 6e65 6374  ation..djconnect
+00000170: 7769 7365 da1f 3030 3935 5f63 6f6e 6e65  wise..0095_conne
+00000180: 6374 7769 7365 626f 6172 645f 776f 726b  ctwiseboard_work
+00000190: 5f74 7970 65da 0941 6772 6565 6d65 6e74  _type..Agreement
+000001a0: da02 6964 5446 da02 4944 2904 da0c 6175  ..idTF..ID)...au
+000001b0: 746f 5f63 7265 6174 6564 da0b 7072 696d  to_created..prim
+000001c0: 6172 795f 6b65 79da 0973 6572 6961 6c69  ary_key..seriali
+000001d0: 7a65 da0c 7665 7262 6f73 655f 6e61 6d65  ze..verbose_name
+000001e0: da07 6372 6561 7465 6429 02da 0c61 7574  ..created)...aut
+000001f0: 6f5f 6e6f 775f 6164 6472 0d00 0000 da08  o_now_addr......
+00000200: 6d6f 6469 6669 6564 2902 da08 6175 746f  modified)...auto
+00000210: 5f6e 6f77 720d 0000 00da 046e 616d 65e9  _nowr......name.
+00000220: 6400 0000 2901 da0a 6d61 785f 6c65 6e67  d...)...max_leng
+00000230: 7468 da09 6269 6c6c 5f74 696d 65da 0842  th..bill_time..B
+00000240: 696c 6c61 626c 65da 0944 6f4e 6f74 4269  illable..DoNotBi
+00000250: 6c6c fa0b 446f 204e 6f74 2042 696c 6cda  ll..Do Not Bill.
+00000260: 084e 6f43 6861 7267 65fa 094e 6f20 4368  .NoCharge..No Ch
+00000270: 6172 6765 e932 0000 0029 04da 0562 6c61  arge.2...)...bla
+00000280: 6e6b da07 6368 6f69 6365 7372 1400 0000  nk..choicesr....
+00000290: da04 6e75 6c6c da09 776f 726b 5f72 6f6c  ..null..work_rol
+000002a0: 657a 1664 6a63 6f6e 6e65 6374 7769 7365  ez.djconnectwise
+000002b0: 2e57 6f72 6b52 6f6c 6529 0372 1e00 0000  .WorkRole).r....
+000002c0: da09 6f6e 5f64 656c 6574 65da 0274 6fda  ..on_delete..to.
+000002d0: 0977 6f72 6b5f 7479 7065 7a16 646a 636f  .work_typez.djco
+000002e0: 6e6e 6563 7477 6973 652e 576f 726b 5479  nnectwise.WorkTy
+000002f0: 7065 fa09 2d6d 6f64 6966 6965 64fa 082d  pe..-modified..-
+00000300: 6372 6561 7465 6429 03da 086f 7264 6572  created)...order
+00000310: 696e 67da 0d67 6574 5f6c 6174 6573 745f  ing..get_latest_
+00000320: 6279 da08 6162 7374 7261 6374 2903 7212  by..abstract).r.
+00000330: 0000 00da 0666 6965 6c64 73da 076f 7074  .....fields..opt
+00000340: 696f 6e73 4e29 0272 0500 0000 7206 0000  ionsN).r....r...
+00000350: 0029 0272 1600 0000 7216 0000 0029 0272  .).r....r....).r
+00000360: 1700 0000 7218 0000 0029 0272 1900 0000  ....r....).r....
+00000370: 721a 0000 0029 0272 2300 0000 7224 0000  r....).r#...r$..
+00000380: 0029 13da 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
+00000390: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000003a0: 6c6e 616d 655f 5fda 0c64 6570 656e 6465  lname__..depende
+000003b0: 6e63 6965 7372 0200 0000 da0b 4372 6561  nciesr......Crea
+000003c0: 7465 4d6f 6465 6c72 0300 0000 da09 4175  teModelr......Au
+000003d0: 746f 4669 656c 64da 1164 6a61 6e67 6f5f  toField..django_
+000003e0: 6578 7465 6e73 696f 6e73 da02 6462 7228  extensions..dbr(
+000003f0: 0000 00da 1543 7265 6174 696f 6e44 6174  .....CreationDat
+00000400: 6554 696d 6546 6965 6c64 da19 4d6f 6469  eTimeField..Modi
+00000410: 6669 6361 7469 6f6e 4461 7465 5469 6d65  ficationDateTime
+00000420: 4669 656c 64da 0943 6861 7246 6965 6c64  Field..CharField
+00000430: da0a 466f 7265 6967 6e4b 6579 da06 646a  ..ForeignKey..dj
+00000440: 616e 676f da08 6465 6c65 7469 6f6e da08  ango..deletion..
+00000450: 5345 545f 4e55 4c4c da0a 6f70 6572 6174  SET_NULL..operat
+00000460: 696f 6e73 a900 723a 0000 0072 3a00 0000  ions..r:...r:...
+00000470: fa5a 2f68 6f6d 652f 6361 6d65 726f 6e2f  .Z/home/cameron/
+00000480: 4465 762f 6b61 6e62 616e 2d64 6576 2f64  Dev/kanban-dev/d
+00000490: 6a61 6e67 6f2d 636f 6e6e 6563 7477 6973  jango-connectwis
+000004a0: 652f 646a 636f 6e6e 6563 7477 6973 652f  e/djconnectwise/
+000004b0: 6d69 6772 6174 696f 6e73 2f30 3039 365f  migrations/0096_
+000004c0: 6167 7265 656d 656e 742e 7079 7204 0000  agreement.pyr...
+000004d0: 0008 0000 0073 1a00 0000 0803 0604 0401  .....s..........
+000004e0: 0202 1401 1401 1401 0e01 1a01 1a01 1c03  ................
+000004f0: 0201 0201 7204 0000 0029 08da 0964 6a61  ....r....)...dja
+00000500: 6e67 6f2e 6462 7202 0000 0072 0300 0000  ngo.dbr....r....
+00000510: da19 646a 616e 676f 2e64 622e 6d6f 6465  ..django.db.mode
+00000520: 6c73 2e64 656c 6574 696f 6e72 3600 0000  ls.deletionr6...
+00000530: da1b 646a 616e 676f 5f65 7874 656e 7369  ..django_extensi
+00000540: 6f6e 732e 6462 2e66 6965 6c64 7372 3000  ons.db.fieldsr0.
+00000550: 0000 7204 0000 0072 3a00 0000 723a 0000  ..r....r:...r:..
+00000560: 0072 3a00 0000 723b 0000 00da 083c 6d6f  .r:...r;.....<mo
+00000570: 6475 6c65 3e03 0000 0073 0600 0000 1001  dule>....s......
+00000580: 0801 0803                                ....
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0062_auto_20180606_1117.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0062_auto_20180606_1117.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,78 @@
-00000000: 160d 0d0a a4b0 1f5d 2005 0000 e300 0000  .......] .......
+00000000: 330d 0d0a 10ec da5c 2005 0000 e300 0000  3......\ .......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 1200 0000 4000 0000 7315 0100 0065 0000  ....@...s....e..
-000000a0: 5a01 0064 0000 5a02 0064 2400 6701 005a  Z..d..Z..d$.g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6506 006a 0700 6407 0064 0800  .d..e..j..d..d..
-000000d0: 6409 0064 0800 640a 0064 0b00 640c 0064  d..d..d..d..d..d
-000000e0: 0d00 8300 0466 0200 6403 0065 0600 6a08  .....f..d..e..j.
-000000f0: 0064 0e00 6408 0064 0f00 6410 0064 1100  .d..d..d..d..d..
-00000100: 6408 0083 0003 6602 0067 0200 6412 0064  d.....f..g..d..d
-00000110: 1300 6414 0064 1500 6425 0069 0200 8300  ..d..d..d%.i....
-00000120: 0365 0400 6a09 0064 0300 6416 0064 1200  .e..j..d..d..d..
-00000130: 6415 0064 2600 6413 0064 1800 6902 0083  d..d&.d..d..i...
-00000140: 0002 6504 006a 0900 6403 0064 1900 6412  ..e..j..d..d..d.
-00000150: 0064 1500 6427 0064 1300 641b 0069 0200  .d..d'.d..d..i..
-00000160: 8300 0265 0400 6a0a 0064 1c00 641d 0064  ...e..j..d..d..d
-00000170: 0300 641e 0064 1f00 6506 006a 0b00 640e  ..d..d..e..j..d.
-00000180: 0064 0800 6411 0064 0800 6420 0065 0c00  .d..d..d..d .e..
-00000190: 6a0d 006a 0600 6a0e 006a 0f00 6421 0064  j..j..j..j..d!.d
-000001a0: 2200 8300 0483 0003 6704 005a 1000 6423  ".......g..Z..d#
-000001b0: 0053 2928 da09 4d69 6772 6174 696f 6eda  .S)(..Migration.
-000001c0: 0d64 6a63 6f6e 6e65 6374 7769 7365 da17  .djconnectwise..
-000001d0: 3030 3631 5f61 7574 6f5f 3230 3138 3036  0061_auto_201806
-000001e0: 3035 5f31 3230 38da 046e 616d 65da 0954  05_1208..name..T
-000001f0: 6572 7269 746f 7279 da06 6669 656c 6473  erritory..fields
-00000200: da02 6964 da0c 6175 746f 5f63 7265 6174  ..id..auto_creat
-00000210: 6564 54da 0b70 7269 6d61 7279 5f6b 6579  edT..primary_key
-00000220: da09 7365 7269 616c 697a 6546 da0c 7665  ..serializeF..ve
-00000230: 7262 6f73 655f 6e61 6d65 da02 4944 da05  rbose_name..ID..
-00000240: 626c 616e 6bda 0a6d 6178 5f6c 656e 6774  blank..max_lengt
-00000250: 68e9 fa00 0000 da04 6e75 6c6c da07 6f70  h.......null..op
-00000260: 7469 6f6e 73da 1376 6572 626f 7365 5f6e  tions..verbose_n
-00000270: 616d 655f 706c 7572 616c da0b 5465 7272  ame_plural..Terr
-00000280: 6974 6f72 6965 73da 086f 7264 6572 696e  itories..orderin
-00000290: 67da 0f6f 7070 6f72 7475 6e69 7479 6e6f  g..opportunityno
-000002a0: 7465 fa0d 2d64 6174 655f 6372 6561 7465  te..-date_create
-000002b0: 647a 114f 7070 6f72 7475 6e69 7479 206e  dz.Opportunity n
-000002c0: 6f74 6573 da09 7469 6d65 656e 7472 79fa  otes..timeentry.
-000002d0: 0b2d 7469 6d65 5f73 7461 7274 7a0c 5469  .-time_startz.Ti
-000002e0: 6d65 2065 6e74 7269 6573 da0a 6d6f 6465  me entries..mode
-000002f0: 6c5f 6e61 6d65 da07 636f 6d70 616e 79da  l_name..company.
-00000300: 0974 6572 7269 746f 7279 da05 6669 656c  .territory..fiel
-00000310: 64da 096f 6e5f 6465 6c65 7465 da02 746f  d..on_delete..to
-00000320: 7a17 646a 636f 6e6e 6563 7477 6973 652e  z.djconnectwise.
-00000330: 5465 7272 6974 6f72 794e 2902 7a0d 646a  TerritoryN).z.dj
-00000340: 636f 6e6e 6563 7477 6973 657a 1730 3036  connectwisez.006
-00000350: 315f 6175 746f 5f32 3031 3830 3630 355f  1_auto_20180605_
-00000360: 3132 3038 2901 7207 0000 0029 0272 1900  1208).r....).r..
-00000370: 0000 fa02 6964 2902 721b 0000 0072 2200  ....id).r....r".
-00000380: 0000 2911 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
-00000390: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000003a0: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
-000003b0: 656e 6369 6573 7202 0000 00da 0b43 7265  enciesr......Cre
-000003c0: 6174 654d 6f64 656c 7203 0000 00da 0941  ateModelr......A
-000003d0: 7574 6f46 6965 6c64 da09 4368 6172 4669  utoField..CharFi
-000003e0: 656c 64da 1141 6c74 6572 4d6f 6465 6c4f  eld..AlterModelO
-000003f0: 7074 696f 6e73 da0a 416c 7465 7246 6965  ptions..AlterFie
-00000400: 6c64 da0a 466f 7265 6967 6e4b 6579 da06  ld..ForeignKey..
-00000410: 646a 616e 676f da02 6462 da08 6465 6c65  django..db..dele
-00000420: 7469 6f6e da08 5345 545f 4e55 4c4c da0a  tion..SET_NULL..
-00000430: 6f70 6572 6174 696f 6e73 a900 7232 0000  operations..r2..
-00000440: 0072 3200 0000 fa6e 2f68 6f6d 652f 7361  .r2....n/home/sa
-00000450: 6d2f 6769 742f 4b61 6e62 616e 2f64 6a61  m/git/Kanban/dja
-00000460: 6e67 6f2d 636f 6e6e 6563 7477 6973 652f  ngo-connectwise/
-00000470: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
-00000480: 7365 2f64 6a63 6f6e 6e65 6374 7769 7365  se/djconnectwise
-00000490: 2f6d 6967 7261 7469 6f6e 732f 3030 3632  /migrations/0062
-000004a0: 5f61 7574 6f5f 3230 3138 3036 3036 5f31  _auto_20180606_1
-000004b0: 3131 372e 7079 7204 0000 0007 0000 0073  117.pyr........s
-000004c0: 2200 0000 0c03 0904 0901 0602 2701 2703  "...........'.'.
-000004d0: 0601 0c03 0901 0601 1202 0901 0601 1202  ................
-000004e0: 0901 0601 0601 7204 0000 0029 06da 0964  ......r....)...d
-000004f0: 6a61 6e67 6f2e 6462 7202 0000 0072 0300  jango.dbr....r..
-00000500: 0000 da19 646a 616e 676f 2e64 622e 6d6f  ....django.db.mo
-00000510: 6465 6c73 2e64 656c 6574 696f 6e72 2d00  dels.deletionr-.
-00000520: 0000 7204 0000 0072 3200 0000 7232 0000  ..r....r2...r2..
-00000530: 0072 3200 0000 7233 0000 00da 083c 6d6f  .r2...r3.....<mo
-00000540: 6475 6c65 3e03 0000 0073 0400 0000 1601  dule>....s......
-00000550: 0c03                                     ..
+00000020: 0073 2e00 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 4700  m.Z...d.d.l.Z.G.
+00000040: 6403 6404 8400 6404 6501 6a05 8303 5a05  d.d...d.e.j...Z.
+00000050: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 734e 6300 0000 0000 0000 0000 0000 000c  sNc.............
+00000080: 0000 0040 0000 0073 9800 0000 6500 5a01  ...@...s....e.Z.
+00000090: 6400 5a02 641d 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000a0: 6404 6506 6a07 6405 6405 6406 6407 6408  d.e.j.d.d.d.d.d.
+000000b0: 8d04 6602 6409 6506 6a08 6405 640a 6405  ..f.d.e.j.d.d.d.
+000000c0: 640b 8d03 6602 6702 640c 641e 640d 9c02  d...f.g.d.d.d...
+000000d0: 640e 8d03 6504 6a09 640f 641f 6411 6412  d...e.j.d.d.d.d.
+000000e0: 9c02 6413 8d02 6504 6a09 6414 6420 6416  ..d...e.j.d.d d.
+000000f0: 6412 9c02 6413 8d02 6504 6a0a 6417 6418  d...d...e.j.d.d.
+00000100: 6506 6a0b 6405 6405 650c 6a0d 6a06 6a0e  e.j.d.d.e.j.j.j.
+00000110: 6a0f 6419 641a 8d04 641b 8d03 6704 5a10  j.d.d...d...g.Z.
+00000120: 641c 5300 2921 da09 4d69 6772 6174 696f  d.S.)!..Migratio
+00000130: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
+00000140: da17 3030 3631 5f61 7574 6f5f 3230 3138  ..0061_auto_2018
+00000150: 3036 3035 5f31 3230 38da 0954 6572 7269  0605_1208..Terri
+00000160: 746f 7279 da02 6964 5446 da02 4944 2904  tory..idTF..ID).
+00000170: da0c 6175 746f 5f63 7265 6174 6564 da0b  ..auto_created..
+00000180: 7072 696d 6172 795f 6b65 79da 0973 6572  primary_key..ser
+00000190: 6961 6c69 7a65 da0c 7665 7262 6f73 655f  ialize..verbose_
+000001a0: 6e61 6d65 da04 6e61 6d65 e9fa 0000 0029  name..name.....)
+000001b0: 03da 0562 6c61 6e6b da0a 6d61 785f 6c65  ...blank..max_le
+000001c0: 6e67 7468 da04 6e75 6c6c da0b 5465 7272  ngth..null..Terr
+000001d0: 6974 6f72 6965 7329 02da 1376 6572 626f  itories)...verbo
+000001e0: 7365 5f6e 616d 655f 706c 7572 616c da08  se_name_plural..
+000001f0: 6f72 6465 7269 6e67 2903 720e 0000 00da  ordering).r.....
+00000200: 0666 6965 6c64 73da 076f 7074 696f 6e73  .fields..options
+00000210: 5a0f 6f70 706f 7274 756e 6974 796e 6f74  Z.opportunitynot
+00000220: 65fa 0d2d 6461 7465 5f63 7265 6174 6564  e..-date_created
+00000230: 7a11 4f70 706f 7274 756e 6974 7920 6e6f  z.Opportunity no
+00000240: 7465 7329 0272 1500 0000 7214 0000 0029  tes).r....r....)
+00000250: 0272 0e00 0000 7217 0000 00da 0974 696d  .r....r......tim
+00000260: 6565 6e74 7279 fa0b 2d74 696d 655f 7374  eentry..-time_st
+00000270: 6172 747a 0c54 696d 6520 656e 7472 6965  artz.Time entrie
+00000280: 73da 0763 6f6d 7061 6e79 da09 7465 7272  s..company..terr
+00000290: 6974 6f72 797a 1764 6a63 6f6e 6e65 6374  itoryz.djconnect
+000002a0: 7769 7365 2e54 6572 7269 746f 7279 2904  wise.Territory).
+000002b0: 7210 0000 0072 1200 0000 da09 6f6e 5f64  r....r......on_d
+000002c0: 656c 6574 65da 0274 6f29 03da 0a6d 6f64  elete..to)...mod
+000002d0: 656c 5f6e 616d 6572 0e00 0000 da05 6669  el_namer......fi
+000002e0: 656c 644e 2902 7205 0000 0072 0600 0000  eldN).r....r....
+000002f0: 2901 720e 0000 0029 0272 1800 0000 7208  ).r....).r....r.
+00000300: 0000 0029 0272 1a00 0000 7208 0000 0029  ...).r....r....)
+00000310: 11da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000320: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000330: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
+00000340: 6965 7372 0200 0000 da0b 4372 6561 7465  iesr......Create
+00000350: 4d6f 6465 6c72 0300 0000 da09 4175 746f  Modelr......Auto
+00000360: 4669 656c 64da 0943 6861 7246 6965 6c64  Field..CharField
+00000370: da11 416c 7465 724d 6f64 656c 4f70 7469  ..AlterModelOpti
+00000380: 6f6e 73da 0a41 6c74 6572 4669 656c 64da  ons..AlterField.
+00000390: 0a46 6f72 6569 676e 4b65 79da 0664 6a61  .ForeignKey..dja
+000003a0: 6e67 6fda 0264 62da 0864 656c 6574 696f  ngo..db..deletio
+000003b0: 6eda 0853 4554 5f4e 554c 4cda 0a6f 7065  n..SET_NULL..ope
+000003c0: 7261 7469 6f6e 73a9 0072 3000 0000 7230  rations..r0...r0
+000003d0: 0000 00fa 632f 686f 6d65 2f63 616d 6572  ....c/home/camer
+000003e0: 6f6e 2f44 6576 2f6b 616e 6261 6e2d 6465  on/Dev/kanban-de
+000003f0: 762f 646a 616e 676f 2d63 6f6e 6e65 6374  v/django-connect
+00000400: 7769 7365 2f64 6a63 6f6e 6e65 6374 7769  wise/djconnectwi
+00000410: 7365 2f6d 6967 7261 7469 6f6e 732f 3030  se/migrations/00
+00000420: 3632 5f61 7574 6f5f 3230 3138 3036 3036  62_auto_20180606
+00000430: 5f31 3131 372e 7079 7204 0000 0007 0000  _1117.pyr.......
+00000440: 0073 2200 0000 0803 0604 0401 0202 1401  .s".............
+00000450: 1403 0201 0a03 0401 0201 0c02 0401 0201  ................
+00000460: 0c02 0401 0201 0201 7204 0000 0029 06da  ........r....)..
+00000470: 0964 6a61 6e67 6f2e 6462 7202 0000 0072  .django.dbr....r
+00000480: 0300 0000 da19 646a 616e 676f 2e64 622e  ......django.db.
+00000490: 6d6f 6465 6c73 2e64 656c 6574 696f 6e72  models.deletionr
+000004a0: 2b00 0000 7204 0000 0072 3000 0000 7230  +...r....r0...r0
+000004b0: 0000 0072 3000 0000 7231 0000 00da 083c  ...r0...r1.....<
+000004c0: 6d6f 6475 6c65 3e03 0000 0073 0400 0000  module>....s....
+000004d0: 1001 0803                                ....
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0031_auto_20170607_2234.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0014_company_status.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,45 @@
-00000000: 160d 0d0a a4b0 1f5d 7903 0000 e300 0000  .......]y.......
+00000000: 330d 0d0a 10ec da5c dd01 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 000d 0000 0040 0000 0073  ...........@...s
-000000b0: c100 0000 6500 005a 0100 6400 005a 0200  ....e..Z..d..Z..
-000000c0: 640f 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 6408 0064 0900 8300 0183 0003  .j..d..d........
-000000f0: 6504 006a 0500 6403 0064 0400 6405 0064  e..j..d..d..d..d
-00000100: 0a00 6407 0065 0600 6a07 0064 0800 6409  ..d..e..j..d..d.
-00000110: 0083 0001 8300 0365 0400 6a05 0064 0300  .......e..j..d..
-00000120: 6404 0064 0500 640b 0064 0700 6506 006a  d..d..d..d..e..j
-00000130: 0800 640c 0064 0900 6408 0064 0900 8300  ..d..d..d..d....
-00000140: 0283 0003 6504 006a 0500 6403 0064 0400  ....e..j..d..d..
-00000150: 6405 0064 0d00 6407 0065 0600 6a07 0064  d..d..d..e..j..d
-00000160: 0800 6409 0083 0001 8300 0367 0400 5a09  ..d........g..Z.
-00000170: 0064 0e00 5329 10da 094d 6967 7261 7469  .d..S)...Migrati
-00000180: 6f6e da0d 646a 636f 6e6e 6563 7477 6973  on..djconnectwis
-00000190: 65da 0a30 3033 305f 6d65 7267 65da 0a6d  e..0030_merge..m
-000001a0: 6f64 656c 5f6e 616d 65da 0773 796e 636a  odel_name..syncj
-000001b0: 6f62 da04 6e61 6d65 da05 6164 6465 64da  ob..name..added.
-000001c0: 0566 6965 6c64 da04 6e75 6c6c 54da 0764  .field..nullT..d
-000001d0: 656c 6574 6564 da07 6d65 7373 6167 65da  eleted..message.
-000001e0: 0562 6c61 6e6b da07 7570 6461 7465 644e  .blank..updatedN
-000001f0: 2902 7a0d 646a 636f 6e6e 6563 7477 6973  ).z.djconnectwis
-00000200: 6572 0700 0000 290a da08 5f5f 6e61 6d65  er....)...__name
-00000210: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000220: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
-00000230: 7065 6e64 656e 6369 6573 7203 0000 00da  pendenciesr.....
-00000240: 0a41 6c74 6572 4669 656c 6472 0400 0000  .AlterFieldr....
-00000250: da14 506f 7369 7469 7665 496e 7465 6765  ..PositiveIntege
-00000260: 7246 6965 6c64 da09 5465 7874 4669 656c  rField..TextFiel
-00000270: 64da 0a6f 7065 7261 7469 6f6e 73a9 0072  d..operations..r
-00000280: 1a00 0000 721a 0000 00fa 6e2f 686f 6d65  ....r.....n/home
-00000290: 2f73 616d 2f67 6974 2f4b 616e 6261 6e2f  /sam/git/Kanban/
-000002a0: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
-000002b0: 7365 2f64 6a61 6e67 6f2d 636f 6e6e 6563  se/django-connec
-000002c0: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
-000002d0: 6973 652f 6d69 6772 6174 696f 6e73 2f30  ise/migrations/0
-000002e0: 3033 315f 6175 746f 5f32 3031 3730 3630  031_auto_2017060
-000002f0: 375f 3232 3334 2e70 7972 0500 0000 0700  7_2234.pyr......
-00000300: 0000 7322 0000 000c 0309 0409 0106 0106  ..s"............
-00000310: 0112 0209 0106 0106 0112 0209 0106 0106  ................
-00000320: 0118 0209 0106 0106 0172 0500 0000 4e29  .........r....N)
-00000330: 06da 0a5f 5f66 7574 7572 655f 5f72 0200  ...__future__r..
-00000340: 0000 da09 646a 616e 676f 2e64 6272 0300  ....django.dbr..
-00000350: 0000 7204 0000 0072 0500 0000 721a 0000  ..r....r....r...
-00000360: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000370: da08 3c6d 6f64 756c 653e 0200 0000 7304  ..<module>....s.
-00000380: 0000 0010 0216 03                        .......
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0900 0000 4000 0000 7334  ..........@...s4
+000000a0: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000c0: 0564 0665 066a 0864 078d 0464 088d 0367  .d.e.j.d...d...g
+000000d0: 015a 0964 0953 0029 0bda 094d 6967 7261  .Z.d.S.)...Migra
+000000e0: 7469 6f6e da0d 646a 636f 6e6e 6563 7477  tion..djconnectw
+000000f0: 6973 65da 1730 3031 335f 6175 746f 5f32  ise..0013_auto_2
+00000100: 3031 3730 3430 335f 3132 3033 da07 636f  0170403_1203..co
+00000110: 6d70 616e 79da 0673 7461 7475 7354 7a1b  mpany..statusTz.
+00000120: 646a 636f 6e6e 6563 7477 6973 652e 436f  djconnectwise.Co
+00000130: 6d70 616e 7953 7461 7475 7329 04da 0562  mpanyStatus)...b
+00000140: 6c61 6e6b da04 6e75 6c6c da02 746f da09  lank..null..to..
+00000150: 6f6e 5f64 656c 6574 6529 03da 0a6d 6f64  on_delete)...mod
+00000160: 656c 5f6e 616d 65da 046e 616d 65da 0566  el_name..name..f
+00000170: 6965 6c64 4e29 0272 0600 0000 7207 0000  ieldN).r....r...
+00000180: 0029 0ada 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
+00000190: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000001a0: 6c6e 616d 655f 5fda 0c64 6570 656e 6465  lname__..depende
+000001b0: 6e63 6965 7372 0300 0000 da08 4164 6446  nciesr......AddF
+000001c0: 6965 6c64 7204 0000 00da 0a46 6f72 6569  ieldr......Forei
+000001d0: 676e 4b65 79da 0853 4554 5f4e 554c 4cda  gnKey..SET_NULL.
+000001e0: 0a6f 7065 7261 7469 6f6e 73a9 0072 1900  .operations..r..
+000001f0: 0000 7219 0000 00fa 5f2f 686f 6d65 2f63  ..r....._/home/c
+00000200: 616d 6572 6f6e 2f44 6576 2f6b 616e 6261  ameron/Dev/kanba
+00000210: 6e2d 6465 762f 646a 616e 676f 2d63 6f6e  n-dev/django-con
+00000220: 6e65 6374 7769 7365 2f64 6a63 6f6e 6e65  nectwise/djconne
+00000230: 6374 7769 7365 2f6d 6967 7261 7469 6f6e  ctwise/migration
+00000240: 732f 3030 3134 5f63 6f6d 7061 6e79 5f73  s/0014_company_s
+00000250: 7461 7475 732e 7079 7205 0000 0007 0000  tatus.pyr.......
+00000260: 0073 0a00 0000 0803 0604 0401 0201 0201  .s..............
+00000270: 7205 0000 004e 2906 da0a 5f5f 6675 7475  r....N)...__futu
+00000280: 7265 5f5f 7202 0000 00da 0964 6a61 6e67  re__r......djang
+00000290: 6f2e 6462 7203 0000 0072 0400 0000 7205  o.dbr....r....r.
+000002a0: 0000 0072 1900 0000 7219 0000 0072 1900  ...r....r....r..
+000002b0: 0000 721a 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000002c0: 3e02 0000 0073 0400 0000 0c02 1003       >....s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0012_auto_20170320_1057.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0009_member_license_class.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,49 @@
-00000000: 160d 0d0a a4b0 1f5d 4802 0000 e300 0000  .......]H.......
+00000000: 330d 0d0a 10ec da5c fb01 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 000c 0000 0040 0000 0073  ...........@...s
-000000b0: 6d00 0000 6500 005a 0100 6400 005a 0200  m...e..Z..d..Z..
-000000c0: 640d 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 8300 0083 0003 6504 006a 0500  .j........e..j..
-000000f0: 6403 0064 0400 6405 0064 0800 6407 0065  d..d..d..d..d..e
-00000100: 0600 6a08 0064 0900 640a 0064 0b00 640a  ..j..d..d..d..d.
-00000110: 0083 0002 8300 0367 0200 5a09 0064 0c00  .......g..Z..d..
-00000120: 5329 0eda 094d 6967 7261 7469 6f6e da0d  S)...Migration..
-00000130: 646a 636f 6e6e 6563 7477 6973 65da 1930  djconnectwise..0
-00000140: 3031 315f 636f 6d70 616e 795f 6465 6c65  011_company_dele
-00000150: 7465 645f 666c 6167 da0a 6d6f 6465 6c5f  ted_flag..model_
-00000160: 6e61 6d65 da06 7469 636b 6574 da04 6e61  name..ticket..na
-00000170: 6d65 da10 6861 735f 6368 696c 645f 7469  me..has_child_ti
-00000180: 636b 6574 da05 6669 656c 64da 1070 6172  cket..field..par
-00000190: 656e 745f 7469 636b 6574 5f69 64da 0562  ent_ticket_id..b
-000001a0: 6c61 6e6b 54da 046e 756c 6c4e 2902 7a0d  lankT..nullN).z.
-000001b0: 646a 636f 6e6e 6563 7477 6973 6572 0700  djconnectwiser..
-000001c0: 0000 290a da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
-000001d0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000001e0: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
-000001f0: 656e 6369 6573 7203 0000 00da 0841 6464  enciesr......Add
-00000200: 4669 656c 6472 0400 0000 da10 4e75 6c6c  Fieldr......Null
-00000210: 426f 6f6c 6561 6e46 6965 6c64 da0c 496e  BooleanField..In
-00000220: 7465 6765 7246 6965 6c64 da0a 6f70 6572  tegerField..oper
-00000230: 6174 696f 6e73 a900 7218 0000 0072 1800  ations..r....r..
-00000240: 0000 fa6e 2f68 6f6d 652f 7361 6d2f 6769  ...n/home/sam/gi
-00000250: 742f 4b61 6e62 616e 2f64 6a61 6e67 6f2d  t/Kanban/django-
-00000260: 636f 6e6e 6563 7477 6973 652f 646a 616e  connectwise/djan
-00000270: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
-00000280: 6a63 6f6e 6e65 6374 7769 7365 2f6d 6967  jconnectwise/mig
-00000290: 7261 7469 6f6e 732f 3030 3132 5f61 7574  rations/0012_aut
-000002a0: 6f5f 3230 3137 3033 3230 5f31 3035 372e  o_20170320_1057.
-000002b0: 7079 7205 0000 0007 0000 0073 1200 0000  pyr........s....
-000002c0: 0c03 0904 0901 0601 0601 0c02 0901 0601  ................
-000002d0: 0601 7205 0000 004e 2906 da0a 5f5f 6675  ..r....N)...__fu
-000002e0: 7475 7265 5f5f 7202 0000 00da 0964 6a61  ture__r......dja
-000002f0: 6e67 6f2e 6462 7203 0000 0072 0400 0000  ngo.dbr....r....
-00000300: 7205 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00000310: 1800 0000 7219 0000 00da 083c 6d6f 6475  ....r......<modu
-00000320: 6c65 3e02 0000 0073 0400 0000 1002 1603  le>....s........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0a00 0000 4000 0000 7338  ..........@...s8
+000000a0: 0000 0065 005a 0164 005a 0264 0e67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0764 0f64  .e.j.d.d.e.j.d.d
+000000c0: 1067 0264 0964 0964 0a64 0964 0b8d 0564  .g.d.d.d.d.d...d
+000000d0: 0c8d 0367 015a 0864 0d53 0029 11da 094d  ...g.Z.d.S.)...M
+000000e0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
+000000f0: 6563 7477 6973 65da 1830 3030 385f 7072  ectwise..0008_pr
+00000100: 6f6a 6563 745f 7374 6174 7573 5f6e 616d  oject_status_nam
+00000110: 65da 066d 656d 6265 72da 0d6c 6963 656e  e..member..licen
+00000120: 7365 5f63 6c61 7373 da01 46fa 0c46 756c  se_class..F..Ful
+00000130: 6c20 6c69 6365 6e73 65da 0141 fa0b 4150  l license..A..AP
+00000140: 4920 6c69 6365 6e73 6554 e914 0000 0029  I licenseT.....)
+00000150: 05da 0763 686f 6963 6573 da08 6462 5f69  ...choices..db_i
+00000160: 6e64 6578 da05 626c 616e 6bda 0a6d 6178  ndex..blank..max
+00000170: 5f6c 656e 6774 68da 046e 756c 6c29 03da  _length..null)..
+00000180: 0a6d 6f64 656c 5f6e 616d 65da 046e 616d  .model_name..nam
+00000190: 65da 0566 6965 6c64 4e29 0272 0600 0000  e..fieldN).r....
+000001a0: 7207 0000 0029 0272 0a00 0000 720b 0000  r....).r....r...
+000001b0: 0029 0272 0c00 0000 720d 0000 0029 09da  .).r....r....)..
+000001c0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000001d0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000001e0: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
+000001f0: 7372 0300 0000 da08 4164 6446 6965 6c64  sr......AddField
+00000200: 7204 0000 00da 0943 6861 7246 6965 6c64  r......CharField
+00000210: da0a 6f70 6572 6174 696f 6e73 a900 721e  ..operations..r.
+00000220: 0000 0072 1e00 0000 fa65 2f68 6f6d 652f  ...r.....e/home/
+00000230: 6361 6d65 726f 6e2f 4465 762f 6b61 6e62  cameron/Dev/kanb
+00000240: 616e 2d64 6576 2f64 6a61 6e67 6f2d 636f  an-dev/django-co
+00000250: 6e6e 6563 7477 6973 652f 646a 636f 6e6e  nnectwise/djconn
+00000260: 6563 7477 6973 652f 6d69 6772 6174 696f  ectwise/migratio
+00000270: 6e73 2f30 3030 395f 6d65 6d62 6572 5f6c  ns/0009_member_l
+00000280: 6963 656e 7365 5f63 6c61 7373 2e70 7972  icense_class.pyr
+00000290: 0500 0000 0700 0000 730a 0000 0008 0306  ........s.......
+000002a0: 0404 0102 0102 0172 0500 0000 4e29 06da  .......r....N)..
+000002b0: 0a5f 5f66 7574 7572 655f 5f72 0200 0000  .__future__r....
+000002c0: da09 646a 616e 676f 2e64 6272 0300 0000  ..django.dbr....
+000002d0: 7204 0000 0072 0500 0000 721e 0000 0072  r....r....r....r
+000002e0: 1e00 0000 721e 0000 0072 1f00 0000 da08  ....r....r......
+000002f0: 3c6d 6f64 756c 653e 0200 0000 7304 0000  <module>....s...
+00000300: 000c 0210 03                             .....
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0020_merge.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0011_company_deleted_flag.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-00000000: 160d 0d0a a4b0 1f5d 3001 0000 e300 0000  .......]0.......
+00000000: 330d 0d0a 10ec da5c a901 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000000b0: 2200 0000 6500 005a 0100 6400 005a 0200  "...e..Z..d..Z..
-000000c0: 6405 0064 0600 6702 005a 0300 6700 005a  d..d..g..Z..g..Z
-000000d0: 0400 6404 0053 2907 da09 4d69 6772 6174  ..d..S)...Migrat
-000000e0: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-000000f0: 7365 da11 3030 3139 5f74 6963 6b65 745f  se..0019_ticket_
-00000100: 6f77 6e65 72da 1830 3031 395f 7379 6e63  owner..0019_sync
-00000110: 6a6f 625f 656e 7469 7479 5f6e 616d 654e  job_entity_nameN
-00000120: 2902 fa0d 646a 636f 6e6e 6563 7477 6973  )...djconnectwis
-00000130: 6572 0700 0000 2902 7209 0000 007a 1830  er....).r....z.0
-00000140: 3031 395f 7379 6e63 6a6f 625f 656e 7469  019_syncjob_enti
-00000150: 7479 5f6e 616d 6529 05da 085f 5f6e 616d  ty_name)...__nam
-00000160: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000170: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
-00000180: 6570 656e 6465 6e63 6965 73da 0a6f 7065  ependencies..ope
-00000190: 7261 7469 6f6e 73a9 0072 0f00 0000 720f  rations..r....r.
-000001a0: 0000 00fa 612f 686f 6d65 2f73 616d 2f67  ....a/home/sam/g
-000001b0: 6974 2f4b 616e 6261 6e2f 646a 616e 676f  it/Kanban/django
-000001c0: 2d63 6f6e 6e65 6374 7769 7365 2f64 6a61  -connectwise/dja
-000001d0: 6e67 6f2d 636f 6e6e 6563 7477 6973 652f  ngo-connectwise/
-000001e0: 646a 636f 6e6e 6563 7477 6973 652f 6d69  djconnectwise/mi
-000001f0: 6772 6174 696f 6e73 2f30 3032 305f 6d65  grations/0020_me
-00000200: 7267 652e 7079 7205 0000 0007 0000 0073  rge.pyr........s
-00000210: 0600 0000 0c03 0301 0903 7205 0000 004e  ..........r....N
-00000220: 2906 da0a 5f5f 6675 7475 7265 5f5f 7202  )...__future__r.
-00000230: 0000 00da 0964 6a61 6e67 6f2e 6462 7203  .....django.dbr.
-00000240: 0000 0072 0400 0000 7205 0000 0072 0f00  ...r....r....r..
-00000250: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00000260: 00da 083c 6d6f 6475 6c65 3e02 0000 0073  ...<module>....s
-00000270: 0400 0000 1002 1603                      ........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0600 0000 4000 0000 732c  ..........@...s,
+000000a0: 0000 0065 005a 0164 005a 0264 0967 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000c0: 068d 0164 078d 0367 015a 0864 0853 0029  ...d...g.Z.d.S.)
+000000d0: 0ada 094d 6967 7261 7469 6f6e da0d 646a  ...Migration..dj
+000000e0: 636f 6e6e 6563 7477 6973 65da 2030 3031  connectwise. 001
+000000f0: 305f 7265 6d6f 7665 5f70 726f 6a65 6374  0_remove_project
+00000100: 5f70 726f 6a65 6374 5f68 7265 66da 0763  _project_href..c
+00000110: 6f6d 7061 6e79 da0c 6465 6c65 7465 645f  ompany..deleted_
+00000120: 666c 6167 4629 01da 0764 6566 6175 6c74  flagF)...default
+00000130: 2903 da0a 6d6f 6465 6c5f 6e61 6d65 da04  )...model_name..
+00000140: 6e61 6d65 da05 6669 656c 644e 2902 7206  name..fieldN).r.
+00000150: 0000 0072 0700 0000 2909 da08 5f5f 6e61  ...r....)...__na
+00000160: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000170: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
+00000180: 6465 7065 6e64 656e 6369 6573 7203 0000  dependenciesr...
+00000190: 00da 0841 6464 4669 656c 6472 0400 0000  ...AddFieldr....
+000001a0: da0c 426f 6f6c 6561 6e46 6965 6c64 da0a  ..BooleanField..
+000001b0: 6f70 6572 6174 696f 6e73 a900 7215 0000  operations..r...
+000001c0: 0072 1500 0000 fa65 2f68 6f6d 652f 6361  .r.....e/home/ca
+000001d0: 6d65 726f 6e2f 4465 762f 6b61 6e62 616e  meron/Dev/kanban
+000001e0: 2d64 6576 2f64 6a61 6e67 6f2d 636f 6e6e  -dev/django-conn
+000001f0: 6563 7477 6973 652f 646a 636f 6e6e 6563  ectwise/djconnec
+00000200: 7477 6973 652f 6d69 6772 6174 696f 6e73  twise/migrations
+00000210: 2f30 3031 315f 636f 6d70 616e 795f 6465  /0011_company_de
+00000220: 6c65 7465 645f 666c 6167 2e70 7972 0500  leted_flag.pyr..
+00000230: 0000 0700 0000 730a 0000 0008 0306 0404  ......s.........
+00000240: 0102 0102 0172 0500 0000 4e29 06da 0a5f  .....r....N)..._
+00000250: 5f66 7574 7572 655f 5f72 0200 0000 da09  _future__r......
+00000260: 646a 616e 676f 2e64 6272 0300 0000 7204  django.dbr....r.
+00000270: 0000 0072 0500 0000 7215 0000 0072 1500  ...r....r....r..
+00000280: 0000 7215 0000 0072 1600 0000 da08 3c6d  ..r....r......<m
+00000290: 6f64 756c 653e 0200 0000 7304 0000 000c  odule>....s.....
+000002a0: 0210 03                                  ...
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0082_auto_20190125_1109.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0058_auto_20180516_1052.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,50 @@
-00000000: 160d 0d0a a4b0 1f5d 0102 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c 3102 0000 e300 0000  3......\1.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 0d00 0000 4000 0000 735e 0000 0065 0000  ....@...s^...e..
-000000a0: 5a01 0064 0000 5a02 0064 0e00 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6407 0065 0600 6a07 0064 0800  .d..d..e..j..d..
-000000d0: 6409 0064 0a00 6508 006a 0900 6a06 006a  d..d..e..j..j..j
-000000e0: 0a00 6a0b 0064 0b00 640c 0083 0003 8300  ..j..d..d.......
-000000f0: 0367 0100 5a0c 0064 0d00 5329 0fda 094d  .g..Z..d..S)...M
-00000100: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
-00000110: 6563 7477 6973 65da 1730 3038 315f 6175  ectwise..0081_au
-00000120: 746f 5f32 3031 3831 3232 305f 3039 3137  to_20181220_0917
-00000130: da0a 6d6f 6465 6c5f 6e61 6d65 da0b 6f70  ..model_name..op
-00000140: 706f 7274 756e 6974 79da 046e 616d 65da  portunity..name.
-00000150: 0870 7269 6f72 6974 79da 0566 6965 6c64  .priority..field
-00000160: da04 6e75 6c6c 54da 096f 6e5f 6465 6c65  ..nullT..on_dele
-00000170: 7465 da02 746f 7a21 646a 636f 6e6e 6563  te..toz!djconnec
-00000180: 7477 6973 652e 4f70 706f 7274 756e 6974  twise.Opportunit
-00000190: 7950 7269 6f72 6974 794e 2902 7a0d 646a  yPriorityN).z.dj
-000001a0: 636f 6e6e 6563 7477 6973 657a 1730 3038  connectwisez.008
-000001b0: 315f 6175 746f 5f32 3031 3831 3232 305f  1_auto_20181220_
-000001c0: 3039 3137 290d da08 5f5f 6e61 6d65 5f5f  0917)...__name__
-000001d0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-000001e0: 7175 616c 6e61 6d65 5f5f da0c 6465 7065  qualname__..depe
-000001f0: 6e64 656e 6369 6573 7202 0000 00da 0a41  ndenciesr......A
-00000200: 6c74 6572 4669 656c 6472 0300 0000 da0a  lterFieldr......
-00000210: 466f 7265 6967 6e4b 6579 da06 646a 616e  ForeignKey..djan
-00000220: 676f da02 6462 da08 6465 6c65 7469 6f6e  go..db..deletion
-00000230: da08 5345 545f 4e55 4c4c da0a 6f70 6572  ..SET_NULL..oper
-00000240: 6174 696f 6e73 a900 721a 0000 0072 1a00  ations..r....r..
-00000250: 0000 fa6e 2f68 6f6d 652f 7361 6d2f 6769  ...n/home/sam/gi
-00000260: 742f 4b61 6e62 616e 2f64 6a61 6e67 6f2d  t/Kanban/django-
-00000270: 636f 6e6e 6563 7477 6973 652f 646a 616e  connectwise/djan
-00000280: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
-00000290: 6a63 6f6e 6e65 6374 7769 7365 2f6d 6967  jconnectwise/mig
-000002a0: 7261 7469 6f6e 732f 3030 3832 5f61 7574  rations/0082_aut
-000002b0: 6f5f 3230 3139 3031 3235 5f31 3130 392e  o_20190125_1109.
-000002c0: 7079 7204 0000 0007 0000 0073 0a00 0000  pyr........s....
-000002d0: 0c03 0904 0901 0601 0601 7204 0000 0029  ..........r....)
-000002e0: 06da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
-000002f0: 0072 0300 0000 da19 646a 616e 676f 2e64  .r......django.d
-00000300: 622e 6d6f 6465 6c73 2e64 656c 6574 696f  b.models.deletio
-00000310: 6e72 1500 0000 7204 0000 0072 1a00 0000  nr....r....r....
-00000320: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
-00000330: 083c 6d6f 6475 6c65 3e03 0000 0073 0400  .<module>....s..
-00000340: 0000 1601 0c03                           ......
+00000020: 0073 2e00 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 4700  m.Z...d.d.l.Z.G.
+00000040: 6403 6404 8400 6404 6501 6a05 8303 5a05  d.d...d.e.j...Z.
+00000050: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 734e 6300 0000 0000 0000 0000 0000 000a  sNc.............
+00000080: 0000 0040 0000 0073 3c00 0000 6500 5a01  ...@...s<...e.Z.
+00000090: 6400 5a02 640b 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000a0: 6404 6506 6a07 6405 6405 6508 6a09 6a06  d.e.j.d.d.e.j.j.
+000000b0: 6a0a 6a0b 6406 6407 6408 8d05 6409 8d03  j.j.d.d.d...d...
+000000c0: 6701 5a0c 640a 5300 290c da09 4d69 6772  g.Z.d.S.)...Migr
+000000d0: 6174 696f 6eda 0d64 6a63 6f6e 6e65 6374  ation..djconnect
+000000e0: 7769 7365 da17 3030 3537 5f61 7574 6f5f  wise..0057_auto_
+000000f0: 3230 3138 3035 3131 5f31 3434 30da 0b6f  20180511_1440..o
+00000100: 7070 6f72 7475 6e69 7479 da0b 7072 6f62  pportunity..prob
+00000110: 6162 696c 6974 7954 da11 7361 6c65 735f  abilityT..sales_
+00000120: 7072 6f62 6162 696c 6974 797a 1e64 6a63  probabilityz.djc
+00000130: 6f6e 6e65 6374 7769 7365 2e53 616c 6573  onnectwise.Sales
+00000140: 5072 6f62 6162 696c 6974 7929 05da 0562  Probability)...b
+00000150: 6c61 6e6b da04 6e75 6c6c da09 6f6e 5f64  lank..null..on_d
+00000160: 656c 6574 65da 0c72 656c 6174 6564 5f6e  elete..related_n
+00000170: 616d 65da 0274 6f29 03da 0a6d 6f64 656c  ame..to)...model
+00000180: 5f6e 616d 65da 046e 616d 65da 0566 6965  _name..name..fie
+00000190: 6c64 4e29 0272 0500 0000 7206 0000 0029  ldN).r....r....)
+000001a0: 0dda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+000001b0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000001c0: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
+000001d0: 6965 7372 0200 0000 da0a 416c 7465 7246  iesr......AlterF
+000001e0: 6965 6c64 7203 0000 00da 0a46 6f72 6569  ieldr......Forei
+000001f0: 676e 4b65 79da 0664 6a61 6e67 6fda 0264  gnKey..django..d
+00000200: 62da 0864 656c 6574 696f 6eda 0853 4554  b..deletion..SET
+00000210: 5f4e 554c 4cda 0a6f 7065 7261 7469 6f6e  _NULL..operation
+00000220: 73a9 0072 1d00 0000 721d 0000 00fa 632f  s..r....r.....c/
+00000230: 686f 6d65 2f63 616d 6572 6f6e 2f44 6576  home/cameron/Dev
+00000240: 2f6b 616e 6261 6e2d 6465 762f 646a 616e  /kanban-dev/djan
+00000250: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
+00000260: 6a63 6f6e 6e65 6374 7769 7365 2f6d 6967  jconnectwise/mig
+00000270: 7261 7469 6f6e 732f 3030 3538 5f61 7574  rations/0058_aut
+00000280: 6f5f 3230 3138 3035 3136 5f31 3035 322e  o_20180516_1052.
+00000290: 7079 7204 0000 0007 0000 0073 0a00 0000  pyr........s....
+000002a0: 0803 0604 0401 0201 0201 7204 0000 0029  ..........r....)
+000002b0: 06da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
+000002c0: 0072 0300 0000 da19 646a 616e 676f 2e64  .r......django.d
+000002d0: 622e 6d6f 6465 6c73 2e64 656c 6574 696f  b.models.deletio
+000002e0: 6e72 1800 0000 7204 0000 0072 1d00 0000  nr....r....r....
+000002f0: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
+00000300: 083c 6d6f 6475 6c65 3e03 0000 0073 0400  .<module>....s..
+00000310: 0000 1001 0803                           ......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0090_auto_20190711_1114.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0096_merge_20190718_1102.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,33 @@
-00000000: 160d 0d0a b7b5 285d 0202 0000 e300 0000  ......(]........
+00000000: 330d 0d0a 05d5 305d 2301 0000 e300 0000  3.....0]#.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 0f00 0000 4000 0000 7364 0000 0065 0000  ....@...sd...e..
-000000a0: 5a01 0064 0000 5a02 0064 0f00 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6407 0065 0600 6a07 0064 0800  .d..d..e..j..d..
-000000d0: 6409 0064 0a00 6409 0064 0b00 6508 006a  d..d..d..d..e..j
-000000e0: 0900 6a06 006a 0a00 6a0b 0064 0c00 640d  ..j..j..j..d..d.
-000000f0: 0083 0004 8300 0367 0100 5a0c 0064 0e00  .......g..Z..d..
-00000100: 5329 10da 094d 6967 7261 7469 6f6e da0d  S)...Migration..
-00000110: 646a 636f 6e6e 6563 7477 6973 65da 1830  djconnectwise..0
-00000120: 3038 395f 6d65 7267 655f 3230 3139 3037  089_merge_201907
-00000130: 3131 5f31 3130 30da 0a6d 6f64 656c 5f6e  11_1100..model_n
-00000140: 616d 65da 0974 696d 6565 6e74 7279 da04  ame..timeentry..
-00000150: 6e61 6d65 da09 776f 726b 5f74 7970 65da  name..work_type.
-00000160: 0566 6965 6c64 da05 626c 616e 6b54 da04  .field..blankT..
-00000170: 6e75 6c6c da09 6f6e 5f64 656c 6574 65da  null..on_delete.
-00000180: 0274 6f7a 1664 6a63 6f6e 6e65 6374 7769  .toz.djconnectwi
-00000190: 7365 2e57 6f72 6b54 7970 654e 2902 7a0d  se.WorkTypeN).z.
-000001a0: 646a 636f 6e6e 6563 7477 6973 6572 0600  djconnectwiser..
-000001b0: 0000 290d da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
-000001c0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000001d0: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
-000001e0: 656e 6369 6573 7202 0000 00da 0a41 6c74  enciesr......Alt
-000001f0: 6572 4669 656c 6472 0300 0000 da0a 466f  erFieldr......Fo
-00000200: 7265 6967 6e4b 6579 da06 646a 616e 676f  reignKey..django
-00000210: da02 6462 da08 6465 6c65 7469 6f6e da08  ..db..deletion..
-00000220: 5345 545f 4e55 4c4c da0a 6f70 6572 6174  SET_NULL..operat
-00000230: 696f 6e73 a900 721b 0000 0072 1b00 0000  ions..r....r....
-00000240: fa6e 2f68 6f6d 652f 7361 6d2f 6769 742f  .n/home/sam/git/
-00000250: 4b61 6e62 616e 2f64 6a61 6e67 6f2d 636f  Kanban/django-co
-00000260: 6e6e 6563 7477 6973 652f 646a 616e 676f  nnectwise/django
-00000270: 2d63 6f6e 6e65 6374 7769 7365 2f64 6a63  -connectwise/djc
-00000280: 6f6e 6e65 6374 7769 7365 2f6d 6967 7261  onnectwise/migra
-00000290: 7469 6f6e 732f 3030 3930 5f61 7574 6f5f  tions/0090_auto_
-000002a0: 3230 3139 3037 3131 5f31 3131 342e 7079  20190711_1114.py
-000002b0: 7204 0000 0007 0000 0073 0a00 0000 0c03  r........s......
-000002c0: 0904 0901 0601 0601 7204 0000 0029 06da  ........r....)..
-000002d0: 0964 6a61 6e67 6f2e 6462 7202 0000 0072  .django.dbr....r
-000002e0: 0300 0000 da19 646a 616e 676f 2e64 622e  ......django.db.
-000002f0: 6d6f 6465 6c73 2e64 656c 6574 696f 6e72  models.deletionr
-00000300: 1600 0000 7204 0000 0072 1b00 0000 721b  ....r....r....r.
-00000310: 0000 0072 1b00 0000 721c 0000 00da 083c  ...r....r......<
-00000320: 6d6f 6475 6c65 3e03 0000 0073 0400 0000  module>....s....
-00000330: 1601 0c03                                ....
+00000020: 0073 2200 0000 6400 6401 6c00 6d01 5a01  .s"...d.d.l.m.Z.
+00000030: 0100 4700 6402 6403 8400 6403 6501 6a02  ..G.d.d...d.e.j.
+00000040: 8303 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
+00000050: 01da 0a6d 6967 7261 7469 6f6e 7363 0000  ...migrationsc..
+00000060: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+00000070: 0000 7318 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00000080: 0564 0667 025a 0367 005a 0464 0453 0029  .d.g.Z.g.Z.d.S.)
+00000090: 07da 094d 6967 7261 7469 6f6e da0d 646a  ...Migration..dj
+000000a0: 636f 6e6e 6563 7477 6973 65da 1f30 3039  connectwise..009
+000000b0: 355f 636f 6e6e 6563 7477 6973 6562 6f61  5_connectwiseboa
+000000c0: 7264 5f77 6f72 6b5f 7479 7065 da17 3030  rd_work_type..00
+000000d0: 3933 5f61 7574 6f5f 3230 3139 3037 3136  93_auto_20190716
+000000e0: 5f31 3633 304e 2902 7204 0000 0072 0500  _1630N).r....r..
+000000f0: 0000 2902 7204 0000 0072 0600 0000 2905  ..).r....r....).
+00000100: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000110: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000120: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
+00000130: 6573 da0a 6f70 6572 6174 696f 6e73 a900  es..operations..
+00000140: 720c 0000 0072 0c00 0000 fa64 2f68 6f6d  r....r.....d/hom
+00000150: 652f 6361 6d65 726f 6e2f 4465 762f 6b61  e/cameron/Dev/ka
+00000160: 6e62 616e 2d64 6576 2f64 6a61 6e67 6f2d  nban-dev/django-
+00000170: 636f 6e6e 6563 7477 6973 652f 646a 636f  connectwise/djco
+00000180: 6e6e 6563 7477 6973 652f 6d69 6772 6174  nnectwise/migrat
+00000190: 696f 6e73 2f30 3039 365f 6d65 7267 655f  ions/0096_merge_
+000001a0: 3230 3139 3037 3138 5f31 3130 322e 7079  20190718_1102.py
+000001b0: 7203 0000 0006 0000 0073 0600 0000 0803  r........s......
+000001c0: 0201 0603 7203 0000 004e 2903 da09 646a  ....r....N)...dj
+000001d0: 616e 676f 2e64 6272 0200 0000 7203 0000  ango.dbr....r...
+000001e0: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
+000001f0: 720d 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
+00000200: 0000 0073 0200 0000 0c03                 ...s......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0102_auto_20190719_1058.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0116_auto_20200522_1107.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,44 @@
-00000000: 160d 0d0a ced8 355d 3e02 0000 e300 0000  ......5]>.......
+00000000: 330d 0d0a cd60 c85e 1c02 0000 e300 0000  3....`.^........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3300 0000 6400 0064 0100 6c00 006d  .s3...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 4764 0200  ..Z..m..Z...Gd..
-00000040: 6403 0084 0000 6403 0065 0100 6a03 0083  d.....d..e..j...
-00000050: 0300 5a03 0064 0400 5329 05e9 0000 0000  ..Z..d..S)......
-00000060: 2902 da0a 6d69 6772 6174 696f 6e73 da06  )...migrations..
-00000070: 6d6f 6465 6c73 6300 0000 0000 0000 0000  modelsc.........
-00000080: 0000 000b 0000 0040 0000 0073 7300 0000  .......@...ss...
-00000090: 6500 005a 0100 6400 005a 0200 6410 0067  e..Z..d..Z..d..g
-000000a0: 0100 5a03 0065 0400 6a05 0064 0300 6404  ..Z..e..j..d..d.
-000000b0: 0064 0500 6406 0064 0700 6506 006a 0700  .d..d..d..e..j..
-000000c0: 6408 0064 0900 640a 0064 0b00 8300 0283  d..d..d..d......
-000000d0: 0003 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000e0: 0064 0c00 6407 0065 0600 6a08 0064 0d00  .d..d..e..j..d..
-000000f0: 640e 0083 0001 8300 0367 0200 5a09 0064  d........g..Z..d
-00000100: 0f00 5329 11da 094d 6967 7261 7469 6f6e  ..S)...Migration
-00000110: da0d 646a 636f 6e6e 6563 7477 6973 65da  ..djconnectwise.
-00000120: 1630 3130 315f 6167 7265 656d 656e 745f  .0101_agreement_
-00000130: 636f 6d70 616e 79da 0a6d 6f64 656c 5f6e  company..model_n
-00000140: 616d 65da 0961 6772 6565 6d65 6e74 da04  ame..agreement..
-00000150: 6e61 6d65 da0e 6167 7265 656d 656e 745f  name..agreement_
-00000160: 7479 7065 da05 6669 656c 64da 0a6d 6178  type..field..max
-00000170: 5f6c 656e 6774 68e9 3200 0000 da04 6e75  _length.2.....nu
-00000180: 6c6c 54da 0e63 616e 6365 6c6c 6564 5f66  llT..cancelled_f
-00000190: 6c61 67da 0764 6566 6175 6c74 464e 2902  lag..defaultFN).
-000001a0: 7a0d 646a 636f 6e6e 6563 7477 6973 657a  z.djconnectwisez
-000001b0: 1630 3130 315f 6167 7265 656d 656e 745f  .0101_agreement_
-000001c0: 636f 6d70 616e 7929 0ada 085f 5f6e 616d  company)...__nam
-000001d0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-000001e0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
-000001f0: 6570 656e 6465 6e63 6965 7372 0200 0000  ependenciesr....
-00000200: da08 4164 6446 6965 6c64 7203 0000 00da  ..AddFieldr.....
-00000210: 0943 6861 7246 6965 6c64 da0c 426f 6f6c  .CharField..Bool
-00000220: 6561 6e46 6965 6c64 da0a 6f70 6572 6174  eanField..operat
-00000230: 696f 6e73 a900 7219 0000 0072 1900 0000  ions..r....r....
-00000240: fa6e 2f68 6f6d 652f 7361 6d2f 6769 742f  .n/home/sam/git/
-00000250: 4b61 6e62 616e 2f64 6a61 6e67 6f2d 636f  Kanban/django-co
-00000260: 6e6e 6563 7477 6973 652f 646a 616e 676f  nnectwise/django
-00000270: 2d63 6f6e 6e65 6374 7769 7365 2f64 6a63  -connectwise/djc
-00000280: 6f6e 6e65 6374 7769 7365 2f6d 6967 7261  onnectwise/migra
-00000290: 7469 6f6e 732f 3031 3032 5f61 7574 6f5f  tions/0102_auto_
-000002a0: 3230 3139 3037 3139 5f31 3035 382e 7079  20190719_1058.py
-000002b0: 7204 0000 0006 0000 0073 1200 0000 0c03  r........s......
-000002c0: 0904 0901 0601 0601 1802 0901 0601 0601  ................
-000002d0: 7204 0000 004e 2904 da09 646a 616e 676f  r....N)...django
-000002e0: 2e64 6272 0200 0000 7203 0000 0072 0400  .dbr....r....r..
-000002f0: 0000 7219 0000 0072 1900 0000 7219 0000  ..r....r....r...
-00000300: 0072 1a00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000310: 0300 0000 7302 0000 0016 03              ....s......
+00000020: 0073 2600 0000 6400 6401 6c00 6d01 5a01  .s&...d.d.l.m.Z.
+00000030: 6d02 5a02 0100 4700 6402 6403 8400 6403  m.Z...G.d.d...d.
+00000040: 6501 6a03 8303 5a03 6404 5300 2905 e900  e.j...Z.d.S.)...
+00000050: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
+00000060: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000070: 0000 0000 0000 0700 0000 4000 0000 7338  ..........@...s8
+00000080: 0000 0065 005a 0164 005a 0264 0b67 015a  ...e.Z.d.Z.d.g.Z
+00000090: 0365 046a 0564 0364 0464 058d 0265 046a  .e.j.d.d.d...e.j
+000000a0: 0664 0364 0665 076a 0864 0764 088d 0164  .d.d.e.j.d.d...d
+000000b0: 098d 0367 025a 0964 0a53 0029 0cda 094d  ...g.Z.d.S.)...M
+000000c0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
+000000d0: 6563 7477 6973 65da 1f30 3131 355f 6167  ectwise..0115_ag
+000000e0: 7265 656d 656e 745f 6167 7265 656d 656e  reement_agreemen
+000000f0: 745f 7374 6174 7573 da07 636f 6d70 616e  t_status..compan
+00000100: 79da 0c63 6f6d 7061 6e79 5f74 7970 6529  y..company_type)
+00000110: 02da 0a6d 6f64 656c 5f6e 616d 65da 046e  ...model_name..n
+00000120: 616d 65da 0d63 6f6d 7061 6e79 5f74 7970  ame..company_typ
+00000130: 6573 7a19 646a 636f 6e6e 6563 7477 6973  esz.djconnectwis
+00000140: 652e 436f 6d70 616e 7954 7970 6529 01da  e.CompanyType)..
+00000150: 0274 6f29 0372 0900 0000 720a 0000 00da  .to).r....r.....
+00000160: 0566 6965 6c64 4e29 0272 0500 0000 7206  .fieldN).r....r.
+00000170: 0000 0029 0ada 085f 5f6e 616d 655f 5fda  ...)...__name__.
+00000180: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000190: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
+000001a0: 6465 6e63 6965 7372 0200 0000 da0b 5265  denciesr......Re
+000001b0: 6d6f 7665 4669 656c 64da 0841 6464 4669  moveField..AddFi
+000001c0: 656c 6472 0300 0000 da0f 4d61 6e79 546f  eldr......ManyTo
+000001d0: 4d61 6e79 4669 656c 64da 0a6f 7065 7261  ManyField..opera
+000001e0: 7469 6f6e 73a9 0072 1600 0000 7216 0000  tions..r....r...
+000001f0: 00fa 632f 686f 6d65 2f63 616d 6572 6f6e  ..c/home/cameron
+00000200: 2f44 6576 2f6b 616e 6261 6e2d 6465 762f  /Dev/kanban-dev/
+00000210: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
+00000220: 7365 2f64 6a63 6f6e 6e65 6374 7769 7365  se/djconnectwise
+00000230: 2f6d 6967 7261 7469 6f6e 732f 3031 3136  /migrations/0116
+00000240: 5f61 7574 6f5f 3230 3230 3035 3232 5f31  _auto_20200522_1
+00000250: 3130 372e 7079 7204 0000 0006 0000 0073  107.pyr........s
+00000260: 1000 0000 0803 0604 0401 0201 0602 0401  ................
+00000270: 0201 0201 7204 0000 004e 2904 da09 646a  ....r....N)...dj
+00000280: 616e 676f 2e64 6272 0200 0000 7203 0000  ango.dbr....r...
+00000290: 0072 0400 0000 7216 0000 0072 1600 0000  .r....r....r....
+000002a0: 7216 0000 0072 1700 0000 da08 3c6d 6f64  r....r......<mod
+000002b0: 756c 653e 0300 0000 7302 0000 0010 03    ule>....s......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0056_auto_20180504_0744.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0049_auto_20180205_1122.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,79 @@
-00000000: 160d 0d0a a4b0 1f5d 6d02 0000 e300 0000  .......]m.......
+00000000: 330d 0d0a 10ec da5c d204 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 000c 0000 0040 0000 0073  ...........@...s
-000000b0: 6d00 0000 6500 005a 0100 6400 005a 0200  m...e..Z..d..Z..
-000000c0: 6412 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6408  ..d..d..d..d..d.
-000000e0: 0064 1300 6902 0083 0002 6504 006a 0600  .d..i.....e..j..
-000000f0: 640b 0064 0400 6403 0064 0c00 640d 0065  d..d..d..d..d..e
-00000100: 0700 6a08 0064 0e00 640f 0064 1000 640f  ..j..d..d..d..d.
-00000110: 0083 0002 8300 0367 0200 5a09 0064 1100  .......g..Z..d..
-00000120: 5329 14da 094d 6967 7261 7469 6f6e da0d  S)...Migration..
-00000130: 646a 636f 6e6e 6563 7477 6973 65da 1730  djconnectwise..0
-00000140: 3035 355f 6175 746f 5f32 3031 3830 3530  055_auto_2018050
-00000150: 315f 3130 3232 da04 6e61 6d65 5a0f 6f70  1_1022..nameZ.op
-00000160: 706f 7274 756e 6974 796e 6f74 65da 076f  portunitynote..o
-00000170: 7074 696f 6e73 da13 7665 7262 6f73 655f  ptions..verbose_
-00000180: 6e61 6d65 5f70 6c75 7261 6c7a 114f 7070  name_pluralz.Opp
-00000190: 6f72 7475 6e69 7479 204e 6f74 6573 da08  ortunity Notes..
-000001a0: 6f72 6465 7269 6e67 fa0d 2d64 6174 655f  ordering..-date_
-000001b0: 6372 6561 7465 64da 0269 64da 0a6d 6f64  created..id..mod
-000001c0: 656c 5f6e 616d 65da 0c64 6174 655f 6372  el_name..date_cr
-000001d0: 6561 7465 64da 0566 6965 6c64 da05 626c  eated..field..bl
-000001e0: 616e 6b54 da04 6e75 6c6c 4e29 027a 0d64  ankT..nullN).z.d
-000001f0: 6a63 6f6e 6e65 6374 7769 7365 7207 0000  jconnectwiser...
-00000200: 0029 0272 0c00 0000 7a02 6964 290a da08  .).r....z.id)...
-00000210: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000220: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000230: 5f5f da0c 6465 7065 6e64 656e 6369 6573  __..dependencies
-00000240: 7203 0000 00da 1141 6c74 6572 4d6f 6465  r......AlterMode
-00000250: 6c4f 7074 696f 6e73 da08 4164 6446 6965  lOptions..AddFie
-00000260: 6c64 7204 0000 00da 0d44 6174 6554 696d  ldr......DateTim
-00000270: 6546 6965 6c64 da0a 6f70 6572 6174 696f  eField..operatio
-00000280: 6e73 a900 721b 0000 0072 1b00 0000 fa6e  ns..r....r.....n
-00000290: 2f68 6f6d 652f 7361 6d2f 6769 742f 4b61  /home/sam/git/Ka
-000002a0: 6e62 616e 2f64 6a61 6e67 6f2d 636f 6e6e  nban/django-conn
-000002b0: 6563 7477 6973 652f 646a 616e 676f 2d63  ectwise/django-c
-000002c0: 6f6e 6e65 6374 7769 7365 2f64 6a63 6f6e  onnectwise/djcon
-000002d0: 6e65 6374 7769 7365 2f6d 6967 7261 7469  nectwise/migrati
-000002e0: 6f6e 732f 3030 3536 5f61 7574 6f5f 3230  ons/0056_auto_20
-000002f0: 3138 3035 3034 5f30 3734 342e 7079 7205  180504_0744.pyr.
-00000300: 0000 0007 0000 0073 1000 0000 0c03 0904  .......s........
-00000310: 0901 0601 1202 0901 0601 0601 7205 0000  ............r...
-00000320: 004e 2906 da0a 5f5f 6675 7475 7265 5f5f  .N)...__future__
-00000330: 7202 0000 00da 0964 6a61 6e67 6f2e 6462  r......django.db
-00000340: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
-00000350: 1b00 0000 721b 0000 0072 1b00 0000 721c  ....r....r....r.
-00000360: 0000 00da 083c 6d6f 6475 6c65 3e02 0000  .....<module>...
-00000370: 0073 0400 0000 1002 1603                 .s........
+00000020: 0073 3a00 0000 6400 6401 6c00 6d01 5a01  .s:...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 6400 6403 6c05 5a06 4700 6404 6405  ..d.d.l.Z.G.d.d.
+00000050: 8400 6405 6503 6a07 8303 5a07 6403 5300  ..d.e.j...Z.d.S.
+00000060: 2906 e900 0000 0029 01da 1075 6e69 636f  )......)...unico
+00000070: 6465 5f6c 6974 6572 616c 7329 02da 0a6d  de_literals)...m
+00000080: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000090: 734e 6300 0000 0000 0000 0000 0000 000b  sNc.............
+000000a0: 0000 0040 0000 0073 9000 0000 6500 5a01  ...@...s....e.Z.
+000000b0: 6400 5a02 6417 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000c0: 6404 6506 6a07 6405 6405 6406 6407 6408  d.e.j.d.d.d.d.d.
+000000d0: 8d04 6602 6409 6508 6a09 6a0a 6a0b 6405  ..f.d.e.j.j.j.d.
+000000e0: 6409 640a 8d02 6602 640b 6508 6a09 6a0a  d.d...f.d.e.j.j.
+000000f0: 6a0c 6405 640b 640c 8d02 6602 640d 6506  j.d.d.d...f.d.e.
+00000100: 6a0d 8300 6602 6704 6418 640e 640f 9c02  j...f.g.d.d.d...
+00000110: 6410 8d03 6504 6a0e 6411 640d 6506 6a0f  d...e.j.d.d.e.j.
+00000120: 6405 6412 6405 6413 6506 6a10 6414 8d05  d.d.d.d.e.j.d...
+00000130: 6415 8d03 6702 5a11 6416 5300 2919 da09  d...g.Z.d.S.)...
+00000140: 4d69 6772 6174 696f 6eda 0d64 6a63 6f6e  Migration..djcon
+00000150: 6e65 6374 7769 7365 da14 3030 3438 5f70  nectwise..0048_p
+00000160: 726f 6a65 6374 5f6d 616e 6167 6572 da10  roject_manager..
+00000170: 5361 6c65 7350 726f 6261 6269 6c69 7479  SalesProbability
+00000180: da02 6964 5446 da02 4944 2904 da0c 6175  ..idTF..ID)...au
+00000190: 746f 5f63 7265 6174 6564 da0b 7072 696d  to_created..prim
+000001a0: 6172 795f 6b65 79da 0973 6572 6961 6c69  ary_key..seriali
+000001b0: 7a65 da0c 7665 7262 6f73 655f 6e61 6d65  ze..verbose_name
+000001c0: da07 6372 6561 7465 6429 02da 0c61 7574  ..created)...aut
+000001d0: 6f5f 6e6f 775f 6164 6472 0e00 0000 da08  o_now_addr......
+000001e0: 6d6f 6469 6669 6564 2902 da08 6175 746f  modified)...auto
+000001f0: 5f6e 6f77 720e 0000 00da 0b70 726f 6261  _nowr......proba
+00000200: 6269 6c69 7479 7a13 5361 6c65 7320 7072  bilityz.Sales pr
+00000210: 6f62 6162 696c 6974 6965 7329 02da 086f  obabilities)...o
+00000220: 7264 6572 696e 67da 1376 6572 626f 7365  rdering..verbose
+00000230: 5f6e 616d 655f 706c 7572 616c 2903 da04  _name_plural)...
+00000240: 6e61 6d65 da06 6669 656c 6473 da07 6f70  name..fields..op
+00000250: 7469 6f6e 73da 0b6f 7070 6f72 7475 6e69  tions..opportuni
+00000260: 7479 7a1e 646a 636f 6e6e 6563 7477 6973  tyz.djconnectwis
+00000270: 652e 5361 6c65 7350 726f 6261 6269 6c69  e.SalesProbabili
+00000280: 7479 da11 7361 6c65 735f 7072 6f62 6162  ty..sales_probab
+00000290: 696c 6974 7929 05da 046e 756c 6cda 0274  ility)...null..t
+000002a0: 6fda 0562 6c61 6e6b da0c 7265 6c61 7465  o..blank..relate
+000002b0: 645f 6e61 6d65 da09 6f6e 5f64 656c 6574  d_name..on_delet
+000002c0: 6529 03da 0a6d 6f64 656c 5f6e 616d 6572  e)...model_namer
+000002d0: 1600 0000 da05 6669 656c 644e 2902 7206  ......fieldN).r.
+000002e0: 0000 0072 0700 0000 2901 7213 0000 0029  ...r....).r....)
+000002f0: 12da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000300: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000310: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
+00000320: 6965 7372 0300 0000 da0b 4372 6561 7465  iesr......Create
+00000330: 4d6f 6465 6c72 0400 0000 da09 4175 746f  Modelr......Auto
+00000340: 4669 656c 64da 1164 6a61 6e67 6f5f 6578  Field..django_ex
+00000350: 7465 6e73 696f 6e73 da02 6462 7217 0000  tensions..dbr...
+00000360: 00da 1543 7265 6174 696f 6e44 6174 6554  ...CreationDateT
+00000370: 696d 6546 6965 6c64 da19 4d6f 6469 6669  imeField..Modifi
+00000380: 6361 7469 6f6e 4461 7465 5469 6d65 4669  cationDateTimeFi
+00000390: 656c 64da 0c49 6e74 6567 6572 4669 656c  eld..IntegerFiel
+000003a0: 64da 0841 6464 4669 656c 64da 0a46 6f72  d..AddField..For
+000003b0: 6569 676e 4b65 79da 0743 4153 4341 4445  eignKey..CASCADE
+000003c0: da0a 6f70 6572 6174 696f 6e73 a900 7231  ..operations..r1
+000003d0: 0000 0072 3100 0000 fa63 2f68 6f6d 652f  ...r1....c/home/
+000003e0: 6361 6d65 726f 6e2f 4465 762f 6b61 6e62  cameron/Dev/kanb
+000003f0: 616e 2d64 6576 2f64 6a61 6e67 6f2d 636f  an-dev/django-co
+00000400: 6e6e 6563 7477 6973 652f 646a 636f 6e6e  nnectwise/djconn
+00000410: 6563 7477 6973 652f 6d69 6772 6174 696f  ectwise/migratio
+00000420: 6e73 2f30 3034 395f 6175 746f 5f32 3031  ns/0049_auto_201
+00000430: 3830 3230 355f 3131 3232 2e70 7972 0500  80205_1122.pyr..
+00000440: 0000 0800 0000 731a 0000 0008 0306 0404  ......s.........
+00000450: 0102 0214 0114 0114 010c 0302 010a 0304  ................
+00000460: 0102 0102 0172 0500 0000 2908 da0a 5f5f  .....r....)...__
+00000470: 6675 7475 7265 5f5f 7202 0000 00da 0964  future__r......d
+00000480: 6a61 6e67 6f2e 6462 7203 0000 0072 0400  jango.dbr....r..
+00000490: 0000 da1b 646a 616e 676f 5f65 7874 656e  ....django_exten
+000004a0: 7369 6f6e 732e 6462 2e66 6965 6c64 7372  sions.db.fieldsr
+000004b0: 2800 0000 7205 0000 0072 3100 0000 7231  (...r....r1...r1
+000004c0: 0000 0072 3100 0000 7232 0000 00da 083c  ...r1...r2.....<
+000004d0: 6d6f 6475 6c65 3e02 0000 0073 0600 0000  module>....s....
+000004e0: 0c02 1001 0803                           ......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0038_auto_20170920_1138.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0038_auto_20170920_1138.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,42 @@
-00000000: 160d 0d0a a4b0 1f5d 9d01 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c 9d01 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0007 0000 0040 0000 0073  ...........@...s
-000000b0: 4000 0000 6500 005a 0100 6400 005a 0200  @...e..Z..d..Z..
-000000c0: 6409 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 8300 0083 0003 6701 005a 0800  .j........g..Z..
-000000f0: 6408 0053 290a da09 4d69 6772 6174 696f  d..S)...Migratio
-00000100: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
-00000110: da17 3030 3337 5f61 7574 6f5f 3230 3137  ..0037_auto_2017
-00000120: 3039 3230 5f30 3935 39da 0a6d 6f64 656c  0920_0959..model
-00000130: 5f6e 616d 65da 0b6f 7070 6f72 7475 6e69  _name..opportuni
-00000140: 7479 da04 6e61 6d65 da13 6578 7065 6374  ty..name..expect
-00000150: 6564 5f63 6c6f 7365 5f64 6174 65da 0566  ed_close_date..f
-00000160: 6965 6c64 4e29 027a 0d64 6a63 6f6e 6e65  ieldN).z.djconne
-00000170: 6374 7769 7365 7207 0000 0029 09da 085f  ctwiser....)..._
-00000180: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000190: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000001a0: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
-000001b0: 0300 0000 da0a 416c 7465 7246 6965 6c64  ......AlterField
-000001c0: 7204 0000 00da 0944 6174 6546 6965 6c64  r......DateField
-000001d0: da0a 6f70 6572 6174 696f 6e73 a900 7214  ..operations..r.
-000001e0: 0000 0072 1400 0000 fa6e 2f68 6f6d 652f  ...r.....n/home/
-000001f0: 7361 6d2f 6769 742f 4b61 6e62 616e 2f64  sam/git/Kanban/d
-00000200: 6a61 6e67 6f2d 636f 6e6e 6563 7477 6973  jango-connectwis
-00000210: 652f 646a 616e 676f 2d63 6f6e 6e65 6374  e/django-connect
-00000220: 7769 7365 2f64 6a63 6f6e 6e65 6374 7769  wise/djconnectwi
-00000230: 7365 2f6d 6967 7261 7469 6f6e 732f 3030  se/migrations/00
-00000240: 3338 5f61 7574 6f5f 3230 3137 3039 3230  38_auto_20170920
-00000250: 5f31 3133 382e 7079 7205 0000 0007 0000  _1138.pyr.......
-00000260: 0073 0a00 0000 0c03 0904 0901 0601 0601  .s..............
-00000270: 7205 0000 004e 2906 da0a 5f5f 6675 7475  r....N)...__futu
-00000280: 7265 5f5f 7202 0000 00da 0964 6a61 6e67  re__r......djang
-00000290: 6f2e 6462 7203 0000 0072 0400 0000 7205  o.dbr....r....r.
-000002a0: 0000 0072 1400 0000 7214 0000 0072 1400  ...r....r....r..
-000002b0: 0000 7215 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000002c0: 3e02 0000 0073 0400 0000 1002 1603       >....s........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0500 0000 4000 0000 7328  ..........@...s(
+000000a0: 0000 0065 005a 0164 005a 0264 0767 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0783 0064  .e.j.d.d.e.j...d
+000000c0: 058d 0367 015a 0864 0653 0029 08da 094d  ...g.Z.d.S.)...M
+000000d0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
+000000e0: 6563 7477 6973 65da 1730 3033 375f 6175  ectwise..0037_au
+000000f0: 746f 5f32 3031 3730 3932 305f 3039 3539  to_20170920_0959
+00000100: da0b 6f70 706f 7274 756e 6974 79da 1365  ..opportunity..e
+00000110: 7870 6563 7465 645f 636c 6f73 655f 6461  xpected_close_da
+00000120: 7465 2903 da0a 6d6f 6465 6c5f 6e61 6d65  te)...model_name
+00000130: da04 6e61 6d65 da05 6669 656c 644e 2902  ..name..fieldN).
+00000140: 7206 0000 0072 0700 0000 2909 da08 5f5f  r....r....)...__
+00000150: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000160: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000170: da0c 6465 7065 6e64 656e 6369 6573 7203  ..dependenciesr.
+00000180: 0000 00da 0a41 6c74 6572 4669 656c 6472  .....AlterFieldr
+00000190: 0400 0000 da09 4461 7465 4669 656c 64da  ......DateField.
+000001a0: 0a6f 7065 7261 7469 6f6e 73a9 0072 1400  .operations..r..
+000001b0: 0000 7214 0000 00fa 632f 686f 6d65 2f63  ..r.....c/home/c
+000001c0: 616d 6572 6f6e 2f44 6576 2f6b 616e 6261  ameron/Dev/kanba
+000001d0: 6e2d 6465 762f 646a 616e 676f 2d63 6f6e  n-dev/django-con
+000001e0: 6e65 6374 7769 7365 2f64 6a63 6f6e 6e65  nectwise/djconne
+000001f0: 6374 7769 7365 2f6d 6967 7261 7469 6f6e  ctwise/migration
+00000200: 732f 3030 3338 5f61 7574 6f5f 3230 3137  s/0038_auto_2017
+00000210: 3039 3230 5f31 3133 382e 7079 7205 0000  0920_1138.pyr...
+00000220: 0007 0000 0073 0a00 0000 0803 0604 0401  .....s..........
+00000230: 0201 0201 7205 0000 004e 2906 da0a 5f5f  ....r....N)...__
+00000240: 6675 7475 7265 5f5f 7202 0000 00da 0964  future__r......d
+00000250: 6a61 6e67 6f2e 6462 7203 0000 0072 0400  jango.dbr....r..
+00000260: 0000 7205 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00000270: 0072 1400 0000 7215 0000 00da 083c 6d6f  .r....r......<mo
+00000280: 6475 6c65 3e02 0000 0073 0400 0000 0c02  dule>....s......
+00000290: 1003                                     ..
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0112_syncjob_synchronizer_class.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0112_syncjob_synchronizer_class.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,41 @@
-00000000: 160d 0d0a a2e7 0b5e ac01 0000 e300 0000  .......^........
+00000000: 330d 0d0a 589f 135e ac01 0000 e300 0000  3...X..^........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3300 0000 6400 0064 0100 6c00 006d  .s3...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 4764 0200  ..Z..m..Z...Gd..
-00000040: 6403 0084 0000 6403 0065 0100 6a03 0083  d.....d..e..j...
-00000050: 0300 5a03 0064 0400 5329 05e9 0000 0000  ..Z..d..S)......
-00000060: 2902 da0a 6d69 6772 6174 696f 6e73 da06  )...migrations..
-00000070: 6d6f 6465 6c73 6300 0000 0000 0000 0000  modelsc.........
-00000080: 0000 000d 0000 0040 0000 0073 5200 0000  .......@...sR...
-00000090: 6500 005a 0100 6400 005a 0200 640e 0067  e..Z..d..Z..d..g
-000000a0: 0100 5a03 0065 0400 6a05 0064 0300 6404  ..Z..e..j..d..d.
-000000b0: 0064 0500 6406 0064 0700 6506 006a 0700  .d..d..d..e..j..
-000000c0: 6408 0064 0900 640a 0064 0b00 640c 0064  d..d..d..d..d..d
-000000d0: 0900 8300 0383 0003 6701 005a 0800 640d  ........g..Z..d.
-000000e0: 0053 290f da09 4d69 6772 6174 696f 6eda  .S)...Migration.
-000000f0: 0d64 6a63 6f6e 6e65 6374 7769 7365 da17  .djconnectwise..
-00000100: 3031 3131 5f61 7574 6f5f 3230 3139 3132  0111_auto_201912
-00000110: 3034 5f30 3833 38da 0a6d 6f64 656c 5f6e  04_0838..model_n
-00000120: 616d 65da 0773 796e 636a 6f62 da04 6e61  ame..syncjob..na
-00000130: 6d65 da12 7379 6e63 6872 6f6e 697a 6572  me..synchronizer
-00000140: 5f63 6c61 7373 da05 6669 656c 64da 0562  _class..field..b
-00000150: 6c61 6e6b 54da 0a6d 6178 5f6c 656e 6774  lankT..max_lengt
-00000160: 68e9 6400 0000 da04 6e75 6c6c 4e29 027a  h.d.....nullN).z
-00000170: 0d64 6a63 6f6e 6e65 6374 7769 7365 7a17  .djconnectwisez.
-00000180: 3031 3131 5f61 7574 6f5f 3230 3139 3132  0111_auto_201912
-00000190: 3034 5f30 3833 3829 09da 085f 5f6e 616d  04_0838)...__nam
-000001a0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-000001b0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
-000001c0: 6570 656e 6465 6e63 6965 7372 0200 0000  ependenciesr....
-000001d0: da08 4164 6446 6965 6c64 7203 0000 00da  ..AddFieldr.....
-000001e0: 0943 6861 7246 6965 6c64 da0a 6f70 6572  .CharField..oper
-000001f0: 6174 696f 6e73 a900 7217 0000 0072 1700  ations..r....r..
-00000200: 0000 fa76 2f68 6f6d 652f 7361 6d2f 6769  ...v/home/sam/gi
-00000210: 742f 4b61 6e62 616e 2f64 6a61 6e67 6f2d  t/Kanban/django-
-00000220: 636f 6e6e 6563 7477 6973 652f 646a 616e  connectwise/djan
-00000230: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
-00000240: 6a63 6f6e 6e65 6374 7769 7365 2f6d 6967  jconnectwise/mig
-00000250: 7261 7469 6f6e 732f 3031 3132 5f73 796e  rations/0112_syn
-00000260: 636a 6f62 5f73 796e 6368 726f 6e69 7a65  cjob_synchronize
-00000270: 725f 636c 6173 732e 7079 7204 0000 0006  r_class.pyr.....
-00000280: 0000 0073 0a00 0000 0c03 0904 0901 0601  ...s............
-00000290: 0601 7204 0000 004e 2904 da09 646a 616e  ..r....N)...djan
-000002a0: 676f 2e64 6272 0200 0000 7203 0000 0072  go.dbr....r....r
-000002b0: 0400 0000 7217 0000 0072 1700 0000 7217  ....r....r....r.
-000002c0: 0000 0072 1800 0000 da08 3c6d 6f64 756c  ...r......<modul
-000002d0: 653e 0300 0000 7302 0000 0016 03         e>....s......
+00000020: 0073 2600 0000 6400 6401 6c00 6d01 5a01  .s&...d.d.l.m.Z.
+00000030: 6d02 5a02 0100 4700 6402 6403 8400 6403  m.Z...G.d.d...d.
+00000040: 6501 6a03 8303 5a03 6404 5300 2905 e900  e.j...Z.d.S.)...
+00000050: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
+00000060: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000070: 0000 0000 0000 0800 0000 4000 0000 7330  ..........@...s0
+00000080: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+00000090: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000a0: 0664 0564 078d 0364 088d 0367 015a 0864  .d.d...d...g.Z.d
+000000b0: 0953 0029 0bda 094d 6967 7261 7469 6f6e  .S.)...Migration
+000000c0: da0d 646a 636f 6e6e 6563 7477 6973 65da  ..djconnectwise.
+000000d0: 1730 3131 315f 6175 746f 5f32 3031 3931  .0111_auto_20191
+000000e0: 3230 345f 3038 3338 da07 7379 6e63 6a6f  204_0838..syncjo
+000000f0: 62da 1273 796e 6368 726f 6e69 7a65 725f  b..synchronizer_
+00000100: 636c 6173 7354 e964 0000 0029 03da 0562  classT.d...)...b
+00000110: 6c61 6e6b da0a 6d61 785f 6c65 6e67 7468  lank..max_length
+00000120: da04 6e75 6c6c 2903 da0a 6d6f 6465 6c5f  ..null)...model_
+00000130: 6e61 6d65 da04 6e61 6d65 da05 6669 656c  name..name..fiel
+00000140: 644e 2902 7205 0000 0072 0600 0000 2909  dN).r....r....).
+00000150: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000160: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000170: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
+00000180: 6573 7202 0000 00da 0841 6464 4669 656c  esr......AddFiel
+00000190: 6472 0300 0000 da09 4368 6172 4669 656c  dr......CharFiel
+000001a0: 64da 0a6f 7065 7261 7469 6f6e 73a9 0072  d..operations..r
+000001b0: 1700 0000 7217 0000 00fa 6b2f 686f 6d65  ....r.....k/home
+000001c0: 2f63 616d 6572 6f6e 2f44 6576 2f6b 616e  /cameron/Dev/kan
+000001d0: 6261 6e2d 6465 762f 646a 616e 676f 2d63  ban-dev/django-c
+000001e0: 6f6e 6e65 6374 7769 7365 2f64 6a63 6f6e  onnectwise/djcon
+000001f0: 6e65 6374 7769 7365 2f6d 6967 7261 7469  nectwise/migrati
+00000200: 6f6e 732f 3031 3132 5f73 796e 636a 6f62  ons/0112_syncjob
+00000210: 5f73 796e 6368 726f 6e69 7a65 725f 636c  _synchronizer_cl
+00000220: 6173 732e 7079 7204 0000 0006 0000 0073  ass.pyr........s
+00000230: 0a00 0000 0803 0604 0401 0201 0201 7204  ..............r.
+00000240: 0000 004e 2904 da09 646a 616e 676f 2e64  ...N)...django.d
+00000250: 6272 0200 0000 7203 0000 0072 0400 0000  br....r....r....
+00000260: 7217 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
+00000270: 1800 0000 da08 3c6d 6f64 756c 653e 0300  ......<module>..
+00000280: 0000 7302 0000 0010 03                   ..s......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0009_member_license_class.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0002_auto_20170223_2143.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,42 @@
-00000000: 160d 0d0a a4b0 1f5d fb01 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c 9c01 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0011 0000 0040 0000 0073  ...........@...s
-000000b0: 6400 0000 6500 005a 0100 6400 005a 0200  d...e..Z..d..Z..
-000000c0: 6414 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 6408 0064 1500 6416 0067 0200  .j..d..d..d..g..
-000000f0: 640d 0064 0e00 640f 0064 0e00 6410 0064  d..d..d..d..d..d
-00000100: 1100 6412 0064 0e00 8300 0583 0003 6701  ..d..d........g.
-00000110: 005a 0800 6413 0053 2917 da09 4d69 6772  .Z..d..S)...Migr
-00000120: 6174 696f 6eda 0d64 6a63 6f6e 6e65 6374  ation..djconnect
-00000130: 7769 7365 da18 3030 3038 5f70 726f 6a65  wise..0008_proje
-00000140: 6374 5f73 7461 7475 735f 6e61 6d65 da0a  ct_status_name..
-00000150: 6d6f 6465 6c5f 6e61 6d65 da06 6d65 6d62  model_name..memb
-00000160: 6572 da04 6e61 6d65 da0d 6c69 6365 6e73  er..name..licens
-00000170: 655f 636c 6173 73da 0566 6965 6c64 da07  e_class..field..
-00000180: 6368 6f69 6365 73da 0146 fa0c 4675 6c6c  choices..F..Full
-00000190: 206c 6963 656e 7365 da01 41fa 0b41 5049   license..A..API
-000001a0: 206c 6963 656e 7365 da08 6462 5f69 6e64   license..db_ind
-000001b0: 6578 54da 0562 6c61 6e6b da0a 6d61 785f  exT..blank..max_
-000001c0: 6c65 6e67 7468 e914 0000 00da 046e 756c  length.......nul
-000001d0: 6c4e 2902 7a0d 646a 636f 6e6e 6563 7477  lN).z.djconnectw
-000001e0: 6973 657a 1830 3030 385f 7072 6f6a 6563  isez.0008_projec
-000001f0: 745f 7374 6174 7573 5f6e 616d 6529 0272  t_status_name).r
-00000200: 0e00 0000 720f 0000 0029 0272 1000 0000  ....r....).r....
-00000210: 7211 0000 0029 09da 085f 5f6e 616d 655f  r....)...__name_
-00000220: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000230: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
-00000240: 656e 6465 6e63 6965 7372 0300 0000 da08  endenciesr......
-00000250: 4164 6446 6965 6c64 7204 0000 00da 0943  AddFieldr......C
-00000260: 6861 7246 6965 6c64 da0a 6f70 6572 6174  harField..operat
-00000270: 696f 6e73 a900 721e 0000 0072 1e00 0000  ions..r....r....
-00000280: fa70 2f68 6f6d 652f 7361 6d2f 6769 742f  .p/home/sam/git/
-00000290: 4b61 6e62 616e 2f64 6a61 6e67 6f2d 636f  Kanban/django-co
-000002a0: 6e6e 6563 7477 6973 652f 646a 616e 676f  nnectwise/django
-000002b0: 2d63 6f6e 6e65 6374 7769 7365 2f64 6a63  -connectwise/djc
-000002c0: 6f6e 6e65 6374 7769 7365 2f6d 6967 7261  onnectwise/migra
-000002d0: 7469 6f6e 732f 3030 3039 5f6d 656d 6265  tions/0009_membe
-000002e0: 725f 6c69 6365 6e73 655f 636c 6173 732e  r_license_class.
-000002f0: 7079 7205 0000 0007 0000 0073 0a00 0000  pyr........s....
-00000300: 0c03 0904 0901 0601 0601 7205 0000 004e  ..........r....N
-00000310: 2906 da0a 5f5f 6675 7475 7265 5f5f 7202  )...__future__r.
-00000320: 0000 00da 0964 6a61 6e67 6f2e 6462 7203  .....django.dbr.
-00000330: 0000 0072 0400 0000 7205 0000 0072 1e00  ...r....r....r..
-00000340: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00000350: 00da 083c 6d6f 6475 6c65 3e02 0000 0073  ...<module>....s
-00000360: 0400 0000 1002 1603                      ........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0600 0000 4000 0000 732c  ..........@...s,
+000000a0: 0000 0065 005a 0164 005a 0264 0967 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000c0: 068d 0164 078d 0367 015a 0864 0853 0029  ...d...g.Z.d.S.)
+000000d0: 0ada 094d 6967 7261 7469 6f6e da0d 646a  ...Migration..dj
+000000e0: 636f 6e6e 6563 7477 6973 65da 0c30 3030  connectwise..000
+000000f0: 315f 696e 6974 6961 6cda 1063 6f6e 6e65  1_initial..conne
+00000100: 6374 7769 7365 626f 6172 64da 0869 6e61  ctwiseboard..ina
+00000110: 6374 6976 6546 2901 da07 6465 6661 756c  ctiveF)...defaul
+00000120: 7429 03da 0a6d 6f64 656c 5f6e 616d 65da  t)...model_name.
+00000130: 046e 616d 65da 0566 6965 6c64 4e29 0272  .name..fieldN).r
+00000140: 0600 0000 7207 0000 0029 09da 085f 5f6e  ....r....)...__n
+00000150: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000160: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000170: 0c64 6570 656e 6465 6e63 6965 7372 0300  .dependenciesr..
+00000180: 0000 da0a 416c 7465 7246 6965 6c64 7204  ....AlterFieldr.
+00000190: 0000 00da 0c42 6f6f 6c65 616e 4669 656c  .....BooleanFiel
+000001a0: 64da 0a6f 7065 7261 7469 6f6e 73a9 0072  d..operations..r
+000001b0: 1500 0000 7215 0000 00fa 632f 686f 6d65  ....r.....c/home
+000001c0: 2f63 616d 6572 6f6e 2f44 6576 2f6b 616e  /cameron/Dev/kan
+000001d0: 6261 6e2d 6465 762f 646a 616e 676f 2d63  ban-dev/django-c
+000001e0: 6f6e 6e65 6374 7769 7365 2f64 6a63 6f6e  onnectwise/djcon
+000001f0: 6e65 6374 7769 7365 2f6d 6967 7261 7469  nectwise/migrati
+00000200: 6f6e 732f 3030 3032 5f61 7574 6f5f 3230  ons/0002_auto_20
+00000210: 3137 3032 3233 5f32 3134 332e 7079 7205  170223_2143.pyr.
+00000220: 0000 0007 0000 0073 0a00 0000 0803 0604  .......s........
+00000230: 0401 0201 0201 7205 0000 004e 2906 da0a  ......r....N)...
+00000240: 5f5f 6675 7475 7265 5f5f 7202 0000 00da  __future__r.....
+00000250: 0964 6a61 6e67 6f2e 6462 7203 0000 0072  .django.dbr....r
+00000260: 0400 0000 7205 0000 0072 1500 0000 7215  ....r....r....r.
+00000270: 0000 0072 1500 0000 7216 0000 00da 083c  ...r....r......<
+00000280: 6d6f 6475 6c65 3e02 0000 0073 0400 0000  module>....s....
+00000290: 0c02 1003                                ....
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0042_auto_20171115_1131.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0042_auto_20171115_1131.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,40 @@
-00000000: 160d 0d0a a4b0 1f5d cd01 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c cd01 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0006 0000 0040 0000 0073  ...........@...s
-000000b0: 4900 0000 6500 005a 0100 6400 005a 0200  I...e..Z..d..Z..
-000000c0: 6409 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0083 0002 6504  ..d..d..d.....e.
-000000e0: 006a 0500 6403 0064 0400 6405 0064 0700  .j..d..d..d..d..
-000000f0: 8300 0267 0200 5a06 0064 0800 5329 0ada  ...g..Z..d..S)..
-00000100: 094d 6967 7261 7469 6f6e da0d 646a 636f  .Migration..djco
-00000110: 6e6e 6563 7477 6973 65da 1730 3034 315f  nnectwise..0041_
-00000120: 6175 746f 5f32 3031 3731 3033 305f 3130  auto_20171030_10
-00000130: 3437 da0a 6d6f 6465 6c5f 6e61 6d65 da06  47..model_name..
-00000140: 7469 636b 6574 da04 6e61 6d65 5a08 6170  ticket..nameZ.ap
-00000150: 695f 7465 7874 da04 7479 7065 4e29 027a  i_text..typeN).z
-00000160: 0d64 6a63 6f6e 6e65 6374 7769 7365 7a17  .djconnectwisez.
-00000170: 3030 3431 5f61 7574 6f5f 3230 3137 3130  0041_auto_201710
-00000180: 3330 5f31 3034 3729 07da 085f 5f6e 616d  30_1047)...__nam
-00000190: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-000001a0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
-000001b0: 6570 656e 6465 6e63 6965 7372 0300 0000  ependenciesr....
-000001c0: da0b 5265 6d6f 7665 4669 656c 64da 0a6f  ..RemoveField..o
-000001d0: 7065 7261 7469 6f6e 73a9 0072 1200 0000  perations..r....
-000001e0: 7212 0000 00fa 6e2f 686f 6d65 2f73 616d  r.....n/home/sam
-000001f0: 2f67 6974 2f4b 616e 6261 6e2f 646a 616e  /git/Kanban/djan
-00000200: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
-00000210: 6a61 6e67 6f2d 636f 6e6e 6563 7477 6973  jango-connectwis
-00000220: 652f 646a 636f 6e6e 6563 7477 6973 652f  e/djconnectwise/
-00000230: 6d69 6772 6174 696f 6e73 2f30 3034 325f  migrations/0042_
-00000240: 6175 746f 5f32 3031 3731 3131 355f 3131  auto_20171115_11
-00000250: 3331 2e70 7972 0500 0000 0700 0000 730e  31.pyr........s.
-00000260: 0000 000c 0309 0409 0106 0106 0209 0106  ................
-00000270: 0172 0500 0000 4e29 06da 0a5f 5f66 7574  .r....N)...__fut
-00000280: 7572 655f 5f72 0200 0000 da09 646a 616e  ure__r......djan
-00000290: 676f 2e64 6272 0300 0000 7204 0000 0072  go.dbr....r....r
-000002a0: 0500 0000 7212 0000 0072 1200 0000 7212  ....r....r....r.
-000002b0: 0000 0072 1300 0000 da08 3c6d 6f64 756c  ...r......<modul
-000002c0: 653e 0200 0000 7304 0000 0010 0216 03    e>....s........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0500 0000 4000 0000 732e  ..........@...s.
+000000a0: 0000 0065 005a 0164 005a 0264 0867 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0464 058d 0265 046a  .e.j.d.d.d...e.j
+000000c0: 0564 0364 0664 058d 0267 025a 0664 0753  .d.d.d...g.Z.d.S
+000000d0: 0029 09da 094d 6967 7261 7469 6f6e da0d  .)...Migration..
+000000e0: 646a 636f 6e6e 6563 7477 6973 65da 1730  djconnectwise..0
+000000f0: 3034 315f 6175 746f 5f32 3031 3731 3033  041_auto_2017103
+00000100: 305f 3130 3437 da06 7469 636b 6574 da08  0_1047..ticket..
+00000110: 6170 695f 7465 7874 2902 da0a 6d6f 6465  api_text)...mode
+00000120: 6c5f 6e61 6d65 da04 6e61 6d65 da04 7479  l_name..name..ty
+00000130: 7065 4e29 0272 0600 0000 7207 0000 0029  peN).r....r....)
+00000140: 07da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000150: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000160: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
+00000170: 6965 7372 0300 0000 da0b 5265 6d6f 7665  iesr......Remove
+00000180: 4669 656c 64da 0a6f 7065 7261 7469 6f6e  Field..operation
+00000190: 73a9 0072 1300 0000 7213 0000 00fa 632f  s..r....r.....c/
+000001a0: 686f 6d65 2f63 616d 6572 6f6e 2f44 6576  home/cameron/Dev
+000001b0: 2f6b 616e 6261 6e2d 6465 762f 646a 616e  /kanban-dev/djan
+000001c0: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
+000001d0: 6a63 6f6e 6e65 6374 7769 7365 2f6d 6967  jconnectwise/mig
+000001e0: 7261 7469 6f6e 732f 3030 3432 5f61 7574  rations/0042_aut
+000001f0: 6f5f 3230 3137 3131 3135 5f31 3133 312e  o_20171115_1131.
+00000200: 7079 7205 0000 0007 0000 0073 0e00 0000  pyr........s....
+00000210: 0803 0604 0401 0201 0602 0401 0201 7205  ..............r.
+00000220: 0000 004e 2906 da0a 5f5f 6675 7475 7265  ...N)...__future
+00000230: 5f5f 7202 0000 00da 0964 6a61 6e67 6f2e  __r......django.
+00000240: 6462 7203 0000 0072 0400 0000 7205 0000  dbr....r....r...
+00000250: 0072 1300 0000 7213 0000 0072 1300 0000  .r....r....r....
+00000260: 7214 0000 00da 083c 6d6f 6475 6c65 3e02  r......<module>.
+00000270: 0000 0073 0400 0000 0c02 1003            ...s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0002_auto_20170223_2143.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0057_auto_20180511_1440.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,42 @@
-00000000: 160d 0d0a a4b0 1f5d 9c01 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c a601 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0009 0000 0040 0000 0073  ...........@...s
-000000b0: 4600 0000 6500 005a 0100 6400 005a 0200  F...e..Z..d..Z..
-000000c0: 640b 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 6408 0064 0900 8300 0183 0003  .j..d..d........
-000000f0: 6701 005a 0800 640a 0053 290c da09 4d69  g..Z..d..S)...Mi
-00000100: 6772 6174 696f 6eda 0d64 6a63 6f6e 6e65  gration..djconne
-00000110: 6374 7769 7365 da0c 3030 3031 5f69 6e69  ctwise..0001_ini
-00000120: 7469 616c da0a 6d6f 6465 6c5f 6e61 6d65  tial..model_name
-00000130: da10 636f 6e6e 6563 7477 6973 6562 6f61  ..connectwiseboa
-00000140: 7264 da04 6e61 6d65 da08 696e 6163 7469  rd..name..inacti
-00000150: 7665 da05 6669 656c 64da 0764 6566 6175  ve..field..defau
-00000160: 6c74 464e 2902 7a0d 646a 636f 6e6e 6563  ltFN).z.djconnec
-00000170: 7477 6973 657a 0c30 3030 315f 696e 6974  twisez.0001_init
-00000180: 6961 6c29 09da 085f 5f6e 616d 655f 5fda  ial)...__name__.
-00000190: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000001a0: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
-000001b0: 6465 6e63 6965 7372 0300 0000 da0a 416c  denciesr......Al
-000001c0: 7465 7246 6965 6c64 7204 0000 00da 0c42  terFieldr......B
-000001d0: 6f6f 6c65 616e 4669 656c 64da 0a6f 7065  ooleanField..ope
-000001e0: 7261 7469 6f6e 73a9 0072 1500 0000 7215  rations..r....r.
-000001f0: 0000 00fa 6e2f 686f 6d65 2f73 616d 2f67  ....n/home/sam/g
-00000200: 6974 2f4b 616e 6261 6e2f 646a 616e 676f  it/Kanban/django
-00000210: 2d63 6f6e 6e65 6374 7769 7365 2f64 6a61  -connectwise/dja
-00000220: 6e67 6f2d 636f 6e6e 6563 7477 6973 652f  ngo-connectwise/
-00000230: 646a 636f 6e6e 6563 7477 6973 652f 6d69  djconnectwise/mi
-00000240: 6772 6174 696f 6e73 2f30 3030 325f 6175  grations/0002_au
-00000250: 746f 5f32 3031 3730 3232 335f 3231 3433  to_20170223_2143
-00000260: 2e70 7972 0500 0000 0700 0000 730a 0000  .pyr........s...
-00000270: 000c 0309 0409 0106 0106 0172 0500 0000  ...........r....
-00000280: 4e29 06da 0a5f 5f66 7574 7572 655f 5f72  N)...__future__r
-00000290: 0200 0000 da09 646a 616e 676f 2e64 6272  ......django.dbr
-000002a0: 0300 0000 7204 0000 0072 0500 0000 7215  ....r....r....r.
-000002b0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-000002c0: 0000 da08 3c6d 6f64 756c 653e 0200 0000  ....<module>....
-000002d0: 7304 0000 0010 0216 03                   s........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0600 0000 4000 0000 732c  ..........@...s,
+000000a0: 0000 0065 005a 0164 005a 0264 0967 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000c0: 068d 0164 078d 0367 015a 0864 0853 0029  ...d...g.Z.d.S.)
+000000d0: 0ada 094d 6967 7261 7469 6f6e da0d 646a  ...Migration..dj
+000000e0: 636f 6e6e 6563 7477 6973 65da 1730 3035  connectwise..005
+000000f0: 365f 6175 746f 5f32 3031 3830 3530 345f  6_auto_20180504_
+00000100: 3037 3434 da0b 6f70 706f 7274 756e 6974  0744..opportunit
+00000110: 79da 1062 7573 696e 6573 735f 756e 6974  y..business_unit
+00000120: 5f69 6454 2901 da04 6e75 6c6c 2903 da0a  _idT)...null)...
+00000130: 6d6f 6465 6c5f 6e61 6d65 da04 6e61 6d65  model_name..name
+00000140: da05 6669 656c 644e 2902 7206 0000 0072  ..fieldN).r....r
+00000150: 0700 0000 2909 da08 5f5f 6e61 6d65 5f5f  ....)...__name__
+00000160: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000170: 7175 616c 6e61 6d65 5f5f da0c 6465 7065  qualname__..depe
+00000180: 6e64 656e 6369 6573 7203 0000 00da 0a41  ndenciesr......A
+00000190: 6c74 6572 4669 656c 6472 0400 0000 da0c  lterFieldr......
+000001a0: 496e 7465 6765 7246 6965 6c64 da0a 6f70  IntegerField..op
+000001b0: 6572 6174 696f 6e73 a900 7215 0000 0072  erations..r....r
+000001c0: 1500 0000 fa63 2f68 6f6d 652f 6361 6d65  .....c/home/came
+000001d0: 726f 6e2f 4465 762f 6b61 6e62 616e 2d64  ron/Dev/kanban-d
+000001e0: 6576 2f64 6a61 6e67 6f2d 636f 6e6e 6563  ev/django-connec
+000001f0: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
+00000200: 6973 652f 6d69 6772 6174 696f 6e73 2f30  ise/migrations/0
+00000210: 3035 375f 6175 746f 5f32 3031 3830 3531  057_auto_2018051
+00000220: 315f 3134 3430 2e70 7972 0500 0000 0700  1_1440.pyr......
+00000230: 0000 730a 0000 0008 0306 0404 0102 0102  ..s.............
+00000240: 0172 0500 0000 4e29 06da 0a5f 5f66 7574  .r....N)...__fut
+00000250: 7572 655f 5f72 0200 0000 da09 646a 616e  ure__r......djan
+00000260: 676f 2e64 6272 0300 0000 7204 0000 0072  go.dbr....r....r
+00000270: 0500 0000 7215 0000 0072 1500 0000 7215  ....r....r....r.
+00000280: 0000 0072 1600 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000290: 653e 0200 0000 7304 0000 000c 0210 03    e>....s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0086_merge_20190507_1402.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0086_merge_20190507_1402.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,33 @@
-00000000: 160d 0d0a a4b0 1f5d 1b01 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c 1b01 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
-00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
-00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
-00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
-00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
-00000070: 0000 0000 0003 0000 0040 0000 0073 2200  .........@...s".
-00000080: 0000 6500 005a 0100 6400 005a 0200 6405  ..e..Z..d..Z..d.
-00000090: 0064 0600 6702 005a 0300 6700 005a 0400  .d..g..Z..g..Z..
-000000a0: 6404 0053 2907 da09 4d69 6772 6174 696f  d..S)...Migratio
-000000b0: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
-000000c0: da17 3030 3835 5f61 7574 6f5f 3230 3139  ..0085_auto_2019
-000000d0: 3035 3036 5f31 3032 38da 1730 3038 355f  0506_1028..0085_
-000000e0: 6175 746f 5f32 3031 3930 3433 305f 3130  auto_20190430_10
-000000f0: 3034 4e29 02fa 0d64 6a63 6f6e 6e65 6374  04N)...djconnect
-00000100: 7769 7365 7a17 3030 3835 5f61 7574 6f5f  wisez.0085_auto_
-00000110: 3230 3139 3035 3036 5f31 3032 3829 0272  20190506_1028).r
-00000120: 0700 0000 7a17 3030 3835 5f61 7574 6f5f  ....z.0085_auto_
-00000130: 3230 3139 3034 3330 5f31 3030 3429 05da  20190430_1004)..
-00000140: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000150: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000160: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
-00000170: 73da 0a6f 7065 7261 7469 6f6e 73a9 0072  s..operations..r
-00000180: 0d00 0000 720d 0000 00fa 6f2f 686f 6d65  ....r.....o/home
-00000190: 2f73 616d 2f67 6974 2f4b 616e 6261 6e2f  /sam/git/Kanban/
-000001a0: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
-000001b0: 7365 2f64 6a61 6e67 6f2d 636f 6e6e 6563  se/django-connec
-000001c0: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
-000001d0: 6973 652f 6d69 6772 6174 696f 6e73 2f30  ise/migrations/0
-000001e0: 3038 365f 6d65 7267 655f 3230 3139 3035  086_merge_201905
-000001f0: 3037 5f31 3430 322e 7079 7203 0000 0006  07_1402.pyr.....
-00000200: 0000 0073 0600 0000 0c03 0301 0903 7203  ...s..........r.
-00000210: 0000 004e 2903 da09 646a 616e 676f 2e64  ...N)...django.d
-00000220: 6272 0200 0000 7203 0000 0072 0d00 0000  br....r....r....
-00000230: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
-00000240: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
-00000250: 0000 1003                                ....
+00000020: 0073 2200 0000 6400 6401 6c00 6d01 5a01  .s"...d.d.l.m.Z.
+00000030: 0100 4700 6402 6403 8400 6403 6501 6a02  ..G.d.d...d.e.j.
+00000040: 8303 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
+00000050: 01da 0a6d 6967 7261 7469 6f6e 7363 0000  ...migrationsc..
+00000060: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+00000070: 0000 7318 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00000080: 0564 0667 025a 0367 005a 0464 0453 0029  .d.g.Z.g.Z.d.S.)
+00000090: 07da 094d 6967 7261 7469 6f6e da0d 646a  ...Migration..dj
+000000a0: 636f 6e6e 6563 7477 6973 65da 1730 3038  connectwise..008
+000000b0: 355f 6175 746f 5f32 3031 3930 3530 365f  5_auto_20190506_
+000000c0: 3130 3238 da17 3030 3835 5f61 7574 6f5f  1028..0085_auto_
+000000d0: 3230 3139 3034 3330 5f31 3030 344e 2902  20190430_1004N).
+000000e0: 7204 0000 0072 0500 0000 2902 7204 0000  r....r....).r...
+000000f0: 0072 0600 0000 2905 da08 5f5f 6e61 6d65  .r....)...__name
+00000100: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000110: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
+00000120: 7065 6e64 656e 6369 6573 da0a 6f70 6572  pendencies..oper
+00000130: 6174 696f 6e73 a900 720c 0000 0072 0c00  ations..r....r..
+00000140: 0000 fa64 2f68 6f6d 652f 6361 6d65 726f  ...d/home/camero
+00000150: 6e2f 4465 762f 6b61 6e62 616e 2d64 6576  n/Dev/kanban-dev
+00000160: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
+00000170: 6973 652f 646a 636f 6e6e 6563 7477 6973  ise/djconnectwis
+00000180: 652f 6d69 6772 6174 696f 6e73 2f30 3038  e/migrations/008
+00000190: 365f 6d65 7267 655f 3230 3139 3035 3037  6_merge_20190507
+000001a0: 5f31 3430 322e 7079 7203 0000 0006 0000  _1402.pyr.......
+000001b0: 0073 0600 0000 0803 0201 0603 7203 0000  .s..........r...
+000001c0: 004e 2903 da09 646a 616e 676f 2e64 6272  .N)...django.dbr
+000001d0: 0200 0000 7203 0000 0072 0c00 0000 720c  ....r....r....r.
+000001e0: 0000 0072 0c00 0000 720d 0000 00da 083c  ...r....r......<
+000001f0: 6d6f 6475 6c65 3e03 0000 0073 0200 0000  module>....s....
+00000200: 0c03                                     ..
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0029_merge.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0029_merge.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-00000000: 160d 0d0a a4b0 1f5d 3201 0000 e300 0000  .......]2.......
+00000000: 330d 0d0a 10ec da5c 3201 0000 e300 0000  3......\2.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000000b0: 2200 0000 6500 005a 0100 6400 005a 0200  "...e..Z..d..Z..
-000000c0: 6405 0064 0600 6702 005a 0300 6700 005a  d..d..g..Z..g..Z
-000000d0: 0400 6404 0053 2907 da09 4d69 6772 6174  ..d..S)...Migrat
-000000e0: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-000000f0: 7365 da21 3030 3238 5f72 656d 6f76 655f  se.!0028_remove_
-00000100: 636f 6d70 616e 795f 636f 6d70 616e 795f  company_company_
-00000110: 616c 6961 73da 0a30 3032 385f 6d65 7267  alias..0028_merg
-00000120: 654e 2902 fa0d 646a 636f 6e6e 6563 7477  eN)...djconnectw
-00000130: 6973 657a 2130 3032 385f 7265 6d6f 7665  isez!0028_remove
-00000140: 5f63 6f6d 7061 6e79 5f63 6f6d 7061 6e79  _company_company
-00000150: 5f61 6c69 6173 2902 7209 0000 007a 0a30  _alias).r....z.0
-00000160: 3032 385f 6d65 7267 6529 05da 085f 5f6e  028_merge)...__n
-00000170: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000180: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000190: 0c64 6570 656e 6465 6e63 6965 73da 0a6f  .dependencies..o
-000001a0: 7065 7261 7469 6f6e 73a9 0072 0f00 0000  perations..r....
-000001b0: 720f 0000 00fa 612f 686f 6d65 2f73 616d  r.....a/home/sam
-000001c0: 2f67 6974 2f4b 616e 6261 6e2f 646a 616e  /git/Kanban/djan
-000001d0: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
-000001e0: 6a61 6e67 6f2d 636f 6e6e 6563 7477 6973  jango-connectwis
-000001f0: 652f 646a 636f 6e6e 6563 7477 6973 652f  e/djconnectwise/
-00000200: 6d69 6772 6174 696f 6e73 2f30 3032 395f  migrations/0029_
-00000210: 6d65 7267 652e 7079 7205 0000 0007 0000  merge.pyr.......
-00000220: 0073 0600 0000 0c03 0301 0903 7205 0000  .s..........r...
-00000230: 004e 2906 da0a 5f5f 6675 7475 7265 5f5f  .N)...__future__
-00000240: 7202 0000 00da 0964 6a61 6e67 6f2e 6462  r......django.db
-00000250: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
-00000260: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-00000270: 0000 00da 083c 6d6f 6475 6c65 3e02 0000  .....<module>...
-00000280: 0073 0400 0000 1002 1603                 .s........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0300 0000 4000 0000 7318  ..........@...s.
+000000a0: 0000 0065 005a 0164 005a 0264 0564 0667  ...e.Z.d.Z.d.d.g
+000000b0: 025a 0367 005a 0464 0453 0029 07da 094d  .Z.g.Z.d.S.)...M
+000000c0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
+000000d0: 6563 7477 6973 65da 2130 3032 385f 7265  ectwise.!0028_re
+000000e0: 6d6f 7665 5f63 6f6d 7061 6e79 5f63 6f6d  move_company_com
+000000f0: 7061 6e79 5f61 6c69 6173 da0a 3030 3238  pany_alias..0028
+00000100: 5f6d 6572 6765 4e29 0272 0600 0000 7207  _mergeN).r....r.
+00000110: 0000 0029 0272 0600 0000 7208 0000 0029  ...).r....r....)
+00000120: 05da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000130: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000140: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
+00000150: 6965 73da 0a6f 7065 7261 7469 6f6e 73a9  ies..operations.
+00000160: 0072 0e00 0000 720e 0000 00fa 562f 686f  .r....r.....V/ho
+00000170: 6d65 2f63 616d 6572 6f6e 2f44 6576 2f6b  me/cameron/Dev/k
+00000180: 616e 6261 6e2d 6465 762f 646a 616e 676f  anban-dev/django
+00000190: 2d63 6f6e 6e65 6374 7769 7365 2f64 6a63  -connectwise/djc
+000001a0: 6f6e 6e65 6374 7769 7365 2f6d 6967 7261  onnectwise/migra
+000001b0: 7469 6f6e 732f 3030 3239 5f6d 6572 6765  tions/0029_merge
+000001c0: 2e70 7972 0500 0000 0700 0000 7306 0000  .pyr........s...
+000001d0: 0008 0302 0106 0372 0500 0000 4e29 06da  .......r....N)..
+000001e0: 0a5f 5f66 7574 7572 655f 5f72 0200 0000  .__future__r....
+000001f0: da09 646a 616e 676f 2e64 6272 0300 0000  ..django.dbr....
+00000200: 7204 0000 0072 0500 0000 720e 0000 0072  r....r....r....r
+00000210: 0e00 0000 720e 0000 0072 0f00 0000 da08  ....r....r......
+00000220: 3c6d 6f64 756c 653e 0200 0000 7304 0000  <module>....s...
+00000230: 000c 0210 03                             .....
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0113_auto_20200204_1054.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0080_auto_20181210_0930.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,39 @@
-00000000: 160d 0d0a 0660 3c5e 1202 0000 e300 0000  .....`<^........
+00000000: 330d 0d0a 10ec da5c 9401 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 0f00 0000 4000 0000 7364 0000 0065 0000  ....@...sd...e..
-000000a0: 5a01 0064 0000 5a02 0064 0f00 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6407 0065 0600 6a07 0064 0800  .d..d..e..j..d..
-000000d0: 6409 0064 0a00 6409 0064 0b00 6508 006a  d..d..d..d..e..j
-000000e0: 0900 6a06 006a 0a00 6a0b 0064 0c00 640d  ..j..j..j..d..d.
-000000f0: 0083 0004 8300 0367 0100 5a0c 0064 0e00  .......g..Z..d..
-00000100: 5329 10da 094d 6967 7261 7469 6f6e da0d  S)...Migration..
-00000110: 646a 636f 6e6e 6563 7477 6973 65da 1f30  djconnectwise..0
-00000120: 3131 325f 7379 6e63 6a6f 625f 7379 6e63  112_syncjob_sync
-00000130: 6872 6f6e 697a 6572 5f63 6c61 7373 da0a  hronizer_class..
-00000140: 6d6f 6465 6c5f 6e61 6d65 da0b 6f70 706f  model_name..oppo
-00000150: 7274 756e 6974 79da 046e 616d 65da 0573  rtunity..name..s
-00000160: 7461 6765 da05 6669 656c 64da 0562 6c61  tage..field..bla
-00000170: 6e6b 54da 046e 756c 6cda 096f 6e5f 6465  nkT..null..on_de
-00000180: 6c65 7465 da02 746f 7a1e 646a 636f 6e6e  lete..toz.djconn
-00000190: 6563 7477 6973 652e 4f70 706f 7274 756e  ectwise.Opportun
-000001a0: 6974 7953 7461 6765 4e29 027a 0d64 6a63  ityStageN).z.djc
-000001b0: 6f6e 6e65 6374 7769 7365 7206 0000 0029  onnectwiser....)
-000001c0: 0dda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000001d0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000001e0: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
-000001f0: 6965 7372 0200 0000 da0a 416c 7465 7246  iesr......AlterF
-00000200: 6965 6c64 7203 0000 00da 0a46 6f72 6569  ieldr......Forei
-00000210: 676e 4b65 79da 0664 6a61 6e67 6fda 0264  gnKey..django..d
-00000220: 62da 0864 656c 6574 696f 6eda 0853 4554  b..deletion..SET
-00000230: 5f4e 554c 4cda 0a6f 7065 7261 7469 6f6e  _NULL..operation
-00000240: 73a9 0072 1b00 0000 721b 0000 00fa 6e2f  s..r....r.....n/
-00000250: 686f 6d65 2f73 616d 2f67 6974 2f4b 616e  home/sam/git/Kan
-00000260: 6261 6e2f 646a 616e 676f 2d63 6f6e 6e65  ban/django-conne
-00000270: 6374 7769 7365 2f64 6a61 6e67 6f2d 636f  ctwise/django-co
-00000280: 6e6e 6563 7477 6973 652f 646a 636f 6e6e  nnectwise/djconn
-00000290: 6563 7477 6973 652f 6d69 6772 6174 696f  ectwise/migratio
-000002a0: 6e73 2f30 3131 335f 6175 746f 5f32 3032  ns/0113_auto_202
-000002b0: 3030 3230 345f 3130 3534 2e70 7972 0400  00204_1054.pyr..
-000002c0: 0000 0700 0000 730a 0000 000c 0309 0409  ......s.........
-000002d0: 0106 0106 0172 0400 0000 2906 da09 646a  .....r....)...dj
-000002e0: 616e 676f 2e64 6272 0200 0000 7203 0000  ango.dbr....r...
-000002f0: 00da 1964 6a61 6e67 6f2e 6462 2e6d 6f64  ...django.db.mod
-00000300: 656c 732e 6465 6c65 7469 6f6e 7216 0000  els.deletionr...
-00000310: 0072 0400 0000 721b 0000 0072 1b00 0000  .r....r....r....
-00000320: 721b 0000 0072 1c00 0000 da08 3c6d 6f64  r....r......<mod
-00000330: 756c 653e 0300 0000 7304 0000 0016 010c  ule>....s.......
-00000340: 03                                       .
+00000020: 0073 2600 0000 6400 6401 6c00 6d01 5a01  .s&...d.d.l.m.Z.
+00000030: 6d02 5a02 0100 4700 6402 6403 8400 6403  m.Z...G.d.d...d.
+00000040: 6501 6a03 8303 5a03 6404 5300 2905 e900  e.j...Z.d.S.)...
+00000050: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
+00000060: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000070: 0000 0000 0000 0700 0000 4000 0000 732e  ..........@...s.
+00000080: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+00000090: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000a0: 0664 078d 0264 088d 0367 015a 0864 0953  .d...d...g.Z.d.S
+000000b0: 0029 0bda 094d 6967 7261 7469 6f6e da0d  .)...Migration..
+000000c0: 646a 636f 6e6e 6563 7477 6973 65da 1730  djconnectwise..0
+000000d0: 3037 395f 6175 746f 5f32 3031 3831 3230  079_auto_2018120
+000000e0: 335f 3136 3036 da06 6d65 6d62 6572 da09  3_1606..member..
+000000f0: 6c61 7374 5f6e 616d 65e9 1e00 0000 5429  last_name.....T)
+00000100: 02da 0a6d 6178 5f6c 656e 6774 68da 046e  ...max_length..n
+00000110: 756c 6c29 03da 0a6d 6f64 656c 5f6e 616d  ull)...model_nam
+00000120: 65da 046e 616d 65da 0566 6965 6c64 4e29  e..name..fieldN)
+00000130: 0272 0500 0000 7206 0000 0029 09da 085f  .r....r....)..._
+00000140: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000150: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000160: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
+00000170: 0200 0000 da0a 416c 7465 7246 6965 6c64  ......AlterField
+00000180: 7203 0000 00da 0943 6861 7246 6965 6c64  r......CharField
+00000190: da0a 6f70 6572 6174 696f 6e73 a900 7216  ..operations..r.
+000001a0: 0000 0072 1600 0000 fa63 2f68 6f6d 652f  ...r.....c/home/
+000001b0: 6361 6d65 726f 6e2f 4465 762f 6b61 6e62  cameron/Dev/kanb
+000001c0: 616e 2d64 6576 2f64 6a61 6e67 6f2d 636f  an-dev/django-co
+000001d0: 6e6e 6563 7477 6973 652f 646a 636f 6e6e  nnectwise/djconn
+000001e0: 6563 7477 6973 652f 6d69 6772 6174 696f  ectwise/migratio
+000001f0: 6e73 2f30 3038 305f 6175 746f 5f32 3031  ns/0080_auto_201
+00000200: 3831 3231 305f 3039 3330 2e70 7972 0400  81210_0930.pyr..
+00000210: 0000 0600 0000 730a 0000 0008 0306 0404  ......s.........
+00000220: 0102 0102 0172 0400 0000 4e29 04da 0964  .....r....N)...d
+00000230: 6a61 6e67 6f2e 6462 7202 0000 0072 0300  jango.dbr....r..
+00000240: 0000 7204 0000 0072 1600 0000 7216 0000  ..r....r....r...
+00000250: 0072 1600 0000 7217 0000 00da 083c 6d6f  .r....r......<mo
+00000260: 6475 6c65 3e03 0000 0073 0200 0000 1003  dule>....s......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0054_auto_20180501_1009.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0051_merge.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,35 @@
-00000000: 160d 0d0a a4b0 1f5d a101 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c 2c01 0000 e300 0000  3......\,.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0009 0000 0040 0000 0073  ...........@...s
-000000b0: 4000 0000 6500 005a 0100 6400 005a 0200  @...e..Z..d..Z..
-000000c0: 640c 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6408  ..d..d..d..d..d.
-000000e0: 0064 0d00 6902 0083 0002 6701 005a 0600  .d..i.....g..Z..
-000000f0: 640b 0053 290e da09 4d69 6772 6174 696f  d..S)...Migratio
-00000100: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
-00000110: da0a 3030 3533 5f6d 6572 6765 da04 6e61  ..0053_merge..na
-00000120: 6d65 da09 7469 6d65 656e 7472 79da 076f  me..timeentry..o
-00000130: 7074 696f 6e73 da13 7665 7262 6f73 655f  ptions..verbose_
-00000140: 6e61 6d65 5f70 6c75 7261 6c7a 0c54 696d  name_pluralz.Tim
-00000150: 6520 456e 7472 6965 73da 086f 7264 6572  e Entries..order
-00000160: 696e 67fa 0b2d 7469 6d65 5f73 7461 7274  ing..-time_start
-00000170: da02 6964 4e29 027a 0d64 6a63 6f6e 6e65  ..idN).z.djconne
-00000180: 6374 7769 7365 7a0a 3030 3533 5f6d 6572  ctwisez.0053_mer
-00000190: 6765 2902 720d 0000 007a 0269 6429 07da  ge).r....z.id)..
-000001a0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000001b0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000001c0: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
-000001d0: 7372 0300 0000 da11 416c 7465 724d 6f64  sr......AlterMod
-000001e0: 656c 4f70 7469 6f6e 73da 0a6f 7065 7261  elOptions..opera
-000001f0: 7469 6f6e 73a9 0072 1500 0000 7215 0000  tions..r....r...
-00000200: 00fa 6e2f 686f 6d65 2f73 616d 2f67 6974  ..n/home/sam/git
-00000210: 2f4b 616e 6261 6e2f 646a 616e 676f 2d63  /Kanban/django-c
-00000220: 6f6e 6e65 6374 7769 7365 2f64 6a61 6e67  onnectwise/djang
-00000230: 6f2d 636f 6e6e 6563 7477 6973 652f 646a  o-connectwise/dj
-00000240: 636f 6e6e 6563 7477 6973 652f 6d69 6772  connectwise/migr
-00000250: 6174 696f 6e73 2f30 3035 345f 6175 746f  ations/0054_auto
-00000260: 5f32 3031 3830 3530 315f 3130 3039 2e70  _20180501_1009.p
-00000270: 7972 0500 0000 0700 0000 7308 0000 000c  yr........s.....
-00000280: 0309 0409 0106 0172 0500 0000 4e29 06da  .......r....N)..
-00000290: 0a5f 5f66 7574 7572 655f 5f72 0200 0000  .__future__r....
-000002a0: da09 646a 616e 676f 2e64 6272 0300 0000  ..django.dbr....
-000002b0: 7204 0000 0072 0500 0000 7215 0000 0072  r....r....r....r
-000002c0: 1500 0000 7215 0000 0072 1600 0000 da08  ....r....r......
-000002d0: 3c6d 6f64 756c 653e 0200 0000 7304 0000  <module>....s...
-000002e0: 0010 0216 03                             .....
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0300 0000 4000 0000 7318  ..........@...s.
+000000a0: 0000 0065 005a 0164 005a 0264 0564 0667  ...e.Z.d.Z.d.d.g
+000000b0: 025a 0367 005a 0464 0453 0029 07da 094d  .Z.g.Z.d.S.)...M
+000000c0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
+000000d0: 6563 7477 6973 65da 1730 3035 305f 6175  ectwise..0050_au
+000000e0: 746f 5f32 3031 3830 3431 375f 3136 3230  to_20180417_1620
+000000f0: da0e 3030 3530 5f74 696d 6565 6e74 7279  ..0050_timeentry
+00000100: 4e29 0272 0600 0000 7207 0000 0029 0272  N).r....r....).r
+00000110: 0600 0000 7208 0000 0029 05da 085f 5f6e  ....r....)...__n
+00000120: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000130: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000140: 0c64 6570 656e 6465 6e63 6965 73da 0a6f  .dependencies..o
+00000150: 7065 7261 7469 6f6e 73a9 0072 0e00 0000  perations..r....
+00000160: 720e 0000 00fa 562f 686f 6d65 2f63 616d  r.....V/home/cam
+00000170: 6572 6f6e 2f44 6576 2f6b 616e 6261 6e2d  eron/Dev/kanban-
+00000180: 6465 762f 646a 616e 676f 2d63 6f6e 6e65  dev/django-conne
+00000190: 6374 7769 7365 2f64 6a63 6f6e 6e65 6374  ctwise/djconnect
+000001a0: 7769 7365 2f6d 6967 7261 7469 6f6e 732f  wise/migrations/
+000001b0: 3030 3531 5f6d 6572 6765 2e70 7972 0500  0051_merge.pyr..
+000001c0: 0000 0700 0000 7306 0000 0008 0302 0106  ......s.........
+000001d0: 0372 0500 0000 4e29 06da 0a5f 5f66 7574  .r....N)...__fut
+000001e0: 7572 655f 5f72 0200 0000 da09 646a 616e  ure__r......djan
+000001f0: 676f 2e64 6272 0300 0000 7204 0000 0072  go.dbr....r....r
+00000200: 0500 0000 720e 0000 0072 0e00 0000 720e  ....r....r....r.
+00000210: 0000 0072 0f00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000220: 653e 0200 0000 7304 0000 000c 0210 03    e>....s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0034_auto_20170727_1243.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0003_auto_20170223_2233.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,42 @@
-00000000: 160d 0d0a a4b0 1f5d a401 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c 9901 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 000b 0000 0040 0000 0073  ...........@...s
-000000b0: 4c00 0000 6500 005a 0100 6400 005a 0200  L...e..Z..d..Z..
-000000c0: 640c 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 6408 0064 0900 640a 0064 0900  .j..d..d..d..d..
-000000f0: 8300 0283 0003 6701 005a 0800 640b 0053  ......g..Z..d..S
-00000100: 290d da09 4d69 6772 6174 696f 6eda 0d64  )...Migration..d
-00000110: 6a63 6f6e 6e65 6374 7769 7365 da17 3030  jconnectwise..00
-00000120: 3333 5f61 7574 6f5f 3230 3137 3036 3136  33_auto_20170616
-00000130: 5f31 3235 31da 0a6d 6f64 656c 5f6e 616d  _1251..model_nam
-00000140: 65da 0b6f 7070 6f72 7475 6e69 7479 da04  e..opportunity..
-00000150: 6e61 6d65 da05 6e6f 7465 73da 0566 6965  name..notes..fie
-00000160: 6c64 da04 6e75 6c6c 54da 0562 6c61 6e6b  ld..nullT..blank
-00000170: 4e29 027a 0d64 6a63 6f6e 6e65 6374 7769  N).z.djconnectwi
-00000180: 7365 7a17 3030 3333 5f61 7574 6f5f 3230  sez.0033_auto_20
-00000190: 3137 3036 3136 5f31 3235 3129 09da 085f  170616_1251)..._
-000001a0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-000001b0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000001c0: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
-000001d0: 0300 0000 da0a 416c 7465 7246 6965 6c64  ......AlterField
-000001e0: 7204 0000 00da 0954 6578 7446 6965 6c64  r......TextField
-000001f0: da0a 6f70 6572 6174 696f 6e73 a900 7216  ..operations..r.
-00000200: 0000 0072 1600 0000 fa6e 2f68 6f6d 652f  ...r.....n/home/
-00000210: 7361 6d2f 6769 742f 4b61 6e62 616e 2f64  sam/git/Kanban/d
-00000220: 6a61 6e67 6f2d 636f 6e6e 6563 7477 6973  jango-connectwis
-00000230: 652f 646a 616e 676f 2d63 6f6e 6e65 6374  e/django-connect
-00000240: 7769 7365 2f64 6a63 6f6e 6e65 6374 7769  wise/djconnectwi
-00000250: 7365 2f6d 6967 7261 7469 6f6e 732f 3030  se/migrations/00
-00000260: 3334 5f61 7574 6f5f 3230 3137 3037 3237  34_auto_20170727
-00000270: 5f31 3234 332e 7079 7205 0000 0007 0000  _1243.pyr.......
-00000280: 0073 0a00 0000 0c03 0904 0901 0601 0601  .s..............
-00000290: 7205 0000 004e 2906 da0a 5f5f 6675 7475  r....N)...__futu
-000002a0: 7265 5f5f 7202 0000 00da 0964 6a61 6e67  re__r......djang
-000002b0: 6f2e 6462 7203 0000 0072 0400 0000 7205  o.dbr....r....r.
-000002c0: 0000 0072 1600 0000 7216 0000 0072 1600  ...r....r....r..
-000002d0: 0000 7217 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000002e0: 3e02 0000 0073 0400 0000 1002 1603       >....s........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0600 0000 4000 0000 7326  ..........@...s&
+000000a0: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0464 0b69 0164 088d  .e.j.d.d.d.i.d..
+000000c0: 0267 015a 0664 0953 0029 0cda 094d 6967  .g.Z.d.S.)...Mig
+000000d0: 7261 7469 6f6e da0d 646a 636f 6e6e 6563  ration..djconnec
+000000e0: 7477 6973 65da 1730 3030 325f 6175 746f  twise..0002_auto
+000000f0: 5f32 3031 3730 3232 335f 3231 3433 da0b  _20170223_2143..
+00000100: 626f 6172 6473 7461 7475 73da 086f 7264  boardstatus..ord
+00000110: 6572 696e 67da 0b62 6f61 7264 5f5f 6e61  ering..board__na
+00000120: 6d65 da0a 736f 7274 5f6f 7264 6572 da04  me..sort_order..
+00000130: 6e61 6d65 2902 720c 0000 00da 076f 7074  name).r......opt
+00000140: 696f 6e73 4e29 0272 0600 0000 7207 0000  ionsN).r....r...
+00000150: 0029 0372 0a00 0000 720b 0000 0072 0c00  .).r....r....r..
+00000160: 0000 2907 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+00000170: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000180: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
+00000190: 656e 6369 6573 7203 0000 00da 1141 6c74  enciesr......Alt
+000001a0: 6572 4d6f 6465 6c4f 7074 696f 6e73 da0a  erModelOptions..
+000001b0: 6f70 6572 6174 696f 6e73 a900 7214 0000  operations..r...
+000001c0: 0072 1400 0000 fa63 2f68 6f6d 652f 6361  .r.....c/home/ca
+000001d0: 6d65 726f 6e2f 4465 762f 6b61 6e62 616e  meron/Dev/kanban
+000001e0: 2d64 6576 2f64 6a61 6e67 6f2d 636f 6e6e  -dev/django-conn
+000001f0: 6563 7477 6973 652f 646a 636f 6e6e 6563  ectwise/djconnec
+00000200: 7477 6973 652f 6d69 6772 6174 696f 6e73  twise/migrations
+00000210: 2f30 3030 335f 6175 746f 5f32 3031 3730  /0003_auto_20170
+00000220: 3232 335f 3232 3333 2e70 7972 0500 0000  223_2233.pyr....
+00000230: 0700 0000 7308 0000 0008 0306 0404 0102  ....s...........
+00000240: 0172 0500 0000 4e29 06da 0a5f 5f66 7574  .r....N)...__fut
+00000250: 7572 655f 5f72 0200 0000 da09 646a 616e  ure__r......djan
+00000260: 676f 2e64 6272 0300 0000 7204 0000 0072  go.dbr....r....r
+00000270: 0500 0000 7214 0000 0072 1400 0000 7214  ....r....r....r.
+00000280: 0000 0072 1500 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000290: 653e 0200 0000 7304 0000 000c 0210 03    e>....s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0063_merge_20180611_0905.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0098_auto_20190718_1406.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,52 @@
-00000000: 160d 0d0a a4b0 1f5d 1b01 0000 e300 0000  .......]........
+00000000: 330d 0d0a 2a3e 545d 8d02 0000 e300 0000  3...*>T]........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
-00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
-00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
-00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
-00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
-00000070: 0000 0000 0003 0000 0040 0000 0073 2200  .........@...s".
-00000080: 0000 6500 005a 0100 6400 005a 0200 6405  ..e..Z..d..Z..d.
-00000090: 0064 0600 6702 005a 0300 6700 005a 0400  .d..g..Z..g..Z..
-000000a0: 6404 0053 2907 da09 4d69 6772 6174 696f  d..S)...Migratio
-000000b0: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
-000000c0: da17 3030 3631 5f61 7574 6f5f 3230 3138  ..0061_auto_2018
-000000d0: 3036 3037 5f31 3231 30da 1730 3036 325f  0607_1210..0062_
-000000e0: 6175 746f 5f32 3031 3830 3630 365f 3131  auto_20180606_11
-000000f0: 3137 4e29 02fa 0d64 6a63 6f6e 6e65 6374  17N)...djconnect
-00000100: 7769 7365 7a17 3030 3631 5f61 7574 6f5f  wisez.0061_auto_
-00000110: 3230 3138 3036 3037 5f31 3231 3029 0272  20180607_1210).r
-00000120: 0700 0000 7a17 3030 3632 5f61 7574 6f5f  ....z.0062_auto_
-00000130: 3230 3138 3036 3036 5f31 3131 3729 05da  20180606_1117)..
-00000140: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000150: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000160: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
-00000170: 73da 0a6f 7065 7261 7469 6f6e 73a9 0072  s..operations..r
-00000180: 0d00 0000 720d 0000 00fa 6f2f 686f 6d65  ....r.....o/home
-00000190: 2f73 616d 2f67 6974 2f4b 616e 6261 6e2f  /sam/git/Kanban/
-000001a0: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
-000001b0: 7365 2f64 6a61 6e67 6f2d 636f 6e6e 6563  se/django-connec
-000001c0: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
-000001d0: 6973 652f 6d69 6772 6174 696f 6e73 2f30  ise/migrations/0
-000001e0: 3036 335f 6d65 7267 655f 3230 3138 3036  063_merge_201806
-000001f0: 3131 5f30 3930 352e 7079 7203 0000 0006  11_0905.pyr.....
-00000200: 0000 0073 0600 0000 0c03 0301 0903 7203  ...s..........r.
-00000210: 0000 004e 2903 da09 646a 616e 676f 2e64  ...N)...django.d
-00000220: 6272 0200 0000 7203 0000 0072 0d00 0000  br....r....r....
-00000230: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
-00000240: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
-00000250: 0000 1003                                ....
+00000020: 0073 2e00 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 4700  m.Z...d.d.l.Z.G.
+00000040: 6403 6404 8400 6404 6501 6a05 8303 5a05  d.d...d.e.j...Z.
+00000050: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 734e 6300 0000 0000 0000 0000 0000 000b  sNc.............
+00000080: 0000 0040 0000 0073 4800 0000 6500 5a01  ...@...sH...e.Z.
+00000090: 6400 5a02 640d 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000a0: 6404 6405 8d02 6504 6a06 6403 6406 6507  d.d...e.j.d.d.e.
+000000b0: 6a08 6407 6407 6509 6a0a 6a07 6a0b 6a0c  j.d.d.e.j.j.j.j.
+000000c0: 6408 6409 640a 8d05 640b 8d03 6702 5a0d  d.d.d...d...g.Z.
+000000d0: 640c 5300 290e da09 4d69 6772 6174 696f  d.S.)...Migratio
+000000e0: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
+000000f0: da18 3030 3937 5f6d 6572 6765 5f32 3031  ..0097_merge_201
+00000100: 3930 3731 385f 3133 3235 da06 7469 636b  90718_1325..tick
+00000110: 6574 da0c 6167 7265 656d 656e 745f 6964  et..agreement_id
+00000120: 2902 da0a 6d6f 6465 6c5f 6e61 6d65 da04  )...model_name..
+00000130: 6e61 6d65 da09 6167 7265 656d 656e 7454  name..agreementT
+00000140: da11 6167 7265 656d 656e 745f 7469 636b  ..agreement_tick
+00000150: 6574 737a 1764 6a63 6f6e 6e65 6374 7769  etsz.djconnectwi
+00000160: 7365 2e41 6772 6565 6d65 6e74 2905 da05  se.Agreement)...
+00000170: 626c 616e 6bda 046e 756c 6cda 096f 6e5f  blank..null..on_
+00000180: 6465 6c65 7465 da0c 7265 6c61 7465 645f  delete..related_
+00000190: 6e61 6d65 da02 746f 2903 7209 0000 0072  name..to).r....r
+000001a0: 0a00 0000 da05 6669 656c 644e 2902 7205  ......fieldN).r.
+000001b0: 0000 0072 0600 0000 290e da08 5f5f 6e61  ...r....)...__na
+000001c0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+000001d0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
+000001e0: 6465 7065 6e64 656e 6369 6573 7202 0000  dependenciesr...
+000001f0: 00da 0b52 656d 6f76 6546 6965 6c64 da08  ...RemoveField..
+00000200: 4164 6446 6965 6c64 7203 0000 00da 0a46  AddFieldr......F
+00000210: 6f72 6569 676e 4b65 79da 0664 6a61 6e67  oreignKey..djang
+00000220: 6fda 0264 62da 0864 656c 6574 696f 6eda  o..db..deletion.
+00000230: 0853 4554 5f4e 554c 4cda 0a6f 7065 7261  .SET_NULL..opera
+00000240: 7469 6f6e 73a9 0072 1f00 0000 721f 0000  tions..r....r...
+00000250: 00fa 632f 686f 6d65 2f63 616d 6572 6f6e  ..c/home/cameron
+00000260: 2f44 6576 2f6b 616e 6261 6e2d 6465 762f  /Dev/kanban-dev/
+00000270: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
+00000280: 7365 2f64 6a63 6f6e 6e65 6374 7769 7365  se/djconnectwise
+00000290: 2f6d 6967 7261 7469 6f6e 732f 3030 3938  /migrations/0098
+000002a0: 5f61 7574 6f5f 3230 3139 3037 3138 5f31  _auto_20190718_1
+000002b0: 3430 362e 7079 7204 0000 0007 0000 0073  406.pyr........s
+000002c0: 1000 0000 0803 0604 0401 0201 0602 0401  ................
+000002d0: 0201 0201 7204 0000 0029 06da 0964 6a61  ....r....)...dja
+000002e0: 6e67 6f2e 6462 7202 0000 0072 0300 0000  ngo.dbr....r....
+000002f0: da19 646a 616e 676f 2e64 622e 6d6f 6465  ..django.db.mode
+00000300: 6c73 2e64 656c 6574 696f 6e72 1a00 0000  ls.deletionr....
+00000310: 7204 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+00000320: 1f00 0000 7220 0000 00da 083c 6d6f 6475  ....r .....<modu
+00000330: 6c65 3e03 0000 0073 0400 0000 1001 0803  le>....s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0068_merge_20180814_1104.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0021_merge.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-00000000: 160d 0d0a a4b0 1f5d 1b01 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c 2d01 0000 e300 0000  3......\-.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
-00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
-00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
-00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
-00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
-00000070: 0000 0000 0003 0000 0040 0000 0073 2200  .........@...s".
-00000080: 0000 6500 005a 0100 6400 005a 0200 6405  ..e..Z..d..Z..d.
-00000090: 0064 0600 6702 005a 0300 6700 005a 0400  .d..g..Z..g..Z..
-000000a0: 6404 0053 2907 da09 4d69 6772 6174 696f  d..S)...Migratio
-000000b0: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
-000000c0: da17 3030 3637 5f61 7574 6f5f 3230 3138  ..0067_auto_2018
-000000d0: 3038 3133 5f31 3335 35da 1730 3036 365f  0813_1355..0066_
-000000e0: 6175 746f 5f32 3031 3830 3831 345f 3130  auto_20180814_10
-000000f0: 3436 4e29 02fa 0d64 6a63 6f6e 6e65 6374  46N)...djconnect
-00000100: 7769 7365 7205 0000 0029 0272 0700 0000  wiser....).r....
-00000110: 7206 0000 0029 05da 085f 5f6e 616d 655f  r....)...__name_
-00000120: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000130: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
-00000140: 656e 6465 6e63 6965 73da 0a6f 7065 7261  endencies..opera
-00000150: 7469 6f6e 73a9 0072 0d00 0000 720d 0000  tions..r....r...
-00000160: 00fa 6f2f 686f 6d65 2f73 616d 2f67 6974  ..o/home/sam/git
-00000170: 2f4b 616e 6261 6e2f 646a 616e 676f 2d63  /Kanban/django-c
-00000180: 6f6e 6e65 6374 7769 7365 2f64 6a61 6e67  onnectwise/djang
-00000190: 6f2d 636f 6e6e 6563 7477 6973 652f 646a  o-connectwise/dj
-000001a0: 636f 6e6e 6563 7477 6973 652f 6d69 6772  connectwise/migr
-000001b0: 6174 696f 6e73 2f30 3036 385f 6d65 7267  ations/0068_merg
-000001c0: 655f 3230 3138 3038 3134 5f31 3130 342e  e_20180814_1104.
-000001d0: 7079 7203 0000 0006 0000 0073 0600 0000  pyr........s....
-000001e0: 0c03 0301 0903 7203 0000 004e 2903 da09  ......r....N)...
-000001f0: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
-00000200: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
-00000210: 0000 720e 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000220: 3e03 0000 0073 0200 0000 1003            >....s......
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0300 0000 4000 0000 7318  ..........@...s.
+000000a0: 0000 0065 005a 0164 005a 0264 0564 0667  ...e.Z.d.Z.d.d.g
+000000b0: 025a 0367 005a 0464 0453 0029 07da 094d  .Z.g.Z.d.S.)...M
+000000c0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
+000000d0: 6563 7477 6973 65da 0a30 3032 305f 6d65  ectwise..0020_me
+000000e0: 7267 65da 1c30 3032 305f 7469 636b 6574  rge..0020_ticket
+000000f0: 5f63 7573 746f 6d65 725f 7570 6461 7465  _customer_update
+00000100: 644e 2902 7206 0000 0072 0700 0000 2902  dN).r....r....).
+00000110: 7206 0000 0072 0800 0000 2905 da08 5f5f  r....r....)...__
+00000120: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000130: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000140: da0c 6465 7065 6e64 656e 6369 6573 da0a  ..dependencies..
+00000150: 6f70 6572 6174 696f 6e73 a900 720e 0000  operations..r...
+00000160: 0072 0e00 0000 fa56 2f68 6f6d 652f 6361  .r.....V/home/ca
+00000170: 6d65 726f 6e2f 4465 762f 6b61 6e62 616e  meron/Dev/kanban
+00000180: 2d64 6576 2f64 6a61 6e67 6f2d 636f 6e6e  -dev/django-conn
+00000190: 6563 7477 6973 652f 646a 636f 6e6e 6563  ectwise/djconnec
+000001a0: 7477 6973 652f 6d69 6772 6174 696f 6e73  twise/migrations
+000001b0: 2f30 3032 315f 6d65 7267 652e 7079 7205  /0021_merge.pyr.
+000001c0: 0000 0007 0000 0073 0600 0000 0803 0201  .......s........
+000001d0: 0603 7205 0000 004e 2906 da0a 5f5f 6675  ..r....N)...__fu
+000001e0: 7475 7265 5f5f 7202 0000 00da 0964 6a61  ture__r......dja
+000001f0: 6e67 6f2e 6462 7203 0000 0072 0400 0000  ngo.dbr....r....
+00000200: 7205 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000210: 0e00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
+00000220: 6c65 3e02 0000 0073 0400 0000 0c02 1003  le>....s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0037_auto_20170920_0959.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0034_auto_20170727_1243.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,42 @@
-00000000: 160d 0d0a a4b0 1f5d 3d03 0000 e300 0000  .......]=.......
+00000000: 330d 0d0a 10ec da5c a401 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0012 0000 0040 0000 0073  ...........@...s
-000000b0: 9d00 0000 6500 005a 0100 6400 005a 0200  ....e..Z..d..Z..
-000000c0: 6416 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6408  ..d..d..d..d..d.
-000000e0: 0083 0003 6504 006a 0600 6403 0064 0400  ....e..j..d..d..
-000000f0: 6409 0064 0a00 640b 0065 0700 6a08 0064  d..d..d..e..j..d
-00000100: 0c00 640d 0064 0e00 640f 0064 1000 6411  ..d..d..d..d..d.
-00000110: 0064 1200 6411 0064 1300 6507 006a 0900  .d..d..d..e..j..
-00000120: 8300 0583 0003 6504 006a 0600 6403 0064  ......e..j..d..d
-00000130: 0400 6409 0064 1400 640b 0065 0700 6a0a  ..d..d..d..e..j.
-00000140: 0083 0000 8300 0367 0300 5a0b 0064 1500  .......g..Z..d..
-00000150: 5329 17da 094d 6967 7261 7469 6f6e da0d  S)...Migration..
-00000160: 646a 636f 6e6e 6563 7477 6973 65da 1730  djconnectwise..0
-00000170: 3033 365f 6175 746f 5f32 3031 3730 3832  036_auto_2017082
-00000180: 335f 3134 3137 da0a 6d6f 6465 6c5f 6e61  3_1417..model_na
-00000190: 6d65 da0b 6f70 706f 7274 756e 6974 79da  me..opportunity.
-000001a0: 086f 6c64 5f6e 616d 65da 0474 7970 65da  .old_name..type.
-000001b0: 086e 6577 5f6e 616d 65da 106f 7070 6f72  .new_name..oppor
-000001c0: 7475 6e69 7479 5f74 7970 65da 046e 616d  tunity_type..nam
-000001d0: 65da 0763 6f6d 7061 6e79 da05 6669 656c  e..company..fiel
-000001e0: 64da 0274 6f7a 1564 6a63 6f6e 6e65 6374  d..toz.djconnect
-000001f0: 7769 7365 2e43 6f6d 7061 6e79 da0c 7265  wise.Company..re
-00000200: 6c61 7465 645f 6e61 6d65 da15 636f 6d70  lated_name..comp
-00000210: 616e 795f 6f70 706f 7274 756e 6974 6965  any_opportunitie
-00000220: 73da 046e 756c 6c54 da05 626c 616e 6bda  s..nullT..blank.
-00000230: 096f 6e5f 6465 6c65 7465 da13 6578 7065  .on_delete..expe
-00000240: 6374 6564 5f63 6c6f 7365 5f64 6174 654e  cted_close_dateN
-00000250: 2902 7a0d 646a 636f 6e6e 6563 7477 6973  ).z.djconnectwis
-00000260: 657a 1730 3033 365f 6175 746f 5f32 3031  ez.0036_auto_201
-00000270: 3730 3832 335f 3134 3137 290c da08 5f5f  70823_1417)...__
-00000280: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000290: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-000002a0: da0c 6465 7065 6e64 656e 6369 6573 7203  ..dependenciesr.
-000002b0: 0000 00da 0b52 656e 616d 6546 6965 6c64  .....RenameField
-000002c0: da0a 416c 7465 7246 6965 6c64 7204 0000  ..AlterFieldr...
-000002d0: 00da 0a46 6f72 6569 676e 4b65 79da 0853  ...ForeignKey..S
-000002e0: 4554 5f4e 554c 4cda 0d44 6174 6554 696d  ET_NULL..DateTim
-000002f0: 6546 6965 6c64 da0a 6f70 6572 6174 696f  eField..operatio
-00000300: 6e73 a900 7222 0000 0072 2200 0000 fa6e  ns..r"...r"....n
-00000310: 2f68 6f6d 652f 7361 6d2f 6769 742f 4b61  /home/sam/git/Ka
-00000320: 6e62 616e 2f64 6a61 6e67 6f2d 636f 6e6e  nban/django-conn
-00000330: 6563 7477 6973 652f 646a 616e 676f 2d63  ectwise/django-c
-00000340: 6f6e 6e65 6374 7769 7365 2f64 6a63 6f6e  onnectwise/djcon
-00000350: 6e65 6374 7769 7365 2f6d 6967 7261 7469  nectwise/migrati
-00000360: 6f6e 732f 3030 3337 5f61 7574 6f5f 3230  ons/0037_auto_20
-00000370: 3137 3039 3230 5f30 3935 392e 7079 7205  170920_0959.pyr.
-00000380: 0000 0007 0000 0073 1a00 0000 0c03 0904  .......s........
-00000390: 0901 0601 0601 0602 0901 0601 0601 2d02  ..............-.
-000003a0: 0901 0601 0601 7205 0000 004e 2906 da0a  ......r....N)...
-000003b0: 5f5f 6675 7475 7265 5f5f 7202 0000 00da  __future__r.....
-000003c0: 0964 6a61 6e67 6f2e 6462 7203 0000 0072  .django.dbr....r
-000003d0: 0400 0000 7205 0000 0072 2200 0000 7222  ....r....r"...r"
-000003e0: 0000 0072 2200 0000 7223 0000 00da 083c  ...r"...r#.....<
-000003f0: 6d6f 6475 6c65 3e02 0000 0073 0400 0000  module>....s....
-00000400: 1002 1603                                ....
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0700 0000 4000 0000 732e  ..........@...s.
+000000a0: 0000 0065 005a 0164 005a 0264 0967 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000c0: 0564 068d 0264 078d 0367 015a 0864 0853  .d...d...g.Z.d.S
+000000d0: 0029 0ada 094d 6967 7261 7469 6f6e da0d  .)...Migration..
+000000e0: 646a 636f 6e6e 6563 7477 6973 65da 1730  djconnectwise..0
+000000f0: 3033 335f 6175 746f 5f32 3031 3730 3631  033_auto_2017061
+00000100: 365f 3132 3531 da0b 6f70 706f 7274 756e  6_1251..opportun
+00000110: 6974 79da 056e 6f74 6573 5429 02da 046e  ity..notesT)...n
+00000120: 756c 6cda 0562 6c61 6e6b 2903 da0a 6d6f  ull..blank)...mo
+00000130: 6465 6c5f 6e61 6d65 da04 6e61 6d65 da05  del_name..name..
+00000140: 6669 656c 644e 2902 7206 0000 0072 0700  fieldN).r....r..
+00000150: 0000 2909 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+00000160: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000170: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
+00000180: 656e 6369 6573 7203 0000 00da 0a41 6c74  enciesr......Alt
+00000190: 6572 4669 656c 6472 0400 0000 da09 5465  erFieldr......Te
+000001a0: 7874 4669 656c 64da 0a6f 7065 7261 7469  xtField..operati
+000001b0: 6f6e 73a9 0072 1600 0000 7216 0000 00fa  ons..r....r.....
+000001c0: 632f 686f 6d65 2f63 616d 6572 6f6e 2f44  c/home/cameron/D
+000001d0: 6576 2f6b 616e 6261 6e2d 6465 762f 646a  ev/kanban-dev/dj
+000001e0: 616e 676f 2d63 6f6e 6e65 6374 7769 7365  ango-connectwise
+000001f0: 2f64 6a63 6f6e 6e65 6374 7769 7365 2f6d  /djconnectwise/m
+00000200: 6967 7261 7469 6f6e 732f 3030 3334 5f61  igrations/0034_a
+00000210: 7574 6f5f 3230 3137 3037 3237 5f31 3234  uto_20170727_124
+00000220: 332e 7079 7205 0000 0007 0000 0073 0a00  3.pyr........s..
+00000230: 0000 0803 0604 0401 0201 0201 7205 0000  ............r...
+00000240: 004e 2906 da0a 5f5f 6675 7475 7265 5f5f  .N)...__future__
+00000250: 7202 0000 00da 0964 6a61 6e67 6f2e 6462  r......django.db
+00000260: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
+00000270: 1600 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
+00000280: 0000 00da 083c 6d6f 6475 6c65 3e02 0000  .....<module>...
+00000290: 0073 0400 0000 0c02 1003                 .s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0058_auto_20180516_1052.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0006_auto_20170303_1242.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,44 @@
-00000000: 160d 0d0a a4b0 1f5d 3102 0000 e300 0000  .......]1.......
+00000000: 330d 0d0a 10ec da5c bc01 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 1100 0000 4000 0000 736a 0000 0065 0000  ....@...sj...e..
-000000a0: 5a01 0064 0000 5a02 0064 1100 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6407 0065 0600 6a07 0064 0800  .d..d..e..j..d..
-000000d0: 6409 0064 0a00 6409 0064 0b00 6508 006a  d..d..d..d..e..j
-000000e0: 0900 6a06 006a 0a00 6a0b 0064 0c00 640d  ..j..j..j..d..d.
-000000f0: 0064 0e00 640f 0083 0005 8300 0367 0100  .d..d........g..
-00000100: 5a0c 0064 1000 5329 12da 094d 6967 7261  Z..d..S)...Migra
-00000110: 7469 6f6e da0d 646a 636f 6e6e 6563 7477  tion..djconnectw
-00000120: 6973 65da 1730 3035 375f 6175 746f 5f32  ise..0057_auto_2
-00000130: 3031 3830 3531 315f 3134 3430 da0a 6d6f  0180511_1440..mo
-00000140: 6465 6c5f 6e61 6d65 da0b 6f70 706f 7274  del_name..opport
-00000150: 756e 6974 79da 046e 616d 65da 0b70 726f  unity..name..pro
-00000160: 6261 6269 6c69 7479 da05 6669 656c 64da  bability..field.
-00000170: 0562 6c61 6e6b 54da 046e 756c 6cda 096f  .blankT..null..o
-00000180: 6e5f 6465 6c65 7465 da0c 7265 6c61 7465  n_delete..relate
-00000190: 645f 6e61 6d65 da11 7361 6c65 735f 7072  d_name..sales_pr
-000001a0: 6f62 6162 696c 6974 79da 0274 6f7a 1e64  obability..toz.d
-000001b0: 6a63 6f6e 6e65 6374 7769 7365 2e53 616c  jconnectwise.Sal
-000001c0: 6573 5072 6f62 6162 696c 6974 794e 2902  esProbabilityN).
-000001d0: 7a0d 646a 636f 6e6e 6563 7477 6973 6572  z.djconnectwiser
-000001e0: 0600 0000 290d da08 5f5f 6e61 6d65 5f5f  ....)...__name__
-000001f0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000200: 7175 616c 6e61 6d65 5f5f da0c 6465 7065  qualname__..depe
-00000210: 6e64 656e 6369 6573 7202 0000 00da 0a41  ndenciesr......A
-00000220: 6c74 6572 4669 656c 6472 0300 0000 da0a  lterFieldr......
-00000230: 466f 7265 6967 6e4b 6579 da06 646a 616e  ForeignKey..djan
-00000240: 676f da02 6462 da08 6465 6c65 7469 6f6e  go..db..deletion
-00000250: da08 5345 545f 4e55 4c4c da0a 6f70 6572  ..SET_NULL..oper
-00000260: 6174 696f 6e73 a900 721d 0000 0072 1d00  ations..r....r..
-00000270: 0000 fa6e 2f68 6f6d 652f 7361 6d2f 6769  ...n/home/sam/gi
-00000280: 742f 4b61 6e62 616e 2f64 6a61 6e67 6f2d  t/Kanban/django-
-00000290: 636f 6e6e 6563 7477 6973 652f 646a 616e  connectwise/djan
-000002a0: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
-000002b0: 6a63 6f6e 6e65 6374 7769 7365 2f6d 6967  jconnectwise/mig
-000002c0: 7261 7469 6f6e 732f 3030 3538 5f61 7574  rations/0058_aut
-000002d0: 6f5f 3230 3138 3035 3136 5f31 3035 322e  o_20180516_1052.
-000002e0: 7079 7204 0000 0007 0000 0073 0a00 0000  pyr........s....
-000002f0: 0c03 0904 0901 0601 0601 7204 0000 0029  ..........r....)
-00000300: 06da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
-00000310: 0072 0300 0000 da19 646a 616e 676f 2e64  .r......django.d
-00000320: 622e 6d6f 6465 6c73 2e64 656c 6574 696f  b.models.deletio
-00000330: 6e72 1800 0000 7204 0000 0072 1d00 0000  nr....r....r....
-00000340: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
-00000350: 083c 6d6f 6475 6c65 3e03 0000 0073 0400  .<module>....s..
-00000360: 0000 1601 0c03                           ......
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0800 0000 4000 0000 7330  ..........@...s0
+000000a0: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000c0: 0664 0664 078d 0364 088d 0367 015a 0864  .d.d...d...g.Z.d
+000000d0: 0953 0029 0bda 094d 6967 7261 7469 6f6e  .S.)...Migration
+000000e0: da0d 646a 636f 6e6e 6563 7477 6973 65da  ..djconnectwise.
+000000f0: 1730 3030 355f 6175 746f 5f32 3031 3730  .0005_auto_20170
+00000100: 3232 355f 3031 3031 da0d 6361 6c6c 6261  225_0101..callba
+00000110: 636b 656e 7472 79da 0b64 6573 6372 6970  ckentry..descrip
+00000120: 7469 6f6e e964 0000 0054 2903 da0a 6d61  tion.d...T)...ma
+00000130: 785f 6c65 6e67 7468 da04 6e75 6c6c da05  x_length..null..
+00000140: 626c 616e 6b29 03da 0a6d 6f64 656c 5f6e  blank)...model_n
+00000150: 616d 65da 046e 616d 65da 0566 6965 6c64  ame..name..field
+00000160: 4e29 0272 0600 0000 7207 0000 0029 09da  N).r....r....)..
+00000170: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000180: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000190: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
+000001a0: 7372 0300 0000 da0a 416c 7465 7246 6965  sr......AlterFie
+000001b0: 6c64 7204 0000 00da 0943 6861 7246 6965  ldr......CharFie
+000001c0: 6c64 da0a 6f70 6572 6174 696f 6e73 a900  ld..operations..
+000001d0: 7218 0000 0072 1800 0000 fa63 2f68 6f6d  r....r.....c/hom
+000001e0: 652f 6361 6d65 726f 6e2f 4465 762f 6b61  e/cameron/Dev/ka
+000001f0: 6e62 616e 2d64 6576 2f64 6a61 6e67 6f2d  nban-dev/django-
+00000200: 636f 6e6e 6563 7477 6973 652f 646a 636f  connectwise/djco
+00000210: 6e6e 6563 7477 6973 652f 6d69 6772 6174  nnectwise/migrat
+00000220: 696f 6e73 2f30 3030 365f 6175 746f 5f32  ions/0006_auto_2
+00000230: 3031 3730 3330 335f 3132 3432 2e70 7972  0170303_1242.pyr
+00000240: 0500 0000 0700 0000 730a 0000 0008 0306  ........s.......
+00000250: 0404 0102 0102 0172 0500 0000 4e29 06da  .......r....N)..
+00000260: 0a5f 5f66 7574 7572 655f 5f72 0200 0000  .__future__r....
+00000270: da09 646a 616e 676f 2e64 6272 0300 0000  ..django.dbr....
+00000280: 7204 0000 0072 0500 0000 7218 0000 0072  r....r....r....r
+00000290: 1800 0000 7218 0000 0072 1900 0000 da08  ....r....r......
+000002a0: 3c6d 6f64 756c 653e 0200 0000 7304 0000  <module>....s...
+000002b0: 000c 0210 03                             .....
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0075_auto_20180910_1629.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0082_auto_20190125_1109.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,47 @@
-00000000: 160d 0d0a a4b0 1f5d fd01 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c 0102 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 0f00 0000 4000 0000 7364 0000 0065 0000  ....@...sd...e..
-000000a0: 5a01 0064 0000 5a02 0064 0f00 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6407 0065 0600 6a07 0064 0800  .d..d..e..j..d..
-000000d0: 6409 0064 0a00 6409 0064 0b00 6508 006a  d..d..d..d..e..j
-000000e0: 0900 6a06 006a 0a00 6a0b 0064 0c00 640d  ..j..j..j..d..d.
-000000f0: 0083 0004 8300 0367 0100 5a0c 0064 0e00  .......g..Z..d..
-00000100: 5329 10da 094d 6967 7261 7469 6f6e da0d  S)...Migration..
-00000110: 646a 636f 6e6e 6563 7477 6973 65da 1730  djconnectwise..0
-00000120: 3037 345f 6175 746f 5f32 3031 3830 3832  074_auto_2018082
-00000130: 375f 3132 3431 da0a 6d6f 6465 6c5f 6e61  7_1241..model_na
-00000140: 6d65 da09 7469 6d65 656e 7472 79da 046e  me..timeentry..n
-00000150: 616d 65da 0763 6f6d 7061 6e79 da05 6669  ame..company..fi
-00000160: 656c 64da 0562 6c61 6e6b 54da 046e 756c  eld..blankT..nul
-00000170: 6cda 096f 6e5f 6465 6c65 7465 da02 746f  l..on_delete..to
-00000180: 7a15 646a 636f 6e6e 6563 7477 6973 652e  z.djconnectwise.
-00000190: 436f 6d70 616e 794e 2902 7a0d 646a 636f  CompanyN).z.djco
-000001a0: 6e6e 6563 7477 6973 657a 1730 3037 345f  nnectwisez.0074_
-000001b0: 6175 746f 5f32 3031 3830 3832 375f 3132  auto_20180827_12
-000001c0: 3431 290d da08 5f5f 6e61 6d65 5f5f da0a  41)...__name__..
-000001d0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000001e0: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
-000001f0: 656e 6369 6573 7202 0000 00da 0a41 6c74  enciesr......Alt
-00000200: 6572 4669 656c 6472 0300 0000 da0a 466f  erFieldr......Fo
-00000210: 7265 6967 6e4b 6579 da06 646a 616e 676f  reignKey..django
-00000220: da02 6462 da08 6465 6c65 7469 6f6e da07  ..db..deletion..
-00000230: 4341 5343 4144 45da 0a6f 7065 7261 7469  CASCADE..operati
-00000240: 6f6e 73a9 0072 1b00 0000 721b 0000 00fa  ons..r....r.....
-00000250: 6e2f 686f 6d65 2f73 616d 2f67 6974 2f4b  n/home/sam/git/K
-00000260: 616e 6261 6e2f 646a 616e 676f 2d63 6f6e  anban/django-con
-00000270: 6e65 6374 7769 7365 2f64 6a61 6e67 6f2d  nectwise/django-
-00000280: 636f 6e6e 6563 7477 6973 652f 646a 636f  connectwise/djco
-00000290: 6e6e 6563 7477 6973 652f 6d69 6772 6174  nnectwise/migrat
-000002a0: 696f 6e73 2f30 3037 355f 6175 746f 5f32  ions/0075_auto_2
-000002b0: 3031 3830 3931 305f 3136 3239 2e70 7972  0180910_1629.pyr
-000002c0: 0400 0000 0700 0000 730a 0000 000c 0309  ........s.......
-000002d0: 0409 0106 0106 0172 0400 0000 2906 da09  .......r....)...
-000002e0: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
-000002f0: 0000 00da 1964 6a61 6e67 6f2e 6462 2e6d  .....django.db.m
-00000300: 6f64 656c 732e 6465 6c65 7469 6f6e 7216  odels.deletionr.
-00000310: 0000 0072 0400 0000 721b 0000 0072 1b00  ...r....r....r..
-00000320: 0000 721b 0000 0072 1c00 0000 da08 3c6d  ..r....r......<m
-00000330: 6f64 756c 653e 0300 0000 7304 0000 0016  odule>....s.....
-00000340: 010c 03                                  ...
+00000020: 0073 2e00 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 4700  m.Z...d.d.l.Z.G.
+00000040: 6403 6404 8400 6404 6501 6a05 8303 5a05  d.d...d.e.j...Z.
+00000050: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 734e 6300 0000 0000 0000 0000 0000 0008  sNc.............
+00000080: 0000 0040 0000 0073 3800 0000 6500 5a01  ...@...s8...e.Z.
+00000090: 6400 5a02 640a 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000a0: 6404 6506 6a07 6405 6508 6a09 6a06 6a0a  d.e.j.d.e.j.j.j.
+000000b0: 6a0b 6406 6407 8d03 6408 8d03 6701 5a0c  j.d.d...d...g.Z.
+000000c0: 6409 5300 290b da09 4d69 6772 6174 696f  d.S.)...Migratio
+000000d0: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
+000000e0: da17 3030 3831 5f61 7574 6f5f 3230 3138  ..0081_auto_2018
+000000f0: 3132 3230 5f30 3931 37da 0b6f 7070 6f72  1220_0917..oppor
+00000100: 7475 6e69 7479 da08 7072 696f 7269 7479  tunity..priority
+00000110: 547a 2164 6a63 6f6e 6e65 6374 7769 7365  Tz!djconnectwise
+00000120: 2e4f 7070 6f72 7475 6e69 7479 5072 696f  .OpportunityPrio
+00000130: 7269 7479 2903 da04 6e75 6c6c da09 6f6e  rity)...null..on
+00000140: 5f64 656c 6574 65da 0274 6f29 03da 0a6d  _delete..to)...m
+00000150: 6f64 656c 5f6e 616d 65da 046e 616d 65da  odel_name..name.
+00000160: 0566 6965 6c64 4e29 0272 0500 0000 7206  .fieldN).r....r.
+00000170: 0000 0029 0dda 085f 5f6e 616d 655f 5fda  ...)...__name__.
+00000180: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000190: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
+000001a0: 6465 6e63 6965 7372 0200 0000 da0a 416c  denciesr......Al
+000001b0: 7465 7246 6965 6c64 7203 0000 00da 0a46  terFieldr......F
+000001c0: 6f72 6569 676e 4b65 79da 0664 6a61 6e67  oreignKey..djang
+000001d0: 6fda 0264 62da 0864 656c 6574 696f 6eda  o..db..deletion.
+000001e0: 0853 4554 5f4e 554c 4cda 0a6f 7065 7261  .SET_NULL..opera
+000001f0: 7469 6f6e 73a9 0072 1a00 0000 721a 0000  tions..r....r...
+00000200: 00fa 632f 686f 6d65 2f63 616d 6572 6f6e  ..c/home/cameron
+00000210: 2f44 6576 2f6b 616e 6261 6e2d 6465 762f  /Dev/kanban-dev/
+00000220: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
+00000230: 7365 2f64 6a63 6f6e 6e65 6374 7769 7365  se/djconnectwise
+00000240: 2f6d 6967 7261 7469 6f6e 732f 3030 3832  /migrations/0082
+00000250: 5f61 7574 6f5f 3230 3139 3031 3235 5f31  _auto_20190125_1
+00000260: 3130 392e 7079 7204 0000 0007 0000 0073  109.pyr........s
+00000270: 0a00 0000 0803 0604 0401 0201 0201 7204  ..............r.
+00000280: 0000 0029 06da 0964 6a61 6e67 6f2e 6462  ...)...django.db
+00000290: 7202 0000 0072 0300 0000 da19 646a 616e  r....r......djan
+000002a0: 676f 2e64 622e 6d6f 6465 6c73 2e64 656c  go.db.models.del
+000002b0: 6574 696f 6e72 1500 0000 7204 0000 0072  etionr....r....r
+000002c0: 1a00 0000 721a 0000 0072 1a00 0000 721b  ....r....r....r.
+000002d0: 0000 00da 083c 6d6f 6475 6c65 3e03 0000  .....<module>...
+000002e0: 0073 0400 0000 1001 0803                 .s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0069_auto_20180815_1116.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0069_auto_20180815_1116.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,61 @@
-00000000: 160d 0d0a a4b0 1f5d 4003 0000 e300 0000  .......]@.......
+00000000: 330d 0d0a 10ec da5c 4003 0000 e300 0000  3......\@.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3300 0000 6400 0064 0100 6c00 006d  .s3...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 4764 0200  ..Z..m..Z...Gd..
-00000040: 6403 0084 0000 6403 0065 0100 6a03 0083  d.....d..e..j...
-00000050: 0300 5a03 0064 0400 5329 05e9 0000 0000  ..Z..d..S)......
-00000060: 2902 da0a 6d69 6772 6174 696f 6e73 da06  )...migrations..
-00000070: 6d6f 6465 6c73 6300 0000 0000 0000 0000  modelsc.........
-00000080: 0000 000e 0000 0040 0000 0073 9100 0000  .......@...s....
-00000090: 6500 005a 0100 6400 005a 0200 641b 0067  e..Z..d..Z..d..g
-000000a0: 0100 5a03 0065 0400 6a05 0064 0300 6404  ..Z..e..j..d..d.
-000000b0: 0064 0500 6406 0064 0700 6506 006a 0700  .d..d..d..e..j..
-000000c0: 6408 0064 1c00 641d 0064 1e00 641f 0067  d..d..d..d..d..g
-000000d0: 0400 6410 0064 1100 8300 0283 0003 6504  ..d..d........e.
-000000e0: 006a 0500 6403 0064 0400 6405 0064 1200  .j..d..d..d..d..
-000000f0: 6407 0065 0600 6a07 0064 0800 6420 0064  d..e..j..d..d .d
-00000100: 2100 6422 0064 2300 6704 0064 1000 6411  !.d".d#.g..d..d.
-00000110: 0083 0002 8300 0367 0200 5a08 0064 1a00  .......g..Z..d..
-00000120: 5329 24da 094d 6967 7261 7469 6f6e da0d  S)$..Migration..
-00000130: 646a 636f 6e6e 6563 7477 6973 65da 1830  djconnectwise..0
-00000140: 3036 385f 6d65 7267 655f 3230 3138 3038  068_merge_201808
-00000150: 3134 5f31 3130 34da 0a6d 6f64 656c 5f6e  14_1104..model_n
-00000160: 616d 655a 0974 696d 6565 6e74 7279 da04  ameZ.timeentry..
-00000170: 6e61 6d65 da0f 6269 6c6c 6162 6c65 5f6f  name..billable_o
-00000180: 7074 696f 6eda 0566 6965 6c64 da07 6368  ption..field..ch
-00000190: 6f69 6365 73da 0842 696c 6c61 626c 65da  oices..Billable.
-000001a0: 0944 6f4e 6f74 4269 6c6c fa0b 446f 204e  .DoNotBill..Do N
-000001b0: 6f74 2042 696c 6cda 084e 6f43 6861 7267  ot Bill..NoCharg
-000001c0: 65fa 094e 6f20 4368 6172 6765 da09 4e6f  e..No Charge..No
-000001d0: 4465 6661 756c 74fa 0a4e 6f20 4465 6661  Default..No Defa
-000001e0: 756c 74da 0a6d 6178 5f6c 656e 6774 68e9  ult..max_length.
-000001f0: fa00 0000 da0e 6368 6172 6765 5f74 6f5f  ......charge_to_
-00000200: 7479 7065 da0d 5365 7276 6963 6554 6963  type..ServiceTic
-00000210: 6b65 74fa 0e53 6572 7669 6365 2054 6963  ket..Service Tic
-00000220: 6b65 74da 0d50 726f 6a65 6374 5469 636b  ket..ProjectTick
-00000230: 6574 fa0e 5072 6f6a 6563 7420 5469 636b  et..Project Tick
-00000240: 6574 da0a 4368 6172 6765 436f 6465 fa0b  et..ChargeCode..
-00000250: 4368 6172 6765 2043 6f64 65da 0841 6374  Charge Code..Act
-00000260: 6976 6974 794e 2902 7a0d 646a 636f 6e6e  ivityN).z.djconn
-00000270: 6563 7477 6973 6572 0600 0000 2902 fa08  ectwiser....)...
-00000280: 4269 6c6c 6162 6c65 721d 0000 0029 027a  Billabler....).z
-00000290: 0944 6f4e 6f74 4269 6c6c 720e 0000 0029  .DoNotBillr....)
-000002a0: 027a 084e 6f43 6861 7267 6572 1000 0000  .z.NoCharger....
-000002b0: 2902 7a09 4e6f 4465 6661 756c 7472 1200  ).z.NoDefaultr..
-000002c0: 0000 2902 7a0d 5365 7276 6963 6554 6963  ..).z.ServiceTic
-000002d0: 6b65 7472 1700 0000 2902 7a0d 5072 6f6a  ketr....).z.Proj
-000002e0: 6563 7454 6963 6b65 7472 1900 0000 2902  ectTicketr....).
-000002f0: 7a0a 4368 6172 6765 436f 6465 721b 0000  z.ChargeCoder...
-00000300: 0029 02fa 0841 6374 6976 6974 7972 1e00  .)...Activityr..
-00000310: 0000 2909 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
-00000320: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000330: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
-00000340: 656e 6369 6573 7202 0000 00da 0a41 6c74  enciesr......Alt
-00000350: 6572 4669 656c 6472 0300 0000 da09 4368  erFieldr......Ch
-00000360: 6172 4669 656c 64da 0a6f 7065 7261 7469  arField..operati
-00000370: 6f6e 73a9 0072 2600 0000 7226 0000 00fa  ons..r&...r&....
-00000380: 6e2f 686f 6d65 2f73 616d 2f67 6974 2f4b  n/home/sam/git/K
-00000390: 616e 6261 6e2f 646a 616e 676f 2d63 6f6e  anban/django-con
-000003a0: 6e65 6374 7769 7365 2f64 6a61 6e67 6f2d  nectwise/django-
-000003b0: 636f 6e6e 6563 7477 6973 652f 646a 636f  connectwise/djco
-000003c0: 6e6e 6563 7477 6973 652f 6d69 6772 6174  nnectwise/migrat
-000003d0: 696f 6e73 2f30 3036 395f 6175 746f 5f32  ions/0069_auto_2
-000003e0: 3031 3830 3831 355f 3131 3136 2e70 7972  0180815_1116.pyr
-000003f0: 0400 0000 0600 0000 7312 0000 000c 0309  ........s.......
-00000400: 0409 0106 0106 0124 0209 0106 0106 0172  .......$.......r
-00000410: 0400 0000 4e29 04da 0964 6a61 6e67 6f2e  ....N)...django.
-00000420: 6462 7202 0000 0072 0300 0000 7204 0000  dbr....r....r...
-00000430: 0072 2600 0000 7226 0000 0072 2600 0000  .r&...r&...r&...
-00000440: 7227 0000 00da 083c 6d6f 6475 6c65 3e03  r'.....<module>.
-00000450: 0000 0073 0200 0000 1603                 ...s......
+00000020: 0073 2600 0000 6400 6401 6c00 6d01 5a01  .s&...d.d.l.m.Z.
+00000030: 6d02 5a02 0100 4700 6402 6403 8400 6403  m.Z...G.d.d...d.
+00000040: 6501 6a03 8303 5a03 6404 5300 2905 e900  e.j...Z.d.S.)...
+00000050: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
+00000060: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000070: 0000 0000 0000 0a00 0000 4000 0000 7356  ..........@...sV
+00000080: 0000 0065 005a 0164 005a 0264 1867 015a  ...e.Z.d.Z.d.g.Z
+00000090: 0365 046a 0564 0364 0465 066a 0764 1964  .e.j.d.d.e.j.d.d
+000000a0: 1a64 1b64 1c67 0464 0c64 0d8d 0264 0e8d  .d.d.g.d.d...d..
+000000b0: 0365 046a 0564 0364 0f65 066a 0764 1d64  .e.j.d.d.e.j.d.d
+000000c0: 1e64 1f64 2067 0464 0c64 0d8d 0264 0e8d  .d.d g.d.d...d..
+000000d0: 0367 025a 0864 1753 0029 21da 094d 6967  .g.Z.d.S.)!..Mig
+000000e0: 7261 7469 6f6e da0d 646a 636f 6e6e 6563  ration..djconnec
+000000f0: 7477 6973 65da 1830 3036 385f 6d65 7267  twise..0068_merg
+00000100: 655f 3230 3138 3038 3134 5f31 3130 34da  e_20180814_1104.
+00000110: 0974 696d 6565 6e74 7279 da0f 6269 6c6c  .timeentry..bill
+00000120: 6162 6c65 5f6f 7074 696f 6eda 0842 696c  able_option..Bil
+00000130: 6c61 626c 65da 0944 6f4e 6f74 4269 6c6c  lable..DoNotBill
+00000140: fa0b 446f 204e 6f74 2042 696c 6cda 084e  ..Do Not Bill..N
+00000150: 6f43 6861 7267 65fa 094e 6f20 4368 6172  oCharge..No Char
+00000160: 6765 da09 4e6f 4465 6661 756c 74fa 0a4e  ge..NoDefault..N
+00000170: 6f20 4465 6661 756c 74e9 fa00 0000 2902  o Default.....).
+00000180: da07 6368 6f69 6365 73da 0a6d 6178 5f6c  ..choices..max_l
+00000190: 656e 6774 6829 03da 0a6d 6f64 656c 5f6e  ength)...model_n
+000001a0: 616d 65da 046e 616d 65da 0566 6965 6c64  ame..name..field
+000001b0: da0e 6368 6172 6765 5f74 6f5f 7479 7065  ..charge_to_type
+000001c0: da0d 5365 7276 6963 6554 6963 6b65 74fa  ..ServiceTicket.
+000001d0: 0e53 6572 7669 6365 2054 6963 6b65 74da  .Service Ticket.
+000001e0: 0d50 726f 6a65 6374 5469 636b 6574 fa0e  .ProjectTicket..
+000001f0: 5072 6f6a 6563 7420 5469 636b 6574 da0a  Project Ticket..
+00000200: 4368 6172 6765 436f 6465 fa0b 4368 6172  ChargeCode..Char
+00000210: 6765 2043 6f64 65da 0841 6374 6976 6974  ge Code..Activit
+00000220: 794e 2902 7205 0000 0072 0600 0000 2902  yN).r....r....).
+00000230: 7209 0000 0072 0900 0000 2902 720a 0000  r....r....).r...
+00000240: 0072 0b00 0000 2902 720c 0000 0072 0d00  .r....).r....r..
+00000250: 0000 2902 720e 0000 0072 0f00 0000 2902  ..).r....r....).
+00000260: 7217 0000 0072 1800 0000 2902 7219 0000  r....r....).r...
+00000270: 0072 1a00 0000 2902 721b 0000 0072 1c00  .r....).r....r..
+00000280: 0000 2902 721d 0000 0072 1d00 0000 2909  ..).r....r....).
+00000290: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+000002a0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+000002b0: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
+000002c0: 6573 7202 0000 00da 0a41 6c74 6572 4669  esr......AlterFi
+000002d0: 656c 6472 0300 0000 da09 4368 6172 4669  eldr......CharFi
+000002e0: 656c 64da 0a6f 7065 7261 7469 6f6e 73a9  eld..operations.
+000002f0: 0072 2500 0000 7225 0000 00fa 632f 686f  .r%...r%....c/ho
+00000300: 6d65 2f63 616d 6572 6f6e 2f44 6576 2f6b  me/cameron/Dev/k
+00000310: 616e 6261 6e2d 6465 762f 646a 616e 676f  anban-dev/django
+00000320: 2d63 6f6e 6e65 6374 7769 7365 2f64 6a63  -connectwise/djc
+00000330: 6f6e 6e65 6374 7769 7365 2f6d 6967 7261  onnectwise/migra
+00000340: 7469 6f6e 732f 3030 3639 5f61 7574 6f5f  tions/0069_auto_
+00000350: 3230 3138 3038 3135 5f31 3131 362e 7079  20180815_1116.py
+00000360: 7204 0000 0006 0000 0073 1200 0000 0803  r........s......
+00000370: 0604 0401 0201 0201 1802 0401 0201 0201  ................
+00000380: 7204 0000 004e 2904 da09 646a 616e 676f  r....N)...django
+00000390: 2e64 6272 0200 0000 7203 0000 0072 0400  .dbr....r....r..
+000003a0: 0000 7225 0000 0072 2500 0000 7225 0000  ..r%...r%...r%..
+000003b0: 0072 2600 0000 da08 3c6d 6f64 756c 653e  .r&.....<module>
+000003c0: 0300 0000 7302 0000 0010 03              ....s......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0074_auto_20180827_1241.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0092_remove_ticket_work_type.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,35 @@
-00000000: 160d 0d0a a4b0 1f5d b902 0000 e300 0000  .......]........
+00000000: 330d 0d0a eb47 2e5d 4f01 0000 e300 0000  3....G.]O.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3300 0000 6400 0064 0100 6c00 006d  .s3...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 4764 0200  ..Z..m..Z...Gd..
-00000040: 6403 0084 0000 6403 0065 0100 6a03 0083  d.....d..e..j...
-00000050: 0300 5a03 0064 0400 5329 05e9 0000 0000  ..Z..d..S)......
-00000060: 2902 da0a 6d69 6772 6174 696f 6e73 da06  )...migrations..
-00000070: 6d6f 6465 6c73 6300 0000 0000 0000 0000  modelsc.........
-00000080: 0000 0009 0000 0040 0000 0073 8200 0000  .......@...s....
-00000090: 6500 005a 0100 6400 005a 0200 640b 0067  e..Z..d..Z..d..g
-000000a0: 0100 5a03 0065 0400 6a05 0064 0300 6404  ..Z..e..j..d..d.
-000000b0: 0064 0500 6406 0064 0700 6506 006a 0700  .d..d..d..e..j..
-000000c0: 8300 0083 0003 6504 006a 0500 6403 0064  ......e..j..d..d
-000000d0: 0400 6405 0064 0800 6407 0065 0600 6a07  ..d..d..d..e..j.
-000000e0: 0083 0000 8300 0365 0400 6a05 0064 0300  .......e..j..d..
-000000f0: 6404 0064 0500 6409 0064 0700 6506 006a  d..d..d..d..e..j
-00000100: 0700 8300 0083 0003 6703 005a 0800 640a  ........g..Z..d.
-00000110: 0053 290c da09 4d69 6772 6174 696f 6eda  .S)...Migration.
-00000120: 0d64 6a63 6f6e 6e65 6374 7769 7365 da17  .djconnectwise..
-00000130: 3030 3733 5f61 7574 6f5f 3230 3138 3038  0073_auto_201808
-00000140: 3234 5f31 3434 36da 0a6d 6f64 656c 5f6e  24_1446..model_n
-00000150: 616d 65da 0b73 6c61 7072 696f 7269 7479  ame..slapriority
-00000160: da04 6e61 6d65 da0b 706c 616e 5f77 6974  ..name..plan_wit
-00000170: 6869 6eda 0566 6965 6c64 da10 7265 736f  hin..field..reso
-00000180: 6c75 7469 6f6e 5f68 6f75 7273 da0d 7265  lution_hours..re
-00000190: 7370 6f6e 645f 686f 7572 734e 2902 7a0d  spond_hoursN).z.
-000001a0: 646a 636f 6e6e 6563 7477 6973 657a 1730  djconnectwisez.0
-000001b0: 3037 335f 6175 746f 5f32 3031 3830 3832  073_auto_2018082
-000001c0: 345f 3134 3436 2909 da08 5f5f 6e61 6d65  4_1446)...__name
-000001d0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-000001e0: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
-000001f0: 7065 6e64 656e 6369 6573 7202 0000 00da  pendenciesr.....
-00000200: 0a41 6c74 6572 4669 656c 6472 0300 0000  .AlterFieldr....
-00000210: da0a 466c 6f61 7446 6965 6c64 da0a 6f70  ..FloatField..op
-00000220: 6572 6174 696f 6e73 a900 7215 0000 0072  erations..r....r
-00000230: 1500 0000 fa6e 2f68 6f6d 652f 7361 6d2f  .....n/home/sam/
-00000240: 6769 742f 4b61 6e62 616e 2f64 6a61 6e67  git/Kanban/djang
-00000250: 6f2d 636f 6e6e 6563 7477 6973 652f 646a  o-connectwise/dj
-00000260: 616e 676f 2d63 6f6e 6e65 6374 7769 7365  ango-connectwise
-00000270: 2f64 6a63 6f6e 6e65 6374 7769 7365 2f6d  /djconnectwise/m
-00000280: 6967 7261 7469 6f6e 732f 3030 3734 5f61  igrations/0074_a
-00000290: 7574 6f5f 3230 3138 3038 3237 5f31 3234  uto_20180827_124
-000002a0: 312e 7079 7204 0000 0006 0000 0073 1a00  1.pyr........s..
-000002b0: 0000 0c03 0904 0901 0601 0601 0c02 0901  ................
-000002c0: 0601 0601 0c02 0901 0601 0601 7204 0000  ............r...
-000002d0: 004e 2904 da09 646a 616e 676f 2e64 6272  .N)...django.dbr
-000002e0: 0200 0000 7203 0000 0072 0400 0000 7215  ....r....r....r.
-000002f0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00000300: 0000 da08 3c6d 6f64 756c 653e 0300 0000  ....<module>....
-00000310: 7302 0000 0016 03                        s......
+00000020: 0073 2200 0000 6400 6401 6c00 6d01 5a01  .s"...d.d.l.m.Z.
+00000030: 0100 4700 6402 6403 8400 6403 6501 6a02  ..G.d.d...d.e.j.
+00000040: 8303 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
+00000050: 01da 0a6d 6967 7261 7469 6f6e 7363 0000  ...migrationsc..
+00000060: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+00000070: 0000 7322 0000 0065 005a 0164 005a 0264  ..s"...e.Z.d.Z.d
+00000080: 0767 015a 0365 046a 0564 0364 0464 058d  .g.Z.e.j.d.d.d..
+00000090: 0267 015a 0664 0653 0029 08da 094d 6967  .g.Z.d.S.)...Mig
+000000a0: 7261 7469 6f6e da0d 646a 636f 6e6e 6563  ration..djconnec
+000000b0: 7477 6973 65da 1730 3039 315f 776f 726b  twise..0091_work
+000000c0: 7479 7065 5f62 696c 6c5f 7469 6d65 da06  type_bill_time..
+000000d0: 7469 636b 6574 da09 776f 726b 5f74 7970  ticket..work_typ
+000000e0: 6529 02da 0a6d 6f64 656c 5f6e 616d 65da  e)...model_name.
+000000f0: 046e 616d 654e 2902 7204 0000 0072 0500  .nameN).r....r..
+00000100: 0000 2907 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+00000110: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000120: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
+00000130: 656e 6369 6573 7202 0000 00da 0b52 656d  enciesr......Rem
+00000140: 6f76 6546 6965 6c64 da0a 6f70 6572 6174  oveField..operat
+00000150: 696f 6e73 a900 7210 0000 0072 1000 0000  ions..r....r....
+00000160: fa68 2f68 6f6d 652f 6361 6d65 726f 6e2f  .h/home/cameron/
+00000170: 4465 762f 6b61 6e62 616e 2d64 6576 2f64  Dev/kanban-dev/d
+00000180: 6a61 6e67 6f2d 636f 6e6e 6563 7477 6973  jango-connectwis
+00000190: 652f 646a 636f 6e6e 6563 7477 6973 652f  e/djconnectwise/
+000001a0: 6d69 6772 6174 696f 6e73 2f30 3039 325f  migrations/0092_
+000001b0: 7265 6d6f 7665 5f74 6963 6b65 745f 776f  remove_ticket_wo
+000001c0: 726b 5f74 7970 652e 7079 7203 0000 0006  rk_type.pyr.....
+000001d0: 0000 0073 0800 0000 0803 0604 0401 0201  ...s............
+000001e0: 7203 0000 004e 2903 da09 646a 616e 676f  r....N)...django
+000001f0: 2e64 6272 0200 0000 7203 0000 0072 1000  .dbr....r....r..
+00000200: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00000210: 00da 083c 6d6f 6475 6c65 3e03 0000 0073  ...<module>....s
+00000220: 0200 0000 0c03                           ......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0023_auto_20170605_0705.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0023_auto_20170605_0705.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,79 @@
-00000000: 160d 0d0a a4b0 1f5d d004 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c d004 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4f00 0000 6400 0064 0100 6c00 006d  .sO...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 6400 0064  ..Z..m..Z...d..d
-00000050: 0300 6c05 005a 0600 4764 0400 6405 0084  ..l..Z..Gd..d...
-00000060: 0000 6405 0065 0300 6a07 0083 0300 5a07  ..d..e..j.....Z.
-00000070: 0064 0300 5329 06e9 0000 0000 2901 da10  .d..S)......)...
-00000080: 756e 6963 6f64 655f 6c69 7465 7261 6c73  unicode_literals
-00000090: 2902 da0a 6d69 6772 6174 696f 6e73 da06  )...migrations..
-000000a0: 6d6f 6465 6c73 4e63 0000 0000 0000 0000  modelsNc........
-000000b0: 0000 0000 0e00 0000 4000 0000 73fa 0000  ........@...s...
-000000c0: 0065 0000 5a01 0064 0000 5a02 0064 2100  .e..Z..d..Z..d!.
-000000d0: 6701 005a 0300 6504 006a 0500 6403 0064  g..Z..e..j..d..d
-000000e0: 0400 6405 0064 0600 6506 006a 0700 6407  ..d..d..e..j..d.
-000000f0: 0064 0800 6409 0064 0a00 640b 0064 0c00  .d..d..d..d..d..
-00000100: 640d 0064 0a00 8300 0466 0200 640e 0065  d..d.....f..d..e
-00000110: 0800 6a09 006a 0a00 6a0b 0064 0700 640e  ..j..j..j..d..d.
-00000120: 0064 0f00 640a 0083 0002 6602 0064 1000  .d..d.....f..d..
-00000130: 6508 006a 0900 6a0a 006a 0c00 6407 0064  e..j..j..j..d..d
-00000140: 1000 6411 0064 0a00 8300 0266 0200 6412  ..d..d.....f..d.
-00000150: 0065 0600 6a0d 0064 1300 6414 0083 0001  .e..j..d..d.....
-00000160: 6602 0064 1500 6506 006a 0e00 6416 0064  f..d..e..j..d..d
-00000170: 0c00 8300 0166 0200 6705 0064 1700 6418  .....f..g..d..d.
-00000180: 0064 2200 641b 0064 1000 641c 0064 0c00  .d".d..d..d..d..
-00000190: 6903 0083 0003 6504 006a 0f00 6403 0064  i.....e..j..d..d
-000001a0: 1d00 6417 0064 1e00 641f 0069 0100 8300  ..d..d..d..i....
-000001b0: 0267 0200 5a10 0064 2000 5329 23da 094d  .g..Z..d .S)#..M
-000001c0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
-000001d0: 6563 7477 6973 65da 1630 3032 325f 6f70  ectwise..0022_op
-000001e0: 706f 7274 756e 6974 7973 7461 7475 73da  portunitystatus.
-000001f0: 046e 616d 65da 0f4f 7070 6f72 7475 6e69  .name..Opportuni
-00000200: 7479 5479 7065 da06 6669 656c 6473 da02  tyType..fields..
-00000210: 6964 da0c 7665 7262 6f73 655f 6e61 6d65  id..verbose_name
-00000220: da02 4944 da0b 7072 696d 6172 795f 6b65  ..ID..primary_ke
-00000230: 7954 da09 7365 7269 616c 697a 6546 da0c  yT..serializeF..
-00000240: 6175 746f 5f63 7265 6174 6564 da07 6372  auto_created..cr
-00000250: 6561 7465 64da 0c61 7574 6f5f 6e6f 775f  eated..auto_now_
-00000260: 6164 64da 086d 6f64 6966 6965 64da 0861  add..modified..a
-00000270: 7574 6f5f 6e6f 77da 0b64 6573 6372 6970  uto_now..descrip
-00000280: 7469 6f6e da0a 6d61 785f 6c65 6e67 7468  tion..max_length
-00000290: e932 0000 00da 0d69 6e61 6374 6976 655f  .2.....inactive_
-000002a0: 666c 6167 da07 6465 6661 756c 74da 076f  flag..default..o
-000002b0: 7074 696f 6e73 da08 6f72 6465 7269 6e67  ptions..ordering
-000002c0: fa09 2d6d 6f64 6966 6965 64fa 082d 6372  ..-modified..-cr
-000002d0: 6561 7465 64da 0d67 6574 5f6c 6174 6573  eated..get_lates
-000002e0: 745f 6279 da08 6162 7374 7261 6374 da11  t_by..abstract..
-000002f0: 6f70 706f 7274 756e 6974 7973 7461 7475  opportunitystatu
-00000300: 73da 1376 6572 626f 7365 5f6e 616d 655f  s..verbose_name_
-00000310: 706c 7572 616c 7a14 4f70 706f 7274 756e  pluralz.Opportun
-00000320: 6974 7920 5374 6174 7573 6573 4e29 027a  ity StatusesN).z
-00000330: 0d64 6a63 6f6e 6e65 6374 7769 7365 7207  .djconnectwiser.
-00000340: 0000 0029 0272 1c00 0000 721d 0000 0029  ...).r....r....)
-00000350: 11da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000360: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000370: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
-00000380: 6965 7372 0300 0000 da0b 4372 6561 7465  iesr......Create
-00000390: 4d6f 6465 6c72 0400 0000 da09 4175 746f  Modelr......Auto
-000003a0: 4669 656c 64da 1164 6a61 6e67 6f5f 6578  Field..django_ex
-000003b0: 7465 6e73 696f 6e73 da02 6462 720a 0000  tensions..dbr...
-000003c0: 00da 1543 7265 6174 696f 6e44 6174 6554  ...CreationDateT
-000003d0: 696d 6546 6965 6c64 da19 4d6f 6469 6669  imeField..Modifi
-000003e0: 6361 7469 6f6e 4461 7465 5469 6d65 4669  cationDateTimeFi
-000003f0: 656c 64da 0943 6861 7246 6965 6c64 da0c  eld..CharField..
-00000400: 426f 6f6c 6561 6e46 6965 6c64 da11 416c  BooleanField..Al
-00000410: 7465 724d 6f64 656c 4f70 7469 6f6e 73da  terModelOptions.
-00000420: 0a6f 7065 7261 7469 6f6e 73a9 0072 3000  .operations..r0.
-00000430: 0000 7230 0000 00fa 6e2f 686f 6d65 2f73  ..r0....n/home/s
-00000440: 616d 2f67 6974 2f4b 616e 6261 6e2f 646a  am/git/Kanban/dj
-00000450: 616e 676f 2d63 6f6e 6e65 6374 7769 7365  ango-connectwise
-00000460: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
-00000470: 6973 652f 646a 636f 6e6e 6563 7477 6973  ise/djconnectwis
-00000480: 652f 6d69 6772 6174 696f 6e73 2f30 3032  e/migrations/002
-00000490: 335f 6175 746f 5f32 3031 3730 3630 355f  3_auto_20170605_
-000004a0: 3037 3035 2e70 7972 0500 0000 0800 0000  0705.pyr........
-000004b0: 731c 0000 000c 0309 0409 0106 0227 0121  s............'.!
-000004c0: 0121 0115 011b 0306 0106 010c 0309 0106  .!..............
-000004d0: 0172 0500 0000 2908 da0a 5f5f 6675 7475  .r....)...__futu
-000004e0: 7265 5f5f 7202 0000 00da 0964 6a61 6e67  re__r......djang
-000004f0: 6f2e 6462 7203 0000 0072 0400 0000 da1b  o.dbr....r......
-00000500: 646a 616e 676f 5f65 7874 656e 7369 6f6e  django_extension
-00000510: 732e 6462 2e66 6965 6c64 7372 2800 0000  s.db.fieldsr(...
-00000520: 7205 0000 0072 3000 0000 7230 0000 0072  r....r0...r0...r
-00000530: 3000 0000 7231 0000 00da 083c 6d6f 6475  0...r1.....<modu
-00000540: 6c65 3e02 0000 0073 0600 0000 1002 1601  le>....s........
-00000550: 0c03                                     ..
+00000020: 0073 3a00 0000 6400 6401 6c00 6d01 5a01  .s:...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 6400 6403 6c05 5a06 4700 6404 6405  ..d.d.l.Z.G.d.d.
+00000050: 8400 6405 6503 6a07 8303 5a07 6403 5300  ..d.e.j...Z.d.S.
+00000060: 2906 e900 0000 0029 01da 1075 6e69 636f  )......)...unico
+00000070: 6465 5f6c 6974 6572 616c 7329 02da 0a6d  de_literals)...m
+00000080: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000090: 734e 6300 0000 0000 0000 0000 0000 000a  sNc.............
+000000a0: 0000 0040 0000 0073 9400 0000 6500 5a01  ...@...s....e.Z.
+000000b0: 6400 5a02 641b 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000c0: 6404 6506 6a07 6405 6406 6407 6406 6408  d.e.j.d.d.d.d.d.
+000000d0: 8d04 6602 6409 6508 6a09 6a0a 6a0b 6409  ..f.d.e.j.j.j.d.
+000000e0: 6406 640a 8d02 6602 640b 6508 6a09 6a0a  d.d...f.d.e.j.j.
+000000f0: 6a0c 640b 6406 640c 8d02 6602 640d 6506  j.d.d.d...f.d.e.
+00000100: 6a0d 640e 640f 8d01 6602 6410 6506 6a0e  j.d.d...f.d.e.j.
+00000110: 6407 6411 8d01 6602 6705 641c 640b 6407  d.d...f.g.d.d.d.
+00000120: 6414 9c03 6415 8d03 6504 6a0f 6416 6417  d...d...e.j.d.d.
+00000130: 6418 6901 6419 8d02 6702 5a10 641a 5300  d.i.d...g.Z.d.S.
+00000140: 291d da09 4d69 6772 6174 696f 6eda 0d64  )...Migration..d
+00000150: 6a63 6f6e 6e65 6374 7769 7365 da16 3030  jconnectwise..00
+00000160: 3232 5f6f 7070 6f72 7475 6e69 7479 7374  22_opportunityst
+00000170: 6174 7573 da0f 4f70 706f 7274 756e 6974  atus..Opportunit
+00000180: 7954 7970 65da 0269 64da 0249 4454 4629  yType..id..IDTF)
+00000190: 04da 0c76 6572 626f 7365 5f6e 616d 65da  ...verbose_name.
+000001a0: 0b70 7269 6d61 7279 5f6b 6579 da09 7365  .primary_key..se
+000001b0: 7269 616c 697a 65da 0c61 7574 6f5f 6372  rialize..auto_cr
+000001c0: 6561 7465 64da 0763 7265 6174 6564 2902  eated..created).
+000001d0: 720b 0000 00da 0c61 7574 6f5f 6e6f 775f  r......auto_now_
+000001e0: 6164 64da 086d 6f64 6966 6965 6429 0272  add..modified).r
+000001f0: 0b00 0000 da08 6175 746f 5f6e 6f77 da0b  ......auto_now..
+00000200: 6465 7363 7269 7074 696f 6ee9 3200 0000  description.2...
+00000210: 2901 da0a 6d61 785f 6c65 6e67 7468 da0d  )...max_length..
+00000220: 696e 6163 7469 7665 5f66 6c61 6729 01da  inactive_flag)..
+00000230: 0764 6566 6175 6c74 fa09 2d6d 6f64 6966  .default..-modif
+00000240: 6965 64fa 082d 6372 6561 7465 6429 03da  ied..-created)..
+00000250: 086f 7264 6572 696e 67da 0d67 6574 5f6c  .ordering..get_l
+00000260: 6174 6573 745f 6279 da08 6162 7374 7261  atest_by..abstra
+00000270: 6374 2903 da04 6e61 6d65 da06 6669 656c  ct)...name..fiel
+00000280: 6473 da07 6f70 7469 6f6e 73da 116f 7070  ds..options..opp
+00000290: 6f72 7475 6e69 7479 7374 6174 7573 da13  ortunitystatus..
+000002a0: 7665 7262 6f73 655f 6e61 6d65 5f70 6c75  verbose_name_plu
+000002b0: 7261 6c7a 144f 7070 6f72 7475 6e69 7479  ralz.Opportunity
+000002c0: 2053 7461 7475 7365 7329 0272 1d00 0000   Statuses).r....
+000002d0: 721f 0000 004e 2902 7206 0000 0072 0700  r....N).r....r..
+000002e0: 0000 2902 7218 0000 0072 1900 0000 2911  ..).r....r....).
+000002f0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000300: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000310: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
+00000320: 6573 7203 0000 00da 0b43 7265 6174 654d  esr......CreateM
+00000330: 6f64 656c 7204 0000 00da 0941 7574 6f46  odelr......AutoF
+00000340: 6965 6c64 da11 646a 616e 676f 5f65 7874  ield..django_ext
+00000350: 656e 7369 6f6e 73da 0264 6272 1e00 0000  ensions..dbr....
+00000360: da15 4372 6561 7469 6f6e 4461 7465 5469  ..CreationDateTi
+00000370: 6d65 4669 656c 64da 194d 6f64 6966 6963  meField..Modific
+00000380: 6174 696f 6e44 6174 6554 696d 6546 6965  ationDateTimeFie
+00000390: 6c64 da09 4368 6172 4669 656c 64da 0c42  ld..CharField..B
+000003a0: 6f6f 6c65 616e 4669 656c 64da 1141 6c74  ooleanField..Alt
+000003b0: 6572 4d6f 6465 6c4f 7074 696f 6e73 da0a  erModelOptions..
+000003c0: 6f70 6572 6174 696f 6e73 a900 7230 0000  operations..r0..
+000003d0: 0072 3000 0000 fa63 2f68 6f6d 652f 6361  .r0....c/home/ca
+000003e0: 6d65 726f 6e2f 4465 762f 6b61 6e62 616e  meron/Dev/kanban
+000003f0: 2d64 6576 2f64 6a61 6e67 6f2d 636f 6e6e  -dev/django-conn
+00000400: 6563 7477 6973 652f 646a 636f 6e6e 6563  ectwise/djconnec
+00000410: 7477 6973 652f 6d69 6772 6174 696f 6e73  twise/migrations
+00000420: 2f30 3032 335f 6175 746f 5f32 3031 3730  /0023_auto_20170
+00000430: 3630 355f 3037 3035 2e70 7972 0500 0000  605_0705.pyr....
+00000440: 0800 0000 731c 0000 0008 0306 0404 0102  ....s...........
+00000450: 0214 0114 0114 010e 0110 0302 0102 010a  ................
+00000460: 0304 0102 0172 0500 0000 2908 da0a 5f5f  .....r....)...__
+00000470: 6675 7475 7265 5f5f 7202 0000 00da 0964  future__r......d
+00000480: 6a61 6e67 6f2e 6462 7203 0000 0072 0400  jango.dbr....r..
+00000490: 0000 da1b 646a 616e 676f 5f65 7874 656e  ....django_exten
+000004a0: 7369 6f6e 732e 6462 2e66 6965 6c64 7372  sions.db.fieldsr
+000004b0: 2800 0000 7205 0000 0072 3000 0000 7230  (...r....r0...r0
+000004c0: 0000 0072 3000 0000 7231 0000 00da 083c  ...r0...r1.....<
+000004d0: 6d6f 6475 6c65 3e02 0000 0073 0600 0000  module>....s....
+000004e0: 0c02 1001 0803                           ......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0093_merge_20190716_1459.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0100_auto_20190718_1417.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,47 @@
-00000000: 160d 0d0a 22b1 305d 1601 0000 e300 0000  ....".0]........
+00000000: 330d 0d0a 2a3e 545d 0302 0000 e300 0000  3...*>T]........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
-00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
-00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
-00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
-00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
-00000070: 0000 0000 0003 0000 0040 0000 0073 2200  .........@...s".
-00000080: 0000 6500 005a 0100 6400 005a 0200 6405  ..e..Z..d..Z..d.
-00000090: 0064 0600 6702 005a 0300 6700 005a 0400  .d..g..Z..g..Z..
-000000a0: 6404 0053 2907 da09 4d69 6772 6174 696f  d..S)...Migratio
-000000b0: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
-000000c0: da0d 3030 3931 5f77 6f72 6b72 6f6c 65da  ..0091_workrole.
-000000d0: 1c30 3039 325f 7265 6d6f 7665 5f74 6963  .0092_remove_tic
-000000e0: 6b65 745f 776f 726b 5f74 7970 654e 2902  ket_work_typeN).
-000000f0: fa0d 646a 636f 6e6e 6563 7477 6973 6572  ..djconnectwiser
-00000100: 0500 0000 2902 7207 0000 007a 1c30 3039  ....).r....z.009
-00000110: 325f 7265 6d6f 7665 5f74 6963 6b65 745f  2_remove_ticket_
-00000120: 776f 726b 5f74 7970 6529 05da 085f 5f6e  work_type)...__n
-00000130: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000140: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000150: 0c64 6570 656e 6465 6e63 6965 73da 0a6f  .dependencies..o
-00000160: 7065 7261 7469 6f6e 73a9 0072 0d00 0000  perations..r....
-00000170: 720d 0000 00fa 6f2f 686f 6d65 2f73 616d  r.....o/home/sam
-00000180: 2f67 6974 2f4b 616e 6261 6e2f 646a 616e  /git/Kanban/djan
-00000190: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
-000001a0: 6a61 6e67 6f2d 636f 6e6e 6563 7477 6973  jango-connectwis
-000001b0: 652f 646a 636f 6e6e 6563 7477 6973 652f  e/djconnectwise/
-000001c0: 6d69 6772 6174 696f 6e73 2f30 3039 335f  migrations/0093_
-000001d0: 6d65 7267 655f 3230 3139 3037 3136 5f31  merge_20190716_1
-000001e0: 3435 392e 7079 7203 0000 0006 0000 0073  459.pyr........s
-000001f0: 0600 0000 0c03 0301 0903 7203 0000 004e  ..........r....N
-00000200: 2903 da09 646a 616e 676f 2e64 6272 0200  )...django.dbr..
-00000210: 0000 7203 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00000220: 0072 0d00 0000 720e 0000 00da 083c 6d6f  .r....r......<mo
-00000230: 6475 6c65 3e03 0000 0073 0200 0000 1003  dule>....s......
+00000020: 0073 2e00 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 4700  m.Z...d.d.l.Z.G.
+00000040: 6403 6404 8400 6404 6501 6a05 8303 5a05  d.d...d.e.j...Z.
+00000050: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 734e 6300 0000 0000 0000 0000 0000 0009  sNc.............
+00000080: 0000 0040 0000 0073 3a00 0000 6500 5a01  ...@...s:...e.Z.
+00000090: 6400 5a02 640a 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000a0: 6404 6506 6a07 6405 6405 6508 6a09 6a06  d.e.j.d.d.e.j.j.
+000000b0: 6a0a 6a0b 6406 6407 8d04 6408 8d03 6701  j.j.d.d...d...g.
+000000c0: 5a0c 6409 5300 290b da09 4d69 6772 6174  Z.d.S.)...Migrat
+000000d0: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
+000000e0: 7365 da18 3030 3939 5f74 696d 6565 6e74  se..0099_timeent
+000000f0: 7279 5f61 6772 6565 6d65 6e74 da09 7469  ry_agreement..ti
+00000100: 6d65 656e 7472 79da 0961 6772 6565 6d65  meentry..agreeme
+00000110: 6e74 547a 1764 6a63 6f6e 6e65 6374 7769  ntTz.djconnectwi
+00000120: 7365 2e41 6772 6565 6d65 6e74 2904 da05  se.Agreement)...
+00000130: 626c 616e 6bda 046e 756c 6cda 096f 6e5f  blank..null..on_
+00000140: 6465 6c65 7465 da02 746f 2903 da0a 6d6f  delete..to)...mo
+00000150: 6465 6c5f 6e61 6d65 da04 6e61 6d65 da05  del_name..name..
+00000160: 6669 656c 644e 2902 7205 0000 0072 0600  fieldN).r....r..
+00000170: 0000 290d da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+00000180: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000190: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
+000001a0: 656e 6369 6573 7202 0000 00da 0a41 6c74  enciesr......Alt
+000001b0: 6572 4669 656c 6472 0300 0000 da0a 466f  erFieldr......Fo
+000001c0: 7265 6967 6e4b 6579 da06 646a 616e 676f  reignKey..django
+000001d0: da02 6462 da08 6465 6c65 7469 6f6e da08  ..db..deletion..
+000001e0: 5345 545f 4e55 4c4c da0a 6f70 6572 6174  SET_NULL..operat
+000001f0: 696f 6e73 a900 721b 0000 0072 1b00 0000  ions..r....r....
+00000200: fa63 2f68 6f6d 652f 6361 6d65 726f 6e2f  .c/home/cameron/
+00000210: 4465 762f 6b61 6e62 616e 2d64 6576 2f64  Dev/kanban-dev/d
+00000220: 6a61 6e67 6f2d 636f 6e6e 6563 7477 6973  jango-connectwis
+00000230: 652f 646a 636f 6e6e 6563 7477 6973 652f  e/djconnectwise/
+00000240: 6d69 6772 6174 696f 6e73 2f30 3130 305f  migrations/0100_
+00000250: 6175 746f 5f32 3031 3930 3731 385f 3134  auto_20190718_14
+00000260: 3137 2e70 7972 0400 0000 0700 0000 730a  17.pyr........s.
+00000270: 0000 0008 0306 0404 0102 0102 0172 0400  .............r..
+00000280: 0000 2906 da09 646a 616e 676f 2e64 6272  ..)...django.dbr
+00000290: 0200 0000 7203 0000 00da 1964 6a61 6e67  ....r......djang
+000002a0: 6f2e 6462 2e6d 6f64 656c 732e 6465 6c65  o.db.models.dele
+000002b0: 7469 6f6e 7216 0000 0072 0400 0000 721b  tionr....r....r.
+000002c0: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
+000002d0: 0000 da08 3c6d 6f64 756c 653e 0300 0000  ....<module>....
+000002e0: 7304 0000 0010 0108 03                   s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0011_company_deleted_flag.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0118_auto_20200623_1016.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,40 @@
-00000000: 160d 0d0a a4b0 1f5d a901 0000 e300 0000  .......]........
+00000000: 330d 0d0a 8740 f55e a801 0000 e300 0000  3....@.^........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0009 0000 0040 0000 0073  ...........@...s
-000000b0: 4600 0000 6500 005a 0100 6400 005a 0200  F...e..Z..d..Z..
-000000c0: 640b 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 6408 0064 0900 8300 0183 0003  .j..d..d........
-000000f0: 6701 005a 0800 640a 0053 290c da09 4d69  g..Z..d..S)...Mi
-00000100: 6772 6174 696f 6eda 0d64 6a63 6f6e 6e65  gration..djconne
-00000110: 6374 7769 7365 da20 3030 3130 5f72 656d  ctwise. 0010_rem
-00000120: 6f76 655f 7072 6f6a 6563 745f 7072 6f6a  ove_project_proj
-00000130: 6563 745f 6872 6566 da0a 6d6f 6465 6c5f  ect_href..model_
-00000140: 6e61 6d65 da07 636f 6d70 616e 79da 046e  name..company..n
-00000150: 616d 65da 0c64 656c 6574 6564 5f66 6c61  ame..deleted_fla
-00000160: 67da 0566 6965 6c64 da07 6465 6661 756c  g..field..defaul
-00000170: 7446 4e29 027a 0d64 6a63 6f6e 6e65 6374  tFN).z.djconnect
-00000180: 7769 7365 7207 0000 0029 09da 085f 5f6e  wiser....)...__n
-00000190: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-000001a0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-000001b0: 0c64 6570 656e 6465 6e63 6965 7372 0300  .dependenciesr..
-000001c0: 0000 da08 4164 6446 6965 6c64 7204 0000  ....AddFieldr...
-000001d0: 00da 0c42 6f6f 6c65 616e 4669 656c 64da  ...BooleanField.
-000001e0: 0a6f 7065 7261 7469 6f6e 73a9 0072 1500  .operations..r..
-000001f0: 0000 7215 0000 00fa 702f 686f 6d65 2f73  ..r.....p/home/s
-00000200: 616d 2f67 6974 2f4b 616e 6261 6e2f 646a  am/git/Kanban/dj
-00000210: 616e 676f 2d63 6f6e 6e65 6374 7769 7365  ango-connectwise
-00000220: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
-00000230: 6973 652f 646a 636f 6e6e 6563 7477 6973  ise/djconnectwis
-00000240: 652f 6d69 6772 6174 696f 6e73 2f30 3031  e/migrations/001
-00000250: 315f 636f 6d70 616e 795f 6465 6c65 7465  1_company_delete
-00000260: 645f 666c 6167 2e70 7972 0500 0000 0700  d_flag.pyr......
-00000270: 0000 730a 0000 000c 0309 0409 0106 0106  ..s.............
-00000280: 0172 0500 0000 4e29 06da 0a5f 5f66 7574  .r....N)...__fut
-00000290: 7572 655f 5f72 0200 0000 da09 646a 616e  ure__r......djan
-000002a0: 676f 2e64 6272 0300 0000 7204 0000 0072  go.dbr....r....r
-000002b0: 0500 0000 7215 0000 0072 1500 0000 7215  ....r....r....r.
-000002c0: 0000 0072 1600 0000 da08 3c6d 6f64 756c  ...r......<modul
-000002d0: 653e 0200 0000 7304 0000 0010 0216 03    e>....s........
+00000020: 0073 2600 0000 6400 6401 6c00 6d01 5a01  .s&...d.d.l.m.Z.
+00000030: 6d02 5a02 0100 4700 6402 6403 8400 6403  m.Z...G.d.d...d.
+00000040: 6501 6a03 8303 5a03 6404 5300 2905 e900  e.j...Z.d.S.)...
+00000050: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
+00000060: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000070: 0000 0000 0000 0800 0000 4000 0000 7330  ..........@...s0
+00000080: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+00000090: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000a0: 0664 0564 078d 0364 088d 0367 015a 0864  .d.d...d...g.Z.d
+000000b0: 0953 0029 0bda 094d 6967 7261 7469 6f6e  .S.)...Migration
+000000c0: da0d 646a 636f 6e6e 6563 7477 6973 65da  ..djconnectwise.
+000000d0: 1730 3131 375f 6175 746f 5f32 3032 3030  .0117_auto_20200
+000000e0: 3630 395f 3135 3134 da06 6d65 6d62 6572  609_1514..member
+000000f0: da0c 6f66 6669 6365 5f65 6d61 696c 54e9  ..office_emailT.
+00000100: fa00 0000 2903 da05 626c 616e 6bda 0a6d  ....)...blank..m
+00000110: 6178 5f6c 656e 6774 68da 046e 756c 6c29  ax_length..null)
+00000120: 03da 0a6d 6f64 656c 5f6e 616d 65da 046e  ...model_name..n
+00000130: 616d 65da 0566 6965 6c64 4e29 0272 0500  ame..fieldN).r..
+00000140: 0000 7206 0000 0029 09da 085f 5f6e 616d  ..r....)...__nam
+00000150: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000160: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
+00000170: 6570 656e 6465 6e63 6965 7372 0200 0000  ependenciesr....
+00000180: da0a 416c 7465 7246 6965 6c64 7203 0000  ..AlterFieldr...
+00000190: 00da 0a45 6d61 696c 4669 656c 64da 0a6f  ...EmailField..o
+000001a0: 7065 7261 7469 6f6e 73a9 0072 1700 0000  perations..r....
+000001b0: 7217 0000 00fa 632f 686f 6d65 2f63 616d  r.....c/home/cam
+000001c0: 6572 6f6e 2f44 6576 2f6b 616e 6261 6e2d  eron/Dev/kanban-
+000001d0: 6465 762f 646a 616e 676f 2d63 6f6e 6e65  dev/django-conne
+000001e0: 6374 7769 7365 2f64 6a63 6f6e 6e65 6374  ctwise/djconnect
+000001f0: 7769 7365 2f6d 6967 7261 7469 6f6e 732f  wise/migrations/
+00000200: 3031 3138 5f61 7574 6f5f 3230 3230 3036  0118_auto_202006
+00000210: 3233 5f31 3031 362e 7079 7204 0000 0006  23_1016.pyr.....
+00000220: 0000 0073 0a00 0000 0803 0604 0401 0201  ...s............
+00000230: 0201 7204 0000 004e 2904 da09 646a 616e  ..r....N)...djan
+00000240: 676f 2e64 6272 0200 0000 7203 0000 0072  go.dbr....r....r
+00000250: 0400 0000 7217 0000 0072 1700 0000 7217  ....r....r....r.
+00000260: 0000 0072 1800 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000270: 653e 0300 0000 7302 0000 0010 03         e>....s......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0117_auto_20200609_1514.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0101_agreement_company.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,46 @@
-00000000: 160d 0d0a d70d e85e 7a03 0000 e300 0000  .......^z.......
+00000000: 330d 0d0a 2a3e 545d f001 0000 e300 0000  3...*>T]........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 1100 0000 4000 0000 73c4 0000 0065 0000  ....@...s....e..
-000000a0: 5a01 0064 0000 5a02 0064 1800 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6407 0065 0600 6a07 0064 0800  .d..d..e..j..d..
-000000d0: 6409 0083 0001 8300 0365 0400 6a05 0064  d........e..j..d
-000000e0: 0300 640a 0064 0500 640b 0064 0700 6506  ..d..d..d..d..e.
-000000f0: 006a 0800 640c 0064 0d00 640e 0064 0d00  .j..d..d..d..d..
-00000100: 640f 0065 0900 6a0a 006a 0600 6a0b 006a  d..e..j..j..j..j
-00000110: 0c00 6410 0064 1100 8300 0483 0003 6504  ..d..d........e.
-00000120: 006a 0500 6403 0064 0a00 6405 0064 1200  .j..d..d..d..d..
-00000130: 6407 0065 0600 6a0d 0064 0c00 640d 0064  d..e..j..d..d..d
-00000140: 1300 6414 0064 1500 6416 0064 0e00 640d  ..d..d..d..d..d.
-00000150: 0083 0004 8300 0367 0300 5a0e 0064 1700  .......g..Z..d..
-00000160: 5329 19da 094d 6967 7261 7469 6f6e da0d  S)...Migration..
-00000170: 646a 636f 6e6e 6563 7477 6973 65da 1730  djconnectwise..0
-00000180: 3131 365f 6175 746f 5f32 3032 3030 3532  116_auto_2020052
-00000190: 325f 3131 3037 da0a 6d6f 6465 6c5f 6e61  2_1107..model_na
-000001a0: 6d65 da10 636f 6e6e 6563 7477 6973 6562  me..connectwiseb
-000001b0: 6f61 7264 da04 6e61 6d65 da0c 7072 6f6a  oard..name..proj
-000001c0: 6563 745f 666c 6167 da05 6669 656c 64da  ect_flag..field.
-000001d0: 0764 6566 6175 6c74 46da 0770 726f 6a65  .defaultF..proje
-000001e0: 6374 da05 626f 6172 64da 0562 6c61 6e6b  ct..board..blank
-000001f0: 54da 046e 756c 6cda 096f 6e5f 6465 6c65  T..null..on_dele
-00000200: 7465 da02 746f 7a1e 646a 636f 6e6e 6563  te..toz.djconnec
-00000210: 7477 6973 652e 436f 6e6e 6563 7457 6973  twise.ConnectWis
-00000220: 6542 6f61 7264 da10 7065 7263 656e 745f  eBoard..percent_
-00000230: 636f 6d70 6c65 7465 da0e 6465 6369 6d61  complete..decima
-00000240: 6c5f 706c 6163 6573 e902 0000 00da 0a6d  l_places.......m
-00000250: 6178 5f64 6967 6974 73e9 0300 0000 4e29  ax_digits.....N)
-00000260: 027a 0d64 6a63 6f6e 6e65 6374 7769 7365  .z.djconnectwise
-00000270: 7206 0000 0029 0fda 085f 5f6e 616d 655f  r....)...__name_
-00000280: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000290: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
-000002a0: 656e 6465 6e63 6965 7372 0200 0000 da08  endenciesr......
-000002b0: 4164 6446 6965 6c64 7203 0000 00da 0c42  AddFieldr......B
-000002c0: 6f6f 6c65 616e 4669 656c 64da 0a46 6f72  ooleanField..For
-000002d0: 6569 676e 4b65 79da 0664 6a61 6e67 6fda  eignKey..django.
-000002e0: 0264 62da 0864 656c 6574 696f 6eda 0743  .db..deletion..C
-000002f0: 4153 4341 4445 da0c 4465 6369 6d61 6c46  ASCADE..DecimalF
-00000300: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
-00000310: a900 7225 0000 0072 2500 0000 fa6e 2f68  ..r%...r%....n/h
-00000320: 6f6d 652f 7361 6d2f 6769 742f 4b61 6e62  ome/sam/git/Kanb
-00000330: 616e 2f64 6a61 6e67 6f2d 636f 6e6e 6563  an/django-connec
-00000340: 7477 6973 652f 646a 616e 676f 2d63 6f6e  twise/django-con
-00000350: 6e65 6374 7769 7365 2f64 6a63 6f6e 6e65  nectwise/djconne
-00000360: 6374 7769 7365 2f6d 6967 7261 7469 6f6e  ctwise/migration
-00000370: 732f 3031 3137 5f61 7574 6f5f 3230 3230  s/0117_auto_2020
-00000380: 3036 3039 5f31 3531 342e 7079 7204 0000  0609_1514.pyr...
-00000390: 0007 0000 0073 1a00 0000 0c03 0904 0901  .....s..........
-000003a0: 0601 0601 1202 0901 0601 0601 3002 0901  ............0...
-000003b0: 0601 0601 7204 0000 0029 06da 0964 6a61  ....r....)...dja
-000003c0: 6e67 6f2e 6462 7202 0000 0072 0300 0000  ngo.dbr....r....
-000003d0: da19 646a 616e 676f 2e64 622e 6d6f 6465  ..django.db.mode
-000003e0: 6c73 2e64 656c 6574 696f 6e72 1f00 0000  ls.deletionr....
-000003f0: 7204 0000 0072 2500 0000 7225 0000 0072  r....r%...r%...r
-00000400: 2500 0000 7226 0000 00da 083c 6d6f 6475  %...r&.....<modu
-00000410: 6c65 3e03 0000 0073 0400 0000 1601 0c03  le>....s........
+00000020: 0073 2e00 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 4700  m.Z...d.d.l.Z.G.
+00000040: 6403 6404 8400 6404 6501 6a05 8303 5a05  d.d...d.e.j...Z.
+00000050: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 734e 6300 0000 0000 0000 0000 0000 0008  sNc.............
+00000080: 0000 0040 0000 0073 3800 0000 6500 5a01  ...@...s8...e.Z.
+00000090: 6400 5a02 640a 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000a0: 6404 6506 6a07 6405 6508 6a09 6a06 6a0a  d.e.j.d.e.j.j.j.
+000000b0: 6a0b 6406 6407 8d03 6408 8d03 6701 5a0c  j.d.d...d...g.Z.
+000000c0: 6409 5300 290b da09 4d69 6772 6174 696f  d.S.)...Migratio
+000000d0: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
+000000e0: da17 3031 3030 5f61 7574 6f5f 3230 3139  ..0100_auto_2019
+000000f0: 3037 3138 5f31 3431 37da 0961 6772 6565  0718_1417..agree
+00000100: 6d65 6e74 da07 636f 6d70 616e 7954 7a15  ment..companyTz.
+00000110: 646a 636f 6e6e 6563 7477 6973 652e 436f  djconnectwise.Co
+00000120: 6d70 616e 7929 03da 046e 756c 6cda 096f  mpany)...null..o
+00000130: 6e5f 6465 6c65 7465 da02 746f 2903 da0a  n_delete..to)...
+00000140: 6d6f 6465 6c5f 6e61 6d65 da04 6e61 6d65  model_name..name
+00000150: da05 6669 656c 644e 2902 7205 0000 0072  ..fieldN).r....r
+00000160: 0600 0000 290d da08 5f5f 6e61 6d65 5f5f  ....)...__name__
+00000170: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000180: 7175 616c 6e61 6d65 5f5f da0c 6465 7065  qualname__..depe
+00000190: 6e64 656e 6369 6573 7202 0000 00da 0841  ndenciesr......A
+000001a0: 6464 4669 656c 6472 0300 0000 da0a 466f  ddFieldr......Fo
+000001b0: 7265 6967 6e4b 6579 da06 646a 616e 676f  reignKey..django
+000001c0: da02 6462 da08 6465 6c65 7469 6f6e da08  ..db..deletion..
+000001d0: 5345 545f 4e55 4c4c da0a 6f70 6572 6174  SET_NULL..operat
+000001e0: 696f 6e73 a900 721a 0000 0072 1a00 0000  ions..r....r....
+000001f0: fa62 2f68 6f6d 652f 6361 6d65 726f 6e2f  .b/home/cameron/
+00000200: 4465 762f 6b61 6e62 616e 2d64 6576 2f64  Dev/kanban-dev/d
+00000210: 6a61 6e67 6f2d 636f 6e6e 6563 7477 6973  jango-connectwis
+00000220: 652f 646a 636f 6e6e 6563 7477 6973 652f  e/djconnectwise/
+00000230: 6d69 6772 6174 696f 6e73 2f30 3130 315f  migrations/0101_
+00000240: 6167 7265 656d 656e 745f 636f 6d70 616e  agreement_compan
+00000250: 792e 7079 7204 0000 0007 0000 0073 0a00  y.pyr........s..
+00000260: 0000 0803 0604 0401 0201 0201 7204 0000  ............r...
+00000270: 0029 06da 0964 6a61 6e67 6f2e 6462 7202  .)...django.dbr.
+00000280: 0000 0072 0300 0000 da19 646a 616e 676f  ...r......django
+00000290: 2e64 622e 6d6f 6465 6c73 2e64 656c 6574  .db.models.delet
+000002a0: 696f 6e72 1500 0000 7204 0000 0072 1a00  ionr....r....r..
+000002b0: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+000002c0: 00da 083c 6d6f 6475 6c65 3e03 0000 0073  ...<module>....s
+000002d0: 0400 0000 1001 0803                      ........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0110_project_company.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0067_auto_20180813_1355.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,39 @@
-00000000: 160d 0d0a c118 795d f701 0000 e300 0000  ......y]........
+00000000: 330d 0d0a 10ec da5c ec01 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 0f00 0000 4000 0000 7364 0000 0065 0000  ....@...sd...e..
-000000a0: 5a01 0064 0000 5a02 0064 0f00 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6407 0065 0600 6a07 0064 0800  .d..d..e..j..d..
-000000d0: 6409 0064 0a00 6409 0064 0b00 6508 006a  d..d..d..d..e..j
-000000e0: 0900 6a06 006a 0a00 6a0b 0064 0c00 640d  ..j..j..j..d..d.
-000000f0: 0083 0004 8300 0367 0100 5a0c 0064 0e00  .......g..Z..d..
-00000100: 5329 10da 094d 6967 7261 7469 6f6e da0d  S)...Migration..
-00000110: 646a 636f 6e6e 6563 7477 6973 65da 1130  djconnectwise..0
-00000120: 3130 395f 7469 636b 6574 5f70 6861 7365  109_ticket_phase
-00000130: da0a 6d6f 6465 6c5f 6e61 6d65 da07 7072  ..model_name..pr
-00000140: 6f6a 6563 74da 046e 616d 65da 0763 6f6d  oject..name..com
-00000150: 7061 6e79 da05 6669 656c 64da 0562 6c61  pany..field..bla
-00000160: 6e6b 54da 046e 756c 6cda 096f 6e5f 6465  nkT..null..on_de
-00000170: 6c65 7465 da02 746f 7a15 646a 636f 6e6e  lete..toz.djconn
-00000180: 6563 7477 6973 652e 436f 6d70 616e 794e  ectwise.CompanyN
-00000190: 2902 7a0d 646a 636f 6e6e 6563 7477 6973  ).z.djconnectwis
-000001a0: 6572 0600 0000 290d da08 5f5f 6e61 6d65  er....)...__name
-000001b0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-000001c0: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
-000001d0: 7065 6e64 656e 6369 6573 7202 0000 00da  pendenciesr.....
-000001e0: 0841 6464 4669 656c 6472 0300 0000 da0a  .AddFieldr......
-000001f0: 466f 7265 6967 6e4b 6579 da06 646a 616e  ForeignKey..djan
-00000200: 676f da02 6462 da08 6465 6c65 7469 6f6e  go..db..deletion
-00000210: da08 5345 545f 4e55 4c4c da0a 6f70 6572  ..SET_NULL..oper
-00000220: 6174 696f 6e73 a900 721b 0000 0072 1b00  ations..r....r..
-00000230: 0000 fa6b 2f68 6f6d 652f 7361 6d2f 6769  ...k/home/sam/gi
-00000240: 742f 4b61 6e62 616e 2f64 6a61 6e67 6f2d  t/Kanban/django-
-00000250: 636f 6e6e 6563 7477 6973 652f 646a 616e  connectwise/djan
-00000260: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
-00000270: 6a63 6f6e 6e65 6374 7769 7365 2f6d 6967  jconnectwise/mig
-00000280: 7261 7469 6f6e 732f 3031 3130 5f70 726f  rations/0110_pro
-00000290: 6a65 6374 5f63 6f6d 7061 6e79 2e70 7972  ject_company.pyr
-000002a0: 0400 0000 0700 0000 730a 0000 000c 0309  ........s.......
-000002b0: 0409 0106 0106 0172 0400 0000 2906 da09  .......r....)...
-000002c0: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
-000002d0: 0000 00da 1964 6a61 6e67 6f2e 6462 2e6d  .....django.db.m
-000002e0: 6f64 656c 732e 6465 6c65 7469 6f6e 7216  odels.deletionr.
-000002f0: 0000 0072 0400 0000 721b 0000 0072 1b00  ...r....r....r..
-00000300: 0000 721b 0000 0072 1c00 0000 da08 3c6d  ..r....r......<m
-00000310: 6f64 756c 653e 0300 0000 7304 0000 0016  odule>....s.....
-00000320: 010c 03                                  ...
+00000020: 0073 2200 0000 6400 6401 6c00 6d01 5a01  .s"...d.d.l.m.Z.
+00000030: 0100 4700 6402 6403 8400 6403 6501 6a02  ..G.d.d...d.e.j.
+00000040: 8303 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
+00000050: 01da 0a6d 6967 7261 7469 6f6e 7363 0000  ...migrationsc..
+00000060: 0000 0000 0000 0000 0000 0500 0000 4000  ..............@.
+00000070: 0000 7336 0000 0065 005a 0164 005a 0264  ..s6...e.Z.d.Z.d
+00000080: 0a67 015a 0365 046a 0564 0364 0464 0569  .g.Z.e.j.d.d.d.i
+00000090: 0164 068d 0265 046a 0564 0764 0464 0869  .d...e.j.d.d.d.i
+000000a0: 0164 068d 0267 025a 0664 0953 0029 0bda  .d...g.Z.d.S.)..
+000000b0: 094d 6967 7261 7469 6f6e da0d 646a 636f  .Migration..djco
+000000c0: 6e6e 6563 7477 6973 65da 1030 3036 365f  nnectwise..0066_
+000000d0: 736c 6170 7269 6f72 6974 79da 0373 6c61  slapriority..sla
+000000e0: da13 7665 7262 6f73 655f 6e61 6d65 5f70  ..verbose_name_p
+000000f0: 6c75 7261 6cda 0453 4c41 7329 02da 046e  lural..SLAs)...n
+00000100: 616d 65da 076f 7074 696f 6e73 5a0b 736c  ame..optionsZ.sl
+00000110: 6170 7269 6f72 6974 797a 0e53 4c41 2050  apriorityz.SLA P
+00000120: 7269 6f72 6974 6965 734e 2902 7204 0000  rioritiesN).r...
+00000130: 0072 0500 0000 2907 da08 5f5f 6e61 6d65  .r....)...__name
+00000140: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000150: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
+00000160: 7065 6e64 656e 6369 6573 7202 0000 00da  pendenciesr.....
+00000170: 1141 6c74 6572 4d6f 6465 6c4f 7074 696f  .AlterModelOptio
+00000180: 6e73 da0a 6f70 6572 6174 696f 6e73 a900  ns..operations..
+00000190: 7211 0000 0072 1100 0000 fa63 2f68 6f6d  r....r.....c/hom
+000001a0: 652f 6361 6d65 726f 6e2f 4465 762f 6b61  e/cameron/Dev/ka
+000001b0: 6e62 616e 2d64 6576 2f64 6a61 6e67 6f2d  nban-dev/django-
+000001c0: 636f 6e6e 6563 7477 6973 652f 646a 636f  connectwise/djco
+000001d0: 6e6e 6563 7477 6973 652f 6d69 6772 6174  nnectwise/migrat
+000001e0: 696f 6e73 2f30 3036 375f 6175 746f 5f32  ions/0067_auto_2
+000001f0: 3031 3830 3831 335f 3133 3535 2e70 7972  0180813_1355.pyr
+00000200: 0300 0000 0600 0000 730e 0000 0008 0306  ........s.......
+00000210: 0404 0102 010a 0204 0102 0172 0300 0000  ...........r....
+00000220: 4e29 03da 0964 6a61 6e67 6f2e 6462 7202  N)...django.dbr.
+00000230: 0000 0072 0300 0000 7211 0000 0072 1100  ...r....r....r..
+00000240: 0000 7211 0000 0072 1200 0000 da08 3c6d  ..r....r......<m
+00000250: 6f64 756c 653e 0300 0000 7302 0000 000c  odule>....s.....
+00000260: 03                                       .
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0081_auto_20181220_0917.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0104_auto_20190722_1232.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,39 @@
-00000000: 160d 0d0a a4b0 1f5d d701 0000 e300 0000  .......]........
+00000000: 330d 0d0a 2a3e 545d 9b01 0000 e300 0000  3...*>T]........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3300 0000 6400 0064 0100 6c00 006d  .s3...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 4764 0200  ..Z..m..Z...Gd..
-00000040: 6403 0084 0000 6403 0065 0100 6a03 0083  d.....d..e..j...
-00000050: 0300 5a03 0064 0400 5329 05e9 0000 0000  ..Z..d..S)......
-00000060: 2902 da0a 6d69 6772 6174 696f 6e73 da06  )...migrations..
-00000070: 6d6f 6465 6c73 6300 0000 0000 0000 0000  modelsc.........
-00000080: 0000 0011 0000 0040 0000 0073 5e00 0000  .......@...s^...
-00000090: 6500 005a 0100 6400 005a 0200 6411 0067  e..Z..d..Z..d..g
-000000a0: 0100 5a03 0065 0400 6a05 0064 0300 6404  ..Z..e..j..d..d.
-000000b0: 0064 0500 6406 0064 0700 6506 006a 0700  .d..d..d..e..j..
-000000c0: 6408 0064 0900 640a 0064 0b00 640c 0064  d..d..d..d..d..d
-000000d0: 0d00 640e 0064 0900 640f 0064 0b00 8300  ..d..d..d..d....
-000000e0: 0583 0003 6701 005a 0800 6410 0053 2912  ....g..Z..d..S).
-000000f0: da09 4d69 6772 6174 696f 6eda 0d64 6a63  ..Migration..djc
-00000100: 6f6e 6e65 6374 7769 7365 da17 3030 3830  onnectwise..0080
-00000110: 5f61 7574 6f5f 3230 3138 3132 3130 5f30  _auto_20181210_0
-00000120: 3933 30da 0a6d 6f64 656c 5f6e 616d 65da  930..model_name.
-00000130: 066d 656d 6265 72da 046e 616d 65da 0661  .member..name..a
-00000140: 7661 7461 72da 0566 6965 6c64 da05 626c  vatar..field..bl
-00000150: 616e 6b54 da09 6865 6c70 5f74 6578 747a  ankT..help_textz
-00000160: 0d4d 656d 6265 7220 4176 6174 6172 da0a  .Member Avatar..
-00000170: 6d61 785f 6c65 6e67 7468 e9fa 0000 00da  max_length......
-00000180: 046e 756c 6cda 0c76 6572 626f 7365 5f6e  .null..verbose_n
-00000190: 616d 654e 2902 7a0d 646a 636f 6e6e 6563  ameN).z.djconnec
-000001a0: 7477 6973 657a 1730 3038 305f 6175 746f  twisez.0080_auto
-000001b0: 5f32 3031 3831 3231 305f 3039 3330 2909  _20181210_0930).
-000001c0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000001d0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000001e0: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
-000001f0: 6573 7202 0000 00da 0a41 6c74 6572 4669  esr......AlterFi
-00000200: 656c 6472 0300 0000 da09 4368 6172 4669  eldr......CharFi
-00000210: 656c 64da 0a6f 7065 7261 7469 6f6e 73a9  eld..operations.
-00000220: 0072 1900 0000 7219 0000 00fa 6e2f 686f  .r....r.....n/ho
-00000230: 6d65 2f73 616d 2f67 6974 2f4b 616e 6261  me/sam/git/Kanba
-00000240: 6e2f 646a 616e 676f 2d63 6f6e 6e65 6374  n/django-connect
-00000250: 7769 7365 2f64 6a61 6e67 6f2d 636f 6e6e  wise/django-conn
-00000260: 6563 7477 6973 652f 646a 636f 6e6e 6563  ectwise/djconnec
-00000270: 7477 6973 652f 6d69 6772 6174 696f 6e73  twise/migrations
-00000280: 2f30 3038 315f 6175 746f 5f32 3031 3831  /0081_auto_20181
-00000290: 3232 305f 3039 3137 2e70 7972 0400 0000  220_0917.pyr....
-000002a0: 0600 0000 730a 0000 000c 0309 0409 0106  ....s...........
-000002b0: 0106 0172 0400 0000 4e29 04da 0964 6a61  ...r....N)...dja
-000002c0: 6e67 6f2e 6462 7202 0000 0072 0300 0000  ngo.dbr....r....
-000002d0: 7204 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-000002e0: 1900 0000 721a 0000 00da 083c 6d6f 6475  ....r......<modu
-000002f0: 6c65 3e03 0000 0073 0200 0000 1603       le>....s......
+00000020: 0073 2200 0000 6400 6401 6c00 6d01 5a01  .s"...d.d.l.m.Z.
+00000030: 0100 4700 6402 6403 8400 6403 6501 6a02  ..G.d.d...d.e.j.
+00000040: 8303 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
+00000050: 01da 0a6d 6967 7261 7469 6f6e 7363 0000  ...migrationsc..
+00000060: 0000 0000 0000 0000 0000 0500 0000 4000  ..............@.
+00000070: 0000 7328 0000 0065 005a 0164 005a 0264  ..s(...e.Z.d.Z.d
+00000080: 0967 015a 0365 046a 0564 0364 0a64 0564  .g.Z.e.j.d.d.d.d
+00000090: 069c 0264 078d 0267 015a 0664 0853 0029  ...d...g.Z.d.S.)
+000000a0: 0bda 094d 6967 7261 7469 6f6e da0d 646a  ...Migration..dj
+000000b0: 636f 6e6e 6563 7477 6973 65da 2030 3130  connectwise. 010
+000000c0: 335f 6163 7469 7669 7479 7374 6174 7573  3_activitystatus
+000000d0: 5f61 6374 6976 6974 7974 7970 655a 0e61  _activitytypeZ.a
+000000e0: 6374 6976 6974 7973 7461 7475 73da 046e  ctivitystatus..n
+000000f0: 616d 657a 1161 6374 6976 6974 7920 7374  amez.activity st
+00000100: 6174 7573 6573 2902 da08 6f72 6465 7269  atuses)...orderi
+00000110: 6e67 da13 7665 7262 6f73 655f 6e61 6d65  ng..verbose_name
+00000120: 5f70 6c75 7261 6c29 0272 0600 0000 da07  _plural).r......
+00000130: 6f70 7469 6f6e 734e 2902 7204 0000 0072  optionsN).r....r
+00000140: 0500 0000 2901 7206 0000 0029 07da 085f  ....).r....)..._
+00000150: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000160: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000170: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
+00000180: 0200 0000 da11 416c 7465 724d 6f64 656c  ......AlterModel
+00000190: 4f70 7469 6f6e 73da 0a6f 7065 7261 7469  Options..operati
+000001a0: 6f6e 73a9 0072 1000 0000 7210 0000 00fa  ons..r....r.....
+000001b0: 632f 686f 6d65 2f63 616d 6572 6f6e 2f44  c/home/cameron/D
+000001c0: 6576 2f6b 616e 6261 6e2d 6465 762f 646a  ev/kanban-dev/dj
+000001d0: 616e 676f 2d63 6f6e 6e65 6374 7769 7365  ango-connectwise
+000001e0: 2f64 6a63 6f6e 6e65 6374 7769 7365 2f6d  /djconnectwise/m
+000001f0: 6967 7261 7469 6f6e 732f 3031 3034 5f61  igrations/0104_a
+00000200: 7574 6f5f 3230 3139 3037 3232 5f31 3233  uto_20190722_123
+00000210: 322e 7079 7203 0000 0006 0000 0073 0800  2.pyr........s..
+00000220: 0000 0803 0604 0401 0201 7203 0000 004e  ..........r....N
+00000230: 2903 da09 646a 616e 676f 2e64 6272 0200  )...django.dbr..
+00000240: 0000 7203 0000 0072 1000 0000 7210 0000  ..r....r....r...
+00000250: 0072 1000 0000 7211 0000 00da 083c 6d6f  .r....r......<mo
+00000260: 6475 6c65 3e03 0000 0073 0200 0000 0c03  dule>....s......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0067_auto_20180813_1355.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0054_auto_20180501_1009.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-00000000: 160d 0d0a a4b0 1f5d ec01 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c a101 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
-00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
-00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
-00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
-00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
-00000070: 0000 0000 0007 0000 0040 0000 0073 5500  .........@...sU.
-00000080: 0000 6500 005a 0100 6400 005a 0200 640b  ..e..Z..d..Z..d.
-00000090: 0067 0100 5a03 0065 0400 6a05 0064 0300  .g..Z..e..j..d..
-000000a0: 6404 0064 0500 6406 0064 0700 6901 0083  d..d..d..d..i...
-000000b0: 0002 6504 006a 0500 6403 0064 0800 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6409 0069 0100 8300 0267 0200  .d..d..i.....g..
-000000d0: 5a06 0064 0a00 5329 0cda 094d 6967 7261  Z..d..S)...Migra
-000000e0: 7469 6f6e da0d 646a 636f 6e6e 6563 7477  tion..djconnectw
-000000f0: 6973 65da 1030 3036 365f 736c 6170 7269  ise..0066_slapri
-00000100: 6f72 6974 79da 046e 616d 65da 0373 6c61  ority..name..sla
-00000110: da07 6f70 7469 6f6e 73da 1376 6572 626f  ..options..verbo
-00000120: 7365 5f6e 616d 655f 706c 7572 616c da04  se_name_plural..
-00000130: 534c 4173 5a0b 736c 6170 7269 6f72 6974  SLAsZ.slapriorit
-00000140: 797a 0e53 4c41 2050 7269 6f72 6974 6965  yz.SLA Prioritie
-00000150: 734e 2902 7a0d 646a 636f 6e6e 6563 7477  sN).z.djconnectw
-00000160: 6973 6572 0500 0000 2907 da08 5f5f 6e61  iser....)...__na
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0500 0000 4000 0000 7328  ..........@...s(
+000000a0: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0464 0b64 079c 0264  .e.j.d.d.d.d...d
+000000c0: 088d 0267 015a 0664 0953 0029 0cda 094d  ...g.Z.d.S.)...M
+000000d0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
+000000e0: 6563 7477 6973 65da 0a30 3035 335f 6d65  ectwise..0053_me
+000000f0: 7267 65da 0974 696d 6565 6e74 7279 7a0c  rge..timeentryz.
+00000100: 5469 6d65 2045 6e74 7269 6573 fa0b 2d74  Time Entries..-t
+00000110: 696d 655f 7374 6172 74da 0269 6429 02da  ime_start..id)..
+00000120: 1376 6572 626f 7365 5f6e 616d 655f 706c  .verbose_name_pl
+00000130: 7572 616c da08 6f72 6465 7269 6e67 2902  ural..ordering).
+00000140: da04 6e61 6d65 da07 6f70 7469 6f6e 734e  ..name..optionsN
+00000150: 2902 7206 0000 0072 0700 0000 2902 7209  ).r....r....).r.
+00000160: 0000 0072 0a00 0000 2907 da08 5f5f 6e61  ...r....)...__na
 00000170: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 00000180: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
-00000190: 6465 7065 6e64 656e 6369 6573 7202 0000  dependenciesr...
+00000190: 6465 7065 6e64 656e 6369 6573 7203 0000  dependenciesr...
 000001a0: 00da 1141 6c74 6572 4d6f 6465 6c4f 7074  ...AlterModelOpt
 000001b0: 696f 6e73 da0a 6f70 6572 6174 696f 6e73  ions..operations
-000001c0: a900 7211 0000 0072 1100 0000 fa6e 2f68  ..r....r.....n/h
-000001d0: 6f6d 652f 7361 6d2f 6769 742f 4b61 6e62  ome/sam/git/Kanb
-000001e0: 616e 2f64 6a61 6e67 6f2d 636f 6e6e 6563  an/django-connec
-000001f0: 7477 6973 652f 646a 616e 676f 2d63 6f6e  twise/django-con
-00000200: 6e65 6374 7769 7365 2f64 6a63 6f6e 6e65  nectwise/djconne
-00000210: 6374 7769 7365 2f6d 6967 7261 7469 6f6e  ctwise/migration
-00000220: 732f 3030 3637 5f61 7574 6f5f 3230 3138  s/0067_auto_2018
-00000230: 3038 3133 5f31 3335 352e 7079 7203 0000  0813_1355.pyr...
-00000240: 0006 0000 0073 0e00 0000 0c03 0904 0901  .....s..........
-00000250: 0601 0c02 0901 0601 7203 0000 004e 2903  ........r....N).
-00000260: da09 646a 616e 676f 2e64 6272 0200 0000  ..django.dbr....
-00000270: 7203 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00000280: 1100 0000 7212 0000 00da 083c 6d6f 6475  ....r......<modu
-00000290: 6c65 3e03 0000 0073 0200 0000 1003       le>....s......
+000001c0: a900 7215 0000 0072 1500 0000 fa63 2f68  ..r....r.....c/h
+000001d0: 6f6d 652f 6361 6d65 726f 6e2f 4465 762f  ome/cameron/Dev/
+000001e0: 6b61 6e62 616e 2d64 6576 2f64 6a61 6e67  kanban-dev/djang
+000001f0: 6f2d 636f 6e6e 6563 7477 6973 652f 646a  o-connectwise/dj
+00000200: 636f 6e6e 6563 7477 6973 652f 6d69 6772  connectwise/migr
+00000210: 6174 696f 6e73 2f30 3035 345f 6175 746f  ations/0054_auto
+00000220: 5f32 3031 3830 3530 315f 3130 3039 2e70  _20180501_1009.p
+00000230: 7972 0500 0000 0700 0000 7308 0000 0008  yr........s.....
+00000240: 0306 0404 0102 0172 0500 0000 4e29 06da  .......r....N)..
+00000250: 0a5f 5f66 7574 7572 655f 5f72 0200 0000  .__future__r....
+00000260: da09 646a 616e 676f 2e64 6272 0300 0000  ..django.dbr....
+00000270: 7204 0000 0072 0500 0000 7215 0000 0072  r....r....r....r
+00000280: 1500 0000 7215 0000 0072 1600 0000 da08  ....r....r......
+00000290: 3c6d 6f64 756c 653e 0200 0000 7304 0000  <module>....s...
+000002a0: 000c 0210 03                             .....
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0066_auto_20180814_1046.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0066_auto_20180814_1046.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,50 @@
-00000000: 160d 0d0a a4b0 1f5d 2a02 0000 e300 0000  .......]*.......
+00000000: 330d 0d0a 10ec da5c 2a02 0000 e300 0000  3......\*.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3300 0000 6400 0064 0100 6c00 006d  .s3...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 4764 0200  ..Z..m..Z...Gd..
-00000040: 6403 0084 0000 6403 0065 0100 6a03 0083  d.....d..e..j...
-00000050: 0300 5a03 0064 0400 5329 05e9 0000 0000  ..Z..d..S)......
-00000060: 2902 da0a 6d69 6772 6174 696f 6e73 da06  )...migrations..
-00000070: 6d6f 6465 6c73 6300 0000 0000 0000 0000  modelsc.........
-00000080: 0000 000d 0000 0040 0000 0073 5e00 0000  .......@...s^...
-00000090: 6500 005a 0100 6400 005a 0200 6415 0067  e..Z..d..Z..d..g
-000000a0: 0100 5a03 0065 0400 6a05 0064 0300 6404  ..Z..e..j..d..d.
-000000b0: 0064 0500 6406 0064 0700 6506 006a 0700  .d..d..d..e..j..
-000000c0: 6408 0064 1600 6417 0064 1800 6419 0067  d..d..d..d..d..g
-000000d0: 0400 6411 0064 0900 6412 0064 1300 8300  ..d..d..d..d....
-000000e0: 0383 0003 6701 005a 0800 6414 0053 291a  ....g..Z..d..S).
-000000f0: da09 4d69 6772 6174 696f 6eda 0d64 6a63  ..Migration..djc
-00000100: 6f6e 6e65 6374 7769 7365 da17 3030 3635  onnectwise..0065
-00000110: 5f61 7574 6f5f 3230 3138 3038 3039 5f31  _auto_20180809_1
-00000120: 3132 34da 0a6d 6f64 656c 5f6e 616d 65da  124..model_name.
-00000130: 0373 6c61 da04 6e61 6d65 da08 6261 7365  .sla..name..base
-00000140: 645f 6f6e da05 6669 656c 64da 0763 686f  d_on..field..cho
-00000150: 6963 6573 da0a 4d79 4361 6c65 6e64 6172  ices..MyCalendar
-00000160: fa13 4d79 2043 6f6d 7061 6e79 2043 616c  ..My Company Cal
-00000170: 656e 6461 72da 0843 7573 746f 6d65 72fa  endar..Customer.
-00000180: 1343 7573 746f 6d65 7227 7320 4361 6c65  .Customer's Cale
-00000190: 6e64 6172 da08 416c 6c48 6f75 7273 fa08  ndar..AllHours..
-000001a0: 3234 2048 6f75 7273 da06 4375 7374 6f6d  24 Hours..Custom
-000001b0: fa0f 4375 7374 6f6d 2043 616c 656e 6461  ..Custom Calenda
-000001c0: 72da 0764 6566 6175 6c74 da0a 6d61 785f  r..default..max_
-000001d0: 6c65 6e67 7468 e932 0000 004e 2902 7a0d  length.2...N).z.
-000001e0: 646a 636f 6e6e 6563 7477 6973 657a 1730  djconnectwisez.0
-000001f0: 3036 355f 6175 746f 5f32 3031 3830 3830  065_auto_2018080
-00000200: 395f 3131 3234 2902 7a0a 4d79 4361 6c65  9_1124).z.MyCale
-00000210: 6e64 6172 720e 0000 0029 027a 0843 7573  ndarr....).z.Cus
-00000220: 746f 6d65 7272 1000 0000 2902 7a08 416c  tomerr....).z.Al
-00000230: 6c48 6f75 7273 7212 0000 0029 027a 0643  lHoursr....).z.C
-00000240: 7573 746f 6d72 1400 0000 2909 da08 5f5f  ustomr....)...__
-00000250: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000260: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000270: da0c 6465 7065 6e64 656e 6369 6573 7202  ..dependenciesr.
-00000280: 0000 00da 0a41 6c74 6572 4669 656c 6472  .....AlterFieldr
-00000290: 0300 0000 da09 4368 6172 4669 656c 64da  ......CharField.
-000002a0: 0a6f 7065 7261 7469 6f6e 73a9 0072 1f00  .operations..r..
-000002b0: 0000 721f 0000 00fa 6e2f 686f 6d65 2f73  ..r.....n/home/s
-000002c0: 616d 2f67 6974 2f4b 616e 6261 6e2f 646a  am/git/Kanban/dj
-000002d0: 616e 676f 2d63 6f6e 6e65 6374 7769 7365  ango-connectwise
-000002e0: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
-000002f0: 6973 652f 646a 636f 6e6e 6563 7477 6973  ise/djconnectwis
-00000300: 652f 6d69 6772 6174 696f 6e73 2f30 3036  e/migrations/006
-00000310: 365f 6175 746f 5f32 3031 3830 3831 345f  6_auto_20180814_
-00000320: 3130 3436 2e70 7972 0400 0000 0600 0000  1046.pyr........
-00000330: 730a 0000 000c 0309 0409 0106 0106 0172  s..............r
-00000340: 0400 0000 4e29 04da 0964 6a61 6e67 6f2e  ....N)...django.
-00000350: 6462 7202 0000 0072 0300 0000 7204 0000  dbr....r....r...
-00000360: 0072 1f00 0000 721f 0000 0072 1f00 0000  .r....r....r....
-00000370: 7220 0000 00da 083c 6d6f 6475 6c65 3e03  r .....<module>.
-00000380: 0000 0073 0200 0000 1603                 ...s......
+00000020: 0073 2600 0000 6400 6401 6c00 6d01 5a01  .s&...d.d.l.m.Z.
+00000030: 6d02 5a02 0100 4700 6402 6403 8400 6403  m.Z...G.d.d...d.
+00000040: 6501 6a03 8303 5a03 6404 5300 2905 e900  e.j...Z.d.S.)...
+00000050: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
+00000060: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000070: 0000 0000 0000 0900 0000 4000 0000 7338  ..........@...s8
+00000080: 0000 0065 005a 0164 005a 0264 1167 015a  ...e.Z.d.Z.d.g.Z
+00000090: 0365 046a 0564 0364 0465 066a 0764 1264  .e.j.d.d.e.j.d.d
+000000a0: 1364 1464 1567 0464 0564 0d64 0e8d 0364  .d.d.g.d.d.d...d
+000000b0: 0f8d 0367 015a 0864 1053 0029 16da 094d  ...g.Z.d.S.)...M
+000000c0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
+000000d0: 6563 7477 6973 65da 1730 3036 355f 6175  ectwise..0065_au
+000000e0: 746f 5f32 3031 3830 3830 395f 3131 3234  to_20180809_1124
+000000f0: da03 736c 61da 0862 6173 6564 5f6f 6eda  ..sla..based_on.
+00000100: 0a4d 7943 616c 656e 6461 72fa 134d 7920  .MyCalendar..My 
+00000110: 436f 6d70 616e 7920 4361 6c65 6e64 6172  Company Calendar
+00000120: da08 4375 7374 6f6d 6572 fa13 4375 7374  ..Customer..Cust
+00000130: 6f6d 6572 2773 2043 616c 656e 6461 72da  omer's Calendar.
+00000140: 0841 6c6c 486f 7572 73fa 0832 3420 486f  .AllHours..24 Ho
+00000150: 7572 73da 0643 7573 746f 6dfa 0f43 7573  urs..Custom..Cus
+00000160: 746f 6d20 4361 6c65 6e64 6172 e932 0000  tom Calendar.2..
+00000170: 0029 03da 0763 686f 6963 6573 da07 6465  .)...choices..de
+00000180: 6661 756c 74da 0a6d 6178 5f6c 656e 6774  fault..max_lengt
+00000190: 6829 03da 0a6d 6f64 656c 5f6e 616d 65da  h)...model_name.
+000001a0: 046e 616d 65da 0566 6965 6c64 4e29 0272  .name..fieldN).r
+000001b0: 0500 0000 7206 0000 0029 0272 0900 0000  ....r....).r....
+000001c0: 720a 0000 0029 0272 0b00 0000 720c 0000  r....).r....r...
+000001d0: 0029 0272 0d00 0000 720e 0000 0029 0272  .).r....r....).r
+000001e0: 0f00 0000 7210 0000 0029 09da 085f 5f6e  ....r....)...__n
+000001f0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000200: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000210: 0c64 6570 656e 6465 6e63 6965 7372 0200  .dependenciesr..
+00000220: 0000 da0a 416c 7465 7246 6965 6c64 7203  ....AlterFieldr.
+00000230: 0000 00da 0943 6861 7246 6965 6c64 da0a  .....CharField..
+00000240: 6f70 6572 6174 696f 6e73 a900 721f 0000  operations..r...
+00000250: 0072 1f00 0000 fa63 2f68 6f6d 652f 6361  .r.....c/home/ca
+00000260: 6d65 726f 6e2f 4465 762f 6b61 6e62 616e  meron/Dev/kanban
+00000270: 2d64 6576 2f64 6a61 6e67 6f2d 636f 6e6e  -dev/django-conn
+00000280: 6563 7477 6973 652f 646a 636f 6e6e 6563  ectwise/djconnec
+00000290: 7477 6973 652f 6d69 6772 6174 696f 6e73  twise/migrations
+000002a0: 2f30 3036 365f 6175 746f 5f32 3031 3830  /0066_auto_20180
+000002b0: 3831 345f 3130 3436 2e70 7972 0400 0000  814_1046.pyr....
+000002c0: 0600 0000 730a 0000 0008 0306 0404 0102  ....s...........
+000002d0: 0102 0172 0400 0000 4e29 04da 0964 6a61  ...r....N)...dja
+000002e0: 6e67 6f2e 6462 7202 0000 0072 0300 0000  ngo.dbr....r....
+000002f0: 7204 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+00000300: 1f00 0000 7220 0000 00da 083c 6d6f 6475  ....r .....<modu
+00000310: 6c65 3e03 0000 0073 0200 0000 1003       le>....s......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0003_auto_20170223_2233.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0008_project_status_name.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,43 @@
-00000000: 160d 0d0a a4b0 1f5d 9901 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c b401 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0008 0000 0040 0000 0073  ...........@...s
-000000b0: 3a00 0000 6500 005a 0100 6400 005a 0200  :...e..Z..d..Z..
-000000c0: 640a 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0b00 6901  ..d..d..d..d..i.
-000000e0: 0083 0002 6701 005a 0600 6409 0053 290c  ....g..Z..d..S).
-000000f0: da09 4d69 6772 6174 696f 6eda 0d64 6a63  ..Migration..djc
-00000100: 6f6e 6e65 6374 7769 7365 da17 3030 3032  onnectwise..0002
-00000110: 5f61 7574 6f5f 3230 3137 3032 3233 5f32  _auto_20170223_2
-00000120: 3134 33da 046e 616d 655a 0b62 6f61 7264  143..nameZ.board
-00000130: 7374 6174 7573 da07 6f70 7469 6f6e 73da  status..options.
-00000140: 086f 7264 6572 696e 67da 0b62 6f61 7264  .ordering..board
-00000150: 5f5f 6e61 6d65 da0a 736f 7274 5f6f 7264  __name..sort_ord
-00000160: 6572 4e29 027a 0d64 6a63 6f6e 6e65 6374  erN).z.djconnect
-00000170: 7769 7365 7207 0000 0029 037a 0b62 6f61  wiser....).z.boa
-00000180: 7264 5f5f 6e61 6d65 7a0a 736f 7274 5f6f  rd__namez.sort_o
-00000190: 7264 6572 7208 0000 0029 07da 085f 5f6e  rderr....)...__n
-000001a0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-000001b0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-000001c0: 0c64 6570 656e 6465 6e63 6965 7372 0300  .dependenciesr..
-000001d0: 0000 da11 416c 7465 724d 6f64 656c 4f70  ....AlterModelOp
-000001e0: 7469 6f6e 73da 0a6f 7065 7261 7469 6f6e  tions..operation
-000001f0: 73a9 0072 1300 0000 7213 0000 00fa 6e2f  s..r....r.....n/
-00000200: 686f 6d65 2f73 616d 2f67 6974 2f4b 616e  home/sam/git/Kan
-00000210: 6261 6e2f 646a 616e 676f 2d63 6f6e 6e65  ban/django-conne
-00000220: 6374 7769 7365 2f64 6a61 6e67 6f2d 636f  ctwise/django-co
-00000230: 6e6e 6563 7477 6973 652f 646a 636f 6e6e  nnectwise/djconn
-00000240: 6563 7477 6973 652f 6d69 6772 6174 696f  ectwise/migratio
-00000250: 6e73 2f30 3030 335f 6175 746f 5f32 3031  ns/0003_auto_201
-00000260: 3730 3232 335f 3232 3333 2e70 7972 0500  70223_2233.pyr..
-00000270: 0000 0700 0000 7308 0000 000c 0309 0409  ......s.........
-00000280: 0106 0172 0500 0000 4e29 06da 0a5f 5f66  ...r....N)...__f
-00000290: 7574 7572 655f 5f72 0200 0000 da09 646a  uture__r......dj
-000002a0: 616e 676f 2e64 6272 0300 0000 7204 0000  ango.dbr....r...
-000002b0: 0072 0500 0000 7213 0000 0072 1300 0000  .r....r....r....
-000002c0: 7213 0000 0072 1400 0000 da08 3c6d 6f64  r....r......<mod
-000002d0: 756c 653e 0200 0000 7304 0000 0010 0216  ule>....s.......
-000002e0: 03                                       .
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0800 0000 4000 0000 7330  ..........@...s0
+000000a0: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000c0: 0664 0664 078d 0364 088d 0367 015a 0864  .d.d...d...g.Z.d
+000000d0: 0953 0029 0bda 094d 6967 7261 7469 6f6e  .S.)...Migration
+000000e0: da0d 646a 636f 6e6e 6563 7477 6973 65da  ..djconnectwise.
+000000f0: 1730 3030 375f 6175 746f 5f32 3031 3730  .0007_auto_20170
+00000100: 3331 315f 3134 3135 da07 7072 6f6a 6563  311_1415..projec
+00000110: 745a 0b73 7461 7475 735f 6e61 6d65 e9c8  tZ.status_name..
+00000120: 0000 0054 2903 da0a 6d61 785f 6c65 6e67  ...T)...max_leng
+00000130: 7468 da05 626c 616e 6bda 046e 756c 6c29  th..blank..null)
+00000140: 03da 0a6d 6f64 656c 5f6e 616d 65da 046e  ...model_name..n
+00000150: 616d 65da 0566 6965 6c64 4e29 0272 0600  ame..fieldN).r..
+00000160: 0000 7207 0000 0029 09da 085f 5f6e 616d  ..r....)...__nam
+00000170: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000180: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
+00000190: 6570 656e 6465 6e63 6965 7372 0300 0000  ependenciesr....
+000001a0: da08 4164 6446 6965 6c64 7204 0000 00da  ..AddFieldr.....
+000001b0: 0943 6861 7246 6965 6c64 da0a 6f70 6572  .CharField..oper
+000001c0: 6174 696f 6e73 a900 7217 0000 0072 1700  ations..r....r..
+000001d0: 0000 fa64 2f68 6f6d 652f 6361 6d65 726f  ...d/home/camero
+000001e0: 6e2f 4465 762f 6b61 6e62 616e 2d64 6576  n/Dev/kanban-dev
+000001f0: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
+00000200: 6973 652f 646a 636f 6e6e 6563 7477 6973  ise/djconnectwis
+00000210: 652f 6d69 6772 6174 696f 6e73 2f30 3030  e/migrations/000
+00000220: 385f 7072 6f6a 6563 745f 7374 6174 7573  8_project_status
+00000230: 5f6e 616d 652e 7079 7205 0000 0007 0000  _name.pyr.......
+00000240: 0073 0a00 0000 0803 0604 0401 0201 0201  .s..............
+00000250: 7205 0000 004e 2906 da0a 5f5f 6675 7475  r....N)...__futu
+00000260: 7265 5f5f 7202 0000 00da 0964 6a61 6e67  re__r......djang
+00000270: 6f2e 6462 7203 0000 0072 0400 0000 7205  o.dbr....r....r.
+00000280: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
+00000290: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000002a0: 3e02 0000 0073 0400 0000 0c02 1003       >....s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0072_remove_callbackentry_member.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0010_remove_project_project_href.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-00000000: 160d 0d0a a4b0 1f5d 5301 0000 e300 0000  .......]S.......
+00000000: 330d 0d0a 10ec da5c 6f01 0000 e300 0000  3......\o.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
-00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
-00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
-00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
-00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
-00000070: 0000 0000 0005 0000 0040 0000 0073 3400  .........@...s4.
-00000080: 0000 6500 005a 0100 6400 005a 0200 6408  ..e..Z..d..Z..d.
-00000090: 0067 0100 5a03 0065 0400 6a05 0064 0300  .g..Z..e..j..d..
-000000a0: 6404 0064 0500 6406 0083 0002 6701 005a  d..d..d.....g..Z
-000000b0: 0600 6407 0053 2909 da09 4d69 6772 6174  ..d..S)...Migrat
-000000c0: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-000000d0: 7365 da17 3030 3731 5f61 7574 6f5f 3230  se..0071_auto_20
-000000e0: 3138 3038 3232 5f31 3330 30da 0a6d 6f64  180822_1300..mod
-000000f0: 656c 5f6e 616d 65da 0d63 616c 6c62 6163  el_name..callbac
-00000100: 6b65 6e74 7279 da04 6e61 6d65 da06 6d65  kentry..name..me
-00000110: 6d62 6572 4e29 027a 0d64 6a63 6f6e 6e65  mberN).z.djconne
-00000120: 6374 7769 7365 7205 0000 0029 07da 085f  ctwiser....)..._
-00000130: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000140: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000150: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
-00000160: 0200 0000 da0b 5265 6d6f 7665 4669 656c  ......RemoveFiel
-00000170: 64da 0a6f 7065 7261 7469 6f6e 73a9 0072  d..operations..r
-00000180: 1000 0000 7210 0000 00fa 772f 686f 6d65  ....r.....w/home
-00000190: 2f73 616d 2f67 6974 2f4b 616e 6261 6e2f  /sam/git/Kanban/
-000001a0: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
-000001b0: 7365 2f64 6a61 6e67 6f2d 636f 6e6e 6563  se/django-connec
-000001c0: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
-000001d0: 6973 652f 6d69 6772 6174 696f 6e73 2f30  ise/migrations/0
-000001e0: 3037 325f 7265 6d6f 7665 5f63 616c 6c62  072_remove_callb
-000001f0: 6163 6b65 6e74 7279 5f6d 656d 6265 722e  ackentry_member.
-00000200: 7079 7203 0000 0006 0000 0073 0800 0000  pyr........s....
-00000210: 0c03 0904 0901 0601 7203 0000 004e 2903  ........r....N).
-00000220: da09 646a 616e 676f 2e64 6272 0200 0000  ..django.dbr....
-00000230: 7203 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
-00000240: 1000 0000 7211 0000 00da 083c 6d6f 6475  ....r......<modu
-00000250: 6c65 3e03 0000 0073 0200 0000 1003       le>....s......
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0400 0000 4000 0000 7322  ..........@...s"
+000000a0: 0000 0065 005a 0164 005a 0264 0767 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0464 058d 0267 015a  .e.j.d.d.d...g.Z
+000000c0: 0664 0653 0029 08da 094d 6967 7261 7469  .d.S.)...Migrati
+000000d0: 6f6e da0d 646a 636f 6e6e 6563 7477 6973  on..djconnectwis
+000000e0: 65da 1930 3030 395f 6d65 6d62 6572 5f6c  e..0009_member_l
+000000f0: 6963 656e 7365 5f63 6c61 7373 da07 7072  icense_class..pr
+00000100: 6f6a 6563 74da 0c70 726f 6a65 6374 5f68  oject..project_h
+00000110: 7265 6629 02da 0a6d 6f64 656c 5f6e 616d  ref)...model_nam
+00000120: 65da 046e 616d 654e 2902 7206 0000 0072  e..nameN).r....r
+00000130: 0700 0000 2907 da08 5f5f 6e61 6d65 5f5f  ....)...__name__
+00000140: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000150: 7175 616c 6e61 6d65 5f5f da0c 6465 7065  qualname__..depe
+00000160: 6e64 656e 6369 6573 7203 0000 00da 0b52  ndenciesr......R
+00000170: 656d 6f76 6546 6965 6c64 da0a 6f70 6572  emoveField..oper
+00000180: 6174 696f 6e73 a900 7212 0000 0072 1200  ations..r....r..
+00000190: 0000 fa6c 2f68 6f6d 652f 6361 6d65 726f  ...l/home/camero
+000001a0: 6e2f 4465 762f 6b61 6e62 616e 2d64 6576  n/Dev/kanban-dev
+000001b0: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
+000001c0: 6973 652f 646a 636f 6e6e 6563 7477 6973  ise/djconnectwis
+000001d0: 652f 6d69 6772 6174 696f 6e73 2f30 3031  e/migrations/001
+000001e0: 305f 7265 6d6f 7665 5f70 726f 6a65 6374  0_remove_project
+000001f0: 5f70 726f 6a65 6374 5f68 7265 662e 7079  _project_href.py
+00000200: 7205 0000 0007 0000 0073 0800 0000 0803  r........s......
+00000210: 0604 0401 0201 7205 0000 004e 2906 da0a  ......r....N)...
+00000220: 5f5f 6675 7475 7265 5f5f 7202 0000 00da  __future__r.....
+00000230: 0964 6a61 6e67 6f2e 6462 7203 0000 0072  .django.dbr....r
+00000240: 0400 0000 7205 0000 0072 1200 0000 7212  ....r....r....r.
+00000250: 0000 0072 1200 0000 7213 0000 00da 083c  ...r....r......<
+00000260: 6d6f 6475 6c65 3e02 0000 0073 0400 0000  module>....s....
+00000270: 0c02 1003                                ....
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0055_auto_20180501_1022.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0055_auto_20180501_1022.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,43 @@
-00000000: 160d 0d0a a4b0 1f5d ab01 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c ab01 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0009 0000 0040 0000 0073  ...........@...s
-000000b0: 4000 0000 6500 005a 0100 6400 005a 0200  @...e..Z..d..Z..
-000000c0: 640c 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6408  ..d..d..d..d..d.
-000000e0: 0064 0d00 6902 0083 0002 6701 005a 0600  .d..i.....g..Z..
-000000f0: 640b 0053 290e da09 4d69 6772 6174 696f  d..S)...Migratio
-00000100: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
-00000110: da17 3030 3534 5f61 7574 6f5f 3230 3138  ..0054_auto_2018
-00000120: 3035 3031 5f31 3030 39da 046e 616d 65da  0501_1009..name.
-00000130: 0b73 6572 7669 6365 6e6f 7465 da07 6f70  .servicenote..op
-00000140: 7469 6f6e 73da 1376 6572 626f 7365 5f6e  tions..verbose_n
-00000150: 616d 655f 706c 7572 616c da05 4e6f 7465  ame_plural..Note
-00000160: 73da 086f 7264 6572 696e 67fa 0d2d 6461  s..ordering..-da
-00000170: 7465 5f63 7265 6174 6564 da02 6964 4e29  te_created..idN)
-00000180: 027a 0d64 6a63 6f6e 6e65 6374 7769 7365  .z.djconnectwise
-00000190: 7207 0000 0029 0272 0e00 0000 7a02 6964  r....).r....z.id
-000001a0: 2907 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000001b0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000001c0: 6e61 6d65 5f5f da0c 6465 7065 6e64 656e  name__..dependen
-000001d0: 6369 6573 7203 0000 00da 1141 6c74 6572  ciesr......Alter
-000001e0: 4d6f 6465 6c4f 7074 696f 6e73 da0a 6f70  ModelOptions..op
-000001f0: 6572 6174 696f 6e73 a900 7216 0000 0072  erations..r....r
-00000200: 1600 0000 fa6e 2f68 6f6d 652f 7361 6d2f  .....n/home/sam/
-00000210: 6769 742f 4b61 6e62 616e 2f64 6a61 6e67  git/Kanban/djang
-00000220: 6f2d 636f 6e6e 6563 7477 6973 652f 646a  o-connectwise/dj
-00000230: 616e 676f 2d63 6f6e 6e65 6374 7769 7365  ango-connectwise
-00000240: 2f64 6a63 6f6e 6e65 6374 7769 7365 2f6d  /djconnectwise/m
-00000250: 6967 7261 7469 6f6e 732f 3030 3535 5f61  igrations/0055_a
-00000260: 7574 6f5f 3230 3138 3035 3031 5f31 3032  uto_20180501_102
-00000270: 322e 7079 7205 0000 0007 0000 0073 0800  2.pyr........s..
-00000280: 0000 0c03 0904 0901 0601 7205 0000 004e  ..........r....N
-00000290: 2906 da0a 5f5f 6675 7475 7265 5f5f 7202  )...__future__r.
-000002a0: 0000 00da 0964 6a61 6e67 6f2e 6462 7203  .....django.dbr.
-000002b0: 0000 0072 0400 0000 7205 0000 0072 1600  ...r....r....r..
-000002c0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-000002d0: 00da 083c 6d6f 6475 6c65 3e02 0000 0073  ...<module>....s
-000002e0: 0400 0000 1002 1603                      ........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0500 0000 4000 0000 7328  ..........@...s(
+000000a0: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0464 0b64 079c 0264  .e.j.d.d.d.d...d
+000000c0: 088d 0267 015a 0664 0953 0029 0cda 094d  ...g.Z.d.S.)...M
+000000d0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
+000000e0: 6563 7477 6973 65da 1730 3035 345f 6175  ectwise..0054_au
+000000f0: 746f 5f32 3031 3830 3530 315f 3130 3039  to_20180501_1009
+00000100: da0b 7365 7276 6963 656e 6f74 65da 054e  ..servicenote..N
+00000110: 6f74 6573 fa0d 2d64 6174 655f 6372 6561  otes..-date_crea
+00000120: 7465 64da 0269 6429 02da 1376 6572 626f  ted..id)...verbo
+00000130: 7365 5f6e 616d 655f 706c 7572 616c da08  se_name_plural..
+00000140: 6f72 6465 7269 6e67 2902 da04 6e61 6d65  ordering)...name
+00000150: da07 6f70 7469 6f6e 734e 2902 7206 0000  ..optionsN).r...
+00000160: 0072 0700 0000 2902 720a 0000 0072 0b00  .r....).r....r..
+00000170: 0000 2907 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+00000180: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000190: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
+000001a0: 656e 6369 6573 7203 0000 00da 1141 6c74  enciesr......Alt
+000001b0: 6572 4d6f 6465 6c4f 7074 696f 6e73 da0a  erModelOptions..
+000001c0: 6f70 6572 6174 696f 6e73 a900 7216 0000  operations..r...
+000001d0: 0072 1600 0000 fa63 2f68 6f6d 652f 6361  .r.....c/home/ca
+000001e0: 6d65 726f 6e2f 4465 762f 6b61 6e62 616e  meron/Dev/kanban
+000001f0: 2d64 6576 2f64 6a61 6e67 6f2d 636f 6e6e  -dev/django-conn
+00000200: 6563 7477 6973 652f 646a 636f 6e6e 6563  ectwise/djconnec
+00000210: 7477 6973 652f 6d69 6772 6174 696f 6e73  twise/migrations
+00000220: 2f30 3035 355f 6175 746f 5f32 3031 3830  /0055_auto_20180
+00000230: 3530 315f 3130 3232 2e70 7972 0500 0000  501_1022.pyr....
+00000240: 0700 0000 7308 0000 0008 0306 0404 0102  ....s...........
+00000250: 0172 0500 0000 4e29 06da 0a5f 5f66 7574  .r....N)...__fut
+00000260: 7572 655f 5f72 0200 0000 da09 646a 616e  ure__r......djan
+00000270: 676f 2e64 6272 0300 0000 7204 0000 0072  go.dbr....r....r
+00000280: 0500 0000 7216 0000 0072 1600 0000 7216  ....r....r....r.
+00000290: 0000 0072 1700 0000 da08 3c6d 6f64 756c  ...r......<modul
+000002a0: 653e 0200 0000 7304 0000 000c 0210 03    e>....s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0059_auto_20180518_0811.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0110_project_company.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,46 @@
-00000000: 160d 0d0a a4b0 1f5d f601 0000 e300 0000  .......]........
+00000000: 330d 0d0a 5ae4 775d f701 0000 e300 0000  3...Z.w]........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 0d00 0000 4000 0000 735e 0000 0065 0000  ....@...s^...e..
-000000a0: 5a01 0064 0000 5a02 0064 0e00 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6407 0065 0600 6a07 0064 0800  .d..d..e..j..d..
-000000d0: 6409 0064 0a00 6508 006a 0900 6a06 006a  d..d..e..j..j..j
-000000e0: 0a00 6a0b 0064 0b00 640c 0083 0003 8300  ..j..d..d.......
-000000f0: 0367 0100 5a0c 0064 0d00 5329 0fda 094d  .g..Z..d..S)...M
-00000100: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
-00000110: 6563 7477 6973 65da 1730 3035 385f 6175  ectwise..0058_au
-00000120: 746f 5f32 3031 3830 3531 365f 3130 3532  to_20180516_1052
-00000130: da0a 6d6f 6465 6c5f 6e61 6d65 da0d 6361  ..model_name..ca
-00000140: 6c6c 6261 636b 656e 7472 79da 046e 616d  llbackentry..nam
-00000150: 65da 066d 656d 6265 72da 0566 6965 6c64  e..member..field
-00000160: da04 6e75 6c6c 54da 096f 6e5f 6465 6c65  ..nullT..on_dele
-00000170: 7465 da02 746f 7a14 646a 636f 6e6e 6563  te..toz.djconnec
-00000180: 7477 6973 652e 4d65 6d62 6572 4e29 027a  twise.MemberN).z
-00000190: 0d64 6a63 6f6e 6e65 6374 7769 7365 7206  .djconnectwiser.
-000001a0: 0000 0029 0dda 085f 5f6e 616d 655f 5fda  ...)...__name__.
-000001b0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000001c0: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
-000001d0: 6465 6e63 6965 7372 0200 0000 da0a 416c  denciesr......Al
-000001e0: 7465 7246 6965 6c64 7203 0000 00da 0a46  terFieldr......F
-000001f0: 6f72 6569 676e 4b65 79da 0664 6a61 6e67  oreignKey..djang
-00000200: 6fda 0264 62da 0864 656c 6574 696f 6eda  o..db..deletion.
-00000210: 0853 4554 5f4e 554c 4cda 0a6f 7065 7261  .SET_NULL..opera
-00000220: 7469 6f6e 73a9 0072 1a00 0000 721a 0000  tions..r....r...
-00000230: 00fa 6e2f 686f 6d65 2f73 616d 2f67 6974  ..n/home/sam/git
-00000240: 2f4b 616e 6261 6e2f 646a 616e 676f 2d63  /Kanban/django-c
-00000250: 6f6e 6e65 6374 7769 7365 2f64 6a61 6e67  onnectwise/djang
-00000260: 6f2d 636f 6e6e 6563 7477 6973 652f 646a  o-connectwise/dj
-00000270: 636f 6e6e 6563 7477 6973 652f 6d69 6772  connectwise/migr
-00000280: 6174 696f 6e73 2f30 3035 395f 6175 746f  ations/0059_auto
-00000290: 5f32 3031 3830 3531 385f 3038 3131 2e70  _20180518_0811.p
-000002a0: 7972 0400 0000 0700 0000 730a 0000 000c  yr........s.....
-000002b0: 0309 0409 0106 0106 0172 0400 0000 2906  .........r....).
-000002c0: da09 646a 616e 676f 2e64 6272 0200 0000  ..django.dbr....
-000002d0: 7203 0000 00da 1964 6a61 6e67 6f2e 6462  r......django.db
-000002e0: 2e6d 6f64 656c 732e 6465 6c65 7469 6f6e  .models.deletion
-000002f0: 7215 0000 0072 0400 0000 721a 0000 0072  r....r....r....r
-00000300: 1a00 0000 721a 0000 0072 1b00 0000 da08  ....r....r......
-00000310: 3c6d 6f64 756c 653e 0300 0000 7304 0000  <module>....s...
-00000320: 0016 010c 03                             .....
+00000020: 0073 2e00 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 4700  m.Z...d.d.l.Z.G.
+00000040: 6403 6404 8400 6404 6501 6a05 8303 5a05  d.d...d.e.j...Z.
+00000050: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 734e 6300 0000 0000 0000 0000 0000 0009  sNc.............
+00000080: 0000 0040 0000 0073 3a00 0000 6500 5a01  ...@...s:...e.Z.
+00000090: 6400 5a02 640a 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000a0: 6404 6506 6a07 6405 6405 6508 6a09 6a06  d.e.j.d.d.e.j.j.
+000000b0: 6a0a 6a0b 6406 6407 8d04 6408 8d03 6701  j.j.d.d...d...g.
+000000c0: 5a0c 6409 5300 290b da09 4d69 6772 6174  Z.d.S.)...Migrat
+000000d0: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
+000000e0: 7365 da11 3031 3039 5f74 6963 6b65 745f  se..0109_ticket_
+000000f0: 7068 6173 65da 0770 726f 6a65 6374 da07  phase..project..
+00000100: 636f 6d70 616e 7954 7a15 646a 636f 6e6e  companyTz.djconn
+00000110: 6563 7477 6973 652e 436f 6d70 616e 7929  ectwise.Company)
+00000120: 04da 0562 6c61 6e6b da04 6e75 6c6c da09  ...blank..null..
+00000130: 6f6e 5f64 656c 6574 65da 0274 6f29 03da  on_delete..to)..
+00000140: 0a6d 6f64 656c 5f6e 616d 65da 046e 616d  .model_name..nam
+00000150: 65da 0566 6965 6c64 4e29 0272 0500 0000  e..fieldN).r....
+00000160: 7206 0000 0029 0dda 085f 5f6e 616d 655f  r....)...__name_
+00000170: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000180: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
+00000190: 656e 6465 6e63 6965 7372 0200 0000 da08  endenciesr......
+000001a0: 4164 6446 6965 6c64 7203 0000 00da 0a46  AddFieldr......F
+000001b0: 6f72 6569 676e 4b65 79da 0664 6a61 6e67  oreignKey..djang
+000001c0: 6fda 0264 62da 0864 656c 6574 696f 6eda  o..db..deletion.
+000001d0: 0853 4554 5f4e 554c 4cda 0a6f 7065 7261  .SET_NULL..opera
+000001e0: 7469 6f6e 73a9 0072 1b00 0000 721b 0000  tions..r....r...
+000001f0: 00fa 602f 686f 6d65 2f63 616d 6572 6f6e  ..`/home/cameron
+00000200: 2f44 6576 2f6b 616e 6261 6e2d 6465 762f  /Dev/kanban-dev/
+00000210: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
+00000220: 7365 2f64 6a63 6f6e 6e65 6374 7769 7365  se/djconnectwise
+00000230: 2f6d 6967 7261 7469 6f6e 732f 3031 3130  /migrations/0110
+00000240: 5f70 726f 6a65 6374 5f63 6f6d 7061 6e79  _project_company
+00000250: 2e70 7972 0400 0000 0700 0000 730a 0000  .pyr........s...
+00000260: 0008 0306 0404 0102 0102 0172 0400 0000  ...........r....
+00000270: 2906 da09 646a 616e 676f 2e64 6272 0200  )...django.dbr..
+00000280: 0000 7203 0000 00da 1964 6a61 6e67 6f2e  ..r......django.
+00000290: 6462 2e6d 6f64 656c 732e 6465 6c65 7469  db.models.deleti
+000002a0: 6f6e 7216 0000 0072 0400 0000 721b 0000  onr....r....r...
+000002b0: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+000002c0: da08 3c6d 6f64 756c 653e 0300 0000 7304  ..<module>....s.
+000002d0: 0000 0010 0108 03                        .......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0070_mycompanyother.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0070_mycompanyother.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,53 @@
-00000000: 160d 0d0a a4b0 1f5d 8e02 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c 8e02 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 0f00 0000 4000 0000 738e 0000 0065 0000  ....@...s....e..
-000000a0: 5a01 0064 0000 5a02 0064 1500 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6506 006a 0700 6407 0064 0800  .d..e..j..d..d..
-000000d0: 6409 0064 0800 640a 0064 0b00 640c 0064  d..d..d..d..d..d
-000000e0: 0d00 8300 0466 0200 640e 0065 0600 6a08  .....f..d..e..j.
-000000f0: 0064 0f00 6408 0064 1000 6408 0064 1100  .d..d..d..d..d..
-00000100: 6509 006a 0a00 6a06 006a 0b00 6a0c 0064  e..j..j..j..j..d
-00000110: 1200 6413 0083 0004 6602 0067 0200 8300  ..d.....f..g....
-00000120: 0267 0100 5a0d 0064 1400 5329 16da 094d  .g..Z..d..S)...M
-00000130: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
-00000140: 6563 7477 6973 65da 1730 3036 395f 6175  ectwise..0069_au
-00000150: 746f 5f32 3031 3830 3831 355f 3131 3136  to_20180815_1116
-00000160: da04 6e61 6d65 da0e 4d79 436f 6d70 616e  ..name..MyCompan
-00000170: 794f 7468 6572 da06 6669 656c 6473 da02  yOther..fields..
-00000180: 6964 da0c 6175 746f 5f63 7265 6174 6564  id..auto_created
-00000190: 54da 0b70 7269 6d61 7279 5f6b 6579 da09  T..primary_key..
-000001a0: 7365 7269 616c 697a 6546 da0c 7665 7262  serializeF..verb
-000001b0: 6f73 655f 6e61 6d65 da02 4944 da10 6465  ose_name..ID..de
-000001c0: 6661 756c 745f 6361 6c65 6e64 6172 da05  fault_calendar..
-000001d0: 626c 616e 6bda 046e 756c 6cda 096f 6e5f  blank..null..on_
-000001e0: 6465 6c65 7465 da02 746f 7a16 646a 636f  delete..toz.djco
-000001f0: 6e6e 6563 7477 6973 652e 4361 6c65 6e64  nnectwise.Calend
-00000200: 6172 4e29 027a 0d64 6a63 6f6e 6e65 6374  arN).z.djconnect
-00000210: 7769 7365 7a17 3030 3639 5f61 7574 6f5f  wisez.0069_auto_
-00000220: 3230 3138 3038 3135 5f31 3131 3629 0eda  20180815_1116)..
-00000230: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000240: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000250: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
-00000260: 7372 0200 0000 da0b 4372 6561 7465 4d6f  sr......CreateMo
-00000270: 6465 6c72 0300 0000 da09 4175 746f 4669  delr......AutoFi
-00000280: 656c 64da 0a46 6f72 6569 676e 4b65 79da  eld..ForeignKey.
-00000290: 0664 6a61 6e67 6fda 0264 62da 0864 656c  .django..db..del
-000002a0: 6574 696f 6eda 0853 4554 5f4e 554c 4cda  etion..SET_NULL.
-000002b0: 0a6f 7065 7261 7469 6f6e 73a9 0072 2100  .operations..r!.
-000002c0: 0000 7221 0000 00fa 6a2f 686f 6d65 2f73  ..r!....j/home/s
-000002d0: 616d 2f67 6974 2f4b 616e 6261 6e2f 646a  am/git/Kanban/dj
-000002e0: 616e 676f 2d63 6f6e 6e65 6374 7769 7365  ango-connectwise
-000002f0: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
-00000300: 6973 652f 646a 636f 6e6e 6563 7477 6973  ise/djconnectwis
-00000310: 652f 6d69 6772 6174 696f 6e73 2f30 3037  e/migrations/007
-00000320: 305f 6d79 636f 6d70 616e 796f 7468 6572  0_mycompanyother
-00000330: 2e70 7972 0400 0000 0700 0000 730a 0000  .pyr........s...
-00000340: 000c 0309 0409 0106 0227 0172 0400 0000  .........'.r....
-00000350: 2906 da09 646a 616e 676f 2e64 6272 0200  )...django.dbr..
-00000360: 0000 7203 0000 00da 1964 6a61 6e67 6f2e  ..r......django.
-00000370: 6462 2e6d 6f64 656c 732e 6465 6c65 7469  db.models.deleti
-00000380: 6f6e 721c 0000 0072 0400 0000 7221 0000  onr....r....r!..
-00000390: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
-000003a0: da08 3c6d 6f64 756c 653e 0300 0000 7304  ..<module>....s.
-000003b0: 0000 0016 010c 03                        .......
+00000020: 0073 2e00 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 4700  m.Z...d.d.l.Z.G.
+00000040: 6403 6404 8400 6404 6501 6a05 8303 5a05  d.d...d.e.j...Z.
+00000050: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 734e 6300 0000 0000 0000 0000 0000 000a  sNc.............
+00000080: 0000 0040 0000 0073 5200 0000 6500 5a01  ...@...sR...e.Z.
+00000090: 6400 5a02 640e 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000a0: 6404 6506 6a07 6405 6405 6406 6407 6408  d.e.j.d.d.d.d.d.
+000000b0: 8d04 6602 6409 6506 6a08 6405 6405 6509  ..f.d.e.j.d.d.e.
+000000c0: 6a0a 6a06 6a0b 6a0c 640a 640b 8d04 6602  j.j.j.j.d.d...f.
+000000d0: 6702 640c 8d02 6701 5a0d 640d 5300 290f  g.d...g.Z.d.S.).
+000000e0: da09 4d69 6772 6174 696f 6eda 0d64 6a63  ..Migration..djc
+000000f0: 6f6e 6e65 6374 7769 7365 da17 3030 3639  onnectwise..0069
+00000100: 5f61 7574 6f5f 3230 3138 3038 3135 5f31  _auto_20180815_1
+00000110: 3131 36da 0e4d 7943 6f6d 7061 6e79 4f74  116..MyCompanyOt
+00000120: 6865 72da 0269 6454 46da 0249 4429 04da  her..idTF..ID)..
+00000130: 0c61 7574 6f5f 6372 6561 7465 64da 0b70  .auto_created..p
+00000140: 7269 6d61 7279 5f6b 6579 da09 7365 7269  rimary_key..seri
+00000150: 616c 697a 65da 0c76 6572 626f 7365 5f6e  alize..verbose_n
+00000160: 616d 65da 1064 6566 6175 6c74 5f63 616c  ame..default_cal
+00000170: 656e 6461 727a 1664 6a63 6f6e 6e65 6374  endarz.djconnect
+00000180: 7769 7365 2e43 616c 656e 6461 7229 04da  wise.Calendar)..
+00000190: 0562 6c61 6e6b da04 6e75 6c6c da09 6f6e  .blank..null..on
+000001a0: 5f64 656c 6574 65da 0274 6f29 02da 046e  _delete..to)...n
+000001b0: 616d 65da 0666 6965 6c64 734e 2902 7205  ame..fieldsN).r.
+000001c0: 0000 0072 0600 0000 290e da08 5f5f 6e61  ...r....)...__na
+000001d0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+000001e0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
+000001f0: 6465 7065 6e64 656e 6369 6573 7202 0000  dependenciesr...
+00000200: 00da 0b43 7265 6174 654d 6f64 656c 7203  ...CreateModelr.
+00000210: 0000 00da 0941 7574 6f46 6965 6c64 da0a  .....AutoField..
+00000220: 466f 7265 6967 6e4b 6579 da06 646a 616e  ForeignKey..djan
+00000230: 676f da02 6462 da08 6465 6c65 7469 6f6e  go..db..deletion
+00000240: da08 5345 545f 4e55 4c4c da0a 6f70 6572  ..SET_NULL..oper
+00000250: 6174 696f 6e73 a900 7221 0000 0072 2100  ations..r!...r!.
+00000260: 0000 fa5f 2f68 6f6d 652f 6361 6d65 726f  ..._/home/camero
+00000270: 6e2f 4465 762f 6b61 6e62 616e 2d64 6576  n/Dev/kanban-dev
+00000280: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
+00000290: 6973 652f 646a 636f 6e6e 6563 7477 6973  ise/djconnectwis
+000002a0: 652f 6d69 6772 6174 696f 6e73 2f30 3037  e/migrations/007
+000002b0: 305f 6d79 636f 6d70 616e 796f 7468 6572  0_mycompanyother
+000002c0: 2e70 7972 0400 0000 0700 0000 730a 0000  .pyr........s...
+000002d0: 0008 0306 0404 0102 0214 0172 0400 0000  ...........r....
+000002e0: 2906 da09 646a 616e 676f 2e64 6272 0200  )...django.dbr..
+000002f0: 0000 7203 0000 00da 1964 6a61 6e67 6f2e  ..r......django.
+00000300: 6462 2e6d 6f64 656c 732e 6465 6c65 7469  db.models.deleti
+00000310: 6f6e 721c 0000 0072 0400 0000 7221 0000  onr....r....r!..
+00000320: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
+00000330: da08 3c6d 6f64 756c 653e 0300 0000 7304  ..<module>....s.
+00000340: 0000 0010 0108 03                        .......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0096_merge_20190718_1102.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0060_auto_20180605_0840.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-00000000: 160d 0d0a 4ce4 305d 2301 0000 e300 0000  ....L.0]#.......
+00000000: 330d 0d0a 10ec da5c 9901 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
-00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
-00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
-00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
-00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
-00000070: 0000 0000 0003 0000 0040 0000 0073 2200  .........@...s".
-00000080: 0000 6500 005a 0100 6400 005a 0200 6405  ..e..Z..d..Z..d.
-00000090: 0064 0600 6702 005a 0300 6700 005a 0400  .d..g..Z..g..Z..
-000000a0: 6404 0053 2907 da09 4d69 6772 6174 696f  d..S)...Migratio
-000000b0: 6eda 0d64 6a63 6f6e 6e65 6374 7769 7365  n..djconnectwise
-000000c0: da1f 3030 3935 5f63 6f6e 6e65 6374 7769  ..0095_connectwi
-000000d0: 7365 626f 6172 645f 776f 726b 5f74 7970  seboard_work_typ
-000000e0: 65da 1730 3039 335f 6175 746f 5f32 3031  e..0093_auto_201
-000000f0: 3930 3731 365f 3136 3330 4e29 02fa 0d64  90716_1630N)...d
-00000100: 6a63 6f6e 6e65 6374 7769 7365 7a1f 3030  jconnectwisez.00
-00000110: 3935 5f63 6f6e 6e65 6374 7769 7365 626f  95_connectwisebo
-00000120: 6172 645f 776f 726b 5f74 7970 6529 0272  ard_work_type).r
-00000130: 0700 0000 7a17 3030 3933 5f61 7574 6f5f  ....z.0093_auto_
-00000140: 3230 3139 3037 3136 5f31 3633 3029 05da  20190716_1630)..
+00000020: 0073 2200 0000 6400 6401 6c00 6d01 5a01  .s"...d.d.l.m.Z.
+00000030: 0100 4700 6402 6403 8400 6403 6501 6a02  ..G.d.d...d.e.j.
+00000040: 8303 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
+00000050: 01da 0a6d 6967 7261 7469 6f6e 7363 0000  ...migrationsc..
+00000060: 0000 0000 0000 0000 0000 0500 0000 4000  ..............@.
+00000070: 0000 7328 0000 0065 005a 0164 005a 0264  ..s(...e.Z.d.Z.d
+00000080: 0a67 015a 0365 046a 0564 0364 0b64 0664  .g.Z.e.j.d.d.d.d
+00000090: 079c 0264 088d 0267 015a 0664 0953 0029  ...d...g.Z.d.S.)
+000000a0: 0cda 094d 6967 7261 7469 6f6e da0d 646a  ...Migration..dj
+000000b0: 636f 6e6e 6563 7477 6973 65da 1730 3035  connectwise..005
+000000c0: 395f 6175 746f 5f32 3031 3830 3531 385f  9_auto_20180518_
+000000d0: 3038 3131 5a0e 7469 636b 6574 7072 696f  0811Z.ticketprio
+000000e0: 7269 7479 da04 736f 7274 da04 6e61 6d65  rity..sort..name
+000000f0: 7a11 7469 636b 6574 2070 7269 6f72 6974  z.ticket priorit
+00000100: 6965 7329 02da 086f 7264 6572 696e 67da  ies)...ordering.
+00000110: 1376 6572 626f 7365 5f6e 616d 655f 706c  .verbose_name_pl
+00000120: 7572 616c 2902 7207 0000 00da 076f 7074  ural).r......opt
+00000130: 696f 6e73 4e29 0272 0400 0000 7205 0000  ionsN).r....r...
+00000140: 0029 0272 0600 0000 7207 0000 0029 07da  .).r....r....)..
 00000150: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
 00000160: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
 00000170: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
-00000180: 73da 0a6f 7065 7261 7469 6f6e 73a9 0072  s..operations..r
-00000190: 0d00 0000 720d 0000 00fa 6f2f 686f 6d65  ....r.....o/home
-000001a0: 2f73 616d 2f67 6974 2f4b 616e 6261 6e2f  /sam/git/Kanban/
-000001b0: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
-000001c0: 7365 2f64 6a61 6e67 6f2d 636f 6e6e 6563  se/django-connec
-000001d0: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
-000001e0: 6973 652f 6d69 6772 6174 696f 6e73 2f30  ise/migrations/0
-000001f0: 3039 365f 6d65 7267 655f 3230 3139 3037  096_merge_201907
-00000200: 3138 5f31 3130 322e 7079 7203 0000 0006  18_1102.pyr.....
-00000210: 0000 0073 0600 0000 0c03 0301 0903 7203  ...s..........r.
-00000220: 0000 004e 2903 da09 646a 616e 676f 2e64  ...N)...django.d
-00000230: 6272 0200 0000 7203 0000 0072 0d00 0000  br....r....r....
-00000240: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
-00000250: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
-00000260: 0000 1003                                ....
+00000180: 7372 0200 0000 da11 416c 7465 724d 6f64  sr......AlterMod
+00000190: 656c 4f70 7469 6f6e 73da 0a6f 7065 7261  elOptions..opera
+000001a0: 7469 6f6e 73a9 0072 1100 0000 7211 0000  tions..r....r...
+000001b0: 00fa 632f 686f 6d65 2f63 616d 6572 6f6e  ..c/home/cameron
+000001c0: 2f44 6576 2f6b 616e 6261 6e2d 6465 762f  /Dev/kanban-dev/
+000001d0: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
+000001e0: 7365 2f64 6a63 6f6e 6e65 6374 7769 7365  se/djconnectwise
+000001f0: 2f6d 6967 7261 7469 6f6e 732f 3030 3630  /migrations/0060
+00000200: 5f61 7574 6f5f 3230 3138 3036 3035 5f30  _auto_20180605_0
+00000210: 3834 302e 7079 7203 0000 0006 0000 0073  840.pyr........s
+00000220: 0800 0000 0803 0604 0401 0201 7203 0000  ............r...
+00000230: 004e 2903 da09 646a 616e 676f 2e64 6272  .N)...django.dbr
+00000240: 0200 0000 7203 0000 0072 1100 0000 7211  ....r....r....r.
+00000250: 0000 0072 1100 0000 7212 0000 00da 083c  ...r....r......<
+00000260: 6d6f 6475 6c65 3e03 0000 0073 0200 0000  module>....s....
+00000270: 0c03                                     ..
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0105_auto_20190722_1444.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0099_timeentry_agreement.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,49 @@
-00000000: 160d 0d0a 5f8c 375d f002 0000 e300 0000  ...._.7]........
+00000000: 330d 0d0a 2a3e 545d 2202 0000 e300 0000  3...*>T]".......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 1000 0000 4000 0000 73a9 0000 0065 0000  ....@...s....e..
-000000a0: 5a01 0064 0000 5a02 0064 1100 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6407 0065 0600 6a07 0064 0800  .d..d..e..j..d..
-000000d0: 6409 0064 0a00 6409 0064 0b00 6508 006a  d..d..d..d..e..j
-000000e0: 0900 6a06 006a 0a00 6a0b 0064 0c00 640d  ..j..j..j..d..d.
-000000f0: 0083 0004 8300 0365 0400 6a05 0064 0300  .......e..j..d..
-00000100: 6404 0064 0500 640e 0064 0700 6506 006a  d..d..d..d..e..j
-00000110: 0700 6408 0064 0900 640a 0064 0900 640b  ..d..d..d..d..d.
-00000120: 0065 0800 6a09 006a 0600 6a0a 006a 0b00  .e..j..j..j..j..
-00000130: 640c 0064 0f00 8300 0483 0003 6702 005a  d..d........g..Z
-00000140: 0c00 6410 0053 2912 da09 4d69 6772 6174  ..d..S)...Migrat
-00000150: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-00000160: 7365 da17 3031 3034 5f61 7574 6f5f 3230  se..0104_auto_20
-00000170: 3139 3037 3232 5f31 3233 32da 0a6d 6f64  190722_1232..mod
-00000180: 656c 5f6e 616d 65da 0861 6374 6976 6974  el_name..activit
-00000190: 79da 046e 616d 65da 0673 7461 7475 73da  y..name..status.
-000001a0: 0566 6965 6c64 da05 626c 616e 6b54 da04  .field..blankT..
-000001b0: 6e75 6c6c da09 6f6e 5f64 656c 6574 65da  null..on_delete.
-000001c0: 0274 6f7a 1c64 6a63 6f6e 6e65 6374 7769  .toz.djconnectwi
-000001d0: 7365 2e41 6374 6976 6974 7953 7461 7475  se.ActivityStatu
-000001e0: 73da 0474 7970 657a 1a64 6a63 6f6e 6e65  s..typez.djconne
-000001f0: 6374 7769 7365 2e41 6374 6976 6974 7954  ctwise.ActivityT
-00000200: 7970 654e 2902 7a0d 646a 636f 6e6e 6563  ypeN).z.djconnec
-00000210: 7477 6973 6572 0600 0000 290d da08 5f5f  twiser....)...__
-00000220: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000230: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000240: da0c 6465 7065 6e64 656e 6369 6573 7202  ..dependenciesr.
-00000250: 0000 00da 0841 6464 4669 656c 6472 0300  .....AddFieldr..
-00000260: 0000 da0a 466f 7265 6967 6e4b 6579 da06  ....ForeignKey..
-00000270: 646a 616e 676f da02 6462 da08 6465 6c65  django..db..dele
-00000280: 7469 6f6e da08 5345 545f 4e55 4c4c da0a  tion..SET_NULL..
-00000290: 6f70 6572 6174 696f 6e73 a900 721c 0000  operations..r...
-000002a0: 0072 1c00 0000 fa6e 2f68 6f6d 652f 7361  .r.....n/home/sa
-000002b0: 6d2f 6769 742f 4b61 6e62 616e 2f64 6a61  m/git/Kanban/dja
-000002c0: 6e67 6f2d 636f 6e6e 6563 7477 6973 652f  ngo-connectwise/
-000002d0: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
-000002e0: 7365 2f64 6a63 6f6e 6e65 6374 7769 7365  se/djconnectwise
-000002f0: 2f6d 6967 7261 7469 6f6e 732f 3031 3035  /migrations/0105
-00000300: 5f61 7574 6f5f 3230 3139 3037 3232 5f31  _auto_20190722_1
-00000310: 3434 342e 7079 7204 0000 0007 0000 0073  444.pyr........s
-00000320: 1200 0000 0c03 0904 0901 0601 0601 3002  ..............0.
-00000330: 0901 0601 0601 7204 0000 0029 06da 0964  ......r....)...d
-00000340: 6a61 6e67 6f2e 6462 7202 0000 0072 0300  jango.dbr....r..
-00000350: 0000 da19 646a 616e 676f 2e64 622e 6d6f  ....django.db.mo
-00000360: 6465 6c73 2e64 656c 6574 696f 6e72 1700  dels.deletionr..
-00000370: 0000 7204 0000 0072 1c00 0000 721c 0000  ..r....r....r...
-00000380: 0072 1c00 0000 721d 0000 00da 083c 6d6f  .r....r......<mo
-00000390: 6475 6c65 3e03 0000 0073 0400 0000 1601  dule>....s......
-000003a0: 0c03                                     ..
+00000020: 0073 2e00 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 4700  m.Z...d.d.l.Z.G.
+00000040: 6403 6404 8400 6404 6501 6a05 8303 5a05  d.d...d.e.j...Z.
+00000050: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 734e 6300 0000 0000 0000 0000 0000 000a  sNc.............
+00000080: 0000 0040 0000 0073 3c00 0000 6500 5a01  ...@...s<...e.Z.
+00000090: 6400 5a02 640b 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000a0: 6404 6506 6a07 6405 6405 6508 6a09 6a06  d.e.j.d.d.e.j.j.
+000000b0: 6a0a 6a0b 6406 6407 6408 8d05 6409 8d03  j.j.d.d.d...d...
+000000c0: 6701 5a0c 640a 5300 290c da09 4d69 6772  g.Z.d.S.)...Migr
+000000d0: 6174 696f 6eda 0d64 6a63 6f6e 6e65 6374  ation..djconnect
+000000e0: 7769 7365 da17 3030 3938 5f61 7574 6f5f  wise..0098_auto_
+000000f0: 3230 3139 3037 3138 5f31 3430 36da 0974  20190718_1406..t
+00000100: 696d 6565 6e74 7279 da09 6167 7265 656d  imeentry..agreem
+00000110: 656e 7454 da11 6167 7265 656d 656e 745f  entT..agreement_
+00000120: 7469 636b 6574 737a 1764 6a63 6f6e 6e65  ticketsz.djconne
+00000130: 6374 7769 7365 2e41 6772 6565 6d65 6e74  ctwise.Agreement
+00000140: 2905 da05 626c 616e 6bda 046e 756c 6cda  )...blank..null.
+00000150: 096f 6e5f 6465 6c65 7465 da0c 7265 6c61  .on_delete..rela
+00000160: 7465 645f 6e61 6d65 da02 746f 2903 da0a  ted_name..to)...
+00000170: 6d6f 6465 6c5f 6e61 6d65 da04 6e61 6d65  model_name..name
+00000180: da05 6669 656c 644e 2902 7205 0000 0072  ..fieldN).r....r
+00000190: 0600 0000 290d da08 5f5f 6e61 6d65 5f5f  ....)...__name__
+000001a0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+000001b0: 7175 616c 6e61 6d65 5f5f da0c 6465 7065  qualname__..depe
+000001c0: 6e64 656e 6369 6573 7202 0000 00da 0841  ndenciesr......A
+000001d0: 6464 4669 656c 6472 0300 0000 da0a 466f  ddFieldr......Fo
+000001e0: 7265 6967 6e4b 6579 da06 646a 616e 676f  reignKey..django
+000001f0: da02 6462 da08 6465 6c65 7469 6f6e da08  ..db..deletion..
+00000200: 5345 545f 4e55 4c4c da0a 6f70 6572 6174  SET_NULL..operat
+00000210: 696f 6e73 a900 721d 0000 0072 1d00 0000  ions..r....r....
+00000220: fa64 2f68 6f6d 652f 6361 6d65 726f 6e2f  .d/home/cameron/
+00000230: 4465 762f 6b61 6e62 616e 2d64 6576 2f64  Dev/kanban-dev/d
+00000240: 6a61 6e67 6f2d 636f 6e6e 6563 7477 6973  jango-connectwis
+00000250: 652f 646a 636f 6e6e 6563 7477 6973 652f  e/djconnectwise/
+00000260: 6d69 6772 6174 696f 6e73 2f30 3039 395f  migrations/0099_
+00000270: 7469 6d65 656e 7472 795f 6167 7265 656d  timeentry_agreem
+00000280: 656e 742e 7079 7204 0000 0007 0000 0073  ent.pyr........s
+00000290: 0a00 0000 0803 0604 0401 0201 0201 7204  ..............r.
+000002a0: 0000 0029 06da 0964 6a61 6e67 6f2e 6462  ...)...django.db
+000002b0: 7202 0000 0072 0300 0000 da19 646a 616e  r....r......djan
+000002c0: 676f 2e64 622e 6d6f 6465 6c73 2e64 656c  go.db.models.del
+000002d0: 6574 696f 6e72 1800 0000 7204 0000 0072  etionr....r....r
+000002e0: 1d00 0000 721d 0000 0072 1d00 0000 721e  ....r....r....r.
+000002f0: 0000 00da 083c 6d6f 6475 6c65 3e03 0000  .....<module>...
+00000300: 0073 0400 0000 1001 0803                 .s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0100_auto_20190718_1417.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0117_auto_20200609_1514.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,60 @@
-00000000: 160d 0d0a ced8 355d 0302 0000 e300 0000  ......5]........
+00000000: 330d 0d0a 525b e15e 7a03 0000 e300 0000  3...R[.^z.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 0f00 0000 4000 0000 7364 0000 0065 0000  ....@...sd...e..
-000000a0: 5a01 0064 0000 5a02 0064 0f00 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6407 0065 0600 6a07 0064 0800  .d..d..e..j..d..
-000000d0: 6409 0064 0a00 6409 0064 0b00 6508 006a  d..d..d..d..e..j
-000000e0: 0900 6a06 006a 0a00 6a0b 0064 0c00 640d  ..j..j..j..d..d.
-000000f0: 0083 0004 8300 0367 0100 5a0c 0064 0e00  .......g..Z..d..
-00000100: 5329 10da 094d 6967 7261 7469 6f6e da0d  S)...Migration..
-00000110: 646a 636f 6e6e 6563 7477 6973 65da 1830  djconnectwise..0
-00000120: 3039 395f 7469 6d65 656e 7472 795f 6167  099_timeentry_ag
-00000130: 7265 656d 656e 74da 0a6d 6f64 656c 5f6e  reement..model_n
-00000140: 616d 65da 0974 696d 6565 6e74 7279 da04  ame..timeentry..
-00000150: 6e61 6d65 da09 6167 7265 656d 656e 74da  name..agreement.
-00000160: 0566 6965 6c64 da05 626c 616e 6b54 da04  .field..blankT..
-00000170: 6e75 6c6c da09 6f6e 5f64 656c 6574 65da  null..on_delete.
-00000180: 0274 6f7a 1764 6a63 6f6e 6e65 6374 7769  .toz.djconnectwi
-00000190: 7365 2e41 6772 6565 6d65 6e74 4e29 027a  se.AgreementN).z
-000001a0: 0d64 6a63 6f6e 6e65 6374 7769 7365 7206  .djconnectwiser.
-000001b0: 0000 0029 0dda 085f 5f6e 616d 655f 5fda  ...)...__name__.
-000001c0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000001d0: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
-000001e0: 6465 6e63 6965 7372 0200 0000 da0a 416c  denciesr......Al
-000001f0: 7465 7246 6965 6c64 7203 0000 00da 0a46  terFieldr......F
-00000200: 6f72 6569 676e 4b65 79da 0664 6a61 6e67  oreignKey..djang
-00000210: 6fda 0264 62da 0864 656c 6574 696f 6eda  o..db..deletion.
-00000220: 0853 4554 5f4e 554c 4cda 0a6f 7065 7261  .SET_NULL..opera
-00000230: 7469 6f6e 73a9 0072 1b00 0000 721b 0000  tions..r....r...
-00000240: 00fa 6e2f 686f 6d65 2f73 616d 2f67 6974  ..n/home/sam/git
-00000250: 2f4b 616e 6261 6e2f 646a 616e 676f 2d63  /Kanban/django-c
-00000260: 6f6e 6e65 6374 7769 7365 2f64 6a61 6e67  onnectwise/djang
-00000270: 6f2d 636f 6e6e 6563 7477 6973 652f 646a  o-connectwise/dj
-00000280: 636f 6e6e 6563 7477 6973 652f 6d69 6772  connectwise/migr
-00000290: 6174 696f 6e73 2f30 3130 305f 6175 746f  ations/0100_auto
-000002a0: 5f32 3031 3930 3731 385f 3134 3137 2e70  _20190718_1417.p
-000002b0: 7972 0400 0000 0700 0000 730a 0000 000c  yr........s.....
-000002c0: 0309 0409 0106 0106 0172 0400 0000 2906  .........r....).
-000002d0: da09 646a 616e 676f 2e64 6272 0200 0000  ..django.dbr....
-000002e0: 7203 0000 00da 1964 6a61 6e67 6f2e 6462  r......django.db
-000002f0: 2e6d 6f64 656c 732e 6465 6c65 7469 6f6e  .models.deletion
-00000300: 7216 0000 0072 0400 0000 721b 0000 0072  r....r....r....r
-00000310: 1b00 0000 721b 0000 0072 1c00 0000 da08  ....r....r......
-00000320: 3c6d 6f64 756c 653e 0300 0000 7304 0000  <module>....s...
-00000330: 0016 010c 03                             .....
+00000020: 0073 2e00 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 4700  m.Z...d.d.l.Z.G.
+00000040: 6403 6404 8400 6404 6501 6a05 8303 5a05  d.d...d.e.j...Z.
+00000050: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 734e 6300 0000 0000 0000 0000 0000 000b  sNc.............
+00000080: 0000 0040 0000 0073 6c00 0000 6500 5a01  ...@...sl...e.Z.
+00000090: 6400 5a02 6412 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000a0: 6404 6506 6a07 6405 6406 8d01 6407 8d03  d.e.j.d.d...d...
+000000b0: 6504 6a05 6408 6409 6506 6a08 640a 640a  e.j.d.d.e.j.d.d.
+000000c0: 6509 6a0a 6a06 6a0b 6a0c 640b 640c 8d04  e.j.j.j.j.d.d...
+000000d0: 6407 8d03 6504 6a05 6408 640d 6506 6a0d  d...e.j.d.d.e.j.
+000000e0: 640a 640e 640f 640a 6410 8d04 6407 8d03  d.d.d.d.d...d...
+000000f0: 6703 5a0e 6411 5300 2913 da09 4d69 6772  g.Z.d.S.)...Migr
+00000100: 6174 696f 6eda 0d64 6a63 6f6e 6e65 6374  ation..djconnect
+00000110: 7769 7365 da17 3031 3136 5f61 7574 6f5f  wise..0116_auto_
+00000120: 3230 3230 3035 3232 5f31 3130 37da 1063  20200522_1107..c
+00000130: 6f6e 6e65 6374 7769 7365 626f 6172 64da  onnectwiseboard.
+00000140: 0c70 726f 6a65 6374 5f66 6c61 6746 2901  .project_flagF).
+00000150: da07 6465 6661 756c 7429 03da 0a6d 6f64  ..default)...mod
+00000160: 656c 5f6e 616d 65da 046e 616d 65da 0566  el_name..name..f
+00000170: 6965 6c64 da07 7072 6f6a 6563 74da 0562  ield..project..b
+00000180: 6f61 7264 547a 1e64 6a63 6f6e 6e65 6374  oardTz.djconnect
+00000190: 7769 7365 2e43 6f6e 6e65 6374 5769 7365  wise.ConnectWise
+000001a0: 426f 6172 6429 04da 0562 6c61 6e6b da04  Board)...blank..
+000001b0: 6e75 6c6c da09 6f6e 5f64 656c 6574 65da  null..on_delete.
+000001c0: 0274 6fda 1070 6572 6365 6e74 5f63 6f6d  .to..percent_com
+000001d0: 706c 6574 65e9 0200 0000 e903 0000 0029  plete..........)
+000001e0: 0472 0f00 0000 da0e 6465 6369 6d61 6c5f  .r......decimal_
+000001f0: 706c 6163 6573 da0a 6d61 785f 6469 6769  places..max_digi
+00000200: 7473 7210 0000 004e 2902 7205 0000 0072  tsr....N).r....r
+00000210: 0600 0000 290f da08 5f5f 6e61 6d65 5f5f  ....)...__name__
+00000220: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000230: 7175 616c 6e61 6d65 5f5f da0c 6465 7065  qualname__..depe
+00000240: 6e64 656e 6369 6573 7202 0000 00da 0841  ndenciesr......A
+00000250: 6464 4669 656c 6472 0300 0000 da0c 426f  ddFieldr......Bo
+00000260: 6f6c 6561 6e46 6965 6c64 da0a 466f 7265  oleanField..Fore
+00000270: 6967 6e4b 6579 da06 646a 616e 676f da02  ignKey..django..
+00000280: 6462 da08 6465 6c65 7469 6f6e da07 4341  db..deletion..CA
+00000290: 5343 4144 45da 0c44 6563 696d 616c 4669  SCADE..DecimalFi
+000002a0: 656c 64da 0a6f 7065 7261 7469 6f6e 73a9  eld..operations.
+000002b0: 0072 2500 0000 7225 0000 00fa 632f 686f  .r%...r%....c/ho
+000002c0: 6d65 2f63 616d 6572 6f6e 2f44 6576 2f6b  me/cameron/Dev/k
+000002d0: 616e 6261 6e2d 6465 762f 646a 616e 676f  anban-dev/django
+000002e0: 2d63 6f6e 6e65 6374 7769 7365 2f64 6a63  -connectwise/djc
+000002f0: 6f6e 6e65 6374 7769 7365 2f6d 6967 7261  onnectwise/migra
+00000300: 7469 6f6e 732f 3031 3137 5f61 7574 6f5f  tions/0117_auto_
+00000310: 3230 3230 3036 3039 5f31 3531 342e 7079  20200609_1514.py
+00000320: 7204 0000 0007 0000 0073 1a00 0000 0803  r........s......
+00000330: 0604 0401 0201 0201 0e02 0401 0201 0201  ................
+00000340: 1c02 0401 0201 0201 7204 0000 0029 06da  ........r....)..
+00000350: 0964 6a61 6e67 6f2e 6462 7202 0000 0072  .django.dbr....r
+00000360: 0300 0000 da19 646a 616e 676f 2e64 622e  ......django.db.
+00000370: 6d6f 6465 6c73 2e64 656c 6574 696f 6e72  models.deletionr
+00000380: 1f00 0000 7204 0000 0072 2500 0000 7225  ....r....r%...r%
+00000390: 0000 0072 2500 0000 7226 0000 00da 083c  ...r%...r&.....<
+000003a0: 6d6f 6475 6c65 3e03 0000 0073 0400 0000  module>....s....
+000003b0: 1001 0803                                ....
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0019_syncjob_entity_name.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0007_auto_20170311_1415.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-00000000: 160d 0d0a a4b0 1f5d cd01 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c 6a02 0000 e300 0000  3......\j.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 000b 0000 0040 0000 0073  ...........@...s
-000000b0: 5200 0000 6500 005a 0100 6400 005a 0200  R...e..Z..d..Z..
-000000c0: 640f 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 6408 0064 0900 640a 0064 0b00  .j..d..d..d..d..
-000000f0: 8300 0264 0c00 640d 0083 0004 6701 005a  ...d..d.....g..Z
-00000100: 0800 640e 0053 2910 da09 4d69 6772 6174  ..d..S)...Migrat
-00000110: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-00000120: 7365 da17 3030 3138 5f61 7574 6f5f 3230  se..0018_auto_20
-00000130: 3137 3035 3035 5f31 3533 31da 0a6d 6f64  170505_1531..mod
-00000140: 656c 5f6e 616d 65da 0773 796e 636a 6f62  el_name..syncjob
-00000150: da04 6e61 6d65 da0b 656e 7469 7479 5f6e  ..name..entity_n
-00000160: 616d 65da 0566 6965 6c64 da0a 6d61 785f  ame..field..max_
-00000170: 6c65 6e67 7468 e964 0000 00da 0764 6566  length.d.....def
-00000180: 6175 6c74 da00 da10 7072 6573 6572 7665  ault....preserve
-00000190: 5f64 6566 6175 6c74 464e 2902 7a0d 646a  _defaultFN).z.dj
-000001a0: 636f 6e6e 6563 7477 6973 657a 1730 3031  connectwisez.001
-000001b0: 385f 6175 746f 5f32 3031 3730 3530 355f  8_auto_20170505_
-000001c0: 3135 3331 2909 da08 5f5f 6e61 6d65 5f5f  1531)...__name__
-000001d0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-000001e0: 7175 616c 6e61 6d65 5f5f da0c 6465 7065  qualname__..depe
-000001f0: 6e64 656e 6369 6573 7203 0000 00da 0841  ndenciesr......A
-00000200: 6464 4669 656c 6472 0400 0000 da09 4368  ddFieldr......Ch
-00000210: 6172 4669 656c 64da 0a6f 7065 7261 7469  arField..operati
-00000220: 6f6e 73a9 0072 1900 0000 7219 0000 00fa  ons..r....r.....
-00000230: 6f2f 686f 6d65 2f73 616d 2f67 6974 2f4b  o/home/sam/git/K
-00000240: 616e 6261 6e2f 646a 616e 676f 2d63 6f6e  anban/django-con
-00000250: 6e65 6374 7769 7365 2f64 6a61 6e67 6f2d  nectwise/django-
-00000260: 636f 6e6e 6563 7477 6973 652f 646a 636f  connectwise/djco
-00000270: 6e6e 6563 7477 6973 652f 6d69 6772 6174  nnectwise/migrat
-00000280: 696f 6e73 2f30 3031 395f 7379 6e63 6a6f  ions/0019_syncjo
-00000290: 625f 656e 7469 7479 5f6e 616d 652e 7079  b_entity_name.py
-000002a0: 7205 0000 0007 0000 0073 0c00 0000 0c03  r........s......
-000002b0: 0904 0901 0601 0601 1801 7205 0000 004e  ..........r....N
-000002c0: 2906 da0a 5f5f 6675 7475 7265 5f5f 7202  )...__future__r.
-000002d0: 0000 00da 0964 6a61 6e67 6f2e 6462 7203  .....django.dbr.
-000002e0: 0000 0072 0400 0000 7205 0000 0072 1900  ...r....r....r..
-000002f0: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000300: 00da 083c 6d6f 6475 6c65 3e02 0000 0073  ...<module>....s
-00000310: 0400 0000 1002 1603                      ........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0600 0000 4000 0000 733a  ..........@...s:
+000000a0: 0000 0065 005a 0164 005a 0264 0e67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0f64 0764 089c 0264  .e.j.d.d.d.d...d
+000000c0: 098d 0265 046a 0564 0a64 0b64 1064 0c9c  ...e.j.d.d.d.d..
+000000d0: 0264 098d 0267 025a 0664 0d53 0029 11da  .d...g.Z.d.S.)..
+000000e0: 094d 6967 7261 7469 6f6e da0d 646a 636f  .Migration..djco
+000000f0: 6e6e 6563 7477 6973 65da 1730 3030 365f  nnectwise..0006_
+00000100: 6175 746f 5f32 3031 3730 3330 335f 3132  auto_20170303_12
+00000110: 3432 5a0b 626f 6172 6473 7461 7475 73da  42Z.boardstatus.
+00000120: 0b62 6f61 7264 5f5f 6e61 6d65 da0a 736f  .board__name..so
+00000130: 7274 5f6f 7264 6572 da04 6e61 6d65 7a0e  rt_order..namez.
+00000140: 426f 6172 6420 7374 6174 7573 6573 2902  Board statuses).
+00000150: da08 6f72 6465 7269 6e67 da13 7665 7262  ..ordering..verb
+00000160: 6f73 655f 6e61 6d65 5f70 6c75 7261 6c29  ose_name_plural)
+00000170: 0272 0a00 0000 da07 6f70 7469 6f6e 735a  .r......optionsZ
+00000180: 1063 6f6e 6e65 6374 7769 7365 626f 6172  .connectwiseboar
+00000190: 647a 1143 6f6e 6e65 6374 5769 7365 2062  dz.ConnectWise b
+000001a0: 6f61 7264 2902 da0c 7665 7262 6f73 655f  oard)...verbose_
+000001b0: 6e61 6d65 720b 0000 004e 2902 7206 0000  namer....N).r...
+000001c0: 0072 0700 0000 2903 7208 0000 0072 0900  .r....).r....r..
+000001d0: 0000 720a 0000 0029 0172 0a00 0000 2907  ..r....).r....).
+000001e0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+000001f0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000200: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
+00000210: 6573 7203 0000 00da 1141 6c74 6572 4d6f  esr......AlterMo
+00000220: 6465 6c4f 7074 696f 6e73 da0a 6f70 6572  delOptions..oper
+00000230: 6174 696f 6e73 a900 7215 0000 0072 1500  ations..r....r..
+00000240: 0000 fa63 2f68 6f6d 652f 6361 6d65 726f  ...c/home/camero
+00000250: 6e2f 4465 762f 6b61 6e62 616e 2d64 6576  n/Dev/kanban-dev
+00000260: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
+00000270: 6973 652f 646a 636f 6e6e 6563 7477 6973  ise/djconnectwis
+00000280: 652f 6d69 6772 6174 696f 6e73 2f30 3030  e/migrations/000
+00000290: 375f 6175 746f 5f32 3031 3730 3331 315f  7_auto_20170311_
+000002a0: 3134 3135 2e70 7972 0500 0000 0700 0000  1415.pyr........
+000002b0: 730e 0000 0008 0306 0404 0102 010c 0204  s...............
+000002c0: 0102 0172 0500 0000 4e29 06da 0a5f 5f66  ...r....N)...__f
+000002d0: 7574 7572 655f 5f72 0200 0000 da09 646a  uture__r......dj
+000002e0: 616e 676f 2e64 6272 0300 0000 7204 0000  ango.dbr....r...
+000002f0: 0072 0500 0000 7215 0000 0072 1500 0000  .r....r....r....
+00000300: 7215 0000 0072 1600 0000 da08 3c6d 6f64  r....r......<mod
+00000310: 756c 653e 0200 0000 7304 0000 000c 0210  ule>....s.......
+00000320: 03                                       .
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0118_auto_20200623_1016.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0004_auto_20170224_1853.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-00000000: 160d 0d0a f859 f25e a801 0000 e300 0000  .....Y.^........
+00000000: 330d 0d0a 10ec da5c b701 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3300 0000 6400 0064 0100 6c00 006d  .s3...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 4764 0200  ..Z..m..Z...Gd..
-00000040: 6403 0084 0000 6403 0065 0100 6a03 0083  d.....d..e..j...
-00000050: 0300 5a03 0064 0400 5329 05e9 0000 0000  ..Z..d..S)......
-00000060: 2902 da0a 6d69 6772 6174 696f 6e73 da06  )...migrations..
-00000070: 6d6f 6465 6c73 6300 0000 0000 0000 0000  modelsc.........
-00000080: 0000 000d 0000 0040 0000 0073 5200 0000  .......@...sR...
-00000090: 6500 005a 0100 6400 005a 0200 640e 0067  e..Z..d..Z..d..g
-000000a0: 0100 5a03 0065 0400 6a05 0064 0300 6404  ..Z..e..j..d..d.
-000000b0: 0064 0500 6406 0064 0700 6506 006a 0700  .d..d..d..e..j..
-000000c0: 6408 0064 0900 640a 0064 0b00 640c 0064  d..d..d..d..d..d
-000000d0: 0900 8300 0383 0003 6701 005a 0800 640d  ........g..Z..d.
-000000e0: 0053 290f da09 4d69 6772 6174 696f 6eda  .S)...Migration.
-000000f0: 0d64 6a63 6f6e 6e65 6374 7769 7365 da17  .djconnectwise..
-00000100: 3031 3137 5f61 7574 6f5f 3230 3230 3036  0117_auto_202006
-00000110: 3039 5f31 3531 34da 0a6d 6f64 656c 5f6e  09_1514..model_n
-00000120: 616d 65da 066d 656d 6265 72da 046e 616d  ame..member..nam
-00000130: 65da 0c6f 6666 6963 655f 656d 6169 6cda  e..office_email.
-00000140: 0566 6965 6c64 da05 626c 616e 6b54 da0a  .field..blankT..
-00000150: 6d61 785f 6c65 6e67 7468 e9fa 0000 00da  max_length......
-00000160: 046e 756c 6c4e 2902 7a0d 646a 636f 6e6e  .nullN).z.djconn
-00000170: 6563 7477 6973 6572 0600 0000 2909 da08  ectwiser....)...
-00000180: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000190: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000001a0: 5f5f da0c 6465 7065 6e64 656e 6369 6573  __..dependencies
-000001b0: 7202 0000 00da 0a41 6c74 6572 4669 656c  r......AlterFiel
-000001c0: 6472 0300 0000 da0a 456d 6169 6c46 6965  dr......EmailFie
-000001d0: 6c64 da0a 6f70 6572 6174 696f 6e73 a900  ld..operations..
-000001e0: 7217 0000 0072 1700 0000 fa6e 2f68 6f6d  r....r.....n/hom
-000001f0: 652f 7361 6d2f 6769 742f 4b61 6e62 616e  e/sam/git/Kanban
-00000200: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
-00000210: 6973 652f 646a 616e 676f 2d63 6f6e 6e65  ise/django-conne
-00000220: 6374 7769 7365 2f64 6a63 6f6e 6e65 6374  ctwise/djconnect
-00000230: 7769 7365 2f6d 6967 7261 7469 6f6e 732f  wise/migrations/
-00000240: 3031 3138 5f61 7574 6f5f 3230 3230 3036  0118_auto_202006
-00000250: 3233 5f31 3031 362e 7079 7204 0000 0006  23_1016.pyr.....
-00000260: 0000 0073 0a00 0000 0c03 0904 0901 0601  ...s............
-00000270: 0601 7204 0000 004e 2904 da09 646a 616e  ..r....N)...djan
-00000280: 676f 2e64 6272 0200 0000 7203 0000 0072  go.dbr....r....r
-00000290: 0400 0000 7217 0000 0072 1700 0000 7217  ....r....r....r.
-000002a0: 0000 0072 1800 0000 da08 3c6d 6f64 756c  ...r......<modul
-000002b0: 653e 0300 0000 7302 0000 0016 03         e>....s......
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0800 0000 4000 0000 7330  ..........@...s0
+000000a0: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000c0: 0664 0664 078d 0364 088d 0367 015a 0864  .d.d...d...g.Z.d
+000000d0: 0953 0029 0bda 094d 6967 7261 7469 6f6e  .S.)...Migration
+000000e0: da0d 646a 636f 6e6e 6563 7477 6973 65da  ..djconnectwise.
+000000f0: 1730 3030 335f 6175 746f 5f32 3031 3730  .0003_auto_20170
+00000100: 3232 335f 3232 3333 da07 7072 6f6a 6563  223_2233..projec
+00000110: 745a 0c70 726f 6a65 6374 5f68 7265 66e9  tZ.project_href.
+00000120: c800 0000 5429 03da 0a6d 6178 5f6c 656e  ....T)...max_len
+00000130: 6774 68da 0562 6c61 6e6b da04 6e75 6c6c  gth..blank..null
+00000140: 2903 da0a 6d6f 6465 6c5f 6e61 6d65 da04  )...model_name..
+00000150: 6e61 6d65 da05 6669 656c 644e 2902 7206  name..fieldN).r.
+00000160: 0000 0072 0700 0000 2909 da08 5f5f 6e61  ...r....)...__na
+00000170: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000180: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
+00000190: 6465 7065 6e64 656e 6369 6573 7203 0000  dependenciesr...
+000001a0: 00da 0a41 6c74 6572 4669 656c 6472 0400  ...AlterFieldr..
+000001b0: 0000 da09 4368 6172 4669 656c 64da 0a6f  ....CharField..o
+000001c0: 7065 7261 7469 6f6e 73a9 0072 1700 0000  perations..r....
+000001d0: 7217 0000 00fa 632f 686f 6d65 2f63 616d  r.....c/home/cam
+000001e0: 6572 6f6e 2f44 6576 2f6b 616e 6261 6e2d  eron/Dev/kanban-
+000001f0: 6465 762f 646a 616e 676f 2d63 6f6e 6e65  dev/django-conne
+00000200: 6374 7769 7365 2f64 6a63 6f6e 6e65 6374  ctwise/djconnect
+00000210: 7769 7365 2f6d 6967 7261 7469 6f6e 732f  wise/migrations/
+00000220: 3030 3034 5f61 7574 6f5f 3230 3137 3032  0004_auto_201702
+00000230: 3234 5f31 3835 332e 7079 7205 0000 0007  24_1853.pyr.....
+00000240: 0000 0073 0a00 0000 0803 0604 0401 0201  ...s............
+00000250: 0201 7205 0000 004e 2906 da0a 5f5f 6675  ..r....N)...__fu
+00000260: 7475 7265 5f5f 7202 0000 00da 0964 6a61  ture__r......dja
+00000270: 6e67 6f2e 6462 7203 0000 0072 0400 0000  ngo.dbr....r....
+00000280: 7205 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
+00000290: 1700 0000 7218 0000 00da 083c 6d6f 6475  ....r......<modu
+000002a0: 6c65 3e02 0000 0073 0400 0000 0c02 1003  le>....s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0026_merge.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0061_auto_20180605_1208.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-00000000: 160d 0d0a a4b0 1f5d 3301 0000 e300 0000  .......]3.......
+00000000: 330d 0d0a 10ec da5c 8101 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000000b0: 2200 0000 6500 005a 0100 6400 005a 0200  "...e..Z..d..Z..
-000000c0: 6405 0064 0600 6702 005a 0300 6700 005a  d..d..g..Z..g..Z
-000000d0: 0400 6404 0053 2907 da09 4d69 6772 6174  ..d..S)...Migrat
-000000e0: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-000000f0: 7365 da1c 3030 3230 5f74 6963 6b65 745f  se..0020_ticket_
-00000100: 6375 7374 6f6d 6572 5f75 7064 6174 6564  customer_updated
-00000110: da10 3030 3235 5f6f 7070 6f72 7475 6e69  ..0025_opportuni
-00000120: 7479 4e29 02fa 0d64 6a63 6f6e 6e65 6374  tyN)...djconnect
-00000130: 7769 7365 7a1c 3030 3230 5f74 6963 6b65  wisez.0020_ticke
-00000140: 745f 6375 7374 6f6d 6572 5f75 7064 6174  t_customer_updat
-00000150: 6564 2902 7209 0000 007a 1030 3032 355f  ed).r....z.0025_
-00000160: 6f70 706f 7274 756e 6974 7929 05da 085f  opportunity)..._
-00000170: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000180: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000190: 5fda 0c64 6570 656e 6465 6e63 6965 73da  _..dependencies.
-000001a0: 0a6f 7065 7261 7469 6f6e 73a9 0072 0f00  .operations..r..
-000001b0: 0000 720f 0000 00fa 612f 686f 6d65 2f73  ..r.....a/home/s
-000001c0: 616d 2f67 6974 2f4b 616e 6261 6e2f 646a  am/git/Kanban/dj
-000001d0: 616e 676f 2d63 6f6e 6e65 6374 7769 7365  ango-connectwise
-000001e0: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
-000001f0: 6973 652f 646a 636f 6e6e 6563 7477 6973  ise/djconnectwis
-00000200: 652f 6d69 6772 6174 696f 6e73 2f30 3032  e/migrations/002
-00000210: 365f 6d65 7267 652e 7079 7205 0000 0007  6_merge.pyr.....
-00000220: 0000 0073 0600 0000 0c03 0301 0903 7205  ...s..........r.
-00000230: 0000 004e 2906 da0a 5f5f 6675 7475 7265  ...N)...__future
-00000240: 5f5f 7202 0000 00da 0964 6a61 6e67 6f2e  __r......django.
-00000250: 6462 7203 0000 0072 0400 0000 7205 0000  dbr....r....r...
-00000260: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
-00000270: 7210 0000 00da 083c 6d6f 6475 6c65 3e02  r......<module>.
-00000280: 0000 0073 0400 0000 1002 1603            ...s........
+00000020: 0073 2200 0000 6400 6401 6c00 6d01 5a01  .s"...d.d.l.m.Z.
+00000030: 0100 4700 6402 6403 8400 6403 6501 6a02  ..G.d.d...d.e.j.
+00000040: 8303 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
+00000050: 01da 0a6d 6967 7261 7469 6f6e 7363 0000  ...migrationsc..
+00000060: 0000 0000 0000 0000 0000 0500 0000 4000  ..............@.
+00000070: 0000 7328 0000 0065 005a 0164 005a 0264  ..s(...e.Z.d.Z.d
+00000080: 0a67 015a 0365 046a 0564 0364 0b64 0664  .g.Z.e.j.d.d.d.d
+00000090: 079c 0264 088d 0267 015a 0664 0953 0029  ...d...g.Z.d.S.)
+000000a0: 0cda 094d 6967 7261 7469 6f6e da0d 646a  ...Migration..dj
+000000b0: 636f 6e6e 6563 7477 6973 65da 1730 3036  connectwise..006
+000000c0: 305f 6175 746f 5f32 3031 3830 3630 355f  0_auto_20180605_
+000000d0: 3038 3430 da04 7465 616d da04 6e61 6d65  0840..team..name
+000000e0: da02 6964 da05 5465 616d 7329 02da 086f  ..id..Teams)...o
+000000f0: 7264 6572 696e 67da 1376 6572 626f 7365  rdering..verbose
+00000100: 5f6e 616d 655f 706c 7572 616c 2902 7207  _name_plural).r.
+00000110: 0000 00da 076f 7074 696f 6e73 4e29 0272  .....optionsN).r
+00000120: 0400 0000 7205 0000 0029 0272 0700 0000  ....r....).r....
+00000130: 7208 0000 0029 07da 085f 5f6e 616d 655f  r....)...__name_
+00000140: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000150: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
+00000160: 656e 6465 6e63 6965 7372 0200 0000 da11  endenciesr......
+00000170: 416c 7465 724d 6f64 656c 4f70 7469 6f6e  AlterModelOption
+00000180: 73da 0a6f 7065 7261 7469 6f6e 73a9 0072  s..operations..r
+00000190: 1300 0000 7213 0000 00fa 632f 686f 6d65  ....r.....c/home
+000001a0: 2f63 616d 6572 6f6e 2f44 6576 2f6b 616e  /cameron/Dev/kan
+000001b0: 6261 6e2d 6465 762f 646a 616e 676f 2d63  ban-dev/django-c
+000001c0: 6f6e 6e65 6374 7769 7365 2f64 6a63 6f6e  onnectwise/djcon
+000001d0: 6e65 6374 7769 7365 2f6d 6967 7261 7469  nectwise/migrati
+000001e0: 6f6e 732f 3030 3631 5f61 7574 6f5f 3230  ons/0061_auto_20
+000001f0: 3138 3036 3035 5f31 3230 382e 7079 7203  180605_1208.pyr.
+00000200: 0000 0006 0000 0073 0800 0000 0803 0604  .......s........
+00000210: 0401 0201 7203 0000 004e 2903 da09 646a  ....r....N)...dj
+00000220: 616e 676f 2e64 6272 0200 0000 7203 0000  ango.dbr....r...
+00000230: 0072 1300 0000 7213 0000 0072 1300 0000  .r....r....r....
+00000240: 7214 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
+00000250: 0000 0073 0200 0000 0c03                 ...s......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0004_auto_20170224_1853.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0106_auto_20190722_1524.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,52 @@
-00000000: 160d 0d0a a4b0 1f5d b701 0000 e300 0000  .......]........
+00000000: 330d 0d0a 2a3e 545d eb02 0000 e300 0000  3...*>T]........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 000d 0000 0040 0000 0073  ...........@...s
-000000b0: 5200 0000 6500 005a 0100 6400 005a 0200  R...e..Z..d..Z..
-000000c0: 640e 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 6408 0064 0900 640a 0064 0b00  .j..d..d..d..d..
-000000f0: 640c 0064 0b00 8300 0383 0003 6701 005a  d..d........g..Z
-00000100: 0800 640d 0053 290f da09 4d69 6772 6174  ..d..S)...Migrat
-00000110: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-00000120: 7365 da17 3030 3033 5f61 7574 6f5f 3230  se..0003_auto_20
-00000130: 3137 3032 3233 5f32 3233 33da 0a6d 6f64  170223_2233..mod
-00000140: 656c 5f6e 616d 65da 0770 726f 6a65 6374  el_name..project
-00000150: da04 6e61 6d65 5a0c 7072 6f6a 6563 745f  ..nameZ.project_
-00000160: 6872 6566 da05 6669 656c 64da 0a6d 6178  href..field..max
-00000170: 5f6c 656e 6774 68e9 c800 0000 da05 626c  _length.......bl
-00000180: 616e 6b54 da04 6e75 6c6c 4e29 027a 0d64  ankT..nullN).z.d
-00000190: 6a63 6f6e 6e65 6374 7769 7365 7207 0000  jconnectwiser...
-000001a0: 0029 09da 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
-000001b0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-000001c0: 6c6e 616d 655f 5fda 0c64 6570 656e 6465  lname__..depende
-000001d0: 6e63 6965 7372 0300 0000 da0a 416c 7465  nciesr......Alte
-000001e0: 7246 6965 6c64 7204 0000 00da 0943 6861  rFieldr......Cha
-000001f0: 7246 6965 6c64 da0a 6f70 6572 6174 696f  rField..operatio
-00000200: 6e73 a900 7217 0000 0072 1700 0000 fa6e  ns..r....r.....n
-00000210: 2f68 6f6d 652f 7361 6d2f 6769 742f 4b61  /home/sam/git/Ka
-00000220: 6e62 616e 2f64 6a61 6e67 6f2d 636f 6e6e  nban/django-conn
-00000230: 6563 7477 6973 652f 646a 616e 676f 2d63  ectwise/django-c
-00000240: 6f6e 6e65 6374 7769 7365 2f64 6a63 6f6e  onnectwise/djcon
-00000250: 6e65 6374 7769 7365 2f6d 6967 7261 7469  nectwise/migrati
-00000260: 6f6e 732f 3030 3034 5f61 7574 6f5f 3230  ons/0004_auto_20
-00000270: 3137 3032 3234 5f31 3835 332e 7079 7205  170224_1853.pyr.
-00000280: 0000 0007 0000 0073 0a00 0000 0c03 0904  .......s........
-00000290: 0901 0601 0601 7205 0000 004e 2906 da0a  ......r....N)...
-000002a0: 5f5f 6675 7475 7265 5f5f 7202 0000 00da  __future__r.....
-000002b0: 0964 6a61 6e67 6f2e 6462 7203 0000 0072  .django.dbr....r
-000002c0: 0400 0000 7205 0000 0072 1700 0000 7217  ....r....r....r.
-000002d0: 0000 0072 1700 0000 7218 0000 00da 083c  ...r....r......<
-000002e0: 6d6f 6475 6c65 3e02 0000 0073 0400 0000  module>....s....
-000002f0: 1002 1603                                ....
+00000020: 0073 2e00 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 4700  m.Z...d.d.l.Z.G.
+00000040: 6403 6404 8400 6404 6501 6a05 8303 5a05  d.d...d.e.j...Z.
+00000050: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 734e 6300 0000 0000 0000 0000 0000 000a  sNc.............
+00000080: 0000 0040 0000 0073 5e00 0000 6500 5a01  ...@...s^...e.Z.
+00000090: 6400 5a02 640c 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000a0: 6404 6506 6a07 6405 6405 6508 6a09 6a06  d.e.j.d.d.e.j.j.
+000000b0: 6a0a 6a0b 6406 6407 8d04 6408 8d03 6504  j.j.d.d...d...e.
+000000c0: 6a05 6403 6409 6506 6a07 6405 6405 6508  j.d.d.e.j.d.d.e.
+000000d0: 6a09 6a06 6a0a 6a0c 640a 6407 8d04 6408  j.j.j.j.d.d...d.
+000000e0: 8d03 6702 5a0d 640b 5300 290d da09 4d69  ..g.Z.d.S.)...Mi
+000000f0: 6772 6174 696f 6eda 0d64 6a63 6f6e 6e65  gration..djconne
+00000100: 6374 7769 7365 da17 3031 3035 5f61 7574  ctwise..0105_aut
+00000110: 6f5f 3230 3139 3037 3232 5f31 3434 34da  o_20190722_1444.
+00000120: 0861 6374 6976 6974 79da 0961 6772 6565  .activity..agree
+00000130: 6d65 6e74 547a 1764 6a63 6f6e 6e65 6374  mentTz.djconnect
+00000140: 7769 7365 2e41 6772 6565 6d65 6e74 2904  wise.Agreement).
+00000150: da05 626c 616e 6bda 046e 756c 6cda 096f  ..blank..null..o
+00000160: 6e5f 6465 6c65 7465 da02 746f 2903 da0a  n_delete..to)...
+00000170: 6d6f 6465 6c5f 6e61 6d65 da04 6e61 6d65  model_name..name
+00000180: da05 6669 656c 64da 0763 6f6d 7061 6e79  ..field..company
+00000190: 7a15 646a 636f 6e6e 6563 7477 6973 652e  z.djconnectwise.
+000001a0: 436f 6d70 616e 794e 2902 7205 0000 0072  CompanyN).r....r
+000001b0: 0600 0000 290e da08 5f5f 6e61 6d65 5f5f  ....)...__name__
+000001c0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+000001d0: 7175 616c 6e61 6d65 5f5f da0c 6465 7065  qualname__..depe
+000001e0: 6e64 656e 6369 6573 7202 0000 00da 0841  ndenciesr......A
+000001f0: 6464 4669 656c 6472 0300 0000 da0a 466f  ddFieldr......Fo
+00000200: 7265 6967 6e4b 6579 da06 646a 616e 676f  reignKey..django
+00000210: da02 6462 da08 6465 6c65 7469 6f6e da08  ..db..deletion..
+00000220: 5345 545f 4e55 4c4c da07 4341 5343 4144  SET_NULL..CASCAD
+00000230: 45da 0a6f 7065 7261 7469 6f6e 73a9 0072  E..operations..r
+00000240: 1d00 0000 721d 0000 00fa 632f 686f 6d65  ....r.....c/home
+00000250: 2f63 616d 6572 6f6e 2f44 6576 2f6b 616e  /cameron/Dev/kan
+00000260: 6261 6e2d 6465 762f 646a 616e 676f 2d63  ban-dev/django-c
+00000270: 6f6e 6e65 6374 7769 7365 2f64 6a63 6f6e  onnectwise/djcon
+00000280: 6e65 6374 7769 7365 2f6d 6967 7261 7469  nectwise/migrati
+00000290: 6f6e 732f 3031 3036 5f61 7574 6f5f 3230  ons/0106_auto_20
+000002a0: 3139 3037 3232 5f31 3532 342e 7079 7204  190722_1524.pyr.
+000002b0: 0000 0007 0000 0073 1200 0000 0803 0604  .......s........
+000002c0: 0401 0201 0201 1c02 0401 0201 0201 7204  ..............r.
+000002d0: 0000 0029 06da 0964 6a61 6e67 6f2e 6462  ...)...django.db
+000002e0: 7202 0000 0072 0300 0000 da19 646a 616e  r....r......djan
+000002f0: 676f 2e64 622e 6d6f 6465 6c73 2e64 656c  go.db.models.del
+00000300: 6574 696f 6e72 1700 0000 7204 0000 0072  etionr....r....r
+00000310: 1d00 0000 721d 0000 0072 1d00 0000 721e  ....r....r....r.
+00000320: 0000 00da 083c 6d6f 6475 6c65 3e03 0000  .....<module>...
+00000330: 0073 0400 0000 1001 0803                 .s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0057_auto_20180511_1440.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0056_auto_20180504_0744.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,52 @@
-00000000: 160d 0d0a a4b0 1f5d a601 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c 6d02 0000 e300 0000  3......\m.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0009 0000 0040 0000 0073  ...........@...s
-000000b0: 4600 0000 6500 005a 0100 6400 005a 0200  F...e..Z..d..Z..
-000000c0: 640b 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6506  ..d..d..d..d..e.
-000000e0: 006a 0700 6408 0064 0900 8300 0183 0003  .j..d..d........
-000000f0: 6701 005a 0800 640a 0053 290c da09 4d69  g..Z..d..S)...Mi
-00000100: 6772 6174 696f 6eda 0d64 6a63 6f6e 6e65  gration..djconne
-00000110: 6374 7769 7365 da17 3030 3536 5f61 7574  ctwise..0056_aut
-00000120: 6f5f 3230 3138 3035 3034 5f30 3734 34da  o_20180504_0744.
-00000130: 0a6d 6f64 656c 5f6e 616d 65da 0b6f 7070  .model_name..opp
-00000140: 6f72 7475 6e69 7479 da04 6e61 6d65 da10  ortunity..name..
-00000150: 6275 7369 6e65 7373 5f75 6e69 745f 6964  business_unit_id
-00000160: da05 6669 656c 64da 046e 756c 6c54 4e29  ..field..nullTN)
-00000170: 027a 0d64 6a63 6f6e 6e65 6374 7769 7365  .z.djconnectwise
-00000180: 7a17 3030 3536 5f61 7574 6f5f 3230 3138  z.0056_auto_2018
-00000190: 3035 3034 5f30 3734 3429 09da 085f 5f6e  0504_0744)...__n
-000001a0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-000001b0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-000001c0: 0c64 6570 656e 6465 6e63 6965 7372 0300  .dependenciesr..
-000001d0: 0000 da0a 416c 7465 7246 6965 6c64 7204  ....AlterFieldr.
-000001e0: 0000 00da 0c49 6e74 6567 6572 4669 656c  .....IntegerFiel
-000001f0: 64da 0a6f 7065 7261 7469 6f6e 73a9 0072  d..operations..r
-00000200: 1500 0000 7215 0000 00fa 6e2f 686f 6d65  ....r.....n/home
-00000210: 2f73 616d 2f67 6974 2f4b 616e 6261 6e2f  /sam/git/Kanban/
-00000220: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
-00000230: 7365 2f64 6a61 6e67 6f2d 636f 6e6e 6563  se/django-connec
-00000240: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
-00000250: 6973 652f 6d69 6772 6174 696f 6e73 2f30  ise/migrations/0
-00000260: 3035 375f 6175 746f 5f32 3031 3830 3531  057_auto_2018051
-00000270: 315f 3134 3430 2e70 7972 0500 0000 0700  1_1440.pyr......
-00000280: 0000 730a 0000 000c 0309 0409 0106 0106  ..s.............
-00000290: 0172 0500 0000 4e29 06da 0a5f 5f66 7574  .r....N)...__fut
-000002a0: 7572 655f 5f72 0200 0000 da09 646a 616e  ure__r......djan
-000002b0: 676f 2e64 6272 0300 0000 7204 0000 0072  go.dbr....r....r
-000002c0: 0500 0000 7215 0000 0072 1500 0000 7215  ....r....r....r.
-000002d0: 0000 0072 1600 0000 da08 3c6d 6f64 756c  ...r......<modul
-000002e0: 653e 0200 0000 7304 0000 0010 0216 03    e>....s........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0800 0000 4000 0000 7340  ..........@...s@
+000000a0: 0000 0065 005a 0164 005a 0264 0e67 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0464 0f64 079c 0264  .e.j.d.d.d.d...d
+000000c0: 088d 0265 046a 0664 0364 0965 076a 0864  ...e.j.d.d.e.j.d
+000000d0: 0a64 0a64 0b8d 0264 0c8d 0367 025a 0964  .d.d...d...g.Z.d
+000000e0: 0d53 0029 10da 094d 6967 7261 7469 6f6e  .S.)...Migration
+000000f0: da0d 646a 636f 6e6e 6563 7477 6973 65da  ..djconnectwise.
+00000100: 1730 3035 355f 6175 746f 5f32 3031 3830  .0055_auto_20180
+00000110: 3530 315f 3130 3232 da0f 6f70 706f 7274  501_1022..opport
+00000120: 756e 6974 796e 6f74 657a 114f 7070 6f72  unitynotez.Oppor
+00000130: 7475 6e69 7479 204e 6f74 6573 fa0d 2d64  tunity Notes..-d
+00000140: 6174 655f 6372 6561 7465 64da 0269 6429  ate_created..id)
+00000150: 02da 1376 6572 626f 7365 5f6e 616d 655f  ...verbose_name_
+00000160: 706c 7572 616c da08 6f72 6465 7269 6e67  plural..ordering
+00000170: 2902 da04 6e61 6d65 da07 6f70 7469 6f6e  )...name..option
+00000180: 73da 0c64 6174 655f 6372 6561 7465 6454  s..date_createdT
+00000190: 2902 da05 626c 616e 6bda 046e 756c 6c29  )...blank..null)
+000001a0: 03da 0a6d 6f64 656c 5f6e 616d 6572 0d00  ...model_namer..
+000001b0: 0000 da05 6669 656c 644e 2902 7206 0000  ....fieldN).r...
+000001c0: 0072 0700 0000 2902 7209 0000 0072 0a00  .r....).r....r..
+000001d0: 0000 290a da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+000001e0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000001f0: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
+00000200: 656e 6369 6573 7203 0000 00da 1141 6c74  enciesr......Alt
+00000210: 6572 4d6f 6465 6c4f 7074 696f 6e73 da08  erModelOptions..
+00000220: 4164 6446 6965 6c64 7204 0000 00da 0d44  AddFieldr......D
+00000230: 6174 6554 696d 6546 6965 6c64 da0a 6f70  ateTimeField..op
+00000240: 6572 6174 696f 6e73 a900 721c 0000 0072  erations..r....r
+00000250: 1c00 0000 fa63 2f68 6f6d 652f 6361 6d65  .....c/home/came
+00000260: 726f 6e2f 4465 762f 6b61 6e62 616e 2d64  ron/Dev/kanban-d
+00000270: 6576 2f64 6a61 6e67 6f2d 636f 6e6e 6563  ev/django-connec
+00000280: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
+00000290: 6973 652f 6d69 6772 6174 696f 6e73 2f30  ise/migrations/0
+000002a0: 3035 365f 6175 746f 5f32 3031 3830 3530  056_auto_2018050
+000002b0: 345f 3037 3434 2e70 7972 0500 0000 0700  4_0744.pyr......
+000002c0: 0000 7310 0000 0008 0306 0404 0102 010c  ..s.............
+000002d0: 0204 0102 0102 0172 0500 0000 4e29 06da  .......r....N)..
+000002e0: 0a5f 5f66 7574 7572 655f 5f72 0200 0000  .__future__r....
+000002f0: da09 646a 616e 676f 2e64 6272 0300 0000  ..django.dbr....
+00000300: 7204 0000 0072 0500 0000 721c 0000 0072  r....r....r....r
+00000310: 1c00 0000 721c 0000 0072 1d00 0000 da08  ....r....r......
+00000320: 3c6d 6f64 756c 653e 0200 0000 7304 0000  <module>....s...
+00000330: 000c 0210 03                             .....
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0052_merge.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0026_merge.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-00000000: 160d 0d0a a4b0 1f5d 2101 0000 e300 0000  .......]!.......
+00000000: 330d 0d0a 10ec da5c 3301 0000 e300 0000  3......\3.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000000b0: 2200 0000 6500 005a 0100 6400 005a 0200  "...e..Z..d..Z..
-000000c0: 6405 0064 0600 6702 005a 0300 6700 005a  d..d..g..Z..g..Z
-000000d0: 0400 6404 0053 2907 da09 4d69 6772 6174  ..d..S)...Migrat
-000000e0: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-000000f0: 7365 da0a 3030 3531 5f6d 6572 6765 da10  se..0051_merge..
-00000100: 3030 3530 5f73 6572 7669 6365 6e6f 7465  0050_servicenote
-00000110: 4e29 02fa 0d64 6a63 6f6e 6e65 6374 7769  N)...djconnectwi
-00000120: 7365 7a0a 3030 3531 5f6d 6572 6765 2902  sez.0051_merge).
-00000130: 7209 0000 007a 1030 3035 305f 7365 7276  r....z.0050_serv
-00000140: 6963 656e 6f74 6529 05da 085f 5f6e 616d  icenote)...__nam
-00000150: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000160: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
-00000170: 6570 656e 6465 6e63 6965 73da 0a6f 7065  ependencies..ope
-00000180: 7261 7469 6f6e 73a9 0072 0f00 0000 720f  rations..r....r.
-00000190: 0000 00fa 612f 686f 6d65 2f73 616d 2f67  ....a/home/sam/g
-000001a0: 6974 2f4b 616e 6261 6e2f 646a 616e 676f  it/Kanban/django
-000001b0: 2d63 6f6e 6e65 6374 7769 7365 2f64 6a61  -connectwise/dja
-000001c0: 6e67 6f2d 636f 6e6e 6563 7477 6973 652f  ngo-connectwise/
-000001d0: 646a 636f 6e6e 6563 7477 6973 652f 6d69  djconnectwise/mi
-000001e0: 6772 6174 696f 6e73 2f30 3035 325f 6d65  grations/0052_me
-000001f0: 7267 652e 7079 7205 0000 0007 0000 0073  rge.pyr........s
-00000200: 0600 0000 0c03 0301 0903 7205 0000 004e  ..........r....N
-00000210: 2906 da0a 5f5f 6675 7475 7265 5f5f 7202  )...__future__r.
-00000220: 0000 00da 0964 6a61 6e67 6f2e 6462 7203  .....django.dbr.
-00000230: 0000 0072 0400 0000 7205 0000 0072 0f00  ...r....r....r..
-00000240: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00000250: 00da 083c 6d6f 6475 6c65 3e02 0000 0073  ...<module>....s
-00000260: 0400 0000 1002 1603                      ........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0300 0000 4000 0000 7318  ..........@...s.
+000000a0: 0000 0065 005a 0164 005a 0264 0564 0667  ...e.Z.d.Z.d.d.g
+000000b0: 025a 0367 005a 0464 0453 0029 07da 094d  .Z.g.Z.d.S.)...M
+000000c0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
+000000d0: 6563 7477 6973 65da 1c30 3032 305f 7469  ectwise..0020_ti
+000000e0: 636b 6574 5f63 7573 746f 6d65 725f 7570  cket_customer_up
+000000f0: 6461 7465 64da 1030 3032 355f 6f70 706f  dated..0025_oppo
+00000100: 7274 756e 6974 794e 2902 7206 0000 0072  rtunityN).r....r
+00000110: 0700 0000 2902 7206 0000 0072 0800 0000  ....).r....r....
+00000120: 2905 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000130: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000140: 6e61 6d65 5f5f da0c 6465 7065 6e64 656e  name__..dependen
+00000150: 6369 6573 da0a 6f70 6572 6174 696f 6e73  cies..operations
+00000160: a900 720e 0000 0072 0e00 0000 fa56 2f68  ..r....r.....V/h
+00000170: 6f6d 652f 6361 6d65 726f 6e2f 4465 762f  ome/cameron/Dev/
+00000180: 6b61 6e62 616e 2d64 6576 2f64 6a61 6e67  kanban-dev/djang
+00000190: 6f2d 636f 6e6e 6563 7477 6973 652f 646a  o-connectwise/dj
+000001a0: 636f 6e6e 6563 7477 6973 652f 6d69 6772  connectwise/migr
+000001b0: 6174 696f 6e73 2f30 3032 365f 6d65 7267  ations/0026_merg
+000001c0: 652e 7079 7205 0000 0007 0000 0073 0600  e.pyr........s..
+000001d0: 0000 0803 0201 0603 7205 0000 004e 2906  ........r....N).
+000001e0: da0a 5f5f 6675 7475 7265 5f5f 7202 0000  ..__future__r...
+000001f0: 00da 0964 6a61 6e67 6f2e 6462 7203 0000  ...django.dbr...
+00000200: 0072 0400 0000 7205 0000 0072 0e00 0000  .r....r....r....
+00000210: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
+00000220: 083c 6d6f 6475 6c65 3e02 0000 0073 0400  .<module>....s..
+00000230: 0000 0c02 1003                           ......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0021_merge.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0078_auto_20181203_1017.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-00000000: 160d 0d0a a4b0 1f5d 2d01 0000 e300 0000  .......]-.......
+00000000: 330d 0d0a 10ec da5c 8501 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000000b0: 2200 0000 6500 005a 0100 6400 005a 0200  "...e..Z..d..Z..
-000000c0: 6405 0064 0600 6702 005a 0300 6700 005a  d..d..g..Z..g..Z
-000000d0: 0400 6404 0053 2907 da09 4d69 6772 6174  ..d..S)...Migrat
-000000e0: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-000000f0: 7365 da0a 3030 3230 5f6d 6572 6765 da1c  se..0020_merge..
-00000100: 3030 3230 5f74 6963 6b65 745f 6375 7374  0020_ticket_cust
-00000110: 6f6d 6572 5f75 7064 6174 6564 4e29 02fa  omer_updatedN)..
-00000120: 0d64 6a63 6f6e 6e65 6374 7769 7365 7207  .djconnectwiser.
-00000130: 0000 0029 0272 0900 0000 7208 0000 0029  ...).r....r....)
-00000140: 05da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000150: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000160: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
-00000170: 6965 73da 0a6f 7065 7261 7469 6f6e 73a9  ies..operations.
-00000180: 0072 0f00 0000 720f 0000 00fa 612f 686f  .r....r.....a/ho
-00000190: 6d65 2f73 616d 2f67 6974 2f4b 616e 6261  me/sam/git/Kanba
-000001a0: 6e2f 646a 616e 676f 2d63 6f6e 6e65 6374  n/django-connect
-000001b0: 7769 7365 2f64 6a61 6e67 6f2d 636f 6e6e  wise/django-conn
+00000020: 0073 2200 0000 6400 6401 6c00 6d01 5a01  .s"...d.d.l.m.Z.
+00000030: 0100 4700 6402 6403 8400 6403 6501 6a02  ..G.d.d...d.e.j.
+00000040: 8303 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
+00000050: 01da 0a6d 6967 7261 7469 6f6e 7363 0000  ...migrationsc..
+00000060: 0000 0000 0000 0000 0000 0500 0000 4000  ..............@.
+00000070: 0000 7328 0000 0065 005a 0164 005a 0264  ..s(...e.Z.d.Z.d
+00000080: 0967 015a 0365 046a 0564 0364 0464 0564  .g.Z.e.j.d.d.d.d
+00000090: 069c 0264 078d 0267 015a 0664 0853 0029  ...d...g.Z.d.S.)
+000000a0: 0ada 094d 6967 7261 7469 6f6e da0d 646a  ...Migration..dj
+000000b0: 636f 6e6e 6563 7477 6973 65da 1630 3037  connectwise..007
+000000c0: 375f 6974 656d 5f73 7562 7479 7065 5f74  7_item_subtype_t
+000000d0: 7970 65da 0773 7562 7479 7065 da07 5375  ype..subtype..Su
+000000e0: 6274 7970 65da 0853 7562 7479 7065 7329  btype..Subtypes)
+000000f0: 02da 0c76 6572 626f 7365 5f6e 616d 65da  ...verbose_name.
+00000100: 1376 6572 626f 7365 5f6e 616d 655f 706c  .verbose_name_pl
+00000110: 7572 616c 2902 da04 6e61 6d65 da07 6f70  ural)...name..op
+00000120: 7469 6f6e 734e 2902 7204 0000 0072 0500  tionsN).r....r..
+00000130: 0000 2907 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+00000140: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000150: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
+00000160: 656e 6369 6573 7202 0000 00da 1141 6c74  enciesr......Alt
+00000170: 6572 4d6f 6465 6c4f 7074 696f 6e73 da0a  erModelOptions..
+00000180: 6f70 6572 6174 696f 6e73 a900 7213 0000  operations..r...
+00000190: 0072 1300 0000 fa63 2f68 6f6d 652f 6361  .r.....c/home/ca
+000001a0: 6d65 726f 6e2f 4465 762f 6b61 6e62 616e  meron/Dev/kanban
+000001b0: 2d64 6576 2f64 6a61 6e67 6f2d 636f 6e6e  -dev/django-conn
 000001c0: 6563 7477 6973 652f 646a 636f 6e6e 6563  ectwise/djconnec
 000001d0: 7477 6973 652f 6d69 6772 6174 696f 6e73  twise/migrations
-000001e0: 2f30 3032 315f 6d65 7267 652e 7079 7205  /0021_merge.pyr.
-000001f0: 0000 0007 0000 0073 0600 0000 0c03 0301  .......s........
-00000200: 0903 7205 0000 004e 2906 da0a 5f5f 6675  ..r....N)...__fu
-00000210: 7475 7265 5f5f 7202 0000 00da 0964 6a61  ture__r......dja
-00000220: 6e67 6f2e 6462 7203 0000 0072 0400 0000  ngo.dbr....r....
-00000230: 7205 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00000240: 0f00 0000 7210 0000 00da 083c 6d6f 6475  ....r......<modu
-00000250: 6c65 3e02 0000 0073 0400 0000 1002 1603  le>....s........
+000001e0: 2f30 3037 385f 6175 746f 5f32 3031 3831  /0078_auto_20181
+000001f0: 3230 335f 3130 3137 2e70 7972 0300 0000  203_1017.pyr....
+00000200: 0600 0000 7308 0000 0008 0306 0404 0102  ....s...........
+00000210: 0172 0300 0000 4e29 03da 0964 6a61 6e67  .r....N)...djang
+00000220: 6f2e 6462 7202 0000 0072 0300 0000 7213  o.dbr....r....r.
+00000230: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+00000240: 0000 da08 3c6d 6f64 756c 653e 0300 0000  ....<module>....
+00000250: 7302 0000 000c 03                        s......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0053_merge.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0089_merge_20190711_1100.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-00000000: 160d 0d0a a4b0 1f5d 2501 0000 e300 0000  .......]%.......
+00000000: 330d 0d0a 94b9 285d 1b01 0000 e300 0000  3.....(]........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000000b0: 2200 0000 6500 005a 0100 6400 005a 0200  "...e..Z..d..Z..
-000000c0: 6405 0064 0600 6702 005a 0300 6700 005a  d..d..g..Z..g..Z
-000000d0: 0400 6404 0053 2907 da09 4d69 6772 6174  ..d..S)...Migrat
-000000e0: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-000000f0: 7365 da14 3030 3531 5f6f 7070 6f72 7475  se..0051_opportu
-00000100: 6e69 7479 6e6f 7465 da0a 3030 3532 5f6d  nitynote..0052_m
-00000110: 6572 6765 4e29 02fa 0d64 6a63 6f6e 6e65  ergeN)...djconne
-00000120: 6374 7769 7365 7a14 3030 3531 5f6f 7070  ctwisez.0051_opp
-00000130: 6f72 7475 6e69 7479 6e6f 7465 2902 7209  ortunitynote).r.
-00000140: 0000 0072 0800 0000 2905 da08 5f5f 6e61  ...r....)...__na
-00000150: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000160: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
-00000170: 6465 7065 6e64 656e 6369 6573 da0a 6f70  dependencies..op
-00000180: 6572 6174 696f 6e73 a900 720f 0000 0072  erations..r....r
-00000190: 0f00 0000 fa61 2f68 6f6d 652f 7361 6d2f  .....a/home/sam/
-000001a0: 6769 742f 4b61 6e62 616e 2f64 6a61 6e67  git/Kanban/djang
-000001b0: 6f2d 636f 6e6e 6563 7477 6973 652f 646a  o-connectwise/dj
-000001c0: 616e 676f 2d63 6f6e 6e65 6374 7769 7365  ango-connectwise
-000001d0: 2f64 6a63 6f6e 6e65 6374 7769 7365 2f6d  /djconnectwise/m
-000001e0: 6967 7261 7469 6f6e 732f 3030 3533 5f6d  igrations/0053_m
-000001f0: 6572 6765 2e70 7972 0500 0000 0700 0000  erge.pyr........
-00000200: 7306 0000 000c 0303 0109 0372 0500 0000  s..........r....
-00000210: 4e29 06da 0a5f 5f66 7574 7572 655f 5f72  N)...__future__r
-00000220: 0200 0000 da09 646a 616e 676f 2e64 6272  ......django.dbr
-00000230: 0300 0000 7204 0000 0072 0500 0000 720f  ....r....r....r.
-00000240: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-00000250: 0000 da08 3c6d 6f64 756c 653e 0200 0000  ....<module>....
-00000260: 7304 0000 0010 0216 03                   s........
+00000020: 0073 2200 0000 6400 6401 6c00 6d01 5a01  .s"...d.d.l.m.Z.
+00000030: 0100 4700 6402 6403 8400 6403 6501 6a02  ..G.d.d...d.e.j.
+00000040: 8303 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
+00000050: 01da 0a6d 6967 7261 7469 6f6e 7363 0000  ...migrationsc..
+00000060: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+00000070: 0000 7318 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00000080: 0564 0667 025a 0367 005a 0464 0453 0029  .d.g.Z.g.Z.d.S.)
+00000090: 07da 094d 6967 7261 7469 6f6e da0d 646a  ...Migration..dj
+000000a0: 636f 6e6e 6563 7477 6973 65da 1730 3038  connectwise..008
+000000b0: 385f 6175 746f 5f32 3031 3930 3731 305f  8_auto_20190710_
+000000c0: 3039 3533 da17 3030 3837 5f61 7574 6f5f  0953..0087_auto_
+000000d0: 3230 3139 3037 3039 5f30 3833 364e 2902  20190709_0836N).
+000000e0: 7204 0000 0072 0500 0000 2902 7204 0000  r....r....).r...
+000000f0: 0072 0600 0000 2905 da08 5f5f 6e61 6d65  .r....)...__name
+00000100: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000110: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
+00000120: 7065 6e64 656e 6369 6573 da0a 6f70 6572  pendencies..oper
+00000130: 6174 696f 6e73 a900 720c 0000 0072 0c00  ations..r....r..
+00000140: 0000 fa64 2f68 6f6d 652f 6361 6d65 726f  ...d/home/camero
+00000150: 6e2f 4465 762f 6b61 6e62 616e 2d64 6576  n/Dev/kanban-dev
+00000160: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
+00000170: 6973 652f 646a 636f 6e6e 6563 7477 6973  ise/djconnectwis
+00000180: 652f 6d69 6772 6174 696f 6e73 2f30 3038  e/migrations/008
+00000190: 395f 6d65 7267 655f 3230 3139 3037 3131  9_merge_20190711
+000001a0: 5f31 3130 302e 7079 7203 0000 0006 0000  _1100.pyr.......
+000001b0: 0073 0600 0000 0803 0201 0603 7203 0000  .s..........r...
+000001c0: 004e 2903 da09 646a 616e 676f 2e64 6272  .N)...django.dbr
+000001d0: 0200 0000 7203 0000 0072 0c00 0000 720c  ....r....r....r.
+000001e0: 0000 0072 0c00 0000 720d 0000 00da 083c  ...r....r......<
+000001f0: 6d6f 6475 6c65 3e03 0000 0073 0200 0000  module>....s....
+00000200: 0c03                                     ..
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0005_auto_20170225_0101.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0005_auto_20170225_0101.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,53 @@
-00000000: 160d 0d0a a4b0 1f5d dc02 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c dc02 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 000d 0000 0040 0000 0073  ...........@...s
-000000b0: 8200 0000 6500 005a 0100 6400 005a 0200  ....e..Z..d..Z..
-000000c0: 6414 0067 0100 5a03 0065 0400 6a05 0064  d..g..Z..e..j..d
-000000d0: 0300 6404 0064 0500 6406 0064 0700 6408  ..d..d..d..d..d.
-000000e0: 0083 0003 6504 006a 0600 6403 0064 0400  ....e..j..d..d..
-000000f0: 6409 0064 0a00 8300 0265 0400 6a07 0064  d..d.....e..j..d
-00000100: 0300 6404 0064 0900 640b 0064 0c00 6508  ..d..d..d..d..e.
-00000110: 006a 0900 640d 0064 0e00 640f 0064 1000  .j..d..d..d..d..
-00000120: 8300 0264 1100 6412 0083 0004 6703 005a  ...d..d.....g..Z
-00000130: 0a00 6413 0053 2915 da09 4d69 6772 6174  ..d..S)...Migrat
-00000140: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-00000150: 7365 da17 3030 3034 5f61 7574 6f5f 3230  se..0004_auto_20
-00000160: 3137 3032 3234 5f31 3835 33da 0a6d 6f64  170224_1853..mod
-00000170: 656c 5f6e 616d 65da 0d63 616c 6c62 6163  el_name..callbac
-00000180: 6b65 6e74 7279 da08 6f6c 645f 6e61 6d65  kentry..old_name
-00000190: da07 656e 6162 6c65 64da 086e 6577 5f6e  ..enabled..new_n
-000001a0: 616d 65da 0d69 6e61 6374 6976 655f 666c  ame..inactive_fl
-000001b0: 6167 da04 6e61 6d65 da08 656e 7472 795f  ag..name..entry_
-000001c0: 6964 da0b 6465 7363 7269 7074 696f 6eda  id..description.
-000001d0: 0566 6965 6c64 da0a 6d61 785f 6c65 6e67  .field..max_leng
-000001e0: 7468 e964 0000 00da 0764 6566 6175 6c74  th.d.....default
-000001f0: da00 da10 7072 6573 6572 7665 5f64 6566  ....preserve_def
-00000200: 6175 6c74 464e 2902 7a0d 646a 636f 6e6e  aultFN).z.djconn
-00000210: 6563 7477 6973 657a 1730 3030 345f 6175  ectwisez.0004_au
-00000220: 746f 5f32 3031 3730 3232 345f 3138 3533  to_20170224_1853
-00000230: 290b da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000240: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000250: 6e61 6d65 5f5f da0c 6465 7065 6e64 656e  name__..dependen
-00000260: 6369 6573 7203 0000 00da 0b52 656e 616d  ciesr......Renam
-00000270: 6546 6965 6c64 da0b 5265 6d6f 7665 4669  eField..RemoveFi
-00000280: 656c 64da 0841 6464 4669 656c 6472 0400  eld..AddFieldr..
-00000290: 0000 da09 4368 6172 4669 656c 64da 0a6f  ....CharField..o
-000002a0: 7065 7261 7469 6f6e 73a9 0072 2000 0000  perations..r ...
-000002b0: 7220 0000 00fa 6e2f 686f 6d65 2f73 616d  r ....n/home/sam
-000002c0: 2f67 6974 2f4b 616e 6261 6e2f 646a 616e  /git/Kanban/djan
-000002d0: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
-000002e0: 6a61 6e67 6f2d 636f 6e6e 6563 7477 6973  jango-connectwis
-000002f0: 652f 646a 636f 6e6e 6563 7477 6973 652f  e/djconnectwise/
-00000300: 6d69 6772 6174 696f 6e73 2f30 3030 355f  migrations/0005_
-00000310: 6175 746f 5f32 3031 3730 3232 355f 3031  auto_20170225_01
-00000320: 3031 2e70 7972 0500 0000 0700 0000 731a  01.pyr........s.
-00000330: 0000 000c 0309 0409 0106 0106 0106 0209  ................
-00000340: 0106 0106 0209 0106 0106 0118 0172 0500  .............r..
-00000350: 0000 4e29 06da 0a5f 5f66 7574 7572 655f  ..N)...__future_
-00000360: 5f72 0200 0000 da09 646a 616e 676f 2e64  _r......django.d
-00000370: 6272 0300 0000 7204 0000 0072 0500 0000  br....r....r....
-00000380: 7220 0000 0072 2000 0000 7220 0000 0072  r ...r ...r ...r
-00000390: 2100 0000 da08 3c6d 6f64 756c 653e 0200  !.....<module>..
-000003a0: 0000 7304 0000 0010 0216 03              ..s........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0900 0000 4000 0000 734a  ..........@...sJ
+000000a0: 0000 0065 005a 0164 005a 0264 1067 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0464 0564 068d 0365  .e.j.d.d.d.d...e
+000000c0: 046a 0664 0364 0764 088d 0265 046a 0764  .j.d.d.d...e.j.d
+000000d0: 0364 0965 086a 0964 0a64 0b64 0c8d 0264  .d.e.j.d.d.d...d
+000000e0: 0d64 0e8d 0467 035a 0a64 0f53 0029 11da  .d...g.Z.d.S.)..
+000000f0: 094d 6967 7261 7469 6f6e da0d 646a 636f  .Migration..djco
+00000100: 6e6e 6563 7477 6973 65da 1730 3030 345f  nnectwise..0004_
+00000110: 6175 746f 5f32 3031 3730 3232 345f 3138  auto_20170224_18
+00000120: 3533 da0d 6361 6c6c 6261 636b 656e 7472  53..callbackentr
+00000130: 79da 0765 6e61 626c 6564 da0d 696e 6163  y..enabled..inac
+00000140: 7469 7665 5f66 6c61 6729 03da 0a6d 6f64  tive_flag)...mod
+00000150: 656c 5f6e 616d 65da 086f 6c64 5f6e 616d  el_name..old_nam
+00000160: 65da 086e 6577 5f6e 616d 65da 0865 6e74  e..new_name..ent
+00000170: 7279 5f69 6429 0272 0b00 0000 da04 6e61  ry_id).r......na
+00000180: 6d65 da0b 6465 7363 7269 7074 696f 6ee9  me..description.
+00000190: 6400 0000 da00 2902 da0a 6d61 785f 6c65  d.....)...max_le
+000001a0: 6e67 7468 da07 6465 6661 756c 7446 2904  ngth..defaultF).
+000001b0: 720b 0000 0072 0f00 0000 da05 6669 656c  r....r......fiel
+000001c0: 64da 1070 7265 7365 7276 655f 6465 6661  d..preserve_defa
+000001d0: 756c 744e 2902 7206 0000 0072 0700 0000  ultN).r....r....
+000001e0: 290b da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000001f0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000200: 6e61 6d65 5f5f da0c 6465 7065 6e64 656e  name__..dependen
+00000210: 6369 6573 7203 0000 00da 0b52 656e 616d  ciesr......Renam
+00000220: 6546 6965 6c64 da0b 5265 6d6f 7665 4669  eField..RemoveFi
+00000230: 656c 64da 0841 6464 4669 656c 6472 0400  eld..AddFieldr..
+00000240: 0000 da09 4368 6172 4669 656c 64da 0a6f  ....CharField..o
+00000250: 7065 7261 7469 6f6e 73a9 0072 2000 0000  perations..r ...
+00000260: 7220 0000 00fa 632f 686f 6d65 2f63 616d  r ....c/home/cam
+00000270: 6572 6f6e 2f44 6576 2f6b 616e 6261 6e2d  eron/Dev/kanban-
+00000280: 6465 762f 646a 616e 676f 2d63 6f6e 6e65  dev/django-conne
+00000290: 6374 7769 7365 2f64 6a63 6f6e 6e65 6374  ctwise/djconnect
+000002a0: 7769 7365 2f6d 6967 7261 7469 6f6e 732f  wise/migrations/
+000002b0: 3030 3035 5f61 7574 6f5f 3230 3137 3032  0005_auto_201702
+000002c0: 3235 5f30 3130 312e 7079 7205 0000 0007  25_0101.pyr.....
+000002d0: 0000 0073 1a00 0000 0803 0604 0401 0201  ...s............
+000002e0: 0201 0602 0401 0201 0602 0401 0201 0201  ................
+000002f0: 0c01 7205 0000 004e 2906 da0a 5f5f 6675  ..r....N)...__fu
+00000300: 7475 7265 5f5f 7202 0000 00da 0964 6a61  ture__r......dja
+00000310: 6e67 6f2e 6462 7203 0000 0072 0400 0000  ngo.dbr....r....
+00000320: 7205 0000 0072 2000 0000 7220 0000 0072  r....r ...r ...r
+00000330: 2000 0000 7221 0000 00da 083c 6d6f 6475   ...r!.....<modu
+00000340: 6c65 3e02 0000 0073 0400 0000 0c02 1003  le>....s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0051_merge.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0020_ticket_customer_updated.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-00000000: 160d 0d0a a4b0 1f5d 2c01 0000 e300 0000  .......],.......
+00000000: 330d 0d0a 10ec da5c 9d01 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000000b0: 2200 0000 6500 005a 0100 6400 005a 0200  "...e..Z..d..Z..
-000000c0: 6405 0064 0600 6702 005a 0300 6700 005a  d..d..g..Z..g..Z
-000000d0: 0400 6404 0053 2907 da09 4d69 6772 6174  ..d..S)...Migrat
-000000e0: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-000000f0: 7365 da17 3030 3530 5f61 7574 6f5f 3230  se..0050_auto_20
-00000100: 3138 3034 3137 5f31 3632 30da 0e30 3035  180417_1620..005
-00000110: 305f 7469 6d65 656e 7472 794e 2902 fa0d  0_timeentryN)...
-00000120: 646a 636f 6e6e 6563 7477 6973 657a 1730  djconnectwisez.0
-00000130: 3035 305f 6175 746f 5f32 3031 3830 3431  050_auto_2018041
-00000140: 375f 3136 3230 2902 7209 0000 007a 0e30  7_1620).r....z.0
-00000150: 3035 305f 7469 6d65 656e 7472 7929 05da  050_timeentry)..
-00000160: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000170: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000180: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
-00000190: 73da 0a6f 7065 7261 7469 6f6e 73a9 0072  s..operations..r
-000001a0: 0f00 0000 720f 0000 00fa 612f 686f 6d65  ....r.....a/home
-000001b0: 2f73 616d 2f67 6974 2f4b 616e 6261 6e2f  /sam/git/Kanban/
-000001c0: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
-000001d0: 7365 2f64 6a61 6e67 6f2d 636f 6e6e 6563  se/django-connec
-000001e0: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
-000001f0: 6973 652f 6d69 6772 6174 696f 6e73 2f30  ise/migrations/0
-00000200: 3035 315f 6d65 7267 652e 7079 7205 0000  051_merge.pyr...
-00000210: 0007 0000 0073 0600 0000 0c03 0301 0903  .....s..........
-00000220: 7205 0000 004e 2906 da0a 5f5f 6675 7475  r....N)...__futu
-00000230: 7265 5f5f 7202 0000 00da 0964 6a61 6e67  re__r......djang
-00000240: 6f2e 6462 7203 0000 0072 0400 0000 7205  o.dbr....r....r.
-00000250: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
-00000260: 0000 7210 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000270: 3e02 0000 0073 0400 0000 1002 1603       >....s........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0600 0000 4000 0000 732c  ..........@...s,
+000000a0: 0000 0065 005a 0164 005a 0264 0967 015a  ...e.Z.d.Z.d.g.Z
+000000b0: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000c0: 068d 0164 078d 0367 015a 0864 0853 0029  ...d...g.Z.d.S.)
+000000d0: 0ada 094d 6967 7261 7469 6f6e da0d 646a  ...Migration..dj
+000000e0: 636f 6e6e 6563 7477 6973 65da 1130 3031  connectwise..001
+000000f0: 395f 7469 636b 6574 5f6f 776e 6572 da06  9_ticket_owner..
+00000100: 7469 636b 6574 da10 6375 7374 6f6d 6572  ticket..customer
+00000110: 5f75 7064 6174 6564 4629 01da 0764 6566  _updatedF)...def
+00000120: 6175 6c74 2903 da0a 6d6f 6465 6c5f 6e61  ault)...model_na
+00000130: 6d65 da04 6e61 6d65 da05 6669 656c 644e  me..name..fieldN
+00000140: 2902 7206 0000 0072 0700 0000 2909 da08  ).r....r....)...
+00000150: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000160: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000170: 5f5f da0c 6465 7065 6e64 656e 6369 6573  __..dependencies
+00000180: 7203 0000 00da 0841 6464 4669 656c 6472  r......AddFieldr
+00000190: 0400 0000 da0c 426f 6f6c 6561 6e46 6965  ......BooleanFie
+000001a0: 6c64 da0a 6f70 6572 6174 696f 6e73 a900  ld..operations..
+000001b0: 7215 0000 0072 1500 0000 fa68 2f68 6f6d  r....r.....h/hom
+000001c0: 652f 6361 6d65 726f 6e2f 4465 762f 6b61  e/cameron/Dev/ka
+000001d0: 6e62 616e 2d64 6576 2f64 6a61 6e67 6f2d  nban-dev/django-
+000001e0: 636f 6e6e 6563 7477 6973 652f 646a 636f  connectwise/djco
+000001f0: 6e6e 6563 7477 6973 652f 6d69 6772 6174  nnectwise/migrat
+00000200: 696f 6e73 2f30 3032 305f 7469 636b 6574  ions/0020_ticket
+00000210: 5f63 7573 746f 6d65 725f 7570 6461 7465  _customer_update
+00000220: 642e 7079 7205 0000 0007 0000 0073 0a00  d.pyr........s..
+00000230: 0000 0803 0604 0401 0201 0201 7205 0000  ............r...
+00000240: 004e 2906 da0a 5f5f 6675 7475 7265 5f5f  .N)...__future__
+00000250: 7202 0000 00da 0964 6a61 6e67 6f2e 6462  r......django.db
+00000260: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
+00000270: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+00000280: 0000 00da 083c 6d6f 6475 6c65 3e02 0000  .....<module>...
+00000290: 0073 0400 0000 0c02 1003                 .s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0094_connectwiseboard_work_role.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0095_connectwiseboard_work_type.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,48 @@
-00000000: 160d 0d0a 22b1 305d 0702 0000 e300 0000  ....".0]........
+00000000: 330d 0d0a 06c1 305d 0e02 0000 e300 0000  3.....0]........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 0f00 0000 4000 0000 7364 0000 0065 0000  ....@...sd...e..
-000000a0: 5a01 0064 0000 5a02 0064 0f00 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6407 0065 0600 6a07 0064 0800  .d..d..e..j..d..
-000000d0: 6409 0064 0a00 6409 0064 0b00 6508 006a  d..d..d..d..e..j
-000000e0: 0900 6a06 006a 0a00 6a0b 0064 0c00 640d  ..j..j..j..d..d.
-000000f0: 0083 0004 8300 0367 0100 5a0c 0064 0e00  .......g..Z..d..
-00000100: 5329 10da 094d 6967 7261 7469 6f6e da0d  S)...Migration..
-00000110: 646a 636f 6e6e 6563 7477 6973 65da 1830  djconnectwise..0
-00000120: 3039 335f 6d65 7267 655f 3230 3139 3037  093_merge_201907
-00000130: 3136 5f31 3435 39da 0a6d 6f64 656c 5f6e  16_1459..model_n
-00000140: 616d 65da 1063 6f6e 6e65 6374 7769 7365  ame..connectwise
-00000150: 626f 6172 64da 046e 616d 65da 0977 6f72  board..name..wor
-00000160: 6b5f 726f 6c65 da05 6669 656c 64da 0562  k_role..field..b
-00000170: 6c61 6e6b 54da 046e 756c 6cda 096f 6e5f  lankT..null..on_
-00000180: 6465 6c65 7465 da02 746f 7a16 646a 636f  delete..toz.djco
-00000190: 6e6e 6563 7477 6973 652e 576f 726b 526f  nnectwise.WorkRo
-000001a0: 6c65 4e29 027a 0d64 6a63 6f6e 6e65 6374  leN).z.djconnect
-000001b0: 7769 7365 7a18 3030 3933 5f6d 6572 6765  wisez.0093_merge
-000001c0: 5f32 3031 3930 3731 365f 3134 3539 290d  _20190716_1459).
-000001d0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000001e0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000001f0: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
-00000200: 6573 7202 0000 00da 0841 6464 4669 656c  esr......AddFiel
-00000210: 6472 0300 0000 da0a 466f 7265 6967 6e4b  dr......ForeignK
-00000220: 6579 da06 646a 616e 676f da02 6462 da08  ey..django..db..
-00000230: 6465 6c65 7469 6f6e da08 5345 545f 4e55  deletion..SET_NU
-00000240: 4c4c da0a 6f70 6572 6174 696f 6e73 a900  LL..operations..
-00000250: 721b 0000 0072 1b00 0000 fa76 2f68 6f6d  r....r.....v/hom
-00000260: 652f 7361 6d2f 6769 742f 4b61 6e62 616e  e/sam/git/Kanban
-00000270: 2f64 6a61 6e67 6f2d 636f 6e6e 6563 7477  /django-connectw
-00000280: 6973 652f 646a 616e 676f 2d63 6f6e 6e65  ise/django-conne
-00000290: 6374 7769 7365 2f64 6a63 6f6e 6e65 6374  ctwise/djconnect
-000002a0: 7769 7365 2f6d 6967 7261 7469 6f6e 732f  wise/migrations/
-000002b0: 3030 3934 5f63 6f6e 6e65 6374 7769 7365  0094_connectwise
-000002c0: 626f 6172 645f 776f 726b 5f72 6f6c 652e  board_work_role.
-000002d0: 7079 7204 0000 0007 0000 0073 0a00 0000  pyr........s....
-000002e0: 0c03 0904 0901 0601 0601 7204 0000 0029  ..........r....)
-000002f0: 06da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
-00000300: 0072 0300 0000 da19 646a 616e 676f 2e64  .r......django.d
-00000310: 622e 6d6f 6465 6c73 2e64 656c 6574 696f  b.models.deletio
-00000320: 6e72 1600 0000 7204 0000 0072 1b00 0000  nr....r....r....
-00000330: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
-00000340: 083c 6d6f 6475 6c65 3e03 0000 0073 0400  .<module>....s..
-00000350: 0000 1601 0c03                           ......
+00000020: 0073 2e00 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 4700  m.Z...d.d.l.Z.G.
+00000040: 6403 6404 8400 6404 6501 6a05 8303 5a05  d.d...d.e.j...Z.
+00000050: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 734e 6300 0000 0000 0000 0000 0000 0009  sNc.............
+00000080: 0000 0040 0000 0073 3a00 0000 6500 5a01  ...@...s:...e.Z.
+00000090: 6400 5a02 640a 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
+000000a0: 6404 6506 6a07 6405 6405 6508 6a09 6a06  d.e.j.d.d.e.j.j.
+000000b0: 6a0a 6a0b 6406 6407 8d04 6408 8d03 6701  j.j.d.d...d...g.
+000000c0: 5a0c 6409 5300 290b da09 4d69 6772 6174  Z.d.S.)...Migrat
+000000d0: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
+000000e0: 7365 da1f 3030 3934 5f63 6f6e 6e65 6374  se..0094_connect
+000000f0: 7769 7365 626f 6172 645f 776f 726b 5f72  wiseboard_work_r
+00000100: 6f6c 65da 1063 6f6e 6e65 6374 7769 7365  ole..connectwise
+00000110: 626f 6172 64da 0977 6f72 6b5f 7479 7065  board..work_type
+00000120: 547a 1664 6a63 6f6e 6e65 6374 7769 7365  Tz.djconnectwise
+00000130: 2e57 6f72 6b54 7970 6529 04da 0562 6c61  .WorkType)...bla
+00000140: 6e6b da04 6e75 6c6c da09 6f6e 5f64 656c  nk..null..on_del
+00000150: 6574 65da 0274 6f29 03da 0a6d 6f64 656c  ete..to)...model
+00000160: 5f6e 616d 65da 046e 616d 65da 0566 6965  _name..name..fie
+00000170: 6c64 4e29 0272 0500 0000 7206 0000 0029  ldN).r....r....)
+00000180: 0dda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000190: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000001a0: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
+000001b0: 6965 7372 0200 0000 da08 4164 6446 6965  iesr......AddFie
+000001c0: 6c64 7203 0000 00da 0a46 6f72 6569 676e  ldr......Foreign
+000001d0: 4b65 79da 0664 6a61 6e67 6fda 0264 62da  Key..django..db.
+000001e0: 0864 656c 6574 696f 6eda 0853 4554 5f4e  .deletion..SET_N
+000001f0: 554c 4cda 0a6f 7065 7261 7469 6f6e 73a9  ULL..operations.
+00000200: 0072 1b00 0000 721b 0000 00fa 6b2f 686f  .r....r.....k/ho
+00000210: 6d65 2f63 616d 6572 6f6e 2f44 6576 2f6b  me/cameron/Dev/k
+00000220: 616e 6261 6e2d 6465 762f 646a 616e 676f  anban-dev/django
+00000230: 2d63 6f6e 6e65 6374 7769 7365 2f64 6a63  -connectwise/djc
+00000240: 6f6e 6e65 6374 7769 7365 2f6d 6967 7261  onnectwise/migra
+00000250: 7469 6f6e 732f 3030 3935 5f63 6f6e 6e65  tions/0095_conne
+00000260: 6374 7769 7365 626f 6172 645f 776f 726b  ctwiseboard_work
+00000270: 5f74 7970 652e 7079 7204 0000 0007 0000  _type.pyr.......
+00000280: 0073 0a00 0000 0803 0604 0401 0201 0201  .s..............
+00000290: 7204 0000 0029 06da 0964 6a61 6e67 6f2e  r....)...django.
+000002a0: 6462 7202 0000 0072 0300 0000 da19 646a  dbr....r......dj
+000002b0: 616e 676f 2e64 622e 6d6f 6465 6c73 2e64  ango.db.models.d
+000002c0: 656c 6574 696f 6e72 1600 0000 7204 0000  eletionr....r...
+000002d0: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
+000002e0: 721c 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
+000002f0: 0000 0073 0400 0000 1001 0803            ...s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0101_agreement_company.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0030_merge.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,35 @@
-00000000: 160d 0d0a ced8 355d f001 0000 e300 0000  ......5]........
+00000000: 330d 0d0a 10ec da5c 2801 0000 e300 0000  3......\(.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3f00 0000 6400 0064 0100 6c00 006d  .s?...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
-00000040: 0200 6c03 005a 0400 4764 0300 6404 0084  ..l..Z..Gd..d...
-00000050: 0000 6404 0065 0100 6a05 0083 0300 5a05  ..d..e..j.....Z.
-00000060: 0064 0200 5329 05e9 0000 0000 2902 da0a  .d..S)......)...
-00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
-00000080: 6c73 4e63 0000 0000 0000 0000 0000 0000  lsNc............
-00000090: 0d00 0000 4000 0000 735e 0000 0065 0000  ....@...s^...e..
-000000a0: 5a01 0064 0000 5a02 0064 0e00 6701 005a  Z..d..Z..d..g..Z
-000000b0: 0300 6504 006a 0500 6403 0064 0400 6405  ..e..j..d..d..d.
-000000c0: 0064 0600 6407 0065 0600 6a07 0064 0800  .d..d..e..j..d..
-000000d0: 6409 0064 0a00 6508 006a 0900 6a06 006a  d..d..e..j..j..j
-000000e0: 0a00 6a0b 0064 0b00 640c 0083 0003 8300  ..j..d..d.......
-000000f0: 0367 0100 5a0c 0064 0d00 5329 0fda 094d  .g..Z..d..S)...M
-00000100: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
-00000110: 6563 7477 6973 65da 1730 3130 305f 6175  ectwise..0100_au
-00000120: 746f 5f32 3031 3930 3731 385f 3134 3137  to_20190718_1417
-00000130: da0a 6d6f 6465 6c5f 6e61 6d65 da09 6167  ..model_name..ag
-00000140: 7265 656d 656e 74da 046e 616d 65da 0763  reement..name..c
-00000150: 6f6d 7061 6e79 da05 6669 656c 64da 046e  ompany..field..n
-00000160: 756c 6c54 da09 6f6e 5f64 656c 6574 65da  ullT..on_delete.
-00000170: 0274 6f7a 1564 6a63 6f6e 6e65 6374 7769  .toz.djconnectwi
-00000180: 7365 2e43 6f6d 7061 6e79 4e29 027a 0d64  se.CompanyN).z.d
-00000190: 6a63 6f6e 6e65 6374 7769 7365 7206 0000  jconnectwiser...
-000001a0: 0029 0dda 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
-000001b0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-000001c0: 6c6e 616d 655f 5fda 0c64 6570 656e 6465  lname__..depende
-000001d0: 6e63 6965 7372 0200 0000 da08 4164 6446  nciesr......AddF
-000001e0: 6965 6c64 7203 0000 00da 0a46 6f72 6569  ieldr......Forei
-000001f0: 676e 4b65 79da 0664 6a61 6e67 6fda 0264  gnKey..django..d
-00000200: 62da 0864 656c 6574 696f 6eda 0853 4554  b..deletion..SET
-00000210: 5f4e 554c 4cda 0a6f 7065 7261 7469 6f6e  _NULL..operation
-00000220: 73a9 0072 1a00 0000 721a 0000 00fa 6d2f  s..r....r.....m/
-00000230: 686f 6d65 2f73 616d 2f67 6974 2f4b 616e  home/sam/git/Kan
-00000240: 6261 6e2f 646a 616e 676f 2d63 6f6e 6e65  ban/django-conne
-00000250: 6374 7769 7365 2f64 6a61 6e67 6f2d 636f  ctwise/django-co
-00000260: 6e6e 6563 7477 6973 652f 646a 636f 6e6e  nnectwise/djconn
-00000270: 6563 7477 6973 652f 6d69 6772 6174 696f  ectwise/migratio
-00000280: 6e73 2f30 3130 315f 6167 7265 656d 656e  ns/0101_agreemen
-00000290: 745f 636f 6d70 616e 792e 7079 7204 0000  t_company.pyr...
-000002a0: 0007 0000 0073 0a00 0000 0c03 0904 0901  .....s..........
-000002b0: 0601 0601 7204 0000 0029 06da 0964 6a61  ....r....)...dja
-000002c0: 6e67 6f2e 6462 7202 0000 0072 0300 0000  ngo.dbr....r....
-000002d0: da19 646a 616e 676f 2e64 622e 6d6f 6465  ..django.db.mode
-000002e0: 6c73 2e64 656c 6574 696f 6e72 1500 0000  ls.deletionr....
-000002f0: 7204 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
-00000300: 1a00 0000 721b 0000 00da 083c 6d6f 6475  ....r......<modu
-00000310: 6c65 3e03 0000 0073 0400 0000 1601 0c03  le>....s........
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0300 0000 4000 0000 7318  ..........@...s.
+000000a0: 0000 0065 005a 0164 005a 0264 0564 0667  ...e.Z.d.Z.d.d.g
+000000b0: 025a 0367 005a 0464 0453 0029 07da 094d  .Z.g.Z.d.S.)...M
+000000c0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
+000000d0: 6563 7477 6973 65da 0a30 3032 395f 6d65  ectwise..0029_me
+000000e0: 7267 65da 1730 3032 395f 6175 746f 5f32  rge..0029_auto_2
+000000f0: 3031 3730 3630 375f 3131 3437 4e29 0272  0170607_1147N).r
+00000100: 0600 0000 7207 0000 0029 0272 0600 0000  ....r....).r....
+00000110: 7208 0000 0029 05da 085f 5f6e 616d 655f  r....)...__name_
+00000120: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000130: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
+00000140: 656e 6465 6e63 6965 73da 0a6f 7065 7261  endencies..opera
+00000150: 7469 6f6e 73a9 0072 0e00 0000 720e 0000  tions..r....r...
+00000160: 00fa 562f 686f 6d65 2f63 616d 6572 6f6e  ..V/home/cameron
+00000170: 2f44 6576 2f6b 616e 6261 6e2d 6465 762f  /Dev/kanban-dev/
+00000180: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
+00000190: 7365 2f64 6a63 6f6e 6e65 6374 7769 7365  se/djconnectwise
+000001a0: 2f6d 6967 7261 7469 6f6e 732f 3030 3330  /migrations/0030
+000001b0: 5f6d 6572 6765 2e70 7972 0500 0000 0700  _merge.pyr......
+000001c0: 0000 7306 0000 0008 0302 0106 0372 0500  ..s..........r..
+000001d0: 0000 4e29 06da 0a5f 5f66 7574 7572 655f  ..N)...__future_
+000001e0: 5f72 0200 0000 da09 646a 616e 676f 2e64  _r......django.d
+000001f0: 6272 0300 0000 7204 0000 0072 0500 0000  br....r....r....
+00000200: 720e 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000210: 0f00 0000 da08 3c6d 6f64 756c 653e 0200  ......<module>..
+00000220: 0000 7304 0000 000c 0210 03              ..s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0028_merge.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0028_merge.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-00000000: 160d 0d0a a4b0 1f5d 2801 0000 e300 0000  .......](.......
+00000000: 330d 0d0a 10ec da5c 2801 0000 e300 0000  3......\(.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4300 0000 6400 0064 0100 6c00 006d  .sC...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 006d 0400 5a04 0001 4764 0300  ..Z..m..Z...Gd..
-00000050: 6404 0084 0000 6404 0065 0300 6a05 0083  d.....d..e..j...
-00000060: 0300 5a05 0064 0500 5329 06e9 0000 0000  ..Z..d..S)......
-00000070: 2901 da10 756e 6963 6f64 655f 6c69 7465  )...unicode_lite
-00000080: 7261 6c73 2902 da0a 6d69 6772 6174 696f  rals)...migratio
-00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
-000000a0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000000b0: 2200 0000 6500 005a 0100 6400 005a 0200  "...e..Z..d..Z..
-000000c0: 6405 0064 0600 6702 005a 0300 6700 005a  d..d..g..Z..g..Z
-000000d0: 0400 6404 0053 2907 da09 4d69 6772 6174  ..d..S)...Migrat
-000000e0: 696f 6eda 0d64 6a63 6f6e 6e65 6374 7769  ion..djconnectwi
-000000f0: 7365 da17 3030 3237 5f61 7574 6f5f 3230  se..0027_auto_20
-00000100: 3137 3036 3035 5f31 3533 34da 0a30 3032  170605_1534..002
-00000110: 315f 6d65 7267 654e 2902 fa0d 646a 636f  1_mergeN)...djco
-00000120: 6e6e 6563 7477 6973 657a 1730 3032 375f  nnectwisez.0027_
-00000130: 6175 746f 5f32 3031 3730 3630 355f 3135  auto_20170605_15
-00000140: 3334 2902 7209 0000 007a 0a30 3032 315f  34).r....z.0021_
-00000150: 6d65 7267 6529 05da 085f 5f6e 616d 655f  merge)...__name_
-00000160: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000170: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
-00000180: 656e 6465 6e63 6965 73da 0a6f 7065 7261  endencies..opera
-00000190: 7469 6f6e 73a9 0072 0f00 0000 720f 0000  tions..r....r...
-000001a0: 00fa 612f 686f 6d65 2f73 616d 2f67 6974  ..a/home/sam/git
-000001b0: 2f4b 616e 6261 6e2f 646a 616e 676f 2d63  /Kanban/django-c
-000001c0: 6f6e 6e65 6374 7769 7365 2f64 6a61 6e67  onnectwise/djang
-000001d0: 6f2d 636f 6e6e 6563 7477 6973 652f 646a  o-connectwise/dj
-000001e0: 636f 6e6e 6563 7477 6973 652f 6d69 6772  connectwise/migr
-000001f0: 6174 696f 6e73 2f30 3032 385f 6d65 7267  ations/0028_merg
-00000200: 652e 7079 7205 0000 0007 0000 0073 0600  e.pyr........s..
-00000210: 0000 0c03 0301 0903 7205 0000 004e 2906  ........r....N).
-00000220: da0a 5f5f 6675 7475 7265 5f5f 7202 0000  ..__future__r...
-00000230: 00da 0964 6a61 6e67 6f2e 6462 7203 0000  ...django.dbr...
-00000240: 0072 0400 0000 7205 0000 0072 0f00 0000  .r....r....r....
-00000250: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
-00000260: 083c 6d6f 6475 6c65 3e02 0000 0073 0400  .<module>....s..
-00000270: 0000 1002 1603                           ......
+00000020: 0073 3200 0000 6400 6401 6c00 6d01 5a01  .s2...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
+00000040: 0100 4700 6403 6404 8400 6404 6503 6a05  ..G.d.d...d.e.j.
+00000050: 8303 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000070: 616c 7329 02da 0a6d 6967 7261 7469 6f6e  als)...migration
+00000080: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000090: 0000 0000 0000 0300 0000 4000 0000 7318  ..........@...s.
+000000a0: 0000 0065 005a 0164 005a 0264 0564 0667  ...e.Z.d.Z.d.d.g
+000000b0: 025a 0367 005a 0464 0453 0029 07da 094d  .Z.g.Z.d.S.)...M
+000000c0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
+000000d0: 6563 7477 6973 65da 1730 3032 375f 6175  ectwise..0027_au
+000000e0: 746f 5f32 3031 3730 3630 355f 3135 3334  to_20170605_1534
+000000f0: da0a 3030 3231 5f6d 6572 6765 4e29 0272  ..0021_mergeN).r
+00000100: 0600 0000 7207 0000 0029 0272 0600 0000  ....r....).r....
+00000110: 7208 0000 0029 05da 085f 5f6e 616d 655f  r....)...__name_
+00000120: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000130: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
+00000140: 656e 6465 6e63 6965 73da 0a6f 7065 7261  endencies..opera
+00000150: 7469 6f6e 73a9 0072 0e00 0000 720e 0000  tions..r....r...
+00000160: 00fa 562f 686f 6d65 2f63 616d 6572 6f6e  ..V/home/cameron
+00000170: 2f44 6576 2f6b 616e 6261 6e2d 6465 762f  /Dev/kanban-dev/
+00000180: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
+00000190: 7365 2f64 6a63 6f6e 6e65 6374 7769 7365  se/djconnectwise
+000001a0: 2f6d 6967 7261 7469 6f6e 732f 3030 3238  /migrations/0028
+000001b0: 5f6d 6572 6765 2e70 7972 0500 0000 0700  _merge.pyr......
+000001c0: 0000 7306 0000 0008 0302 0106 0372 0500  ..s..........r..
+000001d0: 0000 4e29 06da 0a5f 5f66 7574 7572 655f  ..N)...__future_
+000001e0: 5f72 0200 0000 da09 646a 616e 676f 2e64  _r......django.d
+000001f0: 6272 0300 0000 7204 0000 0072 0500 0000  br....r....r....
+00000200: 720e 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000210: 0f00 0000 da08 3c6d 6f64 756c 653e 0200  ......<module>..
+00000220: 0000 7304 0000 000c 0210 03              ..s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/__pycache__/0116_auto_20200522_1107.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/migrations/__pycache__/0102_auto_20190719_1058.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,44 @@
-00000000: 160d 0d0a c065 d15e 1c02 0000 e300 0000  .....e.^........
+00000000: 330d 0d0a 2a3e 545d 3e02 0000 e300 0000  3...*>T]>.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3300 0000 6400 0064 0100 6c00 006d  .s3...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 4764 0200  ..Z..m..Z...Gd..
-00000040: 6403 0084 0000 6403 0065 0100 6a03 0083  d.....d..e..j...
-00000050: 0300 5a03 0064 0400 5329 05e9 0000 0000  ..Z..d..S)......
-00000060: 2902 da0a 6d69 6772 6174 696f 6e73 da06  )...migrations..
-00000070: 6d6f 6465 6c73 6300 0000 0000 0000 0000  modelsc.........
-00000080: 0000 000a 0000 0040 0000 0073 5b00 0000  .......@...s[...
-00000090: 6500 005a 0100 6400 005a 0200 640c 0067  e..Z..d..Z..d..g
-000000a0: 0100 5a03 0065 0400 6a05 0064 0300 6404  ..Z..e..j..d..d.
-000000b0: 0064 0500 6406 0083 0002 6504 006a 0600  .d..d.....e..j..
-000000c0: 6403 0064 0400 6405 0064 0700 6408 0065  d..d..d..d..d..e
-000000d0: 0700 6a08 0064 0900 640a 0083 0001 8300  ..j..d..d.......
-000000e0: 0367 0200 5a09 0064 0b00 5329 0dda 094d  .g..Z..d..S)...M
-000000f0: 6967 7261 7469 6f6e da0d 646a 636f 6e6e  igration..djconn
-00000100: 6563 7477 6973 65da 1f30 3131 355f 6167  ectwise..0115_ag
-00000110: 7265 656d 656e 745f 6167 7265 656d 656e  reement_agreemen
-00000120: 745f 7374 6174 7573 da0a 6d6f 6465 6c5f  t_status..model_
-00000130: 6e61 6d65 da07 636f 6d70 616e 79da 046e  name..company..n
-00000140: 616d 65da 0c63 6f6d 7061 6e79 5f74 7970  ame..company_typ
-00000150: 65da 0d63 6f6d 7061 6e79 5f74 7970 6573  e..company_types
-00000160: da05 6669 656c 64da 0274 6f7a 1964 6a63  ..field..toz.djc
-00000170: 6f6e 6e65 6374 7769 7365 2e43 6f6d 7061  onnectwise.Compa
-00000180: 6e79 5479 7065 4e29 027a 0d64 6a63 6f6e  nyTypeN).z.djcon
-00000190: 6e65 6374 7769 7365 7206 0000 0029 0ada  nectwiser....)..
-000001a0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000001b0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000001c0: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
-000001d0: 7372 0200 0000 da0b 5265 6d6f 7665 4669  sr......RemoveFi
-000001e0: 656c 64da 0841 6464 4669 656c 6472 0300  eld..AddFieldr..
-000001f0: 0000 da0f 4d61 6e79 546f 4d61 6e79 4669  ....ManyToManyFi
-00000200: 656c 64da 0a6f 7065 7261 7469 6f6e 73a9  eld..operations.
-00000210: 0072 1600 0000 7216 0000 00fa 6e2f 686f  .r....r.....n/ho
-00000220: 6d65 2f73 616d 2f67 6974 2f4b 616e 6261  me/sam/git/Kanba
-00000230: 6e2f 646a 616e 676f 2d63 6f6e 6e65 6374  n/django-connect
-00000240: 7769 7365 2f64 6a61 6e67 6f2d 636f 6e6e  wise/django-conn
-00000250: 6563 7477 6973 652f 646a 636f 6e6e 6563  ectwise/djconnec
-00000260: 7477 6973 652f 6d69 6772 6174 696f 6e73  twise/migrations
-00000270: 2f30 3131 365f 6175 746f 5f32 3032 3030  /0116_auto_20200
-00000280: 3532 325f 3131 3037 2e70 7972 0400 0000  522_1107.pyr....
-00000290: 0600 0000 7310 0000 000c 0309 0409 0106  ....s...........
-000002a0: 0106 0209 0106 0106 0172 0400 0000 4e29  .........r....N)
-000002b0: 04da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
-000002c0: 0072 0300 0000 7204 0000 0072 1600 0000  .r....r....r....
-000002d0: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-000002e0: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
-000002f0: 0000 1603                                ....
+00000020: 0073 2600 0000 6400 6401 6c00 6d01 5a01  .s&...d.d.l.m.Z.
+00000030: 6d02 5a02 0100 4700 6402 6403 8400 6403  m.Z...G.d.d...d.
+00000040: 6501 6a03 8303 5a03 6404 5300 2905 e900  e.j...Z.d.S.)...
+00000050: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
+00000060: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
+00000070: 0000 0000 0000 0700 0000 4000 0000 7344  ..........@...sD
+00000080: 0000 0065 005a 0164 005a 0264 0d67 015a  ...e.Z.d.Z.d.g.Z
+00000090: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
+000000a0: 0664 078d 0264 088d 0365 046a 0564 0364  .d...d...e.j.d.d
+000000b0: 0965 066a 0864 0a64 0b8d 0164 088d 0367  .e.j.d.d...d...g
+000000c0: 025a 0964 0c53 0029 0eda 094d 6967 7261  .Z.d.S.)...Migra
+000000d0: 7469 6f6e da0d 646a 636f 6e6e 6563 7477  tion..djconnectw
+000000e0: 6973 65da 1630 3130 315f 6167 7265 656d  ise..0101_agreem
+000000f0: 656e 745f 636f 6d70 616e 79da 0961 6772  ent_company..agr
+00000100: 6565 6d65 6e74 da0e 6167 7265 656d 656e  eement..agreemen
+00000110: 745f 7479 7065 e932 0000 0054 2902 da0a  t_type.2...T)...
+00000120: 6d61 785f 6c65 6e67 7468 da04 6e75 6c6c  max_length..null
+00000130: 2903 da0a 6d6f 6465 6c5f 6e61 6d65 da04  )...model_name..
+00000140: 6e61 6d65 da05 6669 656c 64da 0e63 616e  name..field..can
+00000150: 6365 6c6c 6564 5f66 6c61 6746 2901 da07  celled_flagF)...
+00000160: 6465 6661 756c 744e 2902 7205 0000 0072  defaultN).r....r
+00000170: 0600 0000 290a da08 5f5f 6e61 6d65 5f5f  ....)...__name__
+00000180: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000190: 7175 616c 6e61 6d65 5f5f da0c 6465 7065  qualname__..depe
+000001a0: 6e64 656e 6369 6573 7202 0000 00da 0841  ndenciesr......A
+000001b0: 6464 4669 656c 6472 0300 0000 da09 4368  ddFieldr......Ch
+000001c0: 6172 4669 656c 64da 0c42 6f6f 6c65 616e  arField..Boolean
+000001d0: 4669 656c 64da 0a6f 7065 7261 7469 6f6e  Field..operation
+000001e0: 73a9 0072 1900 0000 7219 0000 00fa 632f  s..r....r.....c/
+000001f0: 686f 6d65 2f63 616d 6572 6f6e 2f44 6576  home/cameron/Dev
+00000200: 2f6b 616e 6261 6e2d 6465 762f 646a 616e  /kanban-dev/djan
+00000210: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
+00000220: 6a63 6f6e 6e65 6374 7769 7365 2f6d 6967  jconnectwise/mig
+00000230: 7261 7469 6f6e 732f 3031 3032 5f61 7574  rations/0102_aut
+00000240: 6f5f 3230 3139 3037 3139 5f31 3035 382e  o_20190719_1058.
+00000250: 7079 7204 0000 0006 0000 0073 1200 0000  pyr........s....
+00000260: 0803 0604 0401 0201 0201 1002 0401 0201  ................
+00000270: 0201 7204 0000 004e 2904 da09 646a 616e  ..r....N)...djan
+00000280: 676f 2e64 6272 0200 0000 7203 0000 0072  go.dbr....r....r
+00000290: 0400 0000 7219 0000 0072 1900 0000 7219  ....r....r....r.
+000002a0: 0000 0072 1a00 0000 da08 3c6d 6f64 756c  ...r......<modul
+000002b0: 653e 0300 0000 7302 0000 0010 03         e>....s......
```

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0071_auto_20180822_1300.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0071_auto_20180822_1300.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0093_auto_20190716_1630.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0093_auto_20190716_1630.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0070_mycompanyother.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0070_mycompanyother.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0043_projectstatus.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0043_projectstatus.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0117_auto_20200609_1514.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0117_auto_20200609_1514.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0105_auto_20190722_1444.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0105_auto_20190722_1444.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0079_auto_20181203_1606.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0079_auto_20181203_1606.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0074_auto_20180827_1241.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0074_auto_20180827_1241.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0022_opportunitystatus.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0022_opportunitystatus.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0050_servicenote.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0050_servicenote.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0120_auto_20200721_1617.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0120_auto_20200721_1617.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0085_auto_20190506_1028.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0085_auto_20190506_1028.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0045_auto_20171222_1725.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0045_auto_20171222_1725.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0106_auto_20190722_1524.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0106_auto_20190722_1524.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0119_auto_20200624_1028.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0119_auto_20200624_1028.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0044_auto_20171222_1700.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0044_auto_20171222_1700.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0095_connectwiseboard_work_type.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0095_connectwiseboard_work_type.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0076_auto_20180925_1618.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0076_auto_20180925_1618.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0114_auto_20200219_1515.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0114_auto_20200219_1515.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0051_opportunitynote.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0051_opportunitynote.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0084_auto_20190404_1532.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0084_auto_20190404_1532.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0069_auto_20180815_1116.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0069_auto_20180815_1116.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0098_auto_20190718_1406.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0098_auto_20190718_1406.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0029_auto_20170607_1147.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0029_auto_20170607_1147.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0023_auto_20170605_0705.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0023_auto_20170605_0705.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0035_activity.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0035_activity.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0102_auto_20190719_1058.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0102_auto_20190719_1058.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0032_auto_20170616_1144.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0032_auto_20170616_1144.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0087_auto_20190705_1015.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0087_auto_20190705_1015.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0036_auto_20170823_1417.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0036_auto_20170823_1417.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0096_agreement.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0096_agreement.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0049_auto_20180205_1122.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0049_auto_20180205_1122.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0073_auto_20180824_1446.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0073_auto_20180824_1446.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0109_ticket_phase.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0109_ticket_phase.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0100_auto_20190718_1417.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0100_auto_20190718_1417.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0082_auto_20190125_1109.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0082_auto_20190125_1109.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0103_activitystatus_activitytype.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0103_activitystatus_activitytype.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0066_auto_20180814_1046.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0066_auto_20180814_1046.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0108_projectphase.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0108_projectphase.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0087_auto_20190709_0836.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0087_auto_20190709_0836.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0085_auto_20190430_1004.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0085_auto_20190430_1004.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0050_auto_20180417_1620.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0050_auto_20180417_1620.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0066_slapriority.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0066_slapriority.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0090_auto_20190711_1114.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0090_auto_20190711_1114.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0037_auto_20170920_0959.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0037_auto_20170920_0959.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0061_auto_20180607_1210.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0061_auto_20180607_1210.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0039_auto_20170925_1418.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0039_auto_20170925_1418.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0005_auto_20170225_0101.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0005_auto_20170225_0101.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0064_auto_20180808_1214.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0064_auto_20180808_1214.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0040_auto_20170926_2145.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0040_auto_20170926_2145.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0058_auto_20180516_1052.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0058_auto_20180516_1052.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/migrations/0099_timeentry_agreement.py` & `django-connectwise-0.3.99/djconnectwise/migrations/0099_timeentry_agreement.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/__pycache__/callbacks.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/__pycache__/callbacks.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,271 +1,249 @@
-00000000: 160d 0d0a 3e9f 0b5e c314 0000 e300 0000  ....>..^........
-00000010: 0000 0000 0000 0000 000f 0000 0040 0000  .............@..
-00000020: 0073 1e01 0000 6400 0064 0100 6c00 005a  .s....d..d..l..Z
-00000030: 0000 6400 0064 0200 6c01 006d 0200 5a02  ..d..d..l..m..Z.
-00000040: 0001 6400 0064 0300 6c03 006d 0400 5a04  ..d..d..l..m..Z.
-00000050: 0001 6500 006a 0500 6506 0083 0100 5a07  ..e..j..e.....Z.
-00000060: 0064 0400 6405 0064 0600 6407 0064 0800  .d..d..d..d..d..
-00000070: 6401 0064 0900 640a 0064 0b00 640c 0069  d..d..d..d..d..i
-00000080: 0500 6404 0064 0d00 6406 0064 0e00 6408  ..d..d..d..d..d.
-00000090: 0064 0100 6409 0064 0a00 640b 0064 0c00  .d..d..d..d..d..
-000000a0: 6905 0064 0400 640f 0064 0600 6410 0064  i..d..d..d..d..d
-000000b0: 0800 6401 0064 0900 640a 0064 0b00 640c  ..d..d..d..d..d.
-000000c0: 0069 0500 6404 0064 1100 6406 0064 1200  .i..d..d..d..d..
-000000d0: 6408 0064 0100 6409 0064 0a00 640b 0064  d..d..d..d..d..d
-000000e0: 0c00 6905 0064 0400 6413 0064 0600 6414  ..i..d..d..d..d.
-000000f0: 0064 0800 6401 0064 0900 640a 0064 0b00  .d..d..d..d..d..
-00000100: 640c 0069 0500 6404 0064 1500 6406 0064  d..i..d..d..d..d
-00000110: 1600 6408 0064 0100 6409 0064 0a00 640b  ..d..d..d..d..d.
-00000120: 0064 0c00 6905 0067 0600 5a08 0047 6417  .d..i..g..Z..Gd.
-00000130: 0064 1800 8400 0064 1800 8302 005a 0900  .d.....d.....Z..
-00000140: 6401 0053 2919 e900 0000 004e 2901 da0f  d..S)......N)...
-00000150: 5379 7374 656d 4150 4943 6c69 656e 7429  SystemAPIClient)
-00000160: 01da 1544 6a63 6f6e 6e65 6374 7769 7365  ...Djconnectwise
-00000170: 5365 7474 696e 6773 da04 7479 7065 da06  Settings..type..
-00000180: 7469 636b 6574 da0b 6465 7363 7269 7074  ticket..descript
-00000190: 696f 6e7a 224b 616e 6261 6e20 6170 706c  ionz"Kanban appl
-000001a0: 6963 6174 696f 6e20 7469 636b 6574 2063  ication ticket c
-000001b0: 616c 6c62 6163 6bda 0375 726c da08 6f62  allback..url..ob
-000001c0: 6a65 6374 4964 e901 0000 00da 056c 6576  jectId.......lev
-000001d0: 656c da05 6f77 6e65 72da 0770 726f 6a65  el..owner..proje
-000001e0: 6374 7a23 4b61 6e62 616e 2061 7070 6c69  ctz#Kanban appli
-000001f0: 6361 7469 6f6e 2070 726f 6a65 6374 2063  cation project c
-00000200: 616c 6c62 6163 6bda 0763 6f6d 7061 6e79  allback..company
-00000210: 7a23 4b61 6e62 616e 2061 7070 6c69 6361  z#Kanban applica
-00000220: 7469 6f6e 2063 6f6d 7061 6e79 2063 616c  tion company cal
-00000230: 6c62 6163 6bda 0b6f 7070 6f72 7475 6e69  lback..opportuni
-00000240: 7479 7a27 4b61 6e62 616e 2061 7070 6c69  tyz'Kanban appli
-00000250: 6361 7469 6f6e 206f 7070 6f72 7475 6e69  cation opportuni
-00000260: 7479 2063 616c 6c62 6163 6bda 0861 6374  ty callback..act
-00000270: 6976 6974 797a 244b 616e 6261 6e20 6170  ivityz$Kanban ap
-00000280: 706c 6963 6174 696f 6e20 6163 7469 7669  plication activi
-00000290: 7479 2063 616c 6c62 6163 6bda 0873 6368  ty callback..sch
-000002a0: 6564 756c 657a 2a4b 616e 6261 6e20 6170  edulez*Kanban ap
-000002b0: 706c 6963 6174 696f 6e20 7363 6865 6475  plication schedu
-000002c0: 6c65 2065 6e74 7279 2063 616c 6c62 6163  le entry callbac
-000002d0: 6b63 0000 0000 0000 0000 0000 0000 0300  kc..............
-000002e0: 0000 0000 0000 7376 0000 0065 0000 5a01  ......sv...e..Z.
-000002f0: 0064 0000 5a02 0087 0000 6601 0064 0100  .d..Z.....f..d..
-00000300: 6402 0086 0000 5a03 0064 0300 6404 0084  d.....Z..d..d...
-00000310: 0000 5a04 0064 0500 6406 0084 0000 5a05  ..Z..d..d.....Z.
-00000320: 0064 0700 6408 0084 0000 5a06 0064 0900  .d..d.....Z..d..
-00000330: 640a 0084 0000 5a07 0064 0b00 640c 0084  d.....Z..d..d...
-00000340: 0000 5a08 0064 0d00 640e 0084 0000 5a09  ..Z..d..d.....Z.
-00000350: 0064 0f00 6410 0084 0000 5a0a 0087 0000  .d..d.....Z.....
-00000360: 5329 11da 1043 616c 6c62 6163 6b73 4861  S)...CallbacksHa
-00000370: 6e64 6c65 7263 0100 0000 0000 0000 0100  ndlerc..........
-00000380: 0000 0200 0000 0300 0000 732f 0000 0074  ..........s/...t
-00000390: 0000 8300 006a 0100 8300 0001 7402 0083  .....j......t...
-000003a0: 0000 7c00 005f 0300 7404 0083 0000 6a05  ..|.._..t.....j.
-000003b0: 0083 0000 7c00 005f 0600 6400 0053 2901  ....|.._..d..S).
-000003c0: 4e29 07da 0573 7570 6572 da08 5f5f 696e  N)...super..__in
-000003d0: 6974 5f5f 7202 0000 00da 0d73 7973 7465  it__r......syste
-000003e0: 6d5f 636c 6965 6e74 7203 0000 00da 0c67  m_clientr......g
-000003f0: 6574 5f73 6574 7469 6e67 73da 0873 6574  et_settings..set
-00000400: 7469 6e67 7329 01da 0473 656c 6629 01da  tings)...self)..
-00000410: 095f 5f63 6c61 7373 5f5f a900 fa55 2f68  .__class__...U/h
-00000420: 6f6d 652f 7361 6d2f 6769 742f 4b61 6e62  ome/sam/git/Kanb
-00000430: 616e 2f64 6a61 6e67 6f2d 636f 6e6e 6563  an/django-connec
-00000440: 7477 6973 652f 646a 616e 676f 2d63 6f6e  twise/django-con
-00000450: 6e65 6374 7769 7365 2f64 6a63 6f6e 6e65  nectwise/djconne
-00000460: 6374 7769 7365 2f63 616c 6c62 6163 6b73  ctwise/callbacks
-00000470: 2e70 7972 1300 0000 3900 0000 7306 0000  .pyr....9...s...
-00000480: 0000 010d 010c 017a 1943 616c 6c62 6163  .......z.Callbac
-00000490: 6b73 4861 6e64 6c65 722e 5f5f 696e 6974  ksHandler.__init
-000004a0: 5f5f 6301 0000 0000 0000 0004 0000 0009  __c.............
-000004b0: 0000 0043 0000 0073 8000 0000 6700 007d  ...C...s....g..}
-000004c0: 0100 6401 007d 0200 786d 007c 0000 6a00  ..d..}..xm.|..j.
-000004d0: 006a 0100 6402 007c 0200 6403 007c 0000  .j..d..|..d..|..
-000004e0: 6a02 0064 0400 1964 0500 6406 006a 0300  j..d...d..d..j..
-000004f0: 7c00 006a 0200 6407 0019 8301 0067 0100  |..j..d......g..
-00000500: 8300 037d 0300 7c01 007c 0300 377d 0100  ...}..|..|..7}..
-00000510: 7c02 0064 0100 377d 0200 7404 007c 0300  |..d..7}..t..|..
-00000520: 8301 007c 0000 6a02 0064 0400 196b 0000  ...|..j..d...k..
-00000530: 720f 0050 710f 0057 7c01 0053 2908 4e72  r..Pq..W|..S).Nr
-00000540: 0900 0000 da04 7061 6765 da09 7061 6765  ......page..page
-00000550: 5f73 697a 65da 0a62 6174 6368 5f73 697a  _size..batch_siz
-00000560: 65da 0a63 6f6e 6469 7469 6f6e 737a 1175  e..conditionsz.u
-00000570: 726c 2063 6f6e 7461 696e 7320 227b 7d22  rl contains "{}"
-00000580: da0d 6361 6c6c 6261 636b 5f68 6f73 7429  ..callback_host)
-00000590: 0572 1400 0000 da0d 6765 745f 6361 6c6c  .r......get_call
-000005a0: 6261 636b 7372 1600 0000 da06 666f 726d  backsr......form
-000005b0: 6174 da03 6c65 6e29 0472 1700 0000 da07  at..len).r......
-000005c0: 7265 7375 6c74 7372 1b00 0000 5a0c 7061  resultsr....Z.pa
-000005d0: 6765 5f72 6563 6f72 6473 7219 0000 0072  ge_recordsr....r
-000005e0: 1900 0000 721a 0000 0072 2000 0000 3e00  ....r....r ...>.
-000005f0: 0000 7318 0000 0000 0106 0106 0103 010c  ..s.............
-00000600: 0106 010d 021c 030a 010a 0119 0305 017a  ...............z
-00000610: 1e43 616c 6c62 6163 6b73 4861 6e64 6c65  .CallbacksHandle
-00000620: 722e 6765 745f 6361 6c6c 6261 636b 7363  r.get_callbacksc
-00000630: 0100 0000 0000 0000 0300 0000 0500 0000  ................
-00000640: 4300 0000 7345 0000 0074 0000 6a01 0083  C...sE...t..j...
-00000650: 0000 7d01 0078 3200 7c01 0044 5d2a 007d  ..}..x2.|..D]*.}
-00000660: 0200 6401 006a 0200 7c00 006a 0300 6402  ..d..j..|..j..d.
-00000670: 0019 7c00 006a 0300 6403 0019 8302 007c  ..|..j..d......|
-00000680: 0200 6404 003c 7113 0057 7c01 0053 2905  ..d..<q..W|..S).
-00000690: 7a2c 0a20 2020 2020 2020 2052 6574 7572  z,.        Retur
-000006a0: 6e20 6120 6c69 7374 206f 6620 6361 6c6c  n a list of call
-000006b0: 6261 636b 730a 2020 2020 2020 2020 7a04  backs.        z.
-000006c0: 7b7d 7b7d 721f 0000 00da 0c63 616c 6c62  {}{}r......callb
-000006d0: 6163 6b5f 7572 6c72 0700 0000 2904 da10  ack_urlr....)...
-000006e0: 4e45 4544 4544 5f43 414c 4c42 4143 4b53  NEEDED_CALLBACKS
-000006f0: da04 636f 7079 7221 0000 0072 1600 0000  ..copyr!...r....
-00000700: 2903 7217 0000 00da 0672 6573 756c 74da  ).r......result.
-00000710: 0263 6272 1900 0000 7219 0000 0072 1a00  .cbr....r....r..
-00000720: 0000 da14 6765 745f 6e65 6564 6564 5f63  ....get_needed_c
-00000730: 616c 6c62 6163 6b73 5100 0000 730c 0000  allbacksQ...s...
-00000740: 0000 040c 010d 0106 010a 0118 027a 2543  .............z%C
-00000750: 616c 6c62 6163 6b73 4861 6e64 6c65 722e  allbacksHandler.
-00000760: 6765 745f 6e65 6564 6564 5f63 616c 6c62  get_needed_callb
-00000770: 6163 6b73 6303 0000 0000 0000 000c 0000  acksc...........
-00000780: 0006 0000 0043 0000 0073 1001 0000 7400  .....C...s....t.
-00000790: 0083 0000 7d03 0074 0000 8300 007d 0400  ....}..t.....}..
-000007a0: 6401 0064 0200 6403 0064 0400 6405 0067  d..d..d..d..d..g
-000007b0: 0500 7d05 0078 8800 7401 007c 0200 8301  ..}..x..t..|....
-000007c0: 0044 5d7a 005c 0200 7d06 007d 0700 786b  .D]z.\..}..}..xk
-000007d0: 0074 0100 7c01 0083 0100 445d 5d00 5c02  .t..|.....D]].\.
-000007e0: 007d 0800 7d09 0064 0600 7d0a 0078 2800  .}..}..d..}..x(.
-000007f0: 7c05 0044 5d20 007d 0b00 7c07 007c 0b00  |..D] .}..|..|..
-00000800: 197c 0900 7c0b 0019 6b03 0072 6600 6407  .|..|...k..rf.d.
-00000810: 007d 0a00 7166 0057 7c0a 0072 4d00 7c03  .}..qf.W|..rM.|.
-00000820: 006a 0200 7c06 0083 0100 017c 0400 6a02  .j..|......|..j.
-00000830: 007c 0800 8301 0001 714d 0057 7134 0057  .|......qM.Wq4.W
-00000840: 7827 0074 0300 7404 007c 0300 8301 0083  x'.t..t..|......
-00000850: 0100 445d 1300 7d06 007c 0200 6a05 007c  ..D]..}..|..j..|
-00000860: 0600 8301 0001 71c5 0057 7827 0074 0300  ......q..Wx'.t..
-00000870: 7404 007c 0400 8301 0083 0100 445d 1300  t..|........D]..
-00000880: 7d08 007c 0100 6a05 007c 0800 8301 0001  }..|..j..|......
-00000890: 71ef 0057 7c01 007c 0200 6602 0053 2908  q..W|..|..f..S).
-000008a0: 7af4 0a20 2020 2020 2020 2047 6976 656e  z..        Given
-000008b0: 2074 6865 206c 6973 7420 6f66 206e 6565   the list of nee
-000008c0: 6465 6420 6361 6c6c 6261 636b 7320 616e  ded callbacks an
-000008d0: 6420 6375 7272 656e 7420 6361 6c6c 6261  d current callba
-000008e0: 636b 732c 2066 6967 7572 6520 6f75 740a  cks, figure out.
-000008f0: 2020 2020 2020 2020 7768 6963 6820 6361          which ca
-00000900: 6c6c 6261 636b 7320 6e65 6564 2074 6f20  llbacks need to 
-00000910: 6265 2072 6567 6973 7465 7265 6420 616e  be registered an
-00000920: 6420 7768 6963 6820 6f6e 6573 206e 6565  d which ones nee
-00000930: 6420 746f 2062 650a 2020 2020 2020 2020  d to be.        
-00000940: 7265 6d6f 7665 642e 0a0a 2020 2020 2020  removed...      
-00000950: 2020 5265 7475 726e 7320 6120 7475 706c    Returns a tupl
-00000960: 6520 6f66 2028 6e65 6564 2d74 6f2d 6164  e of (need-to-ad
-00000970: 642c 206e 6565 642d 746f 2d72 656d 6f76  d, need-to-remov
-00000980: 6529 2063 616c 6c62 6163 6b73 2e0a 2020  e) callbacks..  
-00000990: 2020 2020 2020 7204 0000 0072 0600 0000        r....r....
-000009a0: 7207 0000 0072 0800 0000 720a 0000 0054  r....r....r....T
-000009b0: 4629 06da 0373 6574 da09 656e 756d 6572  F)...set..enumer
-000009c0: 6174 65da 0361 6464 da08 7265 7665 7273  ate..add..revers
-000009d0: 6564 da06 736f 7274 6564 da03 706f 7029  ed..sorted..pop)
-000009e0: 0c72 1700 0000 da10 6e65 6564 6564 5f63  .r......needed_c
-000009f0: 616c 6c62 6163 6b73 da11 6375 7272 656e  allbacks..curren
-00000a00: 745f 6361 6c6c 6261 636b 735a 1663 7572  t_callbacksZ.cur
-00000a10: 7265 6e74 5f69 6e64 6578 6573 5f64 656c  rent_indexes_del
-00000a20: 6574 655a 156e 6565 6465 645f 696e 6465  eteZ.needed_inde
-00000a30: 7865 735f 6465 6c65 7465 da0b 6669 656c  xes_delete..fiel
-00000a40: 645f 6e61 6d65 735a 0569 5f63 7572 da07  d_namesZ.i_cur..
-00000a50: 6375 7272 656e 745a 0669 5f6e 6565 64da  currentZ.i_need.
-00000a60: 066e 6565 6465 645a 0b61 6c6c 5f6d 6174  .neededZ.all_mat
-00000a70: 6368 6564 da05 6669 656c 6472 1900 0000  ched..fieldr....
-00000a80: 7219 0000 0072 1a00 0000 da25 5f63 616c  r....r.....%_cal
-00000a90: 6375 6c61 7465 5f6d 6973 7369 6e67 5f75  culate_missing_u
-00000aa0: 6e6e 6565 6465 645f 6361 6c6c 6261 636b  nneeded_callback
-00000ab0: 735d 0000 0073 2200 0000 000c 0901 0901  s]...s".........
-00000ac0: 1503 1901 1901 0601 0d01 1402 0a01 0601  ................
-00000ad0: 0d01 1501 1902 1101 1902 1102 7a36 4361  ............z6Ca
-00000ae0: 6c6c 6261 636b 7348 616e 646c 6572 2e5f  llbacksHandler._
-00000af0: 6361 6c63 756c 6174 655f 6d69 7373 696e  calculate_missin
-00000b00: 675f 756e 6e65 6564 6564 5f63 616c 6c62  g_unneeded_callb
-00000b10: 6163 6b73 6301 0000 0000 0000 0006 0000  acksc...........
-00000b20: 0003 0000 0043 0000 0073 7000 0000 7c00  .....C...sp...|.
-00000b30: 006a 0000 8300 007d 0100 7c00 006a 0100  .j.....}..|..j..
-00000b40: 8300 007d 0200 7c00 006a 0200 7c01 007c  ...}..|..j..|..|
-00000b50: 0200 8302 005c 0200 7d03 007d 0400 781b  .....\..}..}..x.
-00000b60: 007c 0300 445d 1300 7d05 007c 0000 6a03  .|..D]..}..|..j.
-00000b70: 007c 0500 8301 0001 7137 0057 781b 007c  .|......q7.Wx..|
-00000b80: 0400 445d 1300 7d05 007c 0000 6a04 007c  ..D]..}..|..j..|
-00000b90: 0500 8301 0001 7155 0057 6401 0053 2902  ......qU.Wd..S).
-00000ba0: 7a65 0a20 2020 2020 2020 2044 6f20 7468  ze.        Do th
-00000bb0: 6520 6d69 6e69 6d75 6d20 6368 616e 6765  e minimum change
-00000bc0: 7320 746f 2065 6e73 7572 6520 6f75 7220  s to ensure our 
-00000bd0: 6361 6c6c 6261 636b 7320 6172 6520 7265  callbacks are re
-00000be0: 6769 7374 6572 6564 0a20 2020 2020 2020  gistered.       
-00000bf0: 2065 7861 6374 6c79 206f 6e63 652e 0a20   exactly once.. 
-00000c00: 2020 2020 2020 204e 2905 7229 0000 0072         N).r)...r
-00000c10: 2000 0000 7236 0000 00da 125f 7265 6769   ...r6....._regi
-00000c20: 7374 6572 5f63 616c 6c62 6163 6bda 105f  ster_callback.._
-00000c30: 6465 6c65 7465 5f63 616c 6c62 6163 6b29  delete_callback)
-00000c40: 0672 1700 0000 7230 0000 0072 3100 0000  .r....r0...r1...
-00000c50: 5a10 6361 6c6c 6261 636b 735f 746f 5f61  Z.callbacks_to_a
-00000c60: 6464 5a13 6361 6c6c 6261 636b 735f 746f  ddZ.callbacks_to
-00000c70: 5f72 656d 6f76 65da 0863 616c 6c62 6163  _remove..callbac
-00000c80: 6b72 1900 0000 7219 0000 0072 1a00 0000  kr....r....r....
-00000c90: da11 656e 7375 7265 5f72 6567 6973 7465  ..ensure_registe
-00000ca0: 7265 6481 0000 0073 1000 0000 0005 0c01  red....s........
-00000cb0: 0c02 0601 1203 0d01 1101 0d01 7a22 4361  ............z"Ca
-00000cc0: 6c6c 6261 636b 7348 616e 646c 6572 2e65  llbacksHandler.e
-00000cd0: 6e73 7572 655f 7265 6769 7374 6572 6564  nsure_registered
-00000ce0: 6301 0000 0000 0000 0003 0000 0003 0000  c...............
-00000cf0: 0043 0000 0073 2e00 0000 7c00 006a 0000  .C...s....|..j..
-00000d00: 8300 007d 0100 781b 007c 0100 445d 1300  ...}..x..|..D]..
-00000d10: 7d02 007c 0000 6a01 007c 0200 8301 0001  }..|..j..|......
-00000d20: 7113 0057 6401 0053 2902 7a30 446f 2074  q..Wd..S).z0Do t
-00000d30: 6865 206e 6565 6466 756c 2074 6f20 656e  he needful to en
-00000d40: 7375 7265 206f 7572 2063 616c 6c62 6163  sure our callbac
-00000d50: 6b73 2061 7265 2067 6f6e 652e 4e29 0272  ks are gone.N).r
-00000d60: 2000 0000 7238 0000 0029 0372 1700 0000   ...r8...).r....
-00000d70: da09 6361 6c6c 6261 636b 7372 3900 0000  ..callbacksr9...
-00000d80: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00000d90: 0e65 6e73 7572 655f 6465 6c65 7465 6492  .ensure_deleted.
-00000da0: 0000 0073 0600 0000 0002 0c01 0d01 7a1f  ...s..........z.
-00000db0: 4361 6c6c 6261 636b 7348 616e 646c 6572  CallbacksHandler
-00000dc0: 2e65 6e73 7572 655f 6465 6c65 7465 6463  .ensure_deletedc
-00000dd0: 0200 0000 0000 0000 0200 0000 0400 0000  ................
-00000de0: 4300 0000 732e 0000 0074 0000 6a01 0064  C...s....t..j..d
-00000df0: 0100 6a02 007c 0100 6402 0019 8301 0083  ..j..|..d.......
-00000e00: 0100 017c 0000 6a03 006a 0400 7c01 0083  ...|..j..j..|...
-00000e10: 0100 0164 0000 5329 034e 7a17 5265 6769  ...d..S).Nz.Regi
-00000e20: 7374 6572 696e 6720 7b7d 2063 616c 6c62  stering {} callb
-00000e30: 6163 6b72 0400 0000 2905 da06 6c6f 6767  ackr....)...logg
-00000e40: 6572 da04 696e 666f 7221 0000 0072 1400  er..infor!...r..
-00000e50: 0000 da0f 6372 6561 7465 5f63 616c 6c62  ....create_callb
-00000e60: 6163 6b29 0272 1700 0000 7239 0000 0072  ack).r....r9...r
-00000e70: 1900 0000 7219 0000 0072 1a00 0000 7237  ....r....r....r7
-00000e80: 0000 0098 0000 0073 0400 0000 0001 1a01  .......s........
-00000e90: 7a23 4361 6c6c 6261 636b 7348 616e 646c  z#CallbacksHandl
-00000ea0: 6572 2e5f 7265 6769 7374 6572 5f63 616c  er._register_cal
-00000eb0: 6c62 6163 6b63 0200 0000 0000 0000 0200  lbackc..........
-00000ec0: 0000 0400 0000 4300 0000 7332 0000 0074  ......C...s2...t
-00000ed0: 0000 6a01 0064 0100 6a02 007c 0100 6402  ..j..d..j..|..d.
-00000ee0: 0019 8301 0083 0100 017c 0000 6a03 006a  .........|..j..j
-00000ef0: 0400 7c01 0064 0200 1983 0100 0164 0000  ..|..d.......d..
-00000f00: 5329 034e 7a14 4465 6c65 7469 6e67 2063  S).Nz.Deleting c
-00000f10: 616c 6c62 6163 6b20 7b7d da02 6964 2905  allback {}..id).
-00000f20: 723d 0000 0072 3e00 0000 7221 0000 0072  r=...r>...r!...r
-00000f30: 1400 0000 da0f 6465 6c65 7465 5f63 616c  ......delete_cal
-00000f40: 6c62 6163 6b29 0272 1700 0000 7239 0000  lback).r....r9..
-00000f50: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00000f60: 7238 0000 009c 0000 0073 0400 0000 0001  r8.......s......
-00000f70: 1a01 7a21 4361 6c6c 6261 636b 7348 616e  ..z!CallbacksHan
-00000f80: 646c 6572 2e5f 6465 6c65 7465 5f63 616c  dler._delete_cal
-00000f90: 6c62 6163 6b29 0bda 085f 5f6e 616d 655f  lback)...__name_
-00000fa0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000fb0: 5f71 7561 6c6e 616d 655f 5f72 1300 0000  _qualname__r....
-00000fc0: 7220 0000 0072 2900 0000 7236 0000 0072  r ...r)...r6...r
-00000fd0: 3a00 0000 723c 0000 0072 3700 0000 7238  :...r<...r7...r8
-00000fe0: 0000 0072 1900 0000 7219 0000 0029 0172  ...r....r....).r
-00000ff0: 1800 0000 721a 0000 0072 1100 0000 3800  ....r....r....8.
-00001000: 0000 7310 0000 000c 0112 050c 130c 0c0c  ..s.............
-00001010: 240c 110c 060c 0472 1100 0000 290a da07  $......r....)...
-00001020: 6c6f 6767 696e 675a 1164 6a63 6f6e 6e65  loggingZ.djconne
-00001030: 6374 7769 7365 2e61 7069 7202 0000 00da  ctwise.apir.....
-00001040: 1364 6a63 6f6e 6e65 6374 7769 7365 2e75  .djconnectwise.u
-00001050: 7469 6c73 7203 0000 00da 0967 6574 4c6f  tilsr......getLo
-00001060: 6767 6572 7242 0000 0072 3d00 0000 7225  ggerrB...r=...r%
-00001070: 0000 0072 1100 0000 7219 0000 0072 1900  ...r....r....r..
-00001080: 0000 7219 0000 0072 1a00 0000 da08 3c6d  ..r....r......<m
-00001090: 6f64 756c 653e 0100 0000 7344 0000 000c  odule>....sD....
-000010a0: 0110 0110 030f 0606 0106 0106 0106 0109  ................
-000010b0: 0306 0106 0106 0106 0109 0306 0106 0106  ................
-000010c0: 0106 0109 0306 0106 0106 0106 0109 0306  ................
-000010d0: 0106 0106 0106 0109 0306 0106 0106 0106  ................
-000010e0: 010f 05                                  ...
+00000000: 330d 0d0a 0216 fd5d c314 0000 e300 0000  3......]........
+00000010: 0000 0000 0000 0000 000b 0000 0040 0000  .............@..
+00000020: 0073 9400 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
+00000030: 6402 6c01 6d02 5a02 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
+00000040: 6d04 5a04 0100 6500 6a05 6506 8301 5a07  m.Z...e.j.e...Z.
+00000050: 6404 6405 6401 6406 6407 6408 9c05 6409  d.d.d.d.d.d...d.
+00000060: 640a 6401 6406 6407 6408 9c05 640b 640c  d.d.d.d.d...d.d.
+00000070: 6401 6406 6407 6408 9c05 640d 640e 6401  d.d.d.d...d.d.d.
+00000080: 6406 6407 6408 9c05 640f 6410 6401 6406  d.d.d...d.d.d.d.
+00000090: 6407 6408 9c05 6411 6412 6401 6406 6407  d.d...d.d.d.d.d.
+000000a0: 6408 9c05 6706 5a08 4700 6413 6414 8400  d...g.Z.G.d.d...
+000000b0: 6414 8302 5a09 6401 5300 2915 e900 0000  d...Z.d.S.).....
+000000c0: 004e 2901 da0f 5379 7374 656d 4150 4943  .N)...SystemAPIC
+000000d0: 6c69 656e 7429 01da 1544 6a63 6f6e 6e65  lient)...Djconne
+000000e0: 6374 7769 7365 5365 7474 696e 6773 da06  ctwiseSettings..
+000000f0: 7469 636b 6574 7a22 4b61 6e62 616e 2061  ticketz"Kanban a
+00000100: 7070 6c69 6361 7469 6f6e 2074 6963 6b65  pplication ticke
+00000110: 7420 6361 6c6c 6261 636b e901 0000 00da  t callback......
+00000120: 056f 776e 6572 2905 da04 7479 7065 da0b  .owner)...type..
+00000130: 6465 7363 7269 7074 696f 6eda 0375 726c  description..url
+00000140: da08 6f62 6a65 6374 4964 da05 6c65 7665  ..objectId..leve
+00000150: 6cda 0770 726f 6a65 6374 7a23 4b61 6e62  l..projectz#Kanb
+00000160: 616e 2061 7070 6c69 6361 7469 6f6e 2070  an application p
+00000170: 726f 6a65 6374 2063 616c 6c62 6163 6bda  roject callback.
+00000180: 0763 6f6d 7061 6e79 7a23 4b61 6e62 616e  .companyz#Kanban
+00000190: 2061 7070 6c69 6361 7469 6f6e 2063 6f6d   application com
+000001a0: 7061 6e79 2063 616c 6c62 6163 6bda 0b6f  pany callback..o
+000001b0: 7070 6f72 7475 6e69 7479 7a27 4b61 6e62  pportunityz'Kanb
+000001c0: 616e 2061 7070 6c69 6361 7469 6f6e 206f  an application o
+000001d0: 7070 6f72 7475 6e69 7479 2063 616c 6c62  pportunity callb
+000001e0: 6163 6bda 0861 6374 6976 6974 797a 244b  ack..activityz$K
+000001f0: 616e 6261 6e20 6170 706c 6963 6174 696f  anban applicatio
+00000200: 6e20 6163 7469 7669 7479 2063 616c 6c62  n activity callb
+00000210: 6163 6bda 0873 6368 6564 756c 657a 2a4b  ack..schedulez*K
+00000220: 616e 6261 6e20 6170 706c 6963 6174 696f  anban applicatio
+00000230: 6e20 7363 6865 6475 6c65 2065 6e74 7279  n schedule entry
+00000240: 2063 616c 6c62 6163 6b63 0000 0000 0000   callbackc......
+00000250: 0000 0000 0000 0300 0000 0000 0000 7354  ..............sT
+00000260: 0000 0065 005a 0164 005a 0287 0066 0164  ...e.Z.d.Z...f.d
+00000270: 0164 0284 085a 0364 0364 0484 005a 0464  .d...Z.d.d...Z.d
+00000280: 0564 0684 005a 0564 0764 0884 005a 0664  .d...Z.d.d...Z.d
+00000290: 0964 0a84 005a 0764 0b64 0c84 005a 0864  .d...Z.d.d...Z.d
+000002a0: 0d64 0e84 005a 0964 0f64 1084 005a 0a87  .d...Z.d.d...Z..
+000002b0: 0004 005a 0b53 0029 11da 1043 616c 6c62  ...Z.S.)...Callb
+000002c0: 6163 6b73 4861 6e64 6c65 7263 0100 0000  acksHandlerc....
+000002d0: 0000 0000 0100 0000 0200 0000 0300 0000  ................
+000002e0: 7322 0000 0074 0083 006a 0183 0001 0074  s"...t...j.....t
+000002f0: 0283 007c 005f 0374 0483 006a 0583 007c  ...|._.t...j...|
+00000300: 005f 0664 0053 0029 014e 2907 da05 7375  ._.d.S.).N)...su
+00000310: 7065 72da 085f 5f69 6e69 745f 5f72 0200  per..__init__r..
+00000320: 0000 da0d 7379 7374 656d 5f63 6c69 656e  ....system_clien
+00000330: 7472 0300 0000 da0c 6765 745f 7365 7474  tr......get_sett
+00000340: 696e 6773 da08 7365 7474 696e 6773 2901  ings..settings).
+00000350: da04 7365 6c66 2901 da09 5f5f 636c 6173  ..self)...__clas
+00000360: 735f 5fa9 00fa 4a2f 686f 6d65 2f63 616d  s__...J/home/cam
+00000370: 6572 6f6e 2f44 6576 2f6b 616e 6261 6e2d  eron/Dev/kanban-
+00000380: 6465 762f 646a 616e 676f 2d63 6f6e 6e65  dev/django-conne
+00000390: 6374 7769 7365 2f64 6a63 6f6e 6e65 6374  ctwise/djconnect
+000003a0: 7769 7365 2f63 616c 6c62 6163 6b73 2e70  wise/callbacks.p
+000003b0: 7972 1300 0000 3900 0000 7306 0000 0000  yr....9...s.....
+000003c0: 010a 0108 017a 1943 616c 6c62 6163 6b73  .....z.Callbacks
+000003d0: 4861 6e64 6c65 722e 5f5f 696e 6974 5f5f  Handler.__init__
+000003e0: 6301 0000 0000 0000 0004 0000 0006 0000  c...............
+000003f0: 0043 0000 0073 5c00 0000 6700 7d01 6401  .C...s\...g.}.d.
+00000400: 7d02 784e 7c00 6a00 6a01 7c02 7c00 6a02  }.xN|.j.j.|.|.j.
+00000410: 6402 1900 6403 6a03 7c00 6a02 6404 1900  d...d.j.|.j.d...
+00000420: 8301 6701 6405 8d03 7d03 7c01 7c03 3700  ..g.d...}.|.|.7.
+00000430: 7d01 7c02 6401 3700 7d02 7404 7c03 8301  }.|.d.7.}.t.|...
+00000440: 7c00 6a02 6402 1900 6b00 720a 5000 710a  |.j.d...k.r.P.q.
+00000450: 5700 7c01 5300 2906 4e72 0500 0000 da0a  W.|.S.).Nr......
+00000460: 6261 7463 685f 7369 7a65 7a11 7572 6c20  batch_sizez.url 
+00000470: 636f 6e74 6169 6e73 2022 7b7d 22da 0d63  contains "{}"..c
+00000480: 616c 6c62 6163 6b5f 686f 7374 2903 da04  allback_host)...
+00000490: 7061 6765 da09 7061 6765 5f73 697a 65da  page..page_size.
+000004a0: 0a63 6f6e 6469 7469 6f6e 7329 0572 1400  .conditions).r..
+000004b0: 0000 da0d 6765 745f 6361 6c6c 6261 636b  ....get_callback
+000004c0: 7372 1600 0000 da06 666f 726d 6174 da03  sr......format..
+000004d0: 6c65 6e29 0472 1700 0000 da07 7265 7375  len).r......resu
+000004e0: 6c74 7372 1d00 0000 5a0c 7061 6765 5f72  ltsr....Z.page_r
+000004f0: 6563 6f72 6473 7219 0000 0072 1900 0000  ecordsr....r....
+00000500: 721a 0000 0072 2000 0000 3e00 0000 7318  r....r ...>...s.
+00000510: 0000 0000 0104 0104 0102 0106 0102 0108  ................
+00000520: 0216 0308 0108 0112 0306 017a 1e43 616c  ...........z.Cal
+00000530: 6c62 6163 6b73 4861 6e64 6c65 722e 6765  lbacksHandler.ge
+00000540: 745f 6361 6c6c 6261 636b 7363 0100 0000  t_callbacksc....
+00000550: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
+00000560: 7336 0000 0074 006a 0183 007d 0178 287c  s6...t.j...}.x(|
+00000570: 0144 005d 207d 0264 016a 027c 006a 0364  .D.] }.d.j.|.j.d
+00000580: 0219 007c 006a 0364 0319 0083 027c 0264  ...|.j.d.....|.d
+00000590: 043c 0071 0e57 007c 0153 0029 057a 2c0a  .<.q.W.|.S.).z,.
+000005a0: 2020 2020 2020 2020 5265 7475 726e 2061          Return a
+000005b0: 206c 6973 7420 6f66 2063 616c 6c62 6163   list of callbac
+000005c0: 6b73 0a20 2020 2020 2020 207a 047b 7d7b  ks.        z.{}{
+000005d0: 7d72 1c00 0000 da0c 6361 6c6c 6261 636b  }r......callback
+000005e0: 5f75 726c 7209 0000 0029 04da 104e 4545  _urlr....)...NEE
+000005f0: 4445 445f 4341 4c4c 4241 434b 53da 0463  DED_CALLBACKS..c
+00000600: 6f70 7972 2100 0000 7216 0000 0029 0372  opyr!...r....).r
+00000610: 1700 0000 da06 7265 7375 6c74 da02 6362  ......result..cb
+00000620: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
+00000630: 1467 6574 5f6e 6565 6465 645f 6361 6c6c  .get_needed_call
+00000640: 6261 636b 7351 0000 0073 0c00 0000 0004  backsQ...s......
+00000650: 0801 0a01 0401 0801 1402 7a25 4361 6c6c  ..........z%Call
+00000660: 6261 636b 7348 616e 646c 6572 2e67 6574  backsHandler.get
+00000670: 5f6e 6565 6465 645f 6361 6c6c 6261 636b  _needed_callback
+00000680: 7363 0300 0000 0000 0000 0c00 0000 0600  sc..............
+00000690: 0000 4300 0000 73cc 0000 0074 0083 007d  ..C...s....t...}
+000006a0: 0374 0083 007d 0464 0164 0264 0364 0464  .t...}.d.d.d.d.d
+000006b0: 0567 057d 0578 6874 017c 0283 0144 005d  .g.}.xht.|...D.]
+000006c0: 5c5c 027d 067d 0778 5274 017c 0183 0144  \\.}.}.xRt.|...D
+000006d0: 005d 465c 027d 087d 0964 067d 0a78 207c  .]F\.}.}.d.}.x |
+000006e0: 0544 005d 187d 0b7c 077c 0b19 007c 097c  .D.].}.|.|...|.|
+000006f0: 0b19 006b 0372 4864 077d 0a71 4857 007c  ...k.rHd.}.qHW.|
+00000700: 0a72 367c 036a 027c 0683 0101 007c 046a  .r6|.j.|.....|.j
+00000710: 027c 0883 0101 0071 3657 0071 2457 0078  .|.....q6W.q$W.x
+00000720: 1e74 0374 047c 0383 0183 0144 005d 0e7d  .t.t.|.....D.].}
+00000730: 067c 026a 057c 0683 0101 0071 9257 0078  .|.j.|.....q.W.x
+00000740: 1e74 0374 047c 0483 0183 0144 005d 0e7d  .t.t.|.....D.].}
+00000750: 087c 016a 057c 0883 0101 0071 b257 007c  .|.j.|.....q.W.|
+00000760: 017c 0266 0253 0029 087a f40a 2020 2020  .|.f.S.).z..    
+00000770: 2020 2020 4769 7665 6e20 7468 6520 6c69      Given the li
+00000780: 7374 206f 6620 6e65 6564 6564 2063 616c  st of needed cal
+00000790: 6c62 6163 6b73 2061 6e64 2063 7572 7265  lbacks and curre
+000007a0: 6e74 2063 616c 6c62 6163 6b73 2c20 6669  nt callbacks, fi
+000007b0: 6775 7265 206f 7574 0a20 2020 2020 2020  gure out.       
+000007c0: 2077 6869 6368 2063 616c 6c62 6163 6b73   which callbacks
+000007d0: 206e 6565 6420 746f 2062 6520 7265 6769   need to be regi
+000007e0: 7374 6572 6564 2061 6e64 2077 6869 6368  stered and which
+000007f0: 206f 6e65 7320 6e65 6564 2074 6f20 6265   ones need to be
+00000800: 0a20 2020 2020 2020 2072 656d 6f76 6564  .        removed
+00000810: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00000820: 6e73 2061 2074 7570 6c65 206f 6620 286e  ns a tuple of (n
+00000830: 6565 642d 746f 2d61 6464 2c20 6e65 6564  eed-to-add, need
+00000840: 2d74 6f2d 7265 6d6f 7665 2920 6361 6c6c  -to-remove) call
+00000850: 6261 636b 732e 0a20 2020 2020 2020 2072  backs..        r
+00000860: 0700 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
+00000870: 0000 0072 0b00 0000 5446 2906 da03 7365  ...r....TF)...se
+00000880: 74da 0965 6e75 6d65 7261 7465 da03 6164  t..enumerate..ad
+00000890: 64da 0872 6576 6572 7365 64da 0673 6f72  d..reversed..sor
+000008a0: 7465 64da 0370 6f70 290c 7217 0000 00da  ted..pop).r.....
+000008b0: 106e 6565 6465 645f 6361 6c6c 6261 636b  .needed_callback
+000008c0: 73da 1163 7572 7265 6e74 5f63 616c 6c62  s..current_callb
+000008d0: 6163 6b73 5a16 6375 7272 656e 745f 696e  acksZ.current_in
+000008e0: 6465 7865 735f 6465 6c65 7465 5a15 6e65  dexes_deleteZ.ne
+000008f0: 6564 6564 5f69 6e64 6578 6573 5f64 656c  eded_indexes_del
+00000900: 6574 65da 0b66 6965 6c64 5f6e 616d 6573  ete..field_names
+00000910: 5a05 695f 6375 72da 0763 7572 7265 6e74  Z.i_cur..current
+00000920: 5a06 695f 6e65 6564 da06 6e65 6564 6564  Z.i_need..needed
+00000930: 5a0b 616c 6c5f 6d61 7463 6865 64da 0566  Z.all_matched..f
+00000940: 6965 6c64 7219 0000 0072 1900 0000 721a  ieldr....r....r.
+00000950: 0000 00da 255f 6361 6c63 756c 6174 655f  ....%_calculate_
+00000960: 6d69 7373 696e 675f 756e 6e65 6564 6564  missing_unneeded
+00000970: 5f63 616c 6c62 6163 6b73 5d00 0000 7322  _callbacks]...s"
+00000980: 0000 0000 0c06 0106 010e 0312 0112 0104  ................
+00000990: 010a 0110 0208 0104 010a 0112 0112 020e  ................
+000009a0: 0112 020e 027a 3643 616c 6c62 6163 6b73  .....z6Callbacks
+000009b0: 4861 6e64 6c65 722e 5f63 616c 6375 6c61  Handler._calcula
+000009c0: 7465 5f6d 6973 7369 6e67 5f75 6e6e 6565  te_missing_unnee
+000009d0: 6465 645f 6361 6c6c 6261 636b 7363 0100  ded_callbacksc..
+000009e0: 0000 0000 0000 0600 0000 0300 0000 4300  ..............C.
+000009f0: 0000 7354 0000 007c 006a 0083 007d 017c  ..sT...|.j...}.|
+00000a00: 006a 0183 007d 027c 006a 027c 017c 0283  .j...}.|.j.|.|..
+00000a10: 025c 027d 037d 0478 167c 0344 005d 0e7d  .\.}.}.x.|.D.].}
+00000a20: 057c 006a 037c 0583 0101 0071 2657 0078  .|.j.|.....q&W.x
+00000a30: 167c 0444 005d 0e7d 057c 006a 047c 0583  .|.D.].}.|.j.|..
+00000a40: 0101 0071 3e57 0064 0153 0029 027a 650a  ...q>W.d.S.).ze.
+00000a50: 2020 2020 2020 2020 446f 2074 6865 206d          Do the m
+00000a60: 696e 696d 756d 2063 6861 6e67 6573 2074  inimum changes t
+00000a70: 6f20 656e 7375 7265 206f 7572 2063 616c  o ensure our cal
+00000a80: 6c62 6163 6b73 2061 7265 2072 6567 6973  lbacks are regis
+00000a90: 7465 7265 640a 2020 2020 2020 2020 6578  tered.        ex
+00000aa0: 6163 746c 7920 6f6e 6365 2e0a 2020 2020  actly once..    
+00000ab0: 2020 2020 4e29 0572 2900 0000 7220 0000      N).r)...r ..
+00000ac0: 0072 3600 0000 da12 5f72 6567 6973 7465  .r6....._registe
+00000ad0: 725f 6361 6c6c 6261 636b da10 5f64 656c  r_callback.._del
+00000ae0: 6574 655f 6361 6c6c 6261 636b 2906 7217  ete_callback).r.
+00000af0: 0000 0072 3000 0000 7231 0000 005a 1063  ...r0...r1...Z.c
+00000b00: 616c 6c62 6163 6b73 5f74 6f5f 6164 645a  allbacks_to_addZ
+00000b10: 1363 616c 6c62 6163 6b73 5f74 6f5f 7265  .callbacks_to_re
+00000b20: 6d6f 7665 da08 6361 6c6c 6261 636b 7219  move..callbackr.
+00000b30: 0000 0072 1900 0000 721a 0000 00da 1165  ...r....r......e
+00000b40: 6e73 7572 655f 7265 6769 7374 6572 6564  nsure_registered
+00000b50: 8100 0000 7310 0000 0000 0508 0108 0204  ....s...........
+00000b60: 010c 030a 010e 010a 017a 2243 616c 6c62  .........z"Callb
+00000b70: 6163 6b73 4861 6e64 6c65 722e 656e 7375  acksHandler.ensu
+00000b80: 7265 5f72 6567 6973 7465 7265 6463 0100  re_registeredc..
+00000b90: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
+00000ba0: 0000 7324 0000 007c 006a 0083 007d 0178  ..s$...|.j...}.x
+00000bb0: 167c 0144 005d 0e7d 027c 006a 017c 0283  .|.D.].}.|.j.|..
+00000bc0: 0101 0071 0e57 0064 0153 0029 027a 3044  ...q.W.d.S.).z0D
+00000bd0: 6f20 7468 6520 6e65 6564 6675 6c20 746f  o the needful to
+00000be0: 2065 6e73 7572 6520 6f75 7220 6361 6c6c   ensure our call
+00000bf0: 6261 636b 7320 6172 6520 676f 6e65 2e4e  backs are gone.N
+00000c00: 2902 7220 0000 0072 3800 0000 2903 7217  ).r ...r8...).r.
+00000c10: 0000 00da 0963 616c 6c62 6163 6b73 7239  .....callbacksr9
+00000c20: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+00000c30: 0000 da0e 656e 7375 7265 5f64 656c 6574  ....ensure_delet
+00000c40: 6564 9200 0000 7306 0000 0000 0208 010a  ed....s.........
+00000c50: 017a 1f43 616c 6c62 6163 6b73 4861 6e64  .z.CallbacksHand
+00000c60: 6c65 722e 656e 7375 7265 5f64 656c 6574  ler.ensure_delet
+00000c70: 6564 6302 0000 0000 0000 0002 0000 0004  edc.............
+00000c80: 0000 0043 0000 0073 2400 0000 7400 6a01  ...C...s$...t.j.
+00000c90: 6401 6a02 7c01 6402 1900 8301 8301 0100  d.j.|.d.........
+00000ca0: 7c00 6a03 6a04 7c01 8301 0100 6400 5300  |.j.j.|.....d.S.
+00000cb0: 2903 4e7a 1752 6567 6973 7465 7269 6e67  ).Nz.Registering
+00000cc0: 207b 7d20 6361 6c6c 6261 636b 7207 0000   {} callbackr...
+00000cd0: 0029 05da 066c 6f67 6765 72da 0469 6e66  .)...logger..inf
+00000ce0: 6f72 2100 0000 7214 0000 00da 0f63 7265  or!...r......cre
+00000cf0: 6174 655f 6361 6c6c 6261 636b 2902 7217  ate_callback).r.
+00000d00: 0000 0072 3900 0000 7219 0000 0072 1900  ...r9...r....r..
+00000d10: 0000 721a 0000 0072 3700 0000 9800 0000  ..r....r7.......
+00000d20: 7304 0000 0000 0114 017a 2343 616c 6c62  s........z#Callb
+00000d30: 6163 6b73 4861 6e64 6c65 722e 5f72 6567  acksHandler._reg
+00000d40: 6973 7465 725f 6361 6c6c 6261 636b 6302  ister_callbackc.
+00000d50: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00000d60: 0000 0073 2800 0000 7400 6a01 6401 6a02  ...s(...t.j.d.j.
+00000d70: 7c01 6402 1900 8301 8301 0100 7c00 6a03  |.d.........|.j.
+00000d80: 6a04 7c01 6402 1900 8301 0100 6400 5300  j.|.d.......d.S.
+00000d90: 2903 4e7a 1444 656c 6574 696e 6720 6361  ).Nz.Deleting ca
+00000da0: 6c6c 6261 636b 207b 7dda 0269 6429 0572  llback {}..id).r
+00000db0: 3d00 0000 723e 0000 0072 2100 0000 7214  =...r>...r!...r.
+00000dc0: 0000 00da 0f64 656c 6574 655f 6361 6c6c  .....delete_call
+00000dd0: 6261 636b 2902 7217 0000 0072 3900 0000  back).r....r9...
+00000de0: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00000df0: 3800 0000 9c00 0000 7304 0000 0000 0114  8.......s.......
+00000e00: 017a 2143 616c 6c62 6163 6b73 4861 6e64  .z!CallbacksHand
+00000e10: 6c65 722e 5f64 656c 6574 655f 6361 6c6c  ler._delete_call
+00000e20: 6261 636b 290c da08 5f5f 6e61 6d65 5f5f  back)...__name__
+00000e30: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000e40: 7175 616c 6e61 6d65 5f5f 7213 0000 0072  qualname__r....r
+00000e50: 2000 0000 7229 0000 0072 3600 0000 723a   ...r)...r6...r:
+00000e60: 0000 0072 3c00 0000 7237 0000 0072 3800  ...r<...r7...r8.
+00000e70: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
+00000e80: 5f72 1900 0000 7219 0000 0029 0172 1800  _r....r....).r..
+00000e90: 0000 721a 0000 0072 1100 0000 3800 0000  ..r....r....8...
+00000ea0: 7310 0000 0008 010c 0508 1308 0c08 2408  s.............$.
+00000eb0: 1108 0608 0472 1100 0000 290a da07 6c6f  .....r....)...lo
+00000ec0: 6767 696e 675a 1164 6a63 6f6e 6e65 6374  ggingZ.djconnect
+00000ed0: 7769 7365 2e61 7069 7202 0000 00da 1364  wise.apir......d
+00000ee0: 6a63 6f6e 6e65 6374 7769 7365 2e75 7469  jconnectwise.uti
+00000ef0: 6c73 7203 0000 00da 0967 6574 4c6f 6767  lsr......getLogg
+00000f00: 6572 7242 0000 0072 3d00 0000 7225 0000  errB...r=...r%..
+00000f10: 0072 1100 0000 7219 0000 0072 1900 0000  .r....r....r....
+00000f20: 7219 0000 0072 1a00 0000 da08 3c6d 6f64  r....r......<mod
+00000f30: 756c 653e 0100 0000 7344 0000 0008 010c  ule>....sD......
+00000f40: 010c 030a 0602 0102 0102 0102 0106 0302  ................
+00000f50: 0102 0102 0102 0106 0302 0102 0102 0102  ................
+00000f60: 0106 0302 0102 0102 0102 0106 0302 0102  ................
+00000f70: 0102 0102 0106 0302 0102 0102 0102 010a  ................
+00000f80: 05                                       .
```

### Comparing `django-connectwise-0.3.98/djconnectwise/models.py` & `django-connectwise-0.3.99/djconnectwise/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,19 +113,28 @@
         """
         try:
             closed_status = self.board_statuses.get(
                 name='Closed',
                 closed_status=True,
             )
         except BoardStatus.DoesNotExist:
-            # There's nothing called "Closed".
-            # filter...first returns None if nothing is found.
+            # Using first this time because there could be many and we
+            # still don't know which one it could be, or just get None.
             closed_status = self.board_statuses.filter(
+                name__iregex=r'^[[:punct:]]*Closed[[:punct:]]*$',
                 closed_status=True,
             ).first()
+
+            if not closed_status:
+                # There's nothing called "Closed", or "Closed" surrounded by
+                # special charaters.
+                # filter...first returns None if nothing is found again.
+                closed_status = self.board_statuses.filter(
+                    closed_status=True,
+                ).first()
         return closed_status
 
 
 class AvailableBoardStatusManager(models.Manager):
     """
     Return only statuses whose ConnectWise board is active, and whose
     inactive field is False.
```

### Comparing `django-connectwise-0.3.98/djconnectwise/tests/fixtures.py` & `django-connectwise-0.3.99/djconnectwise/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/tests/test_api.py` & `django-connectwise-0.3.99/djconnectwise/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/tests/AnonymousMember.png` & `django-connectwise-0.3.99/djconnectwise/tests/AnonymousMember.png`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/tests/__pycache__/test_commands.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/tests/__pycache__/test_commands.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,1496 +1,1393 @@
-00000000: 160d 0d0a 7af3 195f d455 0000 e300 0000  ....z.._.U......
+00000000: 330d 0d0a baca 315f d455 0000 e300 0000  3.....1_.U......
 00000010: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
-00000020: 0073 e704 0000 6400 0064 0100 6c00 005a  .s....d..d..l..Z
-00000030: 0000 6400 0064 0200 6c01 006d 0200 5a02  ..d..d..l..m..Z.
-00000040: 0001 6400 0064 0300 6c03 006d 0400 5a04  ..d..d..l..m..Z.
-00000050: 0001 6400 0064 0400 6c05 006d 0600 5a06  ..d..d..l..m..Z.
-00000060: 0001 6405 0064 0600 6c07 006d 0800 5a08  ..d..d..l..m..Z.
-00000070: 0001 6405 0064 0700 6c07 006d 0900 5a09  ..d..d..l..m..Z.
-00000080: 0001 6405 0064 0800 6c07 006d 0a00 5a0a  ..d..d..l..m..Z.
-00000090: 0001 6409 0064 0a00 6c07 006d 0b00 5a0b  ..d..d..l..m..Z.
-000000a0: 0001 640b 0064 0c00 8400 005a 0c00 640d  ..d..d.....Z..d.
-000000b0: 0064 0e00 8400 005a 0d00 640f 0064 1000  .d.....Z..d..d..
-000000c0: 8400 005a 0e00 4764 1100 6412 0084 0000  ...Z..Gd..d.....
-000000d0: 6412 0065 0f00 8303 005a 1000 4764 1300  d..e.....Z..Gd..
-000000e0: 6414 0084 0000 6414 0065 1000 6504 0083  d.....d..e..e...
-000000f0: 0400 5a11 0047 6415 0064 1600 8400 0064  ..Z..Gd..d.....d
-00000100: 1600 6510 0065 0400 8304 005a 1200 4764  ..e..e.....Z..Gd
-00000110: 1700 6418 0084 0000 6418 0065 1000 6504  ..d.....d..e..e.
-00000120: 0083 0400 5a13 0047 6419 0064 1a00 8400  ....Z..Gd..d....
-00000130: 0064 1a00 6510 0065 0400 8304 005a 1400  .d..e..e.....Z..
-00000140: 4764 1b00 641c 0084 0000 641c 0065 1000  Gd..d.....d..e..
-00000150: 6504 0083 0400 5a15 0047 641d 0064 1e00  e.....Z..Gd..d..
-00000160: 8400 0064 1e00 6510 0065 0400 8304 005a  ...d..e..e.....Z
-00000170: 1600 4764 1f00 6420 0084 0000 6420 0065  ..Gd..d ....d .e
-00000180: 1000 6504 0083 0400 5a17 0047 6421 0064  ..e.....Z..Gd!.d
-00000190: 2200 8400 0064 2200 6510 0065 0400 8304  "....d".e..e....
-000001a0: 005a 1800 4764 2300 6424 0084 0000 6424  .Z..Gd#.d$....d$
-000001b0: 0065 1000 6504 0083 0400 5a19 0047 6425  .e..e.....Z..Gd%
-000001c0: 0064 2600 8400 0064 2600 6510 0065 0400  .d&....d&.e..e..
-000001d0: 8304 005a 1a00 4764 2700 6428 0084 0000  ...Z..Gd'.d(....
-000001e0: 6428 0065 1000 6504 0083 0400 5a1b 0047  d(.e..e.....Z..G
-000001f0: 6429 0064 2a00 8400 0064 2a00 6510 0065  d).d*....d*.e..e
-00000200: 0400 8304 005a 1c00 4764 2b00 642c 0084  .....Z..Gd+.d,..
-00000210: 0000 642c 0065 1000 6504 0083 0400 5a1d  ..d,.e..e.....Z.
-00000220: 0047 642d 0064 2e00 8400 0064 2e00 6510  .Gd-.d.....d..e.
-00000230: 0065 0400 8304 005a 1e00 4764 2f00 6430  .e.....Z..Gd/.d0
-00000240: 0084 0000 6430 0065 1000 6504 0083 0400  ....d0.e..e.....
-00000250: 5a1f 0047 6431 0064 3200 8400 0064 3200  Z..Gd1.d2....d2.
-00000260: 6510 0065 0400 8304 005a 2000 4764 3300  e..e.....Z .Gd3.
-00000270: 6434 0084 0000 6434 0065 1000 6504 0083  d4....d4.e..e...
-00000280: 0400 5a21 0047 6435 0064 3600 8400 0064  ..Z!.Gd5.d6....d
-00000290: 3600 6510 0065 0400 8304 005a 2200 4764  6.e..e.....Z".Gd
-000002a0: 3700 6438 0084 0000 6438 0065 1000 6504  7.d8....d8.e..e.
-000002b0: 0083 0400 5a23 0047 6439 0064 3a00 8400  ....Z#.Gd9.d:...
-000002c0: 0064 3a00 6510 0065 0400 8304 005a 2400  .d:.e..e.....Z$.
-000002d0: 4764 3b00 643c 0084 0000 643c 0065 1000  Gd;.d<....d<.e..
-000002e0: 6504 0083 0400 5a25 0047 643d 0064 3e00  e.....Z%.Gd=.d>.
-000002f0: 8400 0064 3e00 6510 0065 0400 8304 005a  ...d>.e..e.....Z
-00000300: 2600 4764 3f00 6440 0084 0000 6440 0065  &.Gd?.d@....d@.e
-00000310: 1000 6504 0083 0400 5a27 0047 6441 0064  ..e.....Z'.GdA.d
-00000320: 4200 8400 0064 4200 6510 0065 0400 8304  B....dB.e..e....
-00000330: 005a 2800 4764 4300 6444 0084 0000 6444  .Z(.GdC.dD....dD
-00000340: 0065 1000 6504 0083 0400 5a29 0047 6445  .e..e.....Z).GdE
-00000350: 0064 4600 8400 0064 4600 6510 0065 0400  .dF....dF.e..e..
-00000360: 8304 005a 2a00 4764 4700 6448 0084 0000  ...Z*.GdG.dH....
-00000370: 6448 0065 1000 6504 0083 0400 5a2b 0047  dH.e..e.....Z+.G
-00000380: 6449 0064 4a00 8400 0064 4a00 6510 0065  dI.dJ....dJ.e..e
-00000390: 0400 8304 005a 2c00 4764 4b00 644c 0084  .....Z,.GdK.dL..
-000003a0: 0000 644c 0065 1000 6504 0083 0400 5a2d  ..dL.e..e.....Z-
-000003b0: 0047 644d 0064 4e00 8400 0064 4e00 6510  .GdM.dN....dN.e.
-000003c0: 0065 0400 8304 005a 2e00 4764 4f00 6450  .e.....Z..GdO.dP
-000003d0: 0084 0000 6450 0065 1000 6504 0083 0400  ....dP.e..e.....
-000003e0: 5a2f 0047 6451 0064 5200 8400 0064 5200  Z/.GdQ.dR....dR.
-000003f0: 6510 0065 0400 8304 005a 3000 4764 5300  e..e.....Z0.GdS.
-00000400: 6454 0084 0000 6454 0065 1000 6504 0083  dT....dT.e..e...
-00000410: 0400 5a31 0047 6455 0064 5600 8400 0064  ..Z1.GdU.dV....d
-00000420: 5600 6510 0065 0400 8304 005a 3200 4764  V.e..e.....Z2.Gd
-00000430: 5700 6458 0084 0000 6458 0065 1000 6504  W.dX....dX.e..e.
-00000440: 0083 0400 5a33 0047 6459 0064 5a00 8400  ....Z3.GdY.dZ...
-00000450: 0064 5a00 6510 0065 0400 8304 005a 3400  .dZ.e..e.....Z4.
-00000460: 4764 5b00 645c 0084 0000 645c 0065 1000  Gd[.d\....d\.e..
-00000470: 6504 0083 0400 5a35 0047 645d 0064 5e00  e.....Z5.Gd].d^.
-00000480: 8400 0064 5e00 6510 0065 0400 8304 005a  ...d^.e..e.....Z
-00000490: 3600 4764 5f00 6460 0084 0000 6460 0065  6.Gd_.d`....d`.e
-000004a0: 1000 6504 0083 0400 5a37 0047 6461 0064  ..e.....Z7.Gda.d
-000004b0: 6200 8400 0064 6200 6510 0065 0400 8304  b....db.e..e....
-000004c0: 005a 3800 4764 6300 6464 0084 0000 6464  .Z8.Gdc.dd....dd
-000004d0: 0065 1000 6504 0083 0400 5a39 0047 6465  .e..e.....Z9.Gde
-000004e0: 0064 6600 8400 0064 6600 6504 0083 0300  .df....df.e.....
-000004f0: 5a3a 0047 6467 0064 6800 8400 0064 6800  Z:.Gdg.dh....dh.
-00000500: 6504 0083 0300 5a3b 0064 0100 5329 69e9  e.....Z;.d..S)i.
-00000510: 0000 0000 4e29 01da 0c63 616c 6c5f 636f  ....N)...call_co
-00000520: 6d6d 616e 6429 01da 0854 6573 7443 6173  mmand)...TestCas
-00000530: 6529 01da 066d 6f64 656c 73e9 0100 0000  e)...models.....
-00000540: 2901 da05 6d6f 636b 7329 01da 0866 6978  )...mocks)...fix
-00000550: 7475 7265 7329 01da 0d66 6978 7475 7265  tures)...fixture
-00000560: 5f75 7469 6c73 e902 0000 0029 01da 0473  _utils.....)...s
-00000570: 796e 6363 0200 0000 0000 0000 0200 0000  yncc............
-00000580: 0300 0000 4300 0000 7310 0000 0064 0100  ....C...s....d..
-00000590: 6a00 007c 0000 7c01 0083 0200 5329 024e  j..|..|.....S).N
-000005a0: 7a29 7b7d 2053 796e 6320 5375 6d6d 6172  z){} Sync Summar
-000005b0: 7920 2d20 4372 6561 7465 643a 207b 7d2c  y - Created: {},
-000005c0: 2055 7064 6174 6564 3a20 3029 01da 0666   Updated: 0)...f
-000005d0: 6f72 6d61 7429 02da 0a63 6c61 7373 5f6e  ormat)...class_n
-000005e0: 616d 655a 0d63 7265 6174 6564 5f63 6f75  ameZ.created_cou
-000005f0: 6e74 a900 720d 0000 00fa 5f2f 686f 6d65  nt..r....._/home
-00000600: 2f73 616d 2f67 6974 2f4b 616e 6261 6e2f  /sam/git/Kanban/
-00000610: 646a 616e 676f 2d63 6f6e 6e65 6374 7769  django-connectwi
-00000620: 7365 2f64 6a61 6e67 6f2d 636f 6e6e 6563  se/django-connec
-00000630: 7477 6973 652f 646a 636f 6e6e 6563 7477  twise/djconnectw
-00000640: 6973 652f 7465 7374 732f 7465 7374 5f63  ise/tests/test_c
-00000650: 6f6d 6d61 6e64 732e 7079 da0c 7379 6e63  ommands.py..sync
-00000660: 5f73 756d 6d61 7279 0e00 0000 7304 0000  _summary....s...
-00000670: 0000 0106 0172 0f00 0000 6302 0000 0000  .....r....c.....
-00000680: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00000690: 1000 0000 6401 006a 0000 7c00 007c 0100  ....d..j..|..|..
-000006a0: 8302 0053 2902 4e7a 357b 7d20 5379 6e63  ...S).Nz5{} Sync
-000006b0: 2053 756d 6d61 7279 202d 2043 7265 6174   Summary - Creat
-000006c0: 6564 3a20 302c 2055 7064 6174 6564 3a20  ed: 0, Updated: 
-000006d0: 302c 2044 656c 6574 6564 3a20 7b7d 2901  0, Deleted: {}).
-000006e0: 720b 0000 0029 0272 0c00 0000 5a0d 6465  r....).r....Z.de
-000006f0: 6c65 7465 645f 636f 756e 7472 0d00 0000  leted_countr....
-00000700: 720d 0000 0072 0e00 0000 da11 6675 6c6c  r....r......full
-00000710: 5f73 796e 635f 7375 6d6d 6172 7914 0000  _sync_summary...
-00000720: 0073 0400 0000 0001 0601 7210 0000 0063  .s........r....c
-00000730: 0100 0000 0000 0000 0100 0000 0300 0000  ................
-00000740: 4300 0000 7316 0000 007c 0000 6a00 0083  C...s....|..j...
-00000750: 0000 6a01 0064 0100 6402 0083 0200 5329  ..j..d..d.....S)
-00000760: 034e da01 5ffa 0120 2902 da05 7469 746c  .N.._.. )...titl
-00000770: 65da 0772 6570 6c61 6365 2901 da04 736c  e..replace)...sl
-00000780: 7567 720d 0000 0072 0d00 0000 720e 0000  ugr....r....r...
-00000790: 00da 0d73 6c75 675f 746f 5f74 6974 6c65  ...slug_to_title
-000007a0: 1a00 0000 7302 0000 0000 0172 1600 0000  ....s......r....
-000007b0: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
-000007c0: 0040 0000 0073 4300 0000 6500 005a 0100  .@...sC...e..Z..
-000007d0: 6400 005a 0200 6401 0064 0200 6403 0084  d..Z..d..d..d...
-000007e0: 0100 5a03 0064 0400 6405 0084 0000 5a04  ..Z..d..d.....Z.
-000007f0: 0064 0600 6407 0084 0000 5a05 0064 0800  .d..d.....Z..d..
-00000800: 6409 0084 0000 5a06 0064 0a00 5329 0bda  d.....Z..d..S)..
-00000810: 1441 6273 7472 6163 7442 6173 6553 796e  .AbstractBaseSyn
-00000820: 6354 6573 7446 6305 0000 0000 0000 0007  cTestFc.........
-00000830: 0000 0004 0000 0043 0000 0073 4900 0000  .......C...sI...
-00000840: 7c01 007c 0200 8301 0001 7400 006a 0100  |..|......t..j..
-00000850: 8300 007d 0500 6401 007c 0300 6702 007d  ...}..d..|..g..}
-00000860: 0600 7c04 0072 3500 7c06 006a 0200 6402  ..|..r5.|..j..d.
-00000870: 0083 0100 0174 0300 7c06 0064 0300 7c05  .....t..|..d..|.
-00000880: 008c 0001 017c 0500 5329 044e da06 6377  .....|..S).N..cw
-00000890: 7379 6e63 7a06 2d2d 6675 6c6c da06 7374  syncz.--full..st
-000008a0: 646f 7574 2904 da02 696f da08 5374 7269  dout)...io..Stri
-000008b0: 6e67 494f da06 6170 7065 6e64 7202 0000  ngIO..appendr...
-000008c0: 0029 07da 0473 656c 66da 096d 6f63 6b5f  .)...self..mock_
-000008d0: 6361 6c6c da0c 7265 7475 726e 5f76 616c  call..return_val
-000008e0: 7565 da09 6377 5f6f 626a 6563 74da 0b66  ue..cw_object..f
-000008f0: 756c 6c5f 6f70 7469 6f6e da03 6f75 74da  ull_option..out.
-00000900: 0461 7267 7372 0d00 0000 720d 0000 0072  .argsr....r....r
-00000910: 0e00 0000 da0a 5f74 6573 745f 7379 6e63  ......_test_sync
-00000920: 2000 0000 730e 0000 0000 020a 010c 020c   ...s...........
-00000930: 0106 010d 0110 017a 1f41 6273 7472 6163  .......z.Abstrac
-00000940: 7442 6173 6553 796e 6354 6573 742e 5f74  tBaseSyncTest._t
-00000950: 6573 745f 7379 6e63 6302 0000 0000 0000  est_syncc.......
-00000960: 0002 0000 0003 0000 0043 0000 0073 1600  .........C...s..
-00000970: 0000 7c01 006a 0000 8300 006a 0100 6401  ..|..j.....j..d.
-00000980: 0064 0200 8302 0053 2903 4e72 1100 0000  .d.....S).Nr....
-00000990: 7212 0000 0029 0272 1300 0000 7214 0000  r....).r....r...
-000009a0: 0029 0272 1d00 0000 7220 0000 0072 0d00  .).r....r ...r..
-000009b0: 0000 720d 0000 0072 0e00 0000 da14 5f74  ..r....r......_t
-000009c0: 6974 6c65 5f66 6f72 5f63 775f 6f62 6a65  itle_for_cw_obje
-000009d0: 6374 2b00 0000 7302 0000 0000 017a 2941  ct+...s......z)A
-000009e0: 6273 7472 6163 7442 6173 6553 796e 6354  bstractBaseSyncT
-000009f0: 6573 742e 5f74 6974 6c65 5f66 6f72 5f63  est._title_for_c
-00000a00: 775f 6f62 6a65 6374 6301 0000 0000 0000  w_objectc.......
-00000a10: 0003 0000 0003 0000 0043 0000 0073 4800  .........C...sH.
-00000a20: 0000 7c00 006a 0000 7c00 006a 0100 8c00  ..|..j..|..j....
-00000a30: 007d 0100 7c00 006a 0200 7c00 006a 0100  .}..|..j..|..j..
-00000a40: 6402 0019 8301 007d 0200 7c00 006a 0300  d......}..|..j..
-00000a50: 7c02 007c 0100 6a04 0083 0000 6a05 0083  |..|..j.....j...
-00000a60: 0000 8302 0001 6400 0053 2903 4e72 0500  ......d..S).Nr..
-00000a70: 0000 e9ff ffff ff29 0672 2400 0000 7223  .......).r$...r#
-00000a80: 0000 0072 2500 0000 da08 6173 7365 7274  ...r%.....assert
-00000a90: 496e da08 6765 7476 616c 7565 da05 7374  In..getvalue..st
-00000aa0: 7269 7029 0372 1d00 0000 7222 0000 005a  rip).r....r"...Z
-00000ab0: 096f 626a 5f74 6974 6c65 720d 0000 0072  .obj_titler....r
-00000ac0: 0d00 0000 720e 0000 00da 0974 6573 745f  ....r......test_
-00000ad0: 7379 6e63 2e00 0000 7306 0000 0000 0112  sync....s.......
-00000ae0: 0116 017a 1e41 6273 7472 6163 7442 6173  ...z.AbstractBas
-00000af0: 6553 796e 6354 6573 742e 7465 7374 5f73  eSyncTest.test_s
-00000b00: 796e 6363 0100 0000 0000 0000 0900 0000  yncc............
-00000b10: 0400 0000 4300 0000 738d 0000 007c 0000  ....C...s....|..
-00000b20: 6a00 0083 0000 017c 0000 6a01 005c 0300  j......|..j..\..
-00000b30: 7d01 007d 0200 7d03 007c 0100 6700 007c  }..}..}..|..g..|
-00000b40: 0300 6703 007d 0400 7c00 006a 0200 7c04  ..g..}..|..j..|.
-00000b50: 0064 0100 6402 008c 0001 7d05 007c 0000  .d..d.....}..|..
-00000b60: 6a03 007c 0300 8301 007d 0600 6403 007d  j..|.....}..d..}
-00000b70: 0700 7c07 006a 0400 7c06 0074 0500 7c02  ..|..j..|..t..|.
-00000b80: 0083 0100 8302 007d 0800 7c00 006a 0600  .......}..|..j..
-00000b90: 7c08 007c 0500 6a07 0083 0000 6a08 0083  |..|..j.....j...
-00000ba0: 0000 8302 0001 6400 0053 2904 4e72 2100  ......d..S).Nr!.
-00000bb0: 0000 547a 357b 7d20 5379 6e63 2053 756d  ..Tz5{} Sync Sum
-00000bc0: 6d61 7279 202d 2043 7265 6174 6564 3a20  mary - Created: 
-00000bd0: 302c 2055 7064 6174 6564 3a20 302c 2044  0, Updated: 0, D
-00000be0: 656c 6574 6564 3a20 7b7d 2909 722a 0000  eleted: {}).r*..
-00000bf0: 0072 2300 0000 7224 0000 0072 2500 0000  .r#...r$...r%...
-00000c00: 720b 0000 00da 036c 656e da0b 6173 7365  r......len..asse
-00000c10: 7274 4571 7561 6c72 2800 0000 7229 0000  rtEqualr(...r)..
-00000c20: 0029 0972 1d00 0000 721e 0000 0072 1f00  .).r....r....r..
-00000c30: 0000 7220 0000 0072 2300 0000 7222 0000  ..r ...r#...r"..
-00000c40: 005a 096f 626a 5f6c 6162 656c 5a08 6d73  .Z.obj_labelZ.ms
-00000c50: 675f 746d 706c da03 6d73 6772 0d00 0000  g_tmpl..msgr....
-00000c60: 720d 0000 0072 0e00 0000 da0e 7465 7374  r....r......test
-00000c70: 5f66 756c 6c5f 7379 6e63 3300 0000 7314  _full_sync3...s.
-00000c80: 0000 0000 010a 0112 0203 0103 0109 0315  ................
-00000c90: 010f 0106 0118 017a 2341 6273 7472 6163  .......z#Abstrac
-00000ca0: 7442 6173 6553 796e 6354 6573 742e 7465  tBaseSyncTest.te
-00000cb0: 7374 5f66 756c 6c5f 7379 6e63 4e29 07da  st_full_syncN)..
-00000cc0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000cd0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000ce0: 655f 5f72 2400 0000 7225 0000 0072 2a00  e__r$...r%...r*.
-00000cf0: 0000 722e 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00000d00: 0072 0d00 0000 720e 0000 0072 1700 0000  .r....r....r....
-00000d10: 1e00 0000 7308 0000 000c 030f 0a0c 030c  ....s...........
-00000d20: 0572 1700 0000 6300 0000 0000 0000 0000  .r....c.........
-00000d30: 0000 0003 0000 0040 0000 0073 2500 0000  .......@...s%...
-00000d40: 6500 005a 0100 6400 005a 0200 6503 006a  e..Z..d..Z..e..j
-00000d50: 0400 6505 006a 0600 6401 0066 0300 5a07  ..e..j..d..f..Z.
-00000d60: 0064 0200 5329 03da 1854 6573 7453 796e  .d..S)...TestSyn
-00000d70: 6343 616c 656e 6461 7273 436f 6d6d 616e  cCalendarsComman
-00000d80: 64da 0863 616c 656e 6461 724e 2908 722f  d..calendarN).r/
-00000d90: 0000 0072 3000 0000 7231 0000 0072 0600  ...r0...r1...r..
-00000da0: 0000 da1f 7363 6865 6475 6c65 5f61 7069  ....schedule_api
-00000db0: 5f67 6574 5f63 616c 656e 6461 7273 5f63  _get_calendars_c
-00000dc0: 616c 6c72 0700 0000 da1a 4150 495f 5343  allr......API_SC
-00000dd0: 4845 4455 4c45 5f43 414c 454e 4441 525f  HEDULE_CALENDAR_
-00000de0: 4c49 5354 7223 0000 0072 0d00 0000 720d  LISTr#...r....r.
-00000df0: 0000 0072 0d00 0000 720e 0000 0072 3200  ...r....r....r2.
-00000e00: 0000 4300 0000 7306 0000 000c 0206 0106  ..C...s.........
-00000e10: 0172 3200 0000 6300 0000 0000 0000 0000  .r2...c.........
-00000e20: 0000 0003 0000 0040 0000 0073 3100 0000  .......@...s1...
-00000e30: 6500 005a 0100 6400 005a 0200 6503 006a  e..Z..d..Z..e..j
-00000e40: 0400 6505 006a 0600 6401 0066 0300 5a07  ..e..j..d..f..Z.
-00000e50: 0064 0200 6403 0084 0000 5a08 0064 0400  .d..d.....Z..d..
-00000e60: 5329 05da 1654 6573 7453 796e 6348 6f6c  S)...TestSyncHol
-00000e70: 6964 6179 436f 6d6d 616e 64da 0768 6f6c  idayCommand..hol
-00000e80: 6964 6179 6301 0000 0000 0000 0001 0000  idayc...........
-00000e90: 0001 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
-00000ea0: 006a 0100 8300 0001 6400 0053 2901 4e29  .j......d..S).N)
-00000eb0: 0272 0800 0000 5a12 696e 6974 5f68 6f6c  .r....Z.init_hol
-00000ec0: 6964 6179 5f6c 6973 7473 2901 721d 0000  iday_lists).r...
-00000ed0: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
-00000ee0: da05 7365 7455 7052 0000 0073 0200 0000  ..setUpR...s....
-00000ef0: 0001 7a1c 5465 7374 5379 6e63 486f 6c69  ..z.TestSyncHoli
-00000f00: 6461 7943 6f6d 6d61 6e64 2e73 6574 5570  dayCommand.setUp
-00000f10: 4e29 0972 2f00 0000 7230 0000 0072 3100  N).r/...r0...r1.
-00000f20: 0000 7206 0000 00da 1e73 6368 6564 756c  ..r......schedul
-00000f30: 655f 6170 695f 6765 745f 686f 6c69 6461  e_api_get_holida
-00000f40: 7973 5f63 616c 6c72 0700 0000 da1f 4150  ys_callr......AP
-00000f50: 495f 5343 4845 4455 4c45 5f48 4f4c 4944  I_SCHEDULE_HOLID
-00000f60: 4159 5f4d 4f44 454c 5f4c 4953 5472 2300  AY_MODEL_LISTr#.
-00000f70: 0000 7238 0000 0072 0d00 0000 720d 0000  ..r8...r....r...
-00000f80: 0072 0d00 0000 720e 0000 0072 3600 0000  .r....r....r6...
-00000f90: 4b00 0000 7308 0000 000c 0206 0106 0109  K...s...........
-00000fa0: 0372 3600 0000 6300 0000 0000 0000 0000  .r6...c.........
-00000fb0: 0000 0003 0000 0040 0000 0073 2500 0000  .......@...s%...
-00000fc0: 6500 005a 0100 6400 005a 0200 6503 006a  e..Z..d..Z..e..j
-00000fd0: 0400 6505 006a 0600 6401 0066 0300 5a07  ..e..j..d..f..Z.
-00000fe0: 0064 0200 5329 03da 1a54 6573 7453 796e  .d..S)...TestSyn
-00000ff0: 6348 6f6c 6964 6179 4c69 7374 436f 6d6d  cHolidayListComm
-00001000: 616e 64da 0c68 6f6c 6964 6179 5f6c 6973  and..holiday_lis
-00001010: 744e 2908 722f 0000 0072 3000 0000 7231  tN).r/...r0...r1
-00001020: 0000 0072 0600 0000 da23 7363 6865 6475  ...r.....#schedu
-00001030: 6c65 5f61 7069 5f67 6574 5f68 6f6c 6964  le_api_get_holid
-00001040: 6179 5f6c 6973 7473 5f63 616c 6c72 0700  ay_lists_callr..
-00001050: 0000 da1e 4150 495f 5343 4845 4455 4c45  ....API_SCHEDULE
-00001060: 5f48 4f4c 4944 4159 5f4c 4953 545f 4c49  _HOLIDAY_LIST_LI
-00001070: 5354 7223 0000 0072 0d00 0000 720d 0000  STr#...r....r...
-00001080: 0072 0d00 0000 720e 0000 0072 3b00 0000  .r....r....r;...
-00001090: 5600 0000 7306 0000 000c 0206 0106 0172  V...s..........r
-000010a0: 3b00 0000 6300 0000 0000 0000 0000 0000  ;...c...........
-000010b0: 0003 0000 0040 0000 0073 2500 0000 6500  .....@...s%...e.
-000010c0: 005a 0100 6400 005a 0200 6503 006a 0400  .Z..d..Z..e..j..
-000010d0: 6505 006a 0600 6401 0066 0300 5a07 0064  e..j..d..f..Z..d
-000010e0: 0200 5329 03da 1e54 6573 7453 796e 6343  ..S)...TestSyncC
-000010f0: 6f6d 7061 6e79 5374 6174 7573 6573 436f  ompanyStatusesCo
-00001100: 6d6d 616e 64da 0e63 6f6d 7061 6e79 5f73  mmand..company_s
-00001110: 7461 7475 734e 2908 722f 0000 0072 3000  tatusN).r/...r0.
-00001120: 0000 7231 0000 0072 0600 0000 da25 636f  ..r1...r.....%co
-00001130: 6d70 616e 795f 6170 695f 6765 745f 636f  mpany_api_get_co
-00001140: 6d70 616e 795f 7374 6174 7573 6573 5f63  mpany_statuses_c
-00001150: 616c 6c72 0700 0000 da17 4150 495f 434f  allr......API_CO
-00001160: 4d50 414e 595f 5354 4154 5553 5f4c 4953  MPANY_STATUS_LIS
-00001170: 5472 2300 0000 720d 0000 0072 0d00 0000  Tr#...r....r....
-00001180: 720d 0000 0072 0e00 0000 723f 0000 005e  r....r....r?...^
-00001190: 0000 0073 0600 0000 0c02 0601 0601 723f  ...s..........r?
-000011a0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000011b0: 0300 0000 4000 0000 7325 0000 0065 0000  ....@...s%...e..
-000011c0: 5a01 0064 0000 5a02 0065 0300 6a04 0065  Z..d..Z..e..j..e
-000011d0: 0500 6a06 0064 0100 6603 005a 0700 6402  ..j..d..f..Z..d.
-000011e0: 0053 2903 da1a 5465 7374 5379 6e63 5465  .S)...TestSyncTe
-000011f0: 7272 6974 6f72 6965 7343 6f6d 6d61 6e64  rritoriesCommand
-00001200: da09 7465 7272 6974 6f72 794e 2908 722f  ..territoryN).r/
-00001210: 0000 0072 3000 0000 7231 0000 0072 0600  ...r0...r1...r..
-00001220: 0000 da1f 7379 7374 656d 5f61 7069 5f67  ....system_api_g
-00001230: 6574 5f74 6572 7269 746f 7269 6573 5f63  et_territories_c
-00001240: 616c 6c72 0700 0000 da19 4150 495f 5359  allr......API_SY
-00001250: 5354 454d 5f54 4552 5249 544f 5259 5f4c  STEM_TERRITORY_L
-00001260: 4953 5472 2300 0000 720d 0000 0072 0d00  ISTr#...r....r..
-00001270: 0000 720d 0000 0072 0e00 0000 7243 0000  ..r....r....rC..
-00001280: 0066 0000 0073 0600 0000 0c02 0601 0601  .f...s..........
-00001290: 7243 0000 0063 0000 0000 0000 0000 0000  rC...c..........
-000012a0: 0000 0300 0000 0000 0000 7337 0000 0065  ..........s7...e
-000012b0: 0000 5a01 0064 0000 5a02 0087 0000 6601  ..Z..d..Z.....f.
-000012c0: 0064 0100 6402 0086 0000 5a03 0065 0400  .d..d.....Z..e..
-000012d0: 6a05 0065 0600 6a07 0064 0300 6603 005a  j..e..j..d..f..Z
-000012e0: 0800 8700 0053 2904 da18 5465 7374 5379  .....S)...TestSy
-000012f0: 6e63 436f 6d70 616e 6965 7343 6f6d 6d61  ncCompaniesComma
-00001300: 6e64 6301 0000 0000 0000 0001 0000 0001  ndc.............
-00001310: 0000 0003 0000 0073 1b00 0000 7400 0083  .......s....t...
-00001320: 0000 6a01 0083 0000 0174 0200 6a03 0083  ..j......t..j...
-00001330: 0000 0164 0000 5329 014e 2904 da05 7375  ...d..S).N)...su
-00001340: 7065 7272 3800 0000 7208 0000 00da 1069  perr8...r......i
-00001350: 6e69 745f 7465 7272 6974 6f72 6965 7329  nit_territories)
-00001360: 0172 1d00 0000 2901 da09 5f5f 636c 6173  .r....)...__clas
-00001370: 735f 5f72 0d00 0000 720e 0000 0072 3800  s__r....r....r8.
-00001380: 0000 6f00 0000 7304 0000 0000 010d 017a  ..o...s........z
-00001390: 1e54 6573 7453 796e 6343 6f6d 7061 6e69  .TestSyncCompani
-000013a0: 6573 436f 6d6d 616e 642e 7365 7455 70da  esCommand.setUp.
-000013b0: 0763 6f6d 7061 6e79 2909 722f 0000 0072  .company).r/...r
-000013c0: 3000 0000 7231 0000 0072 3800 0000 7206  0...r1...r8...r.
-000013d0: 0000 00da 1463 6f6d 7061 6e79 5f61 7069  .....company_api
-000013e0: 5f67 6574 5f63 616c 6c72 0700 0000 da10  _get_callr......
-000013f0: 4150 495f 434f 4d50 414e 595f 4c49 5354  API_COMPANY_LIST
-00001400: 7223 0000 0072 0d00 0000 720d 0000 0029  r#...r....r....)
-00001410: 0172 4a00 0000 720e 0000 0072 4700 0000  .rJ...r....rG...
-00001420: 6e00 0000 7308 0000 000c 0112 0506 0106  n...s...........
-00001430: 0172 4700 0000 6300 0000 0000 0000 0000  .rG...c.........
-00001440: 0000 0003 0000 0040 0000 0073 2500 0000  .......@...s%...
-00001450: 6500 005a 0100 6400 005a 0200 6503 006a  e..Z..d..Z..e..j
-00001460: 0400 6505 006a 0600 6401 0066 0300 5a07  ..e..j..d..f..Z.
-00001470: 0064 0200 5329 03da 1b54 6573 7453 796e  .d..S)...TestSyn
-00001480: 6343 6f6d 7061 6e79 5479 7065 7343 6f6d  cCompanyTypesCom
-00001490: 6d61 6e64 da0c 636f 6d70 616e 795f 7479  mand..company_ty
-000014a0: 7065 4e29 0872 2f00 0000 7230 0000 0072  peN).r/...r0...r
-000014b0: 3100 0000 7206 0000 00da 2263 6f6d 7061  1...r....."compa
-000014c0: 6e79 5f61 7069 5f67 6574 5f63 6f6d 7061  ny_api_get_compa
-000014d0: 6e79 5f74 7970 6573 5f63 616c 6c72 0700  ny_types_callr..
-000014e0: 0000 da16 4150 495f 434f 4d50 414e 595f  ....API_COMPANY_
-000014f0: 5459 5045 535f 4c49 5354 7223 0000 0072  TYPES_LISTr#...r
-00001500: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
-00001510: 0000 0072 4e00 0000 7a00 0000 7306 0000  ...rN...z...s...
-00001520: 000c 0206 0106 0172 4e00 0000 6300 0000  .......rN...c...
-00001530: 0000 0000 0000 0000 0003 0000 0000 0000  ................
-00001540: 0073 3700 0000 6500 005a 0100 6400 005a  .s7...e..Z..d..Z
-00001550: 0200 6503 006a 0400 6505 006a 0600 6401  ..e..j..e..j..d.
-00001560: 0066 0300 5a07 0087 0000 6601 0064 0200  .f..Z.....f..d..
-00001570: 6403 0086 0000 5a08 0087 0000 5329 04da  d.....Z.....S)..
-00001580: 1454 6573 7453 796e 6354 6561 6d73 436f  .TestSyncTeamsCo
-00001590: 6d6d 616e 64da 0474 6561 6d63 0100 0000  mmand..teamc....
-000015a0: 0000 0000 0100 0000 0100 0000 0300 0000  ................
-000015b0: 731b 0000 0074 0000 8300 006a 0100 8300  s....t.....j....
-000015c0: 0001 7402 006a 0300 8300 0001 6400 0053  ..t..j......d..S
-000015d0: 2901 4e29 0472 4800 0000 7238 0000 0072  ).N).rH...r8...r
-000015e0: 0800 0000 da0b 696e 6974 5f62 6f61 7264  ......init_board
-000015f0: 7329 0172 1d00 0000 2901 724a 0000 0072  s).r....).rJ...r
-00001600: 0d00 0000 720e 0000 0072 3800 0000 8900  ....r....r8.....
-00001610: 0000 7304 0000 0000 010d 017a 1a54 6573  ..s........z.Tes
-00001620: 7453 796e 6354 6561 6d73 436f 6d6d 616e  tSyncTeamsComman
-00001630: 642e 7365 7455 7029 0972 2f00 0000 7230  d.setUp).r/...r0
-00001640: 0000 0072 3100 0000 7206 0000 00da 1a73  ...r1...r......s
-00001650: 6572 7669 6365 5f61 7069 5f67 6574 5f74  ervice_api_get_t
-00001660: 6561 6d73 5f63 616c 6c72 0700 0000 da15  eams_callr......
-00001670: 4150 495f 5345 5256 4943 455f 5445 414d  API_SERVICE_TEAM
-00001680: 5f4c 4953 5472 2300 0000 7238 0000 0072  _LISTr#...r8...r
-00001690: 0d00 0000 720d 0000 0029 0172 4a00 0000  ....r....).rJ...
-000016a0: 720e 0000 0072 5200 0000 8200 0000 7308  r....rR.......s.
-000016b0: 0000 000c 0206 0106 0109 0372 5200 0000  ...........rR...
-000016c0: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
-000016d0: 0040 0000 0073 2500 0000 6500 005a 0100  .@...s%...e..Z..
-000016e0: 6400 005a 0200 6503 006a 0400 6505 006a  d..Z..e..j..e..j
-000016f0: 0600 6401 0066 0300 5a07 0064 0200 5329  ..d..f..Z..d..S)
-00001700: 03da 1554 6573 7453 796e 6342 6f61 7264  ...TestSyncBoard
-00001710: 7343 6f6d 6d61 6e64 da05 626f 6172 644e  sCommand..boardN
-00001720: 2908 722f 0000 0072 3000 0000 7231 0000  ).r/...r0...r1..
-00001730: 0072 0600 0000 da1b 7365 7276 6963 655f  .r......service_
-00001740: 6170 695f 6765 745f 626f 6172 6473 5f63  api_get_boards_c
-00001750: 616c 6c72 0700 0000 da0e 4150 495f 424f  allr......API_BO
-00001760: 4152 445f 4c49 5354 7223 0000 0072 0d00  ARD_LISTr#...r..
-00001770: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-00001780: 0072 5700 0000 8e00 0000 7306 0000 000c  .rW.......s.....
-00001790: 0206 0106 0172 5700 0000 6300 0000 0000  .....rW...c.....
-000017a0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000017b0: 2500 0000 6500 005a 0100 6400 005a 0200  %...e..Z..d..Z..
-000017c0: 6503 006a 0400 6505 006a 0600 6401 0066  e..j..e..j..d..f
-000017d0: 0300 5a07 0064 0200 5329 03da 1854 6573  ..Z..d..S)...Tes
-000017e0: 7453 796e 634c 6f63 6174 696f 6e73 436f  tSyncLocationsCo
-000017f0: 6d6d 616e 64da 086c 6f63 6174 696f 6e4e  mmand..locationN
-00001800: 2908 722f 0000 0072 3000 0000 7231 0000  ).r/...r0...r1..
-00001810: 0072 0600 0000 da1e 7365 7276 6963 655f  .r......service_
-00001820: 6170 695f 6765 745f 6c6f 6361 7469 6f6e  api_get_location
-00001830: 735f 6361 6c6c 7207 0000 00da 1941 5049  s_callr......API
-00001840: 5f53 4552 5649 4345 5f4c 4f43 4154 494f  _SERVICE_LOCATIO
-00001850: 4e5f 4c49 5354 7223 0000 0072 0d00 0000  N_LISTr#...r....
-00001860: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00001870: 5b00 0000 9600 0000 7306 0000 000c 0206  [.......s.......
-00001880: 0106 0172 5b00 0000 6300 0000 0000 0000  ...r[...c.......
-00001890: 0000 0000 0003 0000 0040 0000 0073 3100  .........@...s1.
-000018a0: 0000 6500 005a 0100 6400 005a 0200 6503  ..e..Z..d..Z..e.
-000018b0: 006a 0400 6505 006a 0600 6401 0066 0300  .j..e..j..d..f..
-000018c0: 5a07 0064 0200 6403 0084 0000 5a08 0064  Z..d..d.....Z..d
-000018d0: 0400 5329 05da 1d54 6573 7453 796e 634d  ..S)...TestSyncM
-000018e0: 7943 6f6d 7061 6e79 4f74 6865 7243 6f6d  yCompanyOtherCom
-000018f0: 6d61 6e64 da0d 636f 6d70 616e 795f 6f74  mand..company_ot
-00001900: 6865 7263 0100 0000 0000 0000 0100 0000  herc............
-00001910: 0100 0000 4300 0000 730e 0000 0074 0000  ....C...s....t..
-00001920: 6a01 0083 0000 0164 0000 5329 014e 2902  j......d..S).N).
-00001930: 7208 0000 00da 0e69 6e69 745f 6361 6c65  r......init_cale
-00001940: 6e64 6172 7329 0172 1d00 0000 720d 0000  ndars).r....r...
-00001950: 0072 0d00 0000 720e 0000 0072 3800 0000  .r....r....r8...
-00001960: a500 0000 7302 0000 0000 017a 2354 6573  ....s......z#Tes
-00001970: 7453 796e 634d 7943 6f6d 7061 6e79 4f74  tSyncMyCompanyOt
-00001980: 6865 7243 6f6d 6d61 6e64 2e73 6574 5570  herCommand.setUp
-00001990: 4e29 0972 2f00 0000 7230 0000 0072 3100  N).r/...r0...r1.
-000019a0: 0000 7206 0000 00da 1973 7973 7465 6d5f  ..r......system_
-000019b0: 6170 695f 6765 745f 6f74 6865 725f 6361  api_get_other_ca
-000019c0: 6c6c 7207 0000 00da 1541 5049 5f53 5953  llr......API_SYS
-000019d0: 5445 4d5f 4f54 4845 525f 4c49 5354 7223  TEM_OTHER_LISTr#
-000019e0: 0000 0072 3800 0000 720d 0000 0072 0d00  ...r8...r....r..
-000019f0: 0000 720d 0000 0072 0e00 0000 725f 0000  ..r....r....r_..
-00001a00: 009e 0000 0073 0800 0000 0c02 0601 0601  .....s..........
-00001a10: 0903 725f 0000 0063 0000 0000 0000 0000  ..r_...c........
-00001a20: 0000 0000 0300 0000 4000 0000 7325 0000  ........@...s%..
-00001a30: 0065 0000 5a01 0064 0000 5a02 0065 0300  .e..Z..d..Z..e..
-00001a40: 6a04 0065 0500 6a06 0064 0100 6603 005a  j..e..j..d..f..Z
-00001a50: 0700 6402 0053 2903 da19 5465 7374 5379  ..d..S)...TestSy
-00001a60: 6e63 5072 696f 7269 7469 6573 436f 6d6d  ncPrioritiesComm
-00001a70: 616e 64da 0870 7269 6f72 6974 794e 2908  and..priorityN).
-00001a80: 722f 0000 0072 3000 0000 7231 0000 0072  r/...r0...r1...r
-00001a90: 0600 0000 da1f 7365 7276 6963 655f 6170  ......service_ap
-00001aa0: 695f 6765 745f 7072 696f 7269 7469 6573  i_get_priorities
-00001ab0: 5f63 616c 6c72 0700 0000 da19 4150 495f  _callr......API_
-00001ac0: 5345 5256 4943 455f 5052 494f 5249 5459  SERVICE_PRIORITY
-00001ad0: 5f4c 4953 5472 2300 0000 720d 0000 0072  _LISTr#...r....r
-00001ae0: 0d00 0000 720d 0000 0072 0e00 0000 7264  ....r....r....rd
-00001af0: 0000 00a9 0000 0073 0600 0000 0c03 0601  .......s........
-00001b00: 0601 7264 0000 0063 0000 0000 0000 0000  ..rd...c........
-00001b10: 0000 0000 0300 0000 4000 0000 7325 0000  ........@...s%..
-00001b20: 0065 0000 5a01 0064 0000 5a02 0065 0300  .e..Z..d..Z..e..
-00001b30: 6a04 0065 0500 6a06 0064 0100 6603 005a  j..e..j..d..f..Z
-00001b40: 0700 6402 0053 2903 da1e 5465 7374 5379  ..d..S)...TestSy
-00001b50: 6e63 5072 6f6a 6563 7453 7461 7475 7365  ncProjectStatuse
-00001b60: 7343 6f6d 6d61 6e64 da0e 7072 6f6a 6563  sCommand..projec
-00001b70: 745f 7374 6174 7573 4e29 0872 2f00 0000  t_statusN).r/...
-00001b80: 7230 0000 0072 3100 0000 7206 0000 00da  r0...r1...r.....
-00001b90: 2670 726f 6a65 6374 735f 6170 695f 6765  &projects_api_ge
-00001ba0: 745f 7072 6f6a 6563 745f 7374 6174 7573  t_project_status
-00001bb0: 6573 5f63 616c 6c72 0700 0000 da14 4150  es_callr......AP
-00001bc0: 495f 5052 4f4a 4543 545f 5354 4154 5553  I_PROJECT_STATUS
-00001bd0: 4553 7223 0000 0072 0d00 0000 720d 0000  ESr#...r....r...
-00001be0: 0072 0d00 0000 720e 0000 0072 6800 0000  .r....r....rh...
-00001bf0: b200 0000 7306 0000 000c 0206 0106 0172  ....s..........r
-00001c00: 6800 0000 6300 0000 0000 0000 0000 0000  h...c...........
-00001c10: 0003 0000 0040 0000 0073 2500 0000 6500  .....@...s%...e.
-00001c20: 005a 0100 6400 005a 0200 6503 006a 0400  .Z..d..Z..e..j..
-00001c30: 6505 006a 0600 6401 0066 0300 5a07 0064  e..j..d..f..Z..d
-00001c40: 0200 5329 03da 1b54 6573 7453 796e 6350  ..S)...TestSyncP
-00001c50: 726f 6a65 6374 5479 7065 7343 6f6d 6d61  rojectTypesComma
-00001c60: 6e64 da0c 7072 6f6a 6563 745f 7479 7065  nd..project_type
-00001c70: 4e29 0872 2f00 0000 7230 0000 0072 3100  N).r/...r0...r1.
-00001c80: 0000 7206 0000 00da 2370 726f 6a65 6374  ..r.....#project
-00001c90: 735f 6170 695f 6765 745f 7072 6f6a 6563  s_api_get_projec
-00001ca0: 745f 7479 7065 735f 6361 6c6c 7207 0000  t_types_callr...
-00001cb0: 00da 1141 5049 5f50 524f 4a45 4354 5f54  ...API_PROJECT_T
-00001cc0: 5950 4553 7223 0000 0072 0d00 0000 720d  YPESr#...r....r.
-00001cd0: 0000 0072 0d00 0000 720e 0000 0072 6c00  ...r....r....rl.
-00001ce0: 0000 ba00 0000 7306 0000 000c 0206 0106  ......s.........
-00001cf0: 0172 6c00 0000 6300 0000 0000 0000 0000  .rl...c.........
-00001d00: 0000 0003 0000 0000 0000 0073 3700 0000  ...........s7...
-00001d10: 6500 005a 0100 6400 005a 0200 6503 006a  e..Z..d..Z..e..j
-00001d20: 0400 6505 006a 0600 6401 0066 0300 5a07  ..e..j..d..f..Z.
-00001d30: 0087 0000 6601 0064 0200 6403 0086 0000  ....f..d..d.....
-00001d40: 5a08 0087 0000 5329 04da 1754 6573 7453  Z.....S)...TestS
-00001d50: 796e 6350 726f 6a65 6374 7343 6f6d 6d61  yncProjectsComma
-00001d60: 6e64 da07 7072 6f6a 6563 7463 0100 0000  nd..projectc....
-00001d70: 0000 0000 0100 0000 0100 0000 0300 0000  ................
-00001d80: 731b 0000 0074 0000 8300 006a 0100 8300  s....t.....j....
-00001d90: 0001 7402 006a 0300 8300 0001 6400 0053  ..t..j......d..S
-00001da0: 2901 4e29 0472 4800 0000 7238 0000 0072  ).N).rH...r8...r
-00001db0: 0800 0000 da15 696e 6974 5f70 726f 6a65  ......init_proje
-00001dc0: 6374 5f73 7461 7475 7365 7329 0172 1d00  ct_statuses).r..
-00001dd0: 0000 2901 724a 0000 0072 0d00 0000 720e  ..).rJ...r....r.
-00001de0: 0000 0072 3800 0000 c900 0000 7304 0000  ...r8.......s...
-00001df0: 0000 010d 017a 1d54 6573 7453 796e 6350  .....z.TestSyncP
-00001e00: 726f 6a65 6374 7343 6f6d 6d61 6e64 2e73  rojectsCommand.s
-00001e10: 6574 5570 2909 722f 0000 0072 3000 0000  etUp).r/...r0...
-00001e20: 7231 0000 0072 0600 0000 da1d 7072 6f6a  r1...r......proj
-00001e30: 6563 745f 6170 695f 6765 745f 7072 6f6a  ect_api_get_proj
-00001e40: 6563 7473 5f63 616c 6c72 0700 0000 da10  ects_callr......
-00001e50: 4150 495f 5052 4f4a 4543 545f 4c49 5354  API_PROJECT_LIST
-00001e60: 7223 0000 0072 3800 0000 720d 0000 0072  r#...r8...r....r
-00001e70: 0d00 0000 2901 724a 0000 0072 0e00 0000  ....).rJ...r....
-00001e80: 7270 0000 00c2 0000 0073 0800 0000 0c02  rp.......s......
-00001e90: 0601 0601 0903 7270 0000 0063 0000 0000  ......rp...c....
-00001ea0: 0000 0000 0000 0000 0300 0000 0000 0000  ................
-00001eb0: 7337 0000 0065 0000 5a01 0064 0000 5a02  s7...e..Z..d..Z.
-00001ec0: 0065 0300 6a04 0065 0500 6a06 0064 0100  .e..j..e..j..d..
-00001ed0: 6603 005a 0700 8700 0066 0100 6402 0064  f..Z.....f..d..d
-00001ee0: 0300 8600 005a 0800 8700 0053 2904 da1b  .....Z.....S)...
-00001ef0: 5465 7374 5379 6e63 5072 6f6a 6563 7450  TestSyncProjectP
-00001f00: 6861 7365 436f 6d6d 616e 64da 0d70 726f  haseCommand..pro
-00001f10: 6a65 6374 5f70 6861 7365 6301 0000 0000  ject_phasec.....
-00001f20: 0000 0001 0000 0001 0000 0003 0000 0073  ...............s
-00001f30: 2500 0000 7400 0083 0000 6a01 0083 0000  %...t.....j.....
-00001f40: 0174 0200 6a03 0083 0000 0174 0200 6a04  .t..j......t..j.
-00001f50: 0083 0000 0164 0000 5329 014e 2905 7248  .....d..S).N).rH
-00001f60: 0000 0072 3800 0000 7208 0000 00da 0d69  ...r8...r......i
-00001f70: 6e69 745f 7072 6f6a 6563 7473 5a13 696e  nit_projectsZ.in
-00001f80: 6974 5f70 726f 6a65 6374 5f70 6861 7365  it_project_phase
-00001f90: 7329 0172 1d00 0000 2901 724a 0000 0072  s).r....).rJ...r
-00001fa0: 0d00 0000 720e 0000 0072 3800 0000 d500  ....r....r8.....
-00001fb0: 0000 7306 0000 0000 010d 010a 017a 2154  ..s..........z!T
-00001fc0: 6573 7453 796e 6350 726f 6a65 6374 5068  estSyncProjectPh
-00001fd0: 6173 6543 6f6d 6d61 6e64 2e73 6574 5570  aseCommand.setUp
-00001fe0: 2909 722f 0000 0072 3000 0000 7231 0000  ).r/...r0...r1..
-00001ff0: 0072 0600 0000 da24 7072 6f6a 6563 7473  .r.....$projects
-00002000: 5f61 7069 5f67 6574 5f70 726f 6a65 6374  _api_get_project
-00002010: 5f70 6861 7365 735f 6361 6c6c 7207 0000  _phases_callr...
-00002020: 00da 1641 5049 5f50 524f 4a45 4354 5f50  ...API_PROJECT_P
-00002030: 4841 5345 5f4c 4953 5472 2300 0000 7238  HASE_LISTr#...r8
-00002040: 0000 0072 0d00 0000 720d 0000 0029 0172  ...r....r....).r
-00002050: 4a00 0000 720e 0000 0072 7500 0000 ce00  J...r....ru.....
-00002060: 0000 7308 0000 000c 0206 0106 0109 0372  ..s............r
-00002070: 7500 0000 6300 0000 0000 0000 0000 0000  u...c...........
-00002080: 0003 0000 0000 0000 0073 3700 0000 6500  .........s7...e.
-00002090: 005a 0100 6400 005a 0200 6503 006a 0400  .Z..d..Z..e..j..
-000020a0: 6505 006a 0600 6401 0066 0300 5a07 0087  e..j..d..f..Z...
-000020b0: 0000 6601 0064 0200 6403 0086 0000 5a08  ..f..d..d.....Z.
-000020c0: 0087 0000 5329 04da 2054 6573 7453 796e  ....S).. TestSyn
-000020d0: 6350 726f 6a65 6374 5465 616d 4d65 6d62  cProjectTeamMemb
-000020e0: 6572 436f 6d6d 616e 64da 1370 726f 6a65  erCommand..proje
-000020f0: 6374 5f74 6561 6d5f 6d65 6d62 6572 6301  ct_team_memberc.
-00002100: 0000 0000 0000 0001 0000 0003 0000 0003  ................
-00002110: 0000 0073 5f00 0000 7400 0083 0000 6a01  ...s_...t.....j.
-00002120: 0083 0000 0174 0200 6a03 0074 0200 6a04  .....t..j..t..j.
-00002130: 0074 0200 6a05 0083 0000 6602 0083 0100  .t..j.....f.....
-00002140: 0174 0600 6a07 0083 0000 0174 0600 6a08  .t..j......t..j.
-00002150: 0083 0000 0174 0600 6a09 0083 0000 0174  .....t..j......t
-00002160: 0600 6a0a 0083 0000 0174 0600 6a0b 0083  ..j......t..j...
-00002170: 0000 0164 0000 5329 014e 290c 7248 0000  ...d..S).N).rH..
-00002180: 0072 3800 0000 7206 0000 00da 2c73 7973  .r8...r.....,sys
-00002190: 7465 6d5f 6170 695f 6765 745f 6d65 6d62  tem_api_get_memb
-000021a0: 6572 5f69 6d61 6765 5f62 795f 7068 6f74  er_image_by_phot
-000021b0: 6f5f 6964 5f63 616c 6cda 1843 575f 4d45  o_id_call..CW_ME
-000021c0: 4d42 4552 5f49 4d41 4745 5f46 494c 454e  MBER_IMAGE_FILEN
-000021d0: 414d 45da 1167 6574 5f6d 656d 6265 725f  AME..get_member_
-000021e0: 6176 6174 6172 7208 0000 00da 0c69 6e69  avatarr......ini
-000021f0: 745f 6d65 6d62 6572 73da 0f69 6e69 745f  t_members..init_
-00002200: 776f 726b 5f72 6f6c 6573 7272 0000 0072  work_rolesrr...r
-00002210: 7700 0000 5a19 696e 6974 5f70 726f 6a65  w...Z.init_proje
-00002220: 6374 5f74 6561 6d5f 6d65 6d62 6572 7329  ct_team_members)
-00002230: 0172 1d00 0000 2901 724a 0000 0072 0d00  .r....).rJ...r..
-00002240: 0000 720e 0000 0072 3800 0000 e200 0000  ..r....r8.......
-00002250: 7310 0000 0000 010d 0106 0116 010a 010a  s...............
-00002260: 010a 010a 017a 2654 6573 7453 796e 6350  .....z&TestSyncP
-00002270: 726f 6a65 6374 5465 616d 4d65 6d62 6572  rojectTeamMember
-00002280: 436f 6d6d 616e 642e 7365 7455 7029 0972  Command.setUp).r
-00002290: 2f00 0000 7230 0000 0072 3100 0000 7206  /...r0...r1...r.
-000022a0: 0000 00da 2170 726f 6a65 6374 5f61 7069  ....!project_api
-000022b0: 5f67 6574 5f74 6561 6d5f 6d65 6d62 6572  _get_team_member
-000022c0: 735f 6361 6c6c 7207 0000 00da 1c41 5049  s_callr......API
-000022d0: 5f50 524f 4a45 4354 5f54 4541 4d5f 4d45  _PROJECT_TEAM_ME
-000022e0: 4d42 4552 5f4c 4953 5472 2300 0000 7238  MBER_LISTr#...r8
-000022f0: 0000 0072 0d00 0000 720d 0000 0029 0172  ...r....r....).r
-00002300: 4a00 0000 720e 0000 0072 7a00 0000 db00  J...r....rz.....
-00002310: 0000 7308 0000 000c 0206 0106 0109 0372  ..s............r
-00002320: 7a00 0000 6300 0000 0000 0000 0000 0000  z...c...........
-00002330: 0003 0000 0040 0000 0073 3100 0000 6500  .....@...s1...e.
-00002340: 005a 0100 6400 005a 0200 6503 006a 0400  .Z..d..Z..e..j..
-00002350: 6505 006a 0600 6401 0066 0300 5a07 0064  e..j..d..f..Z..d
-00002360: 0200 6403 0084 0000 5a08 0064 0400 5329  ..d.....Z..d..S)
-00002370: 05da 1d54 6573 7453 796e 6342 6f61 7264  ...TestSyncBoard
-00002380: 7353 7461 7475 7365 7343 6f6d 6d61 6e64  sStatusesCommand
-00002390: da0c 626f 6172 645f 7374 6174 7573 6301  ..board_statusc.
-000023a0: 0000 0000 0000 0004 0000 0002 0000 0043  ...............C
-000023b0: 0000 0073 5200 0000 7400 006a 0100 8300  ...sR...t..j....
-000023c0: 007d 0100 7402 006a 0300 6a04 006a 0500  .}..t..j..j..j..
-000023d0: 8300 006a 0600 8300 0001 7407 006a 0800  ...j......t..j..
-000023e0: 7409 006a 0a00 8301 005c 0200 7d02 007d  t..j.....\..}..}
-000023f0: 0300 7c01 006a 0000 8300 0001 7c03 006a  ..|..j......|..j
-00002400: 0b00 8300 0001 6400 0053 2901 4e29 0c72  ......d..S).N).r
-00002410: 0a00 0000 5a11 426f 6172 6453 796e 6368  ....Z.BoardSynch
-00002420: 726f 6e69 7a65 7272 0400 0000 da10 436f  ronizerr......Co
-00002430: 6e6e 6563 7457 6973 6542 6f61 7264 da07  nnectWiseBoard..
-00002440: 6f62 6a65 6374 73da 0361 6c6c da06 6465  objects..all..de
-00002450: 6c65 7465 7206 0000 0072 5900 0000 7207  leter....rY...r.
-00002460: 0000 0072 5a00 0000 da04 7374 6f70 2904  ...rZ.....stop).
-00002470: 721d 0000 005a 1262 6f61 7264 5f73 796e  r....Z.board_syn
-00002480: 6368 726f 6e69 7a65 7272 1100 0000 da06  chronizerr......
-00002490: 5f70 6174 6368 720d 0000 0072 0d00 0000  _patchr....r....
-000024a0: 720e 0000 0072 3800 0000 f400 0000 730a  r....r8.......s.
-000024b0: 0000 0000 010c 0116 0118 010a 017a 2354  .............z#T
-000024c0: 6573 7453 796e 6342 6f61 7264 7353 7461  estSyncBoardsSta
-000024d0: 7475 7365 7343 6f6d 6d61 6e64 2e73 6574  tusesCommand.set
-000024e0: 5570 4e29 0972 2f00 0000 7230 0000 0072  UpN).r/...r0...r
-000024f0: 3100 0000 7206 0000 00da 1d73 6572 7669  1...r......servi
-00002500: 6365 5f61 7069 5f67 6574 5f73 7461 7475  ce_api_get_statu
-00002510: 7365 735f 6361 6c6c 7207 0000 00da 1541  ses_callr......A
-00002520: 5049 5f42 4f41 5244 5f53 5441 5455 535f  PI_BOARD_STATUS_
-00002530: 4c49 5354 7223 0000 0072 3800 0000 720d  LISTr#...r8...r.
-00002540: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00002550: 0000 7283 0000 00ed 0000 0073 0800 0000  ..r........s....
-00002560: 0c02 0601 0601 0903 7283 0000 0063 0000  ........r....c..
-00002570: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00002580: 0000 7331 0000 0065 0000 5a01 0064 0000  ..s1...e..Z..d..
-00002590: 5a02 0065 0300 6a04 0065 0500 6a06 0064  Z..e..j..e..j..d
-000025a0: 0100 6603 005a 0700 6402 0064 0300 8400  ..f..Z..d..d....
-000025b0: 005a 0800 6404 0053 2905 da13 5465 7374  .Z..d..S)...Test
-000025c0: 5379 6e63 534c 4173 436f 6d6d 616e 64da  SyncSLAsCommand.
-000025d0: 0373 6c61 6301 0000 0000 0000 0001 0000  .slac...........
-000025e0: 0001 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
-000025f0: 006a 0100 8300 0001 6400 0053 2901 4e29  .j......d..S).N)
-00002600: 0272 0800 0000 7261 0000 0029 0172 1d00  .r....ra...).r..
-00002610: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-00002620: 0072 3800 0000 0301 0000 7302 0000 0000  .r8.......s.....
-00002630: 017a 1954 6573 7453 796e 6353 4c41 7343  .z.TestSyncSLAsC
-00002640: 6f6d 6d61 6e64 2e73 6574 5570 4e29 0972  ommand.setUpN).r
-00002650: 2f00 0000 7230 0000 0072 3100 0000 7206  /...r0...r1...r.
-00002660: 0000 00da 1973 6572 7669 6365 5f61 7069  .....service_api
-00002670: 5f67 6574 5f73 6c61 735f 6361 6c6c 7207  _get_slas_callr.
-00002680: 0000 00da 1441 5049 5f53 4552 5649 4345  .....API_SERVICE
-00002690: 5f53 4c41 5f4c 4953 5472 2300 0000 7238  _SLA_LISTr#...r8
-000026a0: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
-000026b0: 0000 720e 0000 0072 8d00 0000 fc00 0000  ..r....r........
-000026c0: 7308 0000 000c 0206 0106 0109 0372 8d00  s............r..
-000026d0: 0000 6300 0000 0000 0000 0000 0000 0003  ..c.............
-000026e0: 0000 0040 0000 0073 3100 0000 6500 005a  ...@...s1...e..Z
-000026f0: 0100 6400 005a 0200 6503 006a 0400 6505  ..d..Z..e..j..e.
-00002700: 006a 0600 6401 0066 0300 5a07 0064 0200  .j..d..f..Z..d..
-00002710: 6403 0084 0000 5a08 0064 0400 5329 05da  d.....Z..d..S)..
-00002720: 1c54 6573 7453 796e 6353 4c41 5072 696f  .TestSyncSLAPrio
-00002730: 7269 7469 6573 436f 6d6d 616e 64da 0c73  ritiesCommand..s
-00002740: 6c61 5f70 7269 6f72 6974 7963 0100 0000  la_priorityc....
-00002750: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00002760: 7322 0000 0074 0000 6a01 0083 0000 0174  s"...t..j......t
-00002770: 0000 6a02 0083 0000 0174 0000 6a03 0083  ..j......t..j...
-00002780: 0000 0164 0000 5329 014e 2904 7208 0000  ...d..S).N).r...
-00002790: 0072 6100 0000 5a09 696e 6974 5f73 6c61  .ra...Z.init_sla
-000027a0: 73da 0f69 6e69 745f 7072 696f 7269 7469  s..init_prioriti
-000027b0: 6573 2901 721d 0000 0072 0d00 0000 720d  es).r....r....r.
-000027c0: 0000 0072 0e00 0000 7238 0000 000e 0100  ...r....r8......
-000027d0: 0073 0600 0000 0001 0a01 0a01 7a22 5465  .s..........z"Te
-000027e0: 7374 5379 6e63 534c 4150 7269 6f72 6974  stSyncSLAPriorit
-000027f0: 6965 7343 6f6d 6d61 6e64 2e73 6574 5570  iesCommand.setUp
-00002800: 4e29 0972 2f00 0000 7230 0000 0072 3100  N).r/...r0...r1.
-00002810: 0000 7206 0000 00da 2373 6572 7669 6365  ..r.....#service
-00002820: 5f61 7069 5f67 6574 5f73 6c61 5f70 7269  _api_get_sla_pri
-00002830: 6f72 6974 6965 735f 6361 6c6c 7207 0000  orities_callr...
-00002840: 00da 1d41 5049 5f53 4552 5649 4345 5f53  ...API_SERVICE_S
-00002850: 4c41 5f50 5249 4f52 4954 595f 4c49 5354  LA_PRIORITY_LIST
-00002860: 7223 0000 0072 3800 0000 720d 0000 0072  r#...r8...r....r
-00002870: 0d00 0000 720d 0000 0072 0e00 0000 7291  ....r....r....r.
-00002880: 0000 0007 0100 0073 0800 0000 0c02 0601  .......s........
-00002890: 0601 0903 7291 0000 0063 0000 0000 0000  ....r....c......
-000028a0: 0000 0000 0000 0300 0000 0000 0000 7337  ..............s7
-000028b0: 0000 0065 0000 5a01 0064 0000 5a02 0065  ...e..Z..d..Z..e
-000028c0: 0300 6a04 0065 0500 6a06 0064 0100 6603  ..j..e..j..d..f.
-000028d0: 005a 0700 8700 0066 0100 6402 0064 0300  .Z.....f..d..d..
-000028e0: 8600 005a 0800 8700 0053 2904 da1b 5465  ...Z.....S)...Te
-000028f0: 7374 5379 6e63 5365 7276 6963 654e 6f74  stSyncServiceNot
-00002900: 6573 436f 6d6d 616e 64da 0c73 6572 7669  esCommand..servi
-00002910: 6365 5f6e 6f74 6563 0100 0000 0000 0000  ce_notec........
-00002920: 0100 0000 0100 0000 0300 0000 7357 0000  ............sW..
-00002930: 0074 0000 8300 006a 0100 8300 0001 7402  .t.....j......t.
-00002940: 006a 0300 8300 0001 7402 006a 0400 8300  .j......t..j....
-00002950: 0001 7402 006a 0500 8300 0001 7402 006a  ..t..j......t..j
-00002960: 0600 8300 0001 7402 006a 0700 8300 0001  ......t..j......
-00002970: 7402 006a 0800 8300 0001 7402 006a 0900  t..j......t..j..
-00002980: 8300 0001 6400 0053 2901 4e29 0a72 4800  ....d..S).N).rH.
-00002990: 0000 7238 0000 0072 0800 0000 5a12 696e  ..r8...r....Z.in
-000029a0: 6974 5f73 6572 7669 6365 5f6e 6f74 6573  it_service_notes
-000029b0: 727f 0000 0072 4900 0000 da0e 696e 6974  r....rI.....init
-000029c0: 5f63 6f6d 7061 6e69 6573 7254 0000 00da  _companiesrT....
-000029d0: 1369 6e69 745f 626f 6172 645f 7374 6174  .init_board_stat
-000029e0: 7573 6573 da0c 696e 6974 5f74 6963 6b65  uses..init_ticke
-000029f0: 7473 2901 721d 0000 0029 0172 4a00 0000  ts).r....).rJ...
-00002a00: 720d 0000 0072 0e00 0000 7238 0000 001b  r....r....r8....
-00002a10: 0100 0073 1000 0000 0001 0d01 0a01 0a01  ...s............
-00002a20: 0a01 0a01 0a01 0a01 7a21 5465 7374 5379  ........z!TestSy
-00002a30: 6e63 5365 7276 6963 654e 6f74 6573 436f  ncServiceNotesCo
-00002a40: 6d6d 616e 642e 7365 7455 7029 0972 2f00  mmand.setUp).r/.
-00002a50: 0000 7230 0000 0072 3100 0000 7206 0000  ..r0...r1...r...
-00002a60: 00da 1a73 6572 7669 6365 5f61 7069 5f67  ...service_api_g
-00002a70: 6574 5f6e 6f74 6573 5f63 616c 6c72 0700  et_notes_callr..
-00002a80: 0000 da15 4150 495f 5345 5256 4943 455f  ....API_SERVICE_
-00002a90: 4e4f 5445 5f4c 4953 5472 2300 0000 7238  NOTE_LISTr#...r8
-00002aa0: 0000 0072 0d00 0000 720d 0000 0029 0172  ...r....r....).r
-00002ab0: 4a00 0000 720e 0000 0072 9600 0000 1401  J...r....r......
-00002ac0: 0000 7308 0000 000c 0206 0106 0109 0372  ..s............r
-00002ad0: 9600 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00002ae0: 0003 0000 0000 0000 0073 3700 0000 6500  .........s7...e.
-00002af0: 005a 0100 6400 005a 0200 6503 006a 0400  .Z..d..Z..e..j..
-00002b00: 6505 006a 0600 6401 0066 0300 5a07 0087  e..j..d..f..Z...
-00002b10: 0000 6601 0064 0200 6403 0086 0000 5a08  ..f..d..d.....Z.
-00002b20: 0087 0000 5329 04da 1f54 6573 7453 796e  ....S)...TestSyn
-00002b30: 634f 7070 6f72 7475 6e69 7479 4e6f 7465  cOpportunityNote
-00002b40: 7343 6f6d 6d61 6e64 da10 6f70 706f 7274  sCommand..opport
-00002b50: 756e 6974 795f 6e6f 7465 6301 0000 0000  unity_notec.....
-00002b60: 0000 0001 0000 0001 0000 0003 0000 0073  ...............s
-00002b70: 4300 0000 7400 0083 0000 6a01 0083 0000  C...t.....j.....
-00002b80: 0174 0200 6a03 0083 0000 0174 0200 6a04  .t..j......t..j.
-00002b90: 0083 0000 0174 0200 6a05 0083 0000 0174  .....t..j......t
-00002ba0: 0200 6a06 0083 0000 0174 0200 6a07 0083  ..j......t..j...
-00002bb0: 0000 0164 0000 5329 014e 2908 7248 0000  ...d..S).N).rH..
-00002bc0: 0072 3800 0000 7208 0000 00da 1969 6e69  .r8...r......ini
-00002bd0: 745f 6f70 706f 7274 756e 6974 795f 7374  t_opportunity_st
-00002be0: 6174 7573 6573 da17 696e 6974 5f6f 7070  atuses..init_opp
-00002bf0: 6f72 7475 6e69 7479 5f73 7461 6765 73da  ortunity_stages.
-00002c00: 1669 6e69 745f 6f70 706f 7274 756e 6974  .init_opportunit
-00002c10: 795f 7479 7065 73da 1269 6e69 745f 6f70  y_types..init_op
-00002c20: 706f 7274 756e 6974 6965 735a 1669 6e69  portunitiesZ.ini
-00002c30: 745f 6f70 706f 7274 756e 6974 795f 6e6f  t_opportunity_no
-00002c40: 7465 7329 0172 1d00 0000 2901 724a 0000  tes).r....).rJ..
-00002c50: 0072 0d00 0000 720e 0000 0072 3800 0000  .r....r....r8...
-00002c60: 2d01 0000 730c 0000 0000 010d 010a 010a  -...s...........
-00002c70: 010a 010a 017a 2554 6573 7453 796e 634f  .....z%TestSyncO
-00002c80: 7070 6f72 7475 6e69 7479 4e6f 7465 7343  pportunityNotesC
-00002c90: 6f6d 6d61 6e64 2e73 6574 5570 2909 722f  ommand.setUp).r/
-00002ca0: 0000 0072 3000 0000 7231 0000 0072 0600  ...r0...r1...r..
-00002cb0: 0000 da24 7361 6c65 735f 6170 695f 6765  ...$sales_api_ge
-00002cc0: 745f 6f70 706f 7274 756e 6974 795f 6e6f  t_opportunity_no
-00002cd0: 7465 735f 6361 6c6c 7207 0000 00da 1f41  tes_callr......A
-00002ce0: 5049 5f53 414c 4553 5f4f 5050 4f52 5455  PI_SALES_OPPORTU
-00002cf0: 4e49 5459 5f4e 4f54 455f 4c49 5354 7223  NITY_NOTE_LISTr#
-00002d00: 0000 0072 3800 0000 720d 0000 0072 0d00  ...r8...r....r..
-00002d10: 0000 2901 724a 0000 0072 0e00 0000 729d  ..).rJ...r....r.
-00002d20: 0000 0026 0100 0073 0800 0000 0c02 0601  ...&...s........
-00002d30: 0601 0903 729d 0000 0063 0000 0000 0000  ....r....c......
-00002d40: 0000 0000 0000 0300 0000 0000 0000 733a  ..............s:
-00002d50: 0000 0065 0000 5a01 0064 0000 5a02 0065  ...e..Z..d..Z..e
-00002d60: 0300 6a04 0065 0500 6a06 0067 0100 6401  ..j..e..j..g..d.
-00002d70: 0066 0300 5a07 0087 0000 6601 0064 0200  .f..Z.....f..d..
-00002d80: 6403 0086 0000 5a08 0087 0000 5329 04da  d.....Z.....S)..
-00002d90: 1a54 6573 7453 796e 634f 7070 6f72 7475  .TestSyncOpportu
-00002da0: 6e69 7479 436f 6d6d 616e 64da 0b6f 7070  nityCommand..opp
-00002db0: 6f72 7475 6e69 7479 6301 0000 0000 0000  ortunityc.......
-00002dc0: 0001 0000 0001 0000 0003 0000 0073 4d00  .............sM.
-00002dd0: 0000 7400 0083 0000 6a01 0083 0000 0174  ..t.....j......t
-00002de0: 0200 6a03 0083 0000 0174 0200 6a04 0083  ..j......t..j...
-00002df0: 0000 0174 0200 6a05 0083 0000 0174 0200  ...t..j......t..
-00002e00: 6a06 0083 0000 0174 0200 6a07 0083 0000  j......t..j.....
-00002e10: 0174 0200 6a08 0083 0000 0164 0000 5329  .t..j......d..S)
-00002e20: 014e 2909 7248 0000 0072 3800 0000 7208  .N).rH...r8...r.
-00002e30: 0000 0072 4900 0000 7298 0000 0072 7f00  ...rI...r....r..
-00002e40: 0000 729f 0000 0072 a000 0000 72a1 0000  ..r....r....r...
-00002e50: 0029 0172 1d00 0000 2901 724a 0000 0072  .).r....).rJ...r
-00002e60: 0d00 0000 720e 0000 0072 3800 0000 3d01  ....r....r8...=.
-00002e70: 0000 730e 0000 0000 010d 010a 010a 010a  ..s.............
-00002e80: 010a 010a 017a 2054 6573 7453 796e 634f  .....z TestSyncO
-00002e90: 7070 6f72 7475 6e69 7479 436f 6d6d 616e  pportunityComman
-00002ea0: 642e 7365 7455 7029 0972 2f00 0000 7230  d.setUp).r/...r0
-00002eb0: 0000 0072 3100 0000 7206 0000 00da 2073  ...r1...r..... s
-00002ec0: 616c 6573 5f61 7069 5f67 6574 5f6f 7070  ales_api_get_opp
-00002ed0: 6f72 7475 6e69 7469 6573 5f63 616c 6c72  ortunities_callr
-00002ee0: 0700 0000 da15 4150 495f 5341 4c45 535f  ......API_SALES_
-00002ef0: 4f50 504f 5254 554e 4954 5972 2300 0000  OPPORTUNITYr#...
-00002f00: 7238 0000 0072 0d00 0000 720d 0000 0029  r8...r....r....)
-00002f10: 0172 4a00 0000 720e 0000 0072 a500 0000  .rJ...r....r....
-00002f20: 3601 0000 7308 0000 000c 0206 0109 0109  6...s...........
-00002f30: 0372 a500 0000 6300 0000 0000 0000 0000  .r....c.........
-00002f40: 0000 0003 0000 0040 0000 0073 2500 0000  .......@...s%...
-00002f50: 6500 005a 0100 6400 005a 0200 6503 006a  e..Z..d..Z..e..j
-00002f60: 0400 6505 006a 0600 6401 0066 0300 5a07  ..e..j..d..f..Z.
-00002f70: 0064 0200 5329 03da 2054 6573 7453 796e  .d..S).. TestSyn
-00002f80: 634f 7070 6f72 7475 6e69 7479 5374 6167  cOpportunityStag
-00002f90: 6573 436f 6d6d 616e 64da 116f 7070 6f72  esCommand..oppor
-00002fa0: 7475 6e69 7479 5f73 7461 6765 4e29 0872  tunity_stageN).r
-00002fb0: 2f00 0000 7230 0000 0072 3100 0000 7206  /...r0...r1...r.
-00002fc0: 0000 00da 2573 616c 6573 5f61 7069 5f67  ....%sales_api_g
-00002fd0: 6574 5f6f 7070 6f72 7475 6e69 7479 5f73  et_opportunity_s
-00002fe0: 7461 6765 735f 6361 6c6c 7207 0000 00da  tages_callr.....
-00002ff0: 1c41 5049 5f53 414c 4553 5f4f 5050 4f52  .API_SALES_OPPOR
-00003000: 5455 4e49 5459 5f53 5441 4745 5372 2300  TUNITY_STAGESr#.
-00003010: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00003020: 0072 0e00 0000 72a9 0000 0047 0100 0073  .r....r....G...s
-00003030: 0600 0000 0c02 0601 0601 72a9 0000 0063  ..........r....c
-00003040: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00003050: 4000 0000 7325 0000 0065 0000 5a01 0064  @...s%...e..Z..d
-00003060: 0000 5a02 0065 0300 6a04 0065 0500 6a06  ..Z..e..j..e..j.
-00003070: 0064 0100 6603 005a 0700 6402 0053 2903  .d..f..Z..d..S).
-00003080: da22 5465 7374 5379 6e63 4f70 706f 7274  ."TestSyncOpport
-00003090: 756e 6974 7953 7461 7475 7365 7343 6f6d  unityStatusesCom
-000030a0: 6d61 6e64 da12 6f70 706f 7274 756e 6974  mand..opportunit
-000030b0: 795f 7374 6174 7573 4e29 0872 2f00 0000  y_statusN).r/...
-000030c0: 7230 0000 0072 3100 0000 7206 0000 00da  r0...r1...r.....
-000030d0: 2773 616c 6573 5f61 7069 5f67 6574 5f6f  'sales_api_get_o
-000030e0: 7070 6f72 7475 6e69 7479 5f73 7461 7475  pportunity_statu
-000030f0: 7365 735f 6361 6c6c 7207 0000 00da 1e41  ses_callr......A
-00003100: 5049 5f53 414c 4553 5f4f 5050 4f52 5455  PI_SALES_OPPORTU
-00003110: 4e49 5459 5f53 5441 5455 5345 5372 2300  NITY_STATUSESr#.
-00003120: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00003130: 0072 0e00 0000 72ad 0000 004f 0100 0073  .r....r....O...s
-00003140: 0600 0000 0c02 0601 0601 72ad 0000 0063  ..........r....c
-00003150: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00003160: 4000 0000 7325 0000 0065 0000 5a01 0064  @...s%...e..Z..d
-00003170: 0000 5a02 0065 0300 6a04 0065 0500 6a06  ..Z..e..j..e..j.
-00003180: 0064 0100 6603 005a 0700 6402 0053 2903  .d..f..Z..d..S).
-00003190: da1f 5465 7374 5379 6e63 4f70 706f 7274  ..TestSyncOpport
-000031a0: 756e 6974 7954 7970 6573 436f 6d6d 616e  unityTypesComman
-000031b0: 64da 106f 7070 6f72 7475 6e69 7479 5f74  d..opportunity_t
-000031c0: 7970 654e 2908 722f 0000 0072 3000 0000  ypeN).r/...r0...
-000031d0: 7231 0000 0072 0600 0000 da24 7361 6c65  r1...r.....$sale
-000031e0: 735f 6170 695f 6765 745f 6f70 706f 7274  s_api_get_opport
-000031f0: 756e 6974 795f 7479 7065 735f 6361 6c6c  unity_types_call
-00003200: 7207 0000 00da 1b41 5049 5f53 414c 4553  r......API_SALES
-00003210: 5f4f 5050 4f52 5455 4e49 5459 5f54 5950  _OPPORTUNITY_TYP
-00003220: 4553 7223 0000 0072 0d00 0000 720d 0000  ESr#...r....r...
-00003230: 0072 0d00 0000 720e 0000 0072 b100 0000  .r....r....r....
-00003240: 5701 0000 7306 0000 000c 0206 0106 0172  W...s..........r
-00003250: b100 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00003260: 0003 0000 0040 0000 0073 2500 0000 6500  .....@...s%...e.
-00003270: 005a 0100 6400 005a 0200 6503 006a 0400  .Z..d..Z..e..j..
-00003280: 6505 006a 0600 6401 0066 0300 5a07 0064  e..j..d..f..Z..d
-00003290: 0200 5329 03da 2154 6573 7453 796e 6353  ..S)..!TestSyncS
-000032a0: 616c 6573 5072 6f62 6162 696c 6974 6965  alesProbabilitie
-000032b0: 7343 6f6d 6d61 6e64 da11 7361 6c65 735f  sCommand..sales_
-000032c0: 7072 6f62 6162 696c 6974 794e 2908 722f  probabilityN).r/
-000032d0: 0000 0072 3000 0000 7231 0000 0072 0600  ...r0...r1...r..
-000032e0: 0000 da26 7361 6c65 735f 6170 695f 6765  ...&sales_api_ge
-000032f0: 745f 7361 6c65 735f 7072 6f62 6162 696c  t_sales_probabil
-00003300: 6974 6965 735f 6361 6c6c 7207 0000 00da  ities_callr.....
-00003310: 1a41 5049 5f53 414c 4553 5f50 524f 4241  .API_SALES_PROBA
-00003320: 4249 4c49 5459 5f4c 4953 5472 2300 0000  BILITY_LISTr#...
-00003330: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00003340: 0e00 0000 72b5 0000 005f 0100 0073 0600  ....r...._...s..
-00003350: 0000 0c02 0601 0601 72b5 0000 0063 0000  ........r....c..
-00003360: 0000 0000 0000 0000 0000 0300 0000 0000  ................
-00003370: 0000 7337 0000 0065 0000 5a01 0064 0000  ..s7...e..Z..d..
-00003380: 5a02 0065 0300 6a04 0065 0500 6a06 0064  Z..e..j..e..j..d
-00003390: 0100 6603 005a 0700 8700 0066 0100 6402  ..f..Z.....f..d.
-000033a0: 0064 0300 8600 005a 0800 8700 0053 2904  .d.....Z.....S).
-000033b0: da1a 5465 7374 5379 6e63 5469 6d65 456e  ..TestSyncTimeEn
-000033c0: 7472 6965 7343 6f6d 6d61 6e64 da0a 7469  triesCommand..ti
-000033d0: 6d65 5f65 6e74 7279 6301 0000 0000 0000  me_entryc.......
-000033e0: 0001 0000 0001 0000 0003 0000 0073 4d00  .............sM.
-000033f0: 0000 7400 0083 0000 6a01 0083 0000 0174  ..t.....j......t
-00003400: 0200 6a03 0083 0000 0174 0200 6a04 0083  ..j......t..j...
-00003410: 0000 0174 0200 6a05 0083 0000 0174 0200  ...t..j......t..
-00003420: 6a06 0083 0000 0174 0200 6a07 0083 0000  j......t..j.....
-00003430: 0174 0200 6a08 0083 0000 0164 0000 5329  .t..j......d..S)
-00003440: 014e 2909 7248 0000 0072 3800 0000 7208  .N).rH...r8...r.
-00003450: 0000 0072 5400 0000 7299 0000 0072 9a00  ...rT...r....r..
-00003460: 0000 7249 0000 0072 9800 0000 727f 0000  ..rI...r....r...
-00003470: 0029 0172 1d00 0000 2901 724a 0000 0072  .).r....).rJ...r
-00003480: 0d00 0000 720e 0000 0072 3800 0000 6e01  ....r....r8...n.
-00003490: 0000 730e 0000 0000 010d 010a 010a 010a  ..s.............
-000034a0: 010a 010a 017a 2054 6573 7453 796e 6354  .....z TestSyncT
-000034b0: 696d 6545 6e74 7269 6573 436f 6d6d 616e  imeEntriesComman
-000034c0: 642e 7365 7455 7029 0972 2f00 0000 7230  d.setUp).r/...r0
-000034d0: 0000 0072 3100 0000 7206 0000 00da 1e74  ...r1...r......t
-000034e0: 696d 655f 6170 695f 6765 745f 7469 6d65  ime_api_get_time
-000034f0: 5f65 6e74 7269 6573 5f63 616c 6c72 0700  _entries_callr..
-00003500: 0000 da13 4150 495f 5449 4d45 5f45 4e54  ....API_TIME_ENT
-00003510: 5259 5f4c 4953 5472 2300 0000 7238 0000  RY_LISTr#...r8..
-00003520: 0072 0d00 0000 720d 0000 0029 0172 4a00  .r....r....).rJ.
-00003530: 0000 720e 0000 0072 b900 0000 6701 0000  ..r....r....g...
-00003540: 7308 0000 000c 0206 0106 0109 0372 b900  s............r..
-00003550: 0000 6300 0000 0000 0000 0000 0000 0003  ..c.............
-00003560: 0000 0000 0000 0073 3700 0000 6500 005a  .......s7...e..Z
-00003570: 0100 6400 005a 0200 6503 006a 0400 6505  ..d..Z..e..j..e.
-00003580: 006a 0600 6401 0066 0300 5a07 0087 0000  .j..d..f..Z.....
-00003590: 6601 0064 0200 6403 0086 0000 5a08 0087  f..d..d.....Z...
-000035a0: 0000 5329 04da 1e54 6573 7453 796e 6353  ..S)...TestSyncS
-000035b0: 6368 6564 756c 6545 6e74 7269 6573 436f  cheduleEntriesCo
-000035c0: 6d6d 616e 64da 0e73 6368 6564 756c 655f  mmand..schedule_
-000035d0: 656e 7472 7963 0100 0000 0000 0000 0100  entryc..........
-000035e0: 0000 0100 0000 0300 0000 7389 0000 0074  ..........s....t
-000035f0: 0000 8300 006a 0100 8300 0001 7402 006a  .....j......t..j
-00003600: 0300 8300 0001 7402 006a 0400 8300 0001  ......t..j......
-00003610: 7402 006a 0500 8300 0001 7402 006a 0600  t..j......t..j..
-00003620: 8300 0001 7402 006a 0700 8300 0001 7402  ....t..j......t.
-00003630: 006a 0800 8300 0001 7402 006a 0900 8300  .j......t..j....
-00003640: 0001 7402 006a 0a00 8300 0001 7402 006a  ..t..j......t..j
-00003650: 0b00 8300 0001 7402 006a 0c00 8300 0001  ......t..j......
-00003660: 7402 006a 0d00 8300 0001 7402 006a 0e00  t..j......t..j..
-00003670: 8300 0001 6400 0053 2901 4e29 0f72 4800  ....d..S).N).rH.
-00003680: 0000 7238 0000 0072 0800 0000 7254 0000  ..r8...r....rT..
-00003690: 0072 9900 0000 7249 0000 0072 9800 0000  .r....rI...r....
-000036a0: 5a0e 696e 6974 5f6c 6f63 6174 696f 6e73  Z.init_locations
-000036b0: da0a 696e 6974 5f74 6561 6d73 727f 0000  ..init_teamsr...
-000036c0: 0072 9300 0000 7277 0000 005a 1369 6e69  .r....rw...Z.ini
-000036d0: 745f 7363 6865 6475 6c65 5f74 7970 6573  t_schedule_types
-000036e0: 5a16 696e 6974 5f73 6368 6564 756c 655f  Z.init_schedule_
-000036f0: 7374 6174 7573 6573 729a 0000 0029 0172  statusesr....).r
-00003700: 1d00 0000 2901 724a 0000 0072 0d00 0000  ....).rJ...r....
-00003710: 720e 0000 0072 3800 0000 7f01 0000 731a  r....r8.......s.
-00003720: 0000 0000 010d 010a 010a 010a 010a 010a  ................
-00003730: 010a 010a 010a 010a 010a 010a 017a 2454  .............z$T
-00003740: 6573 7453 796e 6353 6368 6564 756c 6545  estSyncScheduleE
-00003750: 6e74 7269 6573 436f 6d6d 616e 642e 7365  ntriesCommand.se
-00003760: 7455 7029 0972 2f00 0000 7230 0000 0072  tUp).r/...r0...r
-00003770: 3100 0000 7206 0000 00da 2673 6368 6564  1...r.....&sched
-00003780: 756c 655f 6170 695f 6765 745f 7363 6865  ule_api_get_sche
-00003790: 6475 6c65 5f65 6e74 7269 6573 5f63 616c  dule_entries_cal
-000037a0: 6c72 0700 0000 da14 4150 495f 5343 4845  lr......API_SCHE
-000037b0: 4455 4c45 5f45 4e54 5249 4553 7223 0000  DULE_ENTRIESr#..
-000037c0: 0072 3800 0000 720d 0000 0072 0d00 0000  .r8...r....r....
-000037d0: 2901 724a 0000 0072 0e00 0000 72bd 0000  ).rJ...r....r...
-000037e0: 0078 0100 0073 0800 0000 0c02 0601 0601  .x...s..........
-000037f0: 0903 72bd 0000 0063 0000 0000 0000 0000  ..r....c........
-00003800: 0000 0000 0300 0000 4000 0000 7325 0000  ........@...s%..
-00003810: 0065 0000 5a01 0064 0000 5a02 0065 0300  .e..Z..d..Z..e..
-00003820: 6a04 0065 0500 6a06 0064 0100 6603 005a  j..e..j..d..f..Z
-00003830: 0700 6402 0053 2903 da1c 5465 7374 5379  ..d..S)...TestSy
-00003840: 6e63 5363 6865 6475 6c65 5479 7065 7343  ncScheduleTypesC
-00003850: 6f6d 6d61 6e64 da0d 7363 6865 6475 6c65  ommand..schedule
-00003860: 5f74 7970 654e 2908 722f 0000 0072 3000  _typeN).r/...r0.
-00003870: 0000 7231 0000 0072 0600 0000 da24 7363  ..r1...r.....$sc
-00003880: 6865 6475 6c65 5f61 7069 5f67 6574 5f73  hedule_api_get_s
-00003890: 6368 6564 756c 655f 7479 7065 735f 6361  chedule_types_ca
-000038a0: 6c6c 7207 0000 00da 1641 5049 5f53 4348  llr......API_SCH
-000038b0: 4544 554c 455f 5459 5045 5f4c 4953 5472  EDULE_TYPE_LISTr
-000038c0: 2300 0000 720d 0000 0072 0d00 0000 720d  #...r....r....r.
-000038d0: 0000 0072 0e00 0000 72c2 0000 008f 0100  ...r....r.......
-000038e0: 0073 0600 0000 0c02 0601 0601 72c2 0000  .s..........r...
-000038f0: 0063 0000 0000 0000 0000 0000 0000 0300  .c..............
-00003900: 0000 4000 0000 7325 0000 0065 0000 5a01  ..@...s%...e..Z.
-00003910: 0064 0000 5a02 0065 0300 6a04 0065 0500  .d..Z..e..j..e..
-00003920: 6a06 0064 0100 6603 005a 0700 6402 0053  j..d..f..Z..d..S
-00003930: 2903 da1f 5465 7374 5379 6e63 5363 6865  )...TestSyncSche
-00003940: 6475 6c65 5374 6174 7573 6573 436f 6d6d  duleStatusesComm
-00003950: 616e 64da 0f73 6368 6564 756c 655f 7374  and..schedule_st
-00003960: 6174 7573 4e29 0872 2f00 0000 7230 0000  atusN).r/...r0..
-00003970: 0072 3100 0000 7206 0000 00da 2773 6368  .r1...r.....'sch
-00003980: 6564 756c 655f 6170 695f 6765 745f 7363  edule_api_get_sc
-00003990: 6865 6475 6c65 5f73 7461 7475 7365 735f  hedule_statuses_
-000039a0: 6361 6c6c 7207 0000 00da 1841 5049 5f53  callr......API_S
-000039b0: 4348 4544 554c 455f 5354 4154 5553 5f4c  CHEDULE_STATUS_L
-000039c0: 4953 5472 2300 0000 720d 0000 0072 0d00  ISTr#...r....r..
-000039d0: 0000 720d 0000 0072 0e00 0000 72c6 0000  ..r....r....r...
-000039e0: 0097 0100 0073 0600 0000 0c02 0601 0601  .....s..........
-000039f0: 72c6 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00003a00: 0000 0300 0000 4000 0000 7325 0000 0065  ......@...s%...e
-00003a10: 0000 5a01 0064 0000 5a02 0065 0300 6a04  ..Z..d..Z..e..j.
-00003a20: 0065 0500 6a06 0064 0100 6603 005a 0700  .e..j..d..f..Z..
-00003a30: 6402 0053 2903 da1f 5465 7374 5379 6e63  d..S)...TestSync
-00003a40: 4163 7469 7669 7479 5374 6174 7573 6573  ActivityStatuses
-00003a50: 436f 6d6d 616e 64da 0f61 6374 6976 6974  Command..activit
-00003a60: 795f 7374 6174 7573 4e29 0872 2f00 0000  y_statusN).r/...
-00003a70: 7230 0000 0072 3100 0000 7206 0000 00da  r0...r1...r.....
-00003a80: 2673 616c 6573 5f61 7069 5f67 6574 5f61  &sales_api_get_a
-00003a90: 6374 6976 6974 6965 735f 7374 6174 7573  ctivities_status
-00003aa0: 6573 5f63 616c 6c72 0700 0000 da1b 4150  es_callr......AP
-00003ab0: 495f 5341 4c45 535f 4143 5449 5649 5459  I_SALES_ACTIVITY
-00003ac0: 5f53 5441 5455 5345 5372 2300 0000 720d  _STATUSESr#...r.
-00003ad0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00003ae0: 0000 72ca 0000 009f 0100 0073 0600 0000  ..r........s....
-00003af0: 0c02 0601 0601 72ca 0000 0063 0000 0000  ......r....c....
-00003b00: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00003b10: 7325 0000 0065 0000 5a01 0064 0000 5a02  s%...e..Z..d..Z.
-00003b20: 0065 0300 6a04 0065 0500 6a06 0064 0100  .e..j..e..j..d..
-00003b30: 6603 005a 0700 6402 0053 2903 da1c 5465  f..Z..d..S)...Te
-00003b40: 7374 5379 6e63 4163 7469 7669 7479 5479  stSyncActivityTy
-00003b50: 7065 7343 6f6d 6d61 6e64 da0d 6163 7469  pesCommand..acti
-00003b60: 7669 7479 5f74 7970 654e 2908 722f 0000  vity_typeN).r/..
-00003b70: 0072 3000 0000 7231 0000 0072 0600 0000  .r0...r1...r....
-00003b80: da23 7361 6c65 735f 6170 695f 6765 745f  .#sales_api_get_
-00003b90: 6163 7469 7669 7469 6573 5f74 7970 6573  activities_types
-00003ba0: 5f63 616c 6c72 0700 0000 da18 4150 495f  _callr......API_
-00003bb0: 5341 4c45 535f 4143 5449 5649 5459 5f54  SALES_ACTIVITY_T
-00003bc0: 5950 4553 7223 0000 0072 0d00 0000 720d  YPESr#...r....r.
-00003bd0: 0000 0072 0d00 0000 720e 0000 0072 ce00  ...r....r....r..
-00003be0: 0000 a701 0000 7306 0000 000c 0206 0106  ......s.........
-00003bf0: 0172 ce00 0000 6300 0000 0000 0000 0000  .r....c.........
-00003c00: 0000 0003 0000 0000 0000 0073 3700 0000  ...........s7...
-00003c10: 6500 005a 0100 6400 005a 0200 6503 006a  e..Z..d..Z..e..j
-00003c20: 0400 6505 006a 0600 6401 0066 0300 5a07  ..e..j..d..f..Z.
-00003c30: 0087 0000 6601 0064 0200 6403 0086 0000  ....f..d..d.....
-00003c40: 5a08 0087 0000 5329 04da 1754 6573 7453  Z.....S)...TestS
-00003c50: 796e 6341 6374 6976 6974 7943 6f6d 6d61  yncActivityComma
-00003c60: 6e64 da08 6163 7469 7669 7479 6301 0000  nd..activityc...
-00003c70: 0000 0000 0001 0000 0003 0000 0003 0000  ................
-00003c80: 0073 8700 0000 7400 0083 0000 6a01 0083  .s....t.....j...
-00003c90: 0000 0174 0200 6a03 0083 0000 0174 0200  ...t..j......t..
-00003ca0: 6a04 0083 0000 0174 0500 6a06 0074 0500  j......t..j..t..
-00003cb0: 6a07 0074 0500 6a08 0083 0000 6602 0083  j..t..j.....f...
-00003cc0: 0100 0174 0200 6a09 0083 0000 0174 0200  ...t..j......t..
-00003cd0: 6a0a 0083 0000 0174 0200 6a0b 0083 0000  j......t..j.....
-00003ce0: 0174 0200 6a0c 0083 0000 0174 0200 6a0d  .t..j......t..j.
-00003cf0: 0083 0000 0174 0200 6a0e 0083 0000 0174  .....t..j......t
-00003d00: 0200 6a0f 0083 0000 0164 0000 5329 014e  ..j......d..S).N
-00003d10: 2910 7248 0000 0072 3800 0000 7208 0000  ).rH...r8...r...
-00003d20: 0072 4900 0000 7298 0000 0072 0600 0000  .rI...r....r....
-00003d30: 727c 0000 0072 7d00 0000 727e 0000 0072  r|...r}...r~...r
-00003d40: 7f00 0000 729f 0000 0072 a100 0000 72a2  ....r....r....r.
-00003d50: 0000 0072 9a00 0000 7299 0000 005a 0f69  ...r....r....Z.i
-00003d60: 6e69 745f 6163 7469 7669 7469 6573 2901  nit_activities).
-00003d70: 721d 0000 0029 0172 4a00 0000 720d 0000  r....).rJ...r...
-00003d80: 0072 0e00 0000 7238 0000 00b6 0100 0073  .r....r8.......s
-00003d90: 1800 0000 0001 0d01 0a01 0a01 0601 1601  ................
-00003da0: 0a01 0a01 0a01 0a01 0a01 0a01 7a1d 5465  ............z.Te
-00003db0: 7374 5379 6e63 4163 7469 7669 7479 436f  stSyncActivityCo
-00003dc0: 6d6d 616e 642e 7365 7455 7029 0972 2f00  mmand.setUp).r/.
-00003dd0: 0000 7230 0000 0072 3100 0000 7206 0000  ..r0...r1...r...
-00003de0: 00da 1d73 616c 6573 5f61 7069 5f67 6574  ...sales_api_get
-00003df0: 5f61 6374 6976 6974 6965 735f 6361 6c6c  _activities_call
-00003e00: 7207 0000 00da 1441 5049 5f53 414c 4553  r......API_SALES
-00003e10: 5f41 4354 4956 4954 4945 5372 2300 0000  _ACTIVITIESr#...
-00003e20: 7238 0000 0072 0d00 0000 720d 0000 0029  r8...r....r....)
-00003e30: 0172 4a00 0000 720e 0000 0072 d200 0000  .rJ...r....r....
-00003e40: af01 0000 7308 0000 000c 0206 0106 0109  ....s...........
-00003e50: 0372 d200 0000 6300 0000 0000 0000 0000  .r....c.........
-00003e60: 0000 0003 0000 0000 0000 0073 3700 0000  ...........s7...
-00003e70: 6500 005a 0100 6400 005a 0200 8700 0066  e..Z..d..Z.....f
-00003e80: 0100 6401 0064 0200 8600 005a 0300 6504  ..d..d.....Z..e.
-00003e90: 006a 0500 6506 006a 0700 6403 0066 0300  .j..e..j..d..f..
-00003ea0: 5a08 0087 0000 5329 04da 1354 6573 7453  Z.....S)...TestS
-00003eb0: 796e 6354 7970 6543 6f6d 6d61 6e64 6301  yncTypeCommandc.
-00003ec0: 0000 0000 0000 0001 0000 0001 0000 0003  ................
-00003ed0: 0000 0073 2500 0000 7400 0083 0000 6a01  ...s%...t.....j.
-00003ee0: 0083 0000 0174 0200 6a03 0083 0000 0174  .....t..j......t
-00003ef0: 0200 6a04 0083 0000 0164 0000 5329 014e  ..j......d..S).N
-00003f00: 2905 7248 0000 0072 3800 0000 7208 0000  ).rH...r8...r...
-00003f10: 00da 0a69 6e69 745f 7479 7065 7372 5400  ...init_typesrT.
-00003f20: 0000 2901 721d 0000 0029 0172 4a00 0000  ..).r....).rJ...
-00003f30: 720d 0000 0072 0e00 0000 7238 0000 00c7  r....r....r8....
-00003f40: 0100 0073 0600 0000 0001 0d01 0a01 7a19  ...s..........z.
-00003f50: 5465 7374 5379 6e63 5479 7065 436f 6d6d  TestSyncTypeComm
-00003f60: 616e 642e 7365 7455 70da 0474 7970 6529  and.setUp..type)
-00003f70: 0972 2f00 0000 7230 0000 0072 3100 0000  .r/...r0...r1...
-00003f80: 7238 0000 0072 0600 0000 da1a 7365 7276  r8...r......serv
-00003f90: 6963 655f 6170 695f 6765 745f 7479 7065  ice_api_get_type
-00003fa0: 735f 6361 6c6c 7207 0000 00da 0d41 5049  s_callr......API
-00003fb0: 5f54 5950 455f 4c49 5354 7223 0000 0072  _TYPE_LISTr#...r
-00003fc0: 0d00 0000 720d 0000 0029 0172 4a00 0000  ....r....).rJ...
-00003fd0: 720e 0000 0072 d600 0000 c501 0000 7308  r....r........s.
-00003fe0: 0000 000c 0212 0606 0106 0172 d600 0000  ...........r....
-00003ff0: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
-00004000: 0000 0000 0073 3700 0000 6500 005a 0100  .....s7...e..Z..
-00004010: 6400 005a 0200 8700 0066 0100 6401 0064  d..Z.....f..d..d
-00004020: 0200 8600 005a 0300 6504 006a 0500 6506  .....Z..e..j..e.
-00004030: 006a 0700 6403 0066 0300 5a08 0087 0000  .j..d..f..Z.....
-00004040: 5329 04da 1654 6573 7453 796e 6353 7562  S)...TestSyncSub
-00004050: 5479 7065 436f 6d6d 616e 6463 0100 0000  TypeCommandc....
-00004060: 0000 0000 0100 0000 0100 0000 0300 0000  ................
-00004070: 7325 0000 0074 0000 8300 006a 0100 8300  s%...t.....j....
-00004080: 0001 7402 006a 0300 8300 0001 7402 006a  ..t..j......t..j
-00004090: 0400 8300 0001 6400 0053 2901 4e29 0572  ......d..S).N).r
-000040a0: 4800 0000 7238 0000 0072 0800 0000 72d7  H...r8...r....r.
-000040b0: 0000 0072 5400 0000 2901 721d 0000 0029  ...rT...).r....)
-000040c0: 0172 4a00 0000 720d 0000 0072 0e00 0000  .rJ...r....r....
-000040d0: 7238 0000 00d4 0100 0073 0600 0000 0001  r8.......s......
-000040e0: 0d01 0a01 7a1c 5465 7374 5379 6e63 5375  ....z.TestSyncSu
-000040f0: 6254 7970 6543 6f6d 6d61 6e64 2e73 6574  bTypeCommand.set
-00004100: 5570 da08 7375 625f 7479 7065 2909 722f  Up..sub_type).r/
-00004110: 0000 0072 3000 0000 7231 0000 0072 3800  ...r0...r1...r8.
-00004120: 0000 7206 0000 00da 1d73 6572 7669 6365  ..r......service
-00004130: 5f61 7069 5f67 6574 5f73 7562 7479 7065  _api_get_subtype
-00004140: 735f 6361 6c6c 7207 0000 00da 1041 5049  s_callr......API
-00004150: 5f53 5542 5459 5045 5f4c 4953 5472 2300  _SUBTYPE_LISTr#.
-00004160: 0000 720d 0000 0072 0d00 0000 2901 724a  ..r....r....).rJ
-00004170: 0000 0072 0e00 0000 72db 0000 00d3 0100  ...r....r.......
-00004180: 0073 0800 0000 0c01 1206 0601 0601 72db  .s............r.
-00004190: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000041a0: 0300 0000 0000 0000 7337 0000 0065 0000  ........s7...e..
-000041b0: 5a01 0064 0000 5a02 0087 0000 6601 0064  Z..d..Z.....f..d
-000041c0: 0100 6402 0086 0000 5a03 0065 0400 6a05  ..d.....Z..e..j.
-000041d0: 0065 0600 6a07 0064 0300 6603 005a 0800  .e..j..d..f..Z..
-000041e0: 8700 0053 2904 da13 5465 7374 5379 6e63  ...S)...TestSync
-000041f0: 4974 656d 436f 6d6d 616e 6463 0100 0000  ItemCommandc....
-00004200: 0000 0000 0100 0000 0100 0000 0300 0000  ................
-00004210: 7325 0000 0074 0000 8300 006a 0100 8300  s%...t.....j....
-00004220: 0001 7402 006a 0300 8300 0001 7402 006a  ..t..j......t..j
-00004230: 0400 8300 0001 6400 0053 2901 4e29 0572  ......d..S).N).r
-00004240: 4800 0000 7238 0000 0072 0800 0000 72d7  H...r8...r....r.
-00004250: 0000 0072 5400 0000 2901 721d 0000 0029  ...rT...).r....)
-00004260: 0172 4a00 0000 720d 0000 0072 0e00 0000  .rJ...r....r....
-00004270: 7238 0000 00e1 0100 0073 0600 0000 0001  r8.......s......
-00004280: 0d01 0a01 7a19 5465 7374 5379 6e63 4974  ....z.TestSyncIt
-00004290: 656d 436f 6d6d 616e 642e 7365 7455 70da  emCommand.setUp.
-000042a0: 0469 7465 6d29 0972 2f00 0000 7230 0000  .item).r/...r0..
-000042b0: 0072 3100 0000 7238 0000 0072 0600 0000  .r1...r8...r....
-000042c0: da1a 7365 7276 6963 655f 6170 695f 6765  ..service_api_ge
-000042d0: 745f 6974 656d 735f 6361 6c6c 7207 0000  t_items_callr...
-000042e0: 00da 0d41 5049 5f49 5445 4d5f 4c49 5354  ...API_ITEM_LIST
-000042f0: 7223 0000 0072 0d00 0000 720d 0000 0029  r#...r....r....)
-00004300: 0172 4a00 0000 720e 0000 0072 df00 0000  .rJ...r....r....
-00004310: e001 0000 7308 0000 000c 0112 0606 0106  ....s...........
-00004320: 0172 df00 0000 6300 0000 0000 0000 0000  .r....c.........
-00004330: 0000 0003 0000 0000 0000 0073 3700 0000  ...........s7...
-00004340: 6500 005a 0100 6400 005a 0200 8700 0066  e..Z..d..Z.....f
-00004350: 0100 6401 0064 0200 8600 005a 0300 6504  ..d..d.....Z..e.
-00004360: 006a 0500 6506 006a 0700 6403 0066 0300  .j..e..j..d..f..
-00004370: 5a08 0087 0000 5329 04da 1754 6573 7453  Z.....S)...TestS
-00004380: 796e 6357 6f72 6b54 7970 6543 6f6d 6d61  yncWorkTypeComma
-00004390: 6e64 6301 0000 0000 0000 0001 0000 0001  ndc.............
-000043a0: 0000 0003 0000 0073 1b00 0000 7400 0083  .......s....t...
-000043b0: 0000 6a01 0083 0000 0174 0200 6a03 0083  ..j......t..j...
-000043c0: 0000 0164 0000 5329 014e 2904 7248 0000  ...d..S).N).rH..
-000043d0: 0072 3800 0000 7208 0000 005a 0f69 6e69  .r8...r....Z.ini
-000043e0: 745f 776f 726b 5f74 7970 6573 2901 721d  t_work_types).r.
-000043f0: 0000 0029 0172 4a00 0000 720d 0000 0072  ...).rJ...r....r
-00004400: 0e00 0000 7238 0000 00ee 0100 0073 0400  ....r8.......s..
-00004410: 0000 0001 0d01 7a1d 5465 7374 5379 6e63  ......z.TestSync
-00004420: 576f 726b 5479 7065 436f 6d6d 616e 642e  WorkTypeCommand.
-00004430: 7365 7455 70da 0977 6f72 6b5f 7479 7065  setUp..work_type
-00004440: 2909 722f 0000 0072 3000 0000 7231 0000  ).r/...r0...r1..
-00004450: 0072 3800 0000 7206 0000 00da 1c74 696d  .r8...r......tim
-00004460: 655f 6170 695f 6765 745f 776f 726b 5f74  e_api_get_work_t
-00004470: 7970 6573 5f63 616c 6c72 0700 0000 da12  ypes_callr......
-00004480: 4150 495f 574f 524b 5f54 5950 455f 4c49  API_WORK_TYPE_LI
-00004490: 5354 7223 0000 0072 0d00 0000 720d 0000  STr#...r....r...
-000044a0: 0029 0172 4a00 0000 720e 0000 0072 e300  .).rJ...r....r..
-000044b0: 0000 ed01 0000 7308 0000 000c 0112 0506  ......s.........
-000044c0: 0106 0172 e300 0000 6300 0000 0000 0000  ...r....c.......
-000044d0: 0000 0000 0003 0000 0000 0000 0073 3700  .............s7.
-000044e0: 0000 6500 005a 0100 6400 005a 0200 8700  ..e..Z..d..Z....
-000044f0: 0066 0100 6401 0064 0200 8600 005a 0300  .f..d..d.....Z..
-00004500: 6504 006a 0500 6506 006a 0700 6403 0066  e..j..e..j..d..f
-00004510: 0300 5a08 0087 0000 5329 04da 1754 6573  ..Z.....S)...Tes
-00004520: 7453 796e 6357 6f72 6b52 6f6c 6543 6f6d  tSyncWorkRoleCom
-00004530: 6d61 6e64 6301 0000 0000 0000 0001 0000  mandc...........
-00004540: 0001 0000 0003 0000 0073 1b00 0000 7400  .........s....t.
-00004550: 0083 0000 6a01 0083 0000 0174 0200 6a03  ....j......t..j.
-00004560: 0083 0000 0164 0000 5329 014e 2904 7248  .....d..S).N).rH
-00004570: 0000 0072 3800 0000 7208 0000 0072 8000  ...r8...r....r..
-00004580: 0000 2901 721d 0000 0029 0172 4a00 0000  ..).r....).rJ...
-00004590: 720d 0000 0072 0e00 0000 7238 0000 00fa  r....r....r8....
-000045a0: 0100 0073 0400 0000 0001 0d01 7a1d 5465  ...s........z.Te
-000045b0: 7374 5379 6e63 576f 726b 526f 6c65 436f  stSyncWorkRoleCo
-000045c0: 6d6d 616e 642e 7365 7455 70da 0977 6f72  mmand.setUp..wor
-000045d0: 6b5f 726f 6c65 2909 722f 0000 0072 3000  k_role).r/...r0.
-000045e0: 0000 7231 0000 0072 3800 0000 7206 0000  ..r1...r8...r...
-000045f0: 00da 1c74 696d 655f 6170 695f 6765 745f  ...time_api_get_
-00004600: 776f 726b 5f72 6f6c 6573 5f63 616c 6c72  work_roles_callr
-00004610: 0700 0000 da12 4150 495f 574f 524b 5f52  ......API_WORK_R
-00004620: 4f4c 455f 4c49 5354 7223 0000 0072 0d00  OLE_LISTr#...r..
-00004630: 0000 720d 0000 0029 0172 4a00 0000 720e  ..r....).rJ...r.
-00004640: 0000 0072 e700 0000 f901 0000 7308 0000  ...r........s...
-00004650: 000c 0112 0506 0106 0172 e700 0000 6300  .........r....c.
-00004660: 0000 0000 0000 0000 0000 0003 0000 0000  ................
-00004670: 0000 0073 3700 0000 6500 005a 0100 6400  ...s7...e..Z..d.
-00004680: 005a 0200 8700 0066 0100 6401 0064 0200  .Z.....f..d..d..
-00004690: 8600 005a 0300 6504 006a 0500 6506 006a  ...Z..e..j..e..j
-000046a0: 0700 6403 0066 0300 5a08 0087 0000 5329  ..d..f..Z.....S)
-000046b0: 04da 1854 6573 7453 796e 6341 6772 6565  ...TestSyncAgree
-000046c0: 6d65 6e74 436f 6d6d 616e 6463 0100 0000  mentCommandc....
-000046d0: 0000 0000 0100 0000 0100 0000 0300 0000  ................
-000046e0: 731b 0000 0074 0000 8300 006a 0100 8300  s....t.....j....
-000046f0: 0001 7402 006a 0300 8300 0001 6400 0053  ..t..j......d..S
-00004700: 2901 4e29 0472 4800 0000 7238 0000 0072  ).N).rH...r8...r
-00004710: 0800 0000 5a0f 696e 6974 5f61 6772 6565  ....Z.init_agree
-00004720: 6d65 6e74 7329 0172 1d00 0000 2901 724a  ments).r....).rJ
-00004730: 0000 0072 0d00 0000 720e 0000 0072 3800  ...r....r....r8.
-00004740: 0000 0602 0000 7304 0000 0000 010d 017a  ......s........z
-00004750: 1e54 6573 7453 796e 6341 6772 6565 6d65  .TestSyncAgreeme
-00004760: 6e74 436f 6d6d 616e 642e 7365 7455 70da  ntCommand.setUp.
-00004770: 0961 6772 6565 6d65 6e74 2909 722f 0000  .agreement).r/..
-00004780: 0072 3000 0000 7231 0000 0072 3800 0000  .r0...r1...r8...
-00004790: 7206 0000 00da 1f66 696e 616e 6365 5f61  r......finance_a
-000047a0: 7069 5f67 6574 5f61 6772 6565 6d65 6e74  pi_get_agreement
-000047b0: 735f 6361 6c6c 7207 0000 00da 1241 5049  s_callr......API
-000047c0: 5f41 4752 4545 4d45 4e54 5f4c 4953 5472  _AGREEMENT_LISTr
-000047d0: 2300 0000 720d 0000 0072 0d00 0000 2901  #...r....r....).
-000047e0: 724a 0000 0072 0e00 0000 72eb 0000 0005  rJ...r....r.....
-000047f0: 0200 0073 0800 0000 0c01 1205 0601 0601  ...s............
-00004800: 72eb 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00004810: 0000 0300 0000 0000 0000 7337 0000 0065  ..........s7...e
-00004820: 0000 5a01 0064 0000 5a02 0087 0000 6601  ..Z..d..Z.....f.
-00004830: 0064 0100 6402 0086 0000 5a03 0065 0400  .d..d.....Z..e..
-00004840: 6a05 0065 0600 6a07 0064 0300 6603 005a  j..e..j..d..f..Z
-00004850: 0800 8700 0053 2904 da1c 5465 7374 5379  .....S)...TestSy
-00004860: 6e63 5072 6f6a 6563 7454 6963 6b65 7443  ncProjectTicketC
-00004870: 6f6d 6d61 6e64 6301 0000 0000 0000 0001  ommandc.........
-00004880: 0000 0003 0000 0003 0000 0073 4b00 0000  ...........sK...
-00004890: 7400 0083 0000 6a01 0083 0000 0174 0200  t.....j......t..
-000048a0: 6a03 0074 0200 6a04 0074 0200 6a05 0083  j..t..j..t..j...
-000048b0: 0000 6602 0083 0100 0174 0600 6a07 0083  ..f......t..j...
-000048c0: 0000 0174 0600 6a08 0083 0000 0174 0600  ...t..j......t..
-000048d0: 6a09 0083 0000 0164 0000 5329 014e 290a  j......d..S).N).
-000048e0: 7248 0000 0072 3800 0000 7206 0000 0072  rH...r8...r....r
-000048f0: 7c00 0000 727d 0000 0072 7e00 0000 7208  |...r}...r~...r.
-00004900: 0000 0072 7f00 0000 7299 0000 005a 1469  ...r....r....Z.i
-00004910: 6e69 745f 7072 6f6a 6563 745f 7469 636b  nit_project_tick
-00004920: 6574 7329 0172 1d00 0000 2901 724a 0000  ets).r....).rJ..
-00004930: 0072 0d00 0000 720e 0000 0072 3800 0000  .r....r....r8...
-00004940: 1202 0000 730c 0000 0000 010d 0106 0116  ....s...........
-00004950: 010a 010a 017a 2254 6573 7453 796e 6350  .....z"TestSyncP
-00004960: 726f 6a65 6374 5469 636b 6574 436f 6d6d  rojectTicketComm
-00004970: 616e 642e 7365 7455 705a 0e70 726f 6a65  and.setUpZ.proje
-00004980: 6374 5f74 6963 6b65 7429 0972 2f00 0000  ct_ticket).r/...
-00004990: 7230 0000 0072 3100 0000 7238 0000 0072  r0...r1...r8...r
-000049a0: 0600 0000 da20 7072 6f6a 6563 745f 6170  ..... project_ap
-000049b0: 695f 7469 636b 6574 735f 7465 7374 5f63  i_tickets_test_c
-000049c0: 6f6d 6d61 6e64 7207 0000 00da 1741 5049  ommandr......API
-000049d0: 5f50 524f 4a45 4354 5f54 4943 4b45 545f  _PROJECT_TICKET_
-000049e0: 4c49 5354 7223 0000 0072 0d00 0000 720d  LISTr#...r....r.
-000049f0: 0000 0029 0172 4a00 0000 720e 0000 0072  ...).rJ...r....r
-00004a00: ef00 0000 1102 0000 7308 0000 000c 0112  ........s.......
-00004a10: 0906 0106 0172 ef00 0000 6300 0000 0000  .....r....c.....
-00004a20: 0000 0000 0000 0003 0000 0000 0000 0073  ...............s
-00004a30: 4900 0000 6500 005a 0100 6400 005a 0200  I...e..Z..d..Z..
-00004a40: 8700 0066 0100 6401 0064 0200 8600 005a  ...f..d..d.....Z
-00004a50: 0300 6403 0064 0400 6405 0084 0100 5a04  ..d..d..d.....Z.
-00004a60: 0064 0600 6407 0084 0000 5a05 0064 0800  .d..d.....Z..d..
-00004a70: 6409 0084 0000 5a06 0087 0000 5329 0ada  d.....Z.....S)..
-00004a80: 1254 6573 7453 796e 6341 6c6c 436f 6d6d  .TestSyncAllComm
-00004a90: 616e 6463 0100 0000 0000 0000 0600 0000  andc............
-00004aa0: 2800 0000 0300 0000 7321 0100 0074 0000  (.......s!...t..
-00004ab0: 8300 006a 0100 8300 0001 7402 006a 0300  ...j......t..j..
-00004ac0: 7404 006a 0500 6701 0083 0100 0174 0200  t..j..g......t..
-00004ad0: 6a06 0074 0200 6a07 0074 0200 6a08 0083  j..t..j..t..j...
-00004ae0: 0000 6602 0083 0100 0174 0200 6a09 0074  ..f......t..j..t
-00004af0: 0400 6a0a 0083 0100 0174 0200 6a0b 0083  ..j......t..j...
-00004b00: 0000 0174 0c00 740d 0074 0e00 740f 0074  ...t..t..t..t..t
-00004b10: 1000 7411 0074 1200 7413 0074 1400 7415  ..t..t..t..t..t.
-00004b20: 0074 1600 7417 0074 1800 7419 0074 1a00  .t..t..t..t..t..
-00004b30: 741b 0074 1c00 741d 0074 1e00 741f 0074  t..t..t..t..t..t
-00004b40: 2000 7421 0074 2200 7423 0074 2400 7425   .t!.t".t#.t$.t%
-00004b50: 0074 2600 7427 0074 2800 7429 0074 2a00  .t&.t'.t(.t).t*.
-00004b60: 742b 0074 2c00 742d 0074 2e00 742f 0074  t+.t,.t-.t..t/.t
-00004b70: 3000 7431 0074 3200 7433 0067 2800 7d01  0.t1.t2.t3.g(.}.
-00004b80: 0067 0000 7c00 005f 3400 783d 007c 0100  .g..|.._4.x=.|..
-00004b90: 445d 3500 7d02 007c 0000 6a34 006a 3500  D]5.}..|..j4.j5.
-00004ba0: 7c02 006a 3600 8301 0001 7c02 006a 3600  |..j6.....|..j6.
-00004bb0: 5c03 007d 0300 7d04 007d 0500 7c03 007c  \..}..}..}..|..|
-00004bc0: 0400 8301 0001 71e4 0057 6400 0053 2901  ......q..Wd..S).
-00004bd0: 4e29 3772 4800 0000 7238 0000 0072 0600  N)7rH...r8...r..
-00004be0: 0000 da1b 7379 7374 656d 5f61 7069 5f67  ....system_api_g
-00004bf0: 6574 5f6d 656d 6265 7273 5f63 616c 6c72  et_members_callr
-00004c00: 0700 0000 da0a 4150 495f 4d45 4d42 4552  ......API_MEMBER
-00004c10: 727c 0000 0072 7d00 0000 727e 0000 00da  r|...r}...r~....
-00004c20: 1663 6f6d 7061 6e79 5f61 7069 5f62 795f  .company_api_by_
-00004c30: 6964 5f63 616c 6cda 0b41 5049 5f43 4f4d  id_call..API_COM
-00004c40: 5041 4e59 da18 7365 7276 6963 655f 6170  PANY..service_ap
-00004c50: 695f 7469 636b 6574 735f 6361 6c6c 723f  i_tickets_callr?
-00004c60: 0000 0072 4700 0000 724e 0000 0072 5b00  ...rG...rN...r[.
-00004c70: 0000 7264 0000 0072 7500 0000 7268 0000  ..rd...ru...rh..
-00004c80: 0072 7000 0000 7252 0000 0072 8300 0000  .rp...rR...r....
-00004c90: 7257 0000 0072 9600 0000 729d 0000 0072  rW...r....r....r
-00004ca0: ad00 0000 72a9 0000 0072 b100 0000 72a5  ....r....r....r.
-00004cb0: 0000 0072 b500 0000 72ca 0000 0072 ce00  ...r....r....r..
-00004cc0: 0000 72d2 0000 0072 c200 0000 72c6 0000  ..r....r....r...
-00004cd0: 0072 bd00 0000 72b9 0000 0072 4300 0000  .r....r....rC...
-00004ce0: 728d 0000 0072 3200 0000 7291 0000 0072  r....r2...r....r
-00004cf0: 5f00 0000 7236 0000 0072 3b00 0000 72d6  _...r6...r;...r.
-00004d00: 0000 0072 db00 0000 72df 0000 0072 e300  ...r....r....r..
-00004d10: 0000 72e7 0000 0072 eb00 0000 726c 0000  ..r....r....rl..
-00004d20: 0072 7a00 0000 da09 7465 7374 5f61 7267  .rz.....test_arg
-00004d30: 7372 1c00 0000 7223 0000 0029 0672 1d00  sr....r#...).r..
-00004d40: 0000 5a0f 7379 6e63 5f74 6573 745f 6361  ..Z.sync_test_ca
-00004d50: 7365 73da 0974 6573 745f 6361 7365 da07  ses..test_case..
-00004d60: 6170 6963 616c 6cda 0766 6978 7475 7265  apicall..fixture
-00004d70: 7220 0000 0029 0172 4a00 0000 720d 0000  r ...).rJ...r...
-00004d80: 0072 0e00 0000 7238 0000 0023 0200 0073  .r....r8...#...s
-00004d90: 6600 0000 0001 0d01 1301 0601 1601 1001  f...............
-00004da0: 0a02 0301 0301 0301 0301 0301 0301 0301  ................
-00004db0: 0301 0301 0301 0301 0301 0301 0301 0301  ................
-00004dc0: 0301 0301 0301 0301 0301 0301 0301 0301  ................
-00004dd0: 0301 0301 0301 0301 0301 0301 0301 0301  ................
-00004de0: 0301 0301 0301 0301 0301 0301 0301 0301  ................
-00004df0: 0903 0902 0d01 1301 1201 7a18 5465 7374  ..........z.Test
-00004e00: 5379 6e63 416c 6c43 6f6d 6d61 6e64 2e73  SyncAllCommand.s
-00004e10: 6574 5570 4663 0200 0000 0000 0000 0400  etUpFc..........
-00004e20: 0000 0400 0000 4300 0000 7348 0000 0074  ......C...sH...t
-00004e30: 0000 6a01 0083 0000 7d02 0064 0100 6701  ..j.....}..d..g.
-00004e40: 007d 0300 7c01 0072 2800 7c03 006a 0200  .}..|..r(.|..j..
-00004e50: 6402 0083 0100 0174 0300 7c03 0064 0300  d......t..|..d..
-00004e60: 7c02 008c 0001 017c 0200 6a04 0083 0000  |......|..j.....
-00004e70: 6a05 0083 0000 5329 044e 7218 0000 007a  j.....S).Nr....z
-00004e80: 062d 2d66 756c 6c72 1900 0000 2906 721a  .--fullr....).r.
-00004e90: 0000 0072 1b00 0000 721c 0000 0072 0200  ...r....r....r..
-00004ea0: 0000 7228 0000 0072 2900 0000 2904 721d  ..r(...r)...).r.
-00004eb0: 0000 0072 2100 0000 7222 0000 0072 2300  ...r!...r"...r#.
-00004ec0: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-00004ed0: 00da 1072 756e 5f73 796e 635f 636f 6d6d  ...run_sync_comm
-00004ee0: 616e 645c 0200 0073 0c00 0000 0001 0c01  and\...s........
-00004ef0: 0902 0601 0d02 1002 7a23 5465 7374 5379  ........z#TestSy
-00004f00: 6e63 416c 6c43 6f6d 6d61 6e64 2e72 756e  ncAllCommand.run
-00004f10: 5f73 796e 635f 636f 6d6d 616e 6463 0100  _sync_commandc..
-00004f20: 0000 0000 0000 0600 0000 0500 0000 4300  ..............C.
-00004f30: 0000 737f 0100 007c 0000 6a00 0083 0000  ..s....|..j.....
-00004f40: 7d01 0078 4500 7c00 006a 0100 445d 3a00  }..xE.|..j..D]:.
-00004f50: 5c03 007d 0200 7d03 007d 0400 7402 0074  \..}..}..}..t..t
-00004f60: 0300 7c04 0083 0100 7404 007c 0300 8301  ..|.....t..|....
-00004f70: 0083 0200 7d05 007c 0000 6a05 007c 0500  ....}..|..j..|..
-00004f80: 7c01 0083 0200 0171 1600 577c 0000 6a06  |......q..W|..j.
-00004f90: 0074 0700 6a08 006a 0900 6a0a 0083 0000  .t..j..j..j.....
-00004fa0: 6a0b 0083 0000 7404 0074 0c00 6a0d 0083  j.....t..t..j...
-00004fb0: 0100 8302 0001 7c00 006a 0600 7407 006a  ......|..j..t..j
-00004fc0: 0e00 6a09 006a 0a00 8300 006a 0b00 8300  ..j..j.....j....
-00004fd0: 0074 0400 740c 006a 0f00 8301 0083 0200  .t..t..j........
-00004fe0: 017c 0000 6a06 0074 0700 6a10 006a 0900  .|..j..t..j..j..
-00004ff0: 6a0a 0083 0000 6a0b 0083 0000 7404 0074  j.....j.....t..t
-00005000: 0c00 6a11 0083 0100 8302 0001 7c00 006a  ..j.........|..j
-00005010: 0600 7407 006a 1200 6a09 006a 0a00 8300  ..t..j..j..j....
-00005020: 006a 0b00 8300 0074 0400 740c 006a 1300  .j.....t..t..j..
-00005030: 8301 0083 0200 017c 0000 6a06 0074 0700  .......|..j..t..
-00005040: 6a14 006a 0900 6a0a 0083 0000 6a0b 0083  j..j..j.....j...
-00005050: 0000 7404 0074 0c00 6a15 0083 0100 8302  ..t..t..j.......
-00005060: 0001 7c00 006a 0600 7407 006a 1600 6a09  ..|..j..t..j..j.
-00005070: 006a 0a00 8300 006a 0b00 8300 0064 0100  .j.....j.....d..
-00005080: 8302 0001 7c00 006a 0600 7407 006a 1700  ....|..j..t..j..
-00005090: 6a09 006a 0a00 8300 006a 0b00 8300 0074  j..j.....j.....t
-000050a0: 0400 740c 006a 1800 6701 0083 0100 8302  ..t..j..g.......
-000050b0: 0001 6402 0053 2903 7a64 0a20 2020 2020  ..d..S).zd.     
-000050c0: 2020 2054 6573 7420 7468 6520 636f 6d6d     Test the comm
-000050d0: 616e 6420 746f 2072 756e 2061 2073 796e  and to run a syn
-000050e0: 6320 6f66 2061 6c6c 206f 626a 6563 7473  c of all objects
-000050f0: 2077 6974 686f 7574 0a20 2020 2020 2020   without.       
-00005100: 2074 6865 202d 2d66 756c 6c20 6172 6775   the --full argu
-00005110: 6d65 6e74 2e0a 2020 2020 2020 2020 7205  ment..        r.
-00005120: 0000 004e 2919 72fc 0000 0072 f800 0000  ...N).r....r....
-00005130: 720f 0000 0072 1600 0000 722b 0000 0072  r....r....r+...r
-00005140: 2700 0000 722c 0000 0072 0400 0000 da04  '...r,...r......
-00005150: 5465 616d 7286 0000 0072 8700 0000 da05  Teamr....r......
-00005160: 636f 756e 7472 0700 0000 7256 0000 00da  countr....rV....
-00005170: 0d43 6f6d 7061 6e79 5374 6174 7573 7242  .CompanyStatusrB
-00005180: 0000 00da 0e54 6963 6b65 7450 7269 6f72  .....TicketPrior
-00005190: 6974 7972 6700 0000 7285 0000 0072 5a00  ityrg...r....rZ.
-000051a0: 0000 da0b 426f 6172 6453 7461 7475 7372  ....BoardStatusr
-000051b0: 8c00 0000 da08 4c6f 6361 7469 6f6e da06  ......Location..
-000051c0: 5469 636b 6574 da12 4150 495f 5345 5256  Ticket..API_SERV
-000051d0: 4943 455f 5449 434b 4554 2906 721d 0000  ICE_TICKET).r...
-000051e0: 00da 066f 7574 7075 7472 fa00 0000 72fb  ...outputr....r.
-000051f0: 0000 0072 2000 0000 da07 7375 6d6d 6172  ...r .....summar
-00005200: 7972 0d00 0000 720d 0000 0072 0e00 0000  yr....r....r....
-00005210: da11 7465 7374 5f70 6172 7469 616c 5f73  ..test_partial_s
-00005220: 796e 6367 0200 0073 2400 0000 0005 0c02  yncg...s$.......
-00005230: 1901 1b01 1402 1b01 1001 1b01 1002 1b01  ................
-00005240: 1001 1b01 1001 1b01 1001 1b01 0702 1b01  ................
-00005250: 7a24 5465 7374 5379 6e63 416c 6c43 6f6d  z$TestSyncAllCom
-00005260: 6d61 6e64 2e74 6573 745f 7061 7274 6961  mand.test_partia
-00005270: 6c5f 7379 6e63 6301 0000 0000 0000 000b  l_syncc.........
-00005280: 0000 0054 0000 0043 0000 0073 b502 0000  ...T...C...s....
-00005290: 6401 0074 0000 6a01 0064 0200 7400 006a  d..t..j..d..t..j
-000052a0: 0200 6403 0074 0000 6a03 0064 0400 7400  ..d..t..j..d..t.
-000052b0: 006a 0400 6405 0074 0000 6a05 0064 0600  .j..d..t..j..d..
-000052c0: 7400 006a 0600 6407 0074 0000 6a07 0064  t..j..d..t..j..d
-000052d0: 0800 7400 006a 0800 6409 0074 0000 6a09  ..t..j..d..t..j.
-000052e0: 0064 0a00 7400 006a 0a00 640b 0074 0000  .d..t..j..d..t..
-000052f0: 6a0b 0064 0c00 7400 006a 0c00 640d 0074  j..d..t..j..d..t
-00005300: 0000 6a0d 0064 0e00 7400 006a 0e00 640f  ..j..d..t..j..d.
-00005310: 0074 0000 6a0f 0064 1000 7400 006a 1000  .t..j..d..t..j..
-00005320: 6411 0074 0000 6a11 0064 1200 7400 006a  d..t..j..d..t..j
-00005330: 1200 6413 0074 0000 6a13 0064 1400 7400  ..d..t..j..d..t.
-00005340: 006a 1400 6415 0074 0000 6a15 0064 1600  .j..d..t..j..d..
-00005350: 7400 006a 1600 6417 0074 0000 6a17 0064  t..j..d..t..j..d
-00005360: 1800 7400 006a 1800 6419 0074 0000 6a19  ..t..j..d..t..j.
-00005370: 0064 1a00 7400 006a 1a00 641b 0074 0000  .d..t..j..d..t..
-00005380: 6a1b 0064 1c00 7400 006a 1c00 641d 0074  j..d..t..j..d..t
-00005390: 0000 6a1d 0064 1e00 7400 006a 1e00 641f  ..j..d..t..j..d.
-000053a0: 0074 0000 6a1f 0064 2000 7400 006a 2000  .t..j..d .t..j .
-000053b0: 6421 0074 0000 6a21 0064 2200 7400 006a  d!.t..j!.d".t..j
-000053c0: 2200 6423 0074 0000 6a23 0064 2400 7400  ".d#.t..j#.d$.t.
-000053d0: 006a 2400 6425 0074 0000 6a25 0064 2600  .j$.d%.t..j%.d&.
-000053e0: 7400 006a 2600 6427 0074 0000 6a27 0064  t..j&.d'.t..j'.d
-000053f0: 2800 7400 006a 2800 6429 0074 0000 6a29  (.t..j(.d).t..j)
-00005400: 0064 2a00 7400 006a 2a00 692a 007d 0100  .d*.t..j*.i*.}..
-00005410: 7c00 006a 2b00 8300 0001 742c 006a 2d00  |..j+.....t,.j-.
-00005420: 8300 0001 742c 006a 2e00 8300 0001 742c  ....t,.j......t,
-00005430: 006a 2f00 8300 0001 742c 006a 3000 8300  .j/.....t,.j0...
-00005440: 0001 6900 007d 0200 7833 007c 0100 6a31  ..i..}..x3.|..j1
-00005450: 0083 0000 445d 2500 5c02 007d 0300 7d04  ....D]%.\..}..}.
-00005460: 007c 0400 6a32 006a 3300 8300 006a 3400  .|..j2.j3....j4.
-00005470: 8300 007c 0200 7c03 003c 71c5 0157 7435  ...|..|..<q..Wt5
-00005480: 006a 3600 6700 0083 0100 0174 3500 6a37  .j6.g......t5.j7
-00005490: 0067 0000 8301 0001 7824 007c 0000 6a38  .g......x$.|..j8
-000054a0: 0044 5d19 005c 0300 7d05 007d 0600 7d06  .D]..\..}..}..}.
-000054b0: 007c 0500 6700 0083 0100 0171 1202 577c  .|..g......q..W|
-000054c0: 0000 6a2b 0064 2b00 642c 0083 0001 7d07  ..j+.d+.d,....}.
-000054d0: 0078 6d00 7c00 006a 3800 445d 6200 5c03  .xm.|..j8.D]b.\.
-000054e0: 007d 0500 7d08 007d 0900 7c09 0064 2f00  .}..}..}..|..d/.
-000054f0: 6b06 0072 8402 7c00 006a 3900 7c02 007c  k..r..|..j9.|..|
-00005500: 0900 1964 2d00 8302 0001 642d 007c 0200  ...d-.....d-.|..
-00005510: 7c09 003c 743a 0074 3b00 7c09 0083 0100  |..<t:.t;.|.....
-00005520: 7c02 007c 0900 1983 0200 7d0a 007c 0000  |..|......}..|..
-00005530: 6a3c 007c 0a00 7c07 0083 0200 0171 4b02  j<.|..|......qK.
-00005540: 5764 2e00 5329 307a 3354 6573 7420 7468  Wd..S)0z3Test th
-00005550: 6520 636f 6d6d 616e 6420 746f 2072 756e  e command to run
-00005560: 2061 2066 756c 6c20 7379 6e63 206f 6620   a full sync of 
-00005570: 616c 6c20 6f62 6a65 6374 732e da06 6d65  all objects...me
-00005580: 6d62 6572 7258 0000 0072 6500 0000 7269  mberrX...re...ri
-00005590: 0000 0072 7100 0000 7276 0000 0072 8400  ...rq...rv...r..
-000055a0: 0000 7244 0000 0072 4000 0000 724f 0000  ..rD...r@...rO..
-000055b0: 0072 5300 0000 725c 0000 00da 0674 6963  .rS...r\.....tic
-000055c0: 6b65 7472 9700 0000 729e 0000 0072 4b00  ketr....r....rK.
-000055d0: 0000 72a6 0000 0072 ae00 0000 72aa 0000  ..r....r....r...
-000055e0: 0072 b200 0000 72b6 0000 0072 cb00 0000  .r....r....r....
-000055f0: 72cf 0000 0072 d300 0000 72be 0000 0072  r....r....r....r
-00005600: c300 0000 72c7 0000 0072 ba00 0000 728e  ....r....r....r.
-00005610: 0000 0072 3300 0000 7292 0000 0072 6000  ...r3...r....r`.
-00005620: 0000 7237 0000 0072 3c00 0000 72d8 0000  ..r7...r<...r...
-00005630: 0072 dc00 0000 72e0 0000 0072 e400 0000  .r....r....r....
-00005640: 72e8 0000 0072 ec00 0000 726d 0000 0072  r....r....rm...r
-00005650: 7b00 0000 7221 0000 0054 7201 0000 004e  {...r!...Tr....N
-00005660: 2905 7a04 7465 616d 7a0c 626f 6172 645f  ).z.teamz.board_
-00005670: 7374 6174 7573 7a10 6f70 706f 7274 756e  statusz.opportun
-00005680: 6974 795f 6e6f 7465 7a0c 736c 615f 7072  ity_notez.sla_pr
-00005690: 696f 7269 7479 7a07 686f 6c69 6461 7929  iorityz.holiday)
-000056a0: 3d72 0400 0000 da06 4d65 6d62 6572 7285  =r......Memberr.
-000056b0: 0000 0072 0001 0000 da0d 5072 6f6a 6563  ...r......Projec
-000056c0: 7453 7461 7475 73da 0750 726f 6a65 6374  tStatus..Project
-000056d0: da0c 5072 6f6a 6563 7450 6861 7365 7201  ..ProjectPhaser.
-000056e0: 0100 00da 0954 6572 7269 746f 7279 72ff  .....Territoryr.
-000056f0: 0000 00da 0b43 6f6d 7061 6e79 5479 7065  .....CompanyType
-00005700: 72fd 0000 0072 0201 0000 7203 0100 00da  r....r....r.....
-00005710: 0b53 6572 7669 6365 4e6f 7465 da0f 4f70  .ServiceNote..Op
-00005720: 706f 7274 756e 6974 794e 6f74 65da 0743  portunityNote..C
-00005730: 6f6d 7061 6e79 da0b 4f70 706f 7274 756e  ompany..Opportun
-00005740: 6974 79da 114f 7070 6f72 7475 6e69 7479  ity..Opportunity
-00005750: 5374 6174 7573 da10 4f70 706f 7274 756e  Status..Opportun
-00005760: 6974 7953 7461 6765 da0f 4f70 706f 7274  ityStage..Opport
-00005770: 756e 6974 7954 7970 65da 1053 616c 6573  unityType..Sales
-00005780: 5072 6f62 6162 696c 6974 79da 0e41 6374  Probability..Act
-00005790: 6976 6974 7953 7461 7475 73da 0c41 6374  ivityStatus..Act
-000057a0: 6976 6974 7954 7970 65da 0841 6374 6976  ivityType..Activ
-000057b0: 6974 79da 0d53 6368 6564 756c 6545 6e74  ity..ScheduleEnt
-000057c0: 7279 da0c 5363 6865 6475 6c65 5479 7065  ry..ScheduleType
-000057d0: da0e 5363 6865 6475 6c65 5374 6174 7573  ..ScheduleStatus
-000057e0: da09 5469 6d65 456e 7472 79da 0353 6c61  ..TimeEntry..Sla
-000057f0: da08 4361 6c65 6e64 6172 da0b 536c 6150  ..Calendar..SlaP
-00005800: 7269 6f72 6974 79da 0e4d 7943 6f6d 7061  riority..MyCompa
-00005810: 6e79 4f74 6865 72da 0748 6f6c 6964 6179  nyOther..Holiday
-00005820: da0b 486f 6c69 6461 794c 6973 74da 0454  ..HolidayList..T
-00005830: 7970 65da 0753 7562 5479 7065 da04 4974  ype..SubType..It
-00005840: 656d da08 576f 726b 5479 7065 da08 576f  em..WorkType..Wo
-00005850: 726b 526f 6c65 da09 4167 7265 656d 656e  rkRole..Agreemen
-00005860: 74da 0b50 726f 6a65 6374 5479 7065 da11  t..ProjectType..
-00005870: 5072 6f6a 6563 7454 6561 6d4d 656d 6265  ProjectTeamMembe
-00005880: 7272 fc00 0000 7208 0000 0072 7700 0000  rr....r....rw...
-00005890: 727f 0000 0072 9900 0000 72bf 0000 00da  r....r....r.....
-000058a0: 0569 7465 6d73 7286 0000 0072 8700 0000  .itemsr....r....
-000058b0: 72fe 0000 0072 0600 0000 72f3 0000 0072  r....r....r....r
-000058c0: f500 0000 72f8 0000 00da 0d61 7373 6572  ....r......asser
-000058d0: 7447 7265 6174 6572 7210 0000 0072 1600  tGreaterr....r..
-000058e0: 0000 7227 0000 0029 0b72 1d00 0000 5a0d  ..r'...).r....Z.
-000058f0: 6377 5f6f 626a 6563 745f 6d61 705a 1470  cw_object_mapZ.p
-00005900: 7265 5f66 756c 6c5f 7379 6e63 5f63 6f75  re_full_sync_cou
-00005910: 6e74 73da 036b 6579 da0b 6d6f 6465 6c5f  nts..key..model_
-00005920: 636c 6173 7372 fa00 0000 7211 0000 0072  classr....r....r
-00005930: 0501 0000 72fb 0000 0072 2000 0000 7206  ....r....r ...r.
-00005940: 0100 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00005950: 0000 722e 0000 0083 0200 0073 8800 0000  ..r........s....
-00005960: 0003 0901 0901 0901 0901 0901 0901 0901  ................
-00005970: 0901 0901 0901 0901 0901 0901 0901 0901  ................
-00005980: 0901 0901 0901 0901 0901 0901 0901 0901  ................
-00005990: 0901 0901 0901 0901 0901 0901 0901 0901  ................
-000059a0: 0901 0901 0901 0901 0901 0901 0901 0901  ................
-000059b0: 0901 0901 0f04 0a02 0a01 0a01 0a01 0a02  ................
-000059c0: 0602 1901 1d02 0d01 0d02 1901 0e02 1202  ................
-000059d0: 1901 0301 0001 0001 0001 0001 0906 1401  ................
-000059e0: 0a01 0301 0901 0d02 7a21 5465 7374 5379  ........z!TestSy
-000059f0: 6e63 416c 6c43 6f6d 6d61 6e64 2e74 6573  ncAllCommand.tes
-00005a00: 745f 6675 6c6c 5f73 796e 6329 0772 2f00  t_full_sync).r/.
-00005a10: 0000 7230 0000 0072 3100 0000 7238 0000  ..r0...r1...r8..
-00005a20: 0072 fc00 0000 7207 0100 0072 2e00 0000  .r....r....r....
-00005a30: 720d 0000 0072 0d00 0000 2901 724a 0000  r....r....).rJ..
-00005a40: 0072 0e00 0000 72f2 0000 0021 0200 0073  .r....r....!...s
-00005a50: 0800 0000 0c02 1239 0f0b 0c1c 72f2 0000  .......9....r...
-00005a60: 0063 0000 0000 0000 0000 0000 0000 0200  .c..............
-00005a70: 0000 4000 0000 731c 0000 0065 0000 5a01  ..@...s....e..Z.
-00005a80: 0064 0000 5a02 0064 0100 6402 0084 0000  .d..Z..d..d.....
-00005a90: 5a03 0064 0300 5329 04da 1454 6573 744c  Z..d..S)...TestL
-00005aa0: 6973 7455 7365 7273 436f 6d6d 616e 6463  istUsersCommandc
-00005ab0: 0100 0000 0000 0000 0100 0000 0300 0000  ................
-00005ac0: 4300 0000 731a 0000 007c 0000 6a00 0074  C...s....|..j..t
-00005ad0: 0100 6401 0083 0100 6400 0083 0200 0164  ..d.....d......d
-00005ae0: 0000 5329 024e 5a0a 6c69 7374 5f75 7365  ..S).NZ.list_use
-00005af0: 7273 2902 722c 0000 0072 0200 0000 2901  rs).r,...r....).
-00005b00: 721d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00005b10: 0e00 0000 da0c 7465 7374 5f63 6f6d 6d61  ......test_comma
-00005b20: 6e64 dd02 0000 7306 0000 0000 0306 0109  nd....s.........
-00005b30: 017a 2154 6573 744c 6973 7455 7365 7273  .z!TestListUsers
-00005b40: 436f 6d6d 616e 642e 7465 7374 5f63 6f6d  Command.test_com
-00005b50: 6d61 6e64 4e29 0472 2f00 0000 7230 0000  mandN).r/...r0..
-00005b60: 0072 3100 0000 7232 0100 0072 0d00 0000  .r1...r2...r....
-00005b70: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00005b80: 3101 0000 dc02 0000 7302 0000 000c 0172  1.......s......r
-00005b90: 3101 0000 293c 721a 0000 00da 1664 6a61  1...)<r......dja
-00005ba0: 6e67 6f2e 636f 7265 2e6d 616e 6167 656d  ngo.core.managem
-00005bb0: 656e 7472 0200 0000 da0b 646a 616e 676f  entr......django
-00005bc0: 2e74 6573 7472 0300 0000 da0d 646a 636f  .testr......djco
-00005bd0: 6e6e 6563 7477 6973 6572 0400 0000 da00  nnectwiser......
-00005be0: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
-00005bf0: 0a00 0000 720f 0000 0072 1000 0000 7216  ....r....r....r.
-00005c00: 0000 00da 066f 626a 6563 7472 1700 0000  .....objectr....
-00005c10: 7232 0000 0072 3600 0000 723b 0000 0072  r2...r6...r;...r
-00005c20: 3f00 0000 7243 0000 0072 4700 0000 724e  ?...rC...rG...rN
-00005c30: 0000 0072 5200 0000 7257 0000 0072 5b00  ...rR...rW...r[.
-00005c40: 0000 725f 0000 0072 6400 0000 7268 0000  ..r_...rd...rh..
-00005c50: 0072 6c00 0000 7270 0000 0072 7500 0000  .rl...rp...ru...
-00005c60: 727a 0000 0072 8300 0000 728d 0000 0072  rz...r....r....r
-00005c70: 9100 0000 7296 0000 0072 9d00 0000 72a5  ....r....r....r.
-00005c80: 0000 0072 a900 0000 72ad 0000 0072 b100  ...r....r....r..
-00005c90: 0000 72b5 0000 0072 b900 0000 72bd 0000  ..r....r....r...
-00005ca0: 0072 c200 0000 72c6 0000 0072 ca00 0000  .r....r....r....
-00005cb0: 72ce 0000 0072 d200 0000 72d6 0000 0072  r....r....r....r
-00005cc0: db00 0000 72df 0000 0072 e300 0000 72e7  ....r....r....r.
-00005cd0: 0000 0072 eb00 0000 72ef 0000 0072 f200  ...r....r....r..
-00005ce0: 0000 7231 0100 0072 0d00 0000 720d 0000  ..r1...r....r...
-00005cf0: 0072 0d00 0000 720e 0000 00da 083c 6d6f  .r....r......<mo
-00005d00: 6475 6c65 3e01 0000 0073 6c00 0000 0c02  dule>....sl.....
-00005d10: 1001 1002 1002 1001 1001 1001 1003 0c06  ................
-00005d20: 0c06 0c04 1625 1908 190b 1908 1908 1908  .....%..........
-00005d30: 190c 1908 190c 1908 1908 190b 1909 1908  ................
-00005d40: 1908 190c 190d 1912 190f 190b 190d 1912  ................
-00005d50: 1910 1911 1908 1908 1908 1908 1911 1917  ................
-00005d60: 1908 1908 1908 1908 1916 190e 190d 190d  ................
-00005d70: 190c 190c 190c 1910 16bb                 ..........
+00000020: 0073 8a03 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
+00000030: 6402 6c01 6d02 5a02 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
+00000040: 6d04 5a04 0100 6400 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
+00000050: 0100 6405 6406 6c07 6d08 5a08 0100 6405  ..d.d.l.m.Z...d.
+00000060: 6407 6c07 6d09 5a09 0100 6405 6408 6c07  d.l.m.Z...d.d.l.
+00000070: 6d0a 5a0a 0100 6409 640a 6c07 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000080: 0100 640b 640c 8400 5a0c 640d 640e 8400  ..d.d...Z.d.d...
+00000090: 5a0d 640f 6410 8400 5a0e 4700 6411 6412  Z.d.d...Z.G.d.d.
+000000a0: 8400 6412 650f 8303 5a10 4700 6413 6414  ..d.e...Z.G.d.d.
+000000b0: 8400 6414 6510 6504 8304 5a11 4700 6415  ..d.e.e...Z.G.d.
+000000c0: 6416 8400 6416 6510 6504 8304 5a12 4700  d...d.e.e...Z.G.
+000000d0: 6417 6418 8400 6418 6510 6504 8304 5a13  d.d...d.e.e...Z.
+000000e0: 4700 6419 641a 8400 641a 6510 6504 8304  G.d.d...d.e.e...
+000000f0: 5a14 4700 641b 641c 8400 641c 6510 6504  Z.G.d.d...d.e.e.
+00000100: 8304 5a15 4700 641d 641e 8400 641e 6510  ..Z.G.d.d...d.e.
+00000110: 6504 8304 5a16 4700 641f 6420 8400 6420  e...Z.G.d.d ..d 
+00000120: 6510 6504 8304 5a17 4700 6421 6422 8400  e.e...Z.G.d!d"..
+00000130: 6422 6510 6504 8304 5a18 4700 6423 6424  d"e.e...Z.G.d#d$
+00000140: 8400 6424 6510 6504 8304 5a19 4700 6425  ..d$e.e...Z.G.d%
+00000150: 6426 8400 6426 6510 6504 8304 5a1a 4700  d&..d&e.e...Z.G.
+00000160: 6427 6428 8400 6428 6510 6504 8304 5a1b  d'd(..d(e.e...Z.
+00000170: 4700 6429 642a 8400 642a 6510 6504 8304  G.d)d*..d*e.e...
+00000180: 5a1c 4700 642b 642c 8400 642c 6510 6504  Z.G.d+d,..d,e.e.
+00000190: 8304 5a1d 4700 642d 642e 8400 642e 6510  ..Z.G.d-d...d.e.
+000001a0: 6504 8304 5a1e 4700 642f 6430 8400 6430  e...Z.G.d/d0..d0
+000001b0: 6510 6504 8304 5a1f 4700 6431 6432 8400  e.e...Z.G.d1d2..
+000001c0: 6432 6510 6504 8304 5a20 4700 6433 6434  d2e.e...Z G.d3d4
+000001d0: 8400 6434 6510 6504 8304 5a21 4700 6435  ..d4e.e...Z!G.d5
+000001e0: 6436 8400 6436 6510 6504 8304 5a22 4700  d6..d6e.e...Z"G.
+000001f0: 6437 6438 8400 6438 6510 6504 8304 5a23  d7d8..d8e.e...Z#
+00000200: 4700 6439 643a 8400 643a 6510 6504 8304  G.d9d:..d:e.e...
+00000210: 5a24 4700 643b 643c 8400 643c 6510 6504  Z$G.d;d<..d<e.e.
+00000220: 8304 5a25 4700 643d 643e 8400 643e 6510  ..Z%G.d=d>..d>e.
+00000230: 6504 8304 5a26 4700 643f 6440 8400 6440  e...Z&G.d?d@..d@
+00000240: 6510 6504 8304 5a27 4700 6441 6442 8400  e.e...Z'G.dAdB..
+00000250: 6442 6510 6504 8304 5a28 4700 6443 6444  dBe.e...Z(G.dCdD
+00000260: 8400 6444 6510 6504 8304 5a29 4700 6445  ..dDe.e...Z)G.dE
+00000270: 6446 8400 6446 6510 6504 8304 5a2a 4700  dF..dFe.e...Z*G.
+00000280: 6447 6448 8400 6448 6510 6504 8304 5a2b  dGdH..dHe.e...Z+
+00000290: 4700 6449 644a 8400 644a 6510 6504 8304  G.dIdJ..dJe.e...
+000002a0: 5a2c 4700 644b 644c 8400 644c 6510 6504  Z,G.dKdL..dLe.e.
+000002b0: 8304 5a2d 4700 644d 644e 8400 644e 6510  ..Z-G.dMdN..dNe.
+000002c0: 6504 8304 5a2e 4700 644f 6450 8400 6450  e...Z.G.dOdP..dP
+000002d0: 6510 6504 8304 5a2f 4700 6451 6452 8400  e.e...Z/G.dQdR..
+000002e0: 6452 6510 6504 8304 5a30 4700 6453 6454  dRe.e...Z0G.dSdT
+000002f0: 8400 6454 6510 6504 8304 5a31 4700 6455  ..dTe.e...Z1G.dU
+00000300: 6456 8400 6456 6510 6504 8304 5a32 4700  dV..dVe.e...Z2G.
+00000310: 6457 6458 8400 6458 6510 6504 8304 5a33  dWdX..dXe.e...Z3
+00000320: 4700 6459 645a 8400 645a 6510 6504 8304  G.dYdZ..dZe.e...
+00000330: 5a34 4700 645b 645c 8400 645c 6510 6504  Z4G.d[d\..d\e.e.
+00000340: 8304 5a35 4700 645d 645e 8400 645e 6510  ..Z5G.d]d^..d^e.
+00000350: 6504 8304 5a36 4700 645f 6460 8400 6460  e...Z6G.d_d`..d`
+00000360: 6510 6504 8304 5a37 4700 6461 6462 8400  e.e...Z7G.dadb..
+00000370: 6462 6510 6504 8304 5a38 4700 6463 6464  dbe.e...Z8G.dcdd
+00000380: 8400 6464 6510 6504 8304 5a39 4700 6465  ..dde.e...Z9G.de
+00000390: 6466 8400 6466 6504 8303 5a3a 4700 6467  df..dfe...Z:G.dg
+000003a0: 6468 8400 6468 6504 8303 5a3b 6401 5300  dh..dhe...Z;d.S.
+000003b0: 2969 e900 0000 004e 2901 da0c 6361 6c6c  )i.....N)...call
+000003c0: 5f63 6f6d 6d61 6e64 2901 da08 5465 7374  _command)...Test
+000003d0: 4361 7365 2901 da06 6d6f 6465 6c73 e901  Case)...models..
+000003e0: 0000 0029 01da 056d 6f63 6b73 2901 da08  ...)...mocks)...
+000003f0: 6669 7874 7572 6573 2901 da0d 6669 7874  fixtures)...fixt
+00000400: 7572 655f 7574 696c 73e9 0200 0000 2901  ure_utils.....).
+00000410: da04 7379 6e63 6302 0000 0000 0000 0002  ..syncc.........
+00000420: 0000 0003 0000 0043 0000 0073 0c00 0000  .......C...s....
+00000430: 6401 6a00 7c00 7c01 8302 5300 2902 4e7a  d.j.|.|...S.).Nz
+00000440: 297b 7d20 5379 6e63 2053 756d 6d61 7279  ){} Sync Summary
+00000450: 202d 2043 7265 6174 6564 3a20 7b7d 2c20   - Created: {}, 
+00000460: 5570 6461 7465 643a 2030 2901 da06 666f  Updated: 0)...fo
+00000470: 726d 6174 2902 da0a 636c 6173 735f 6e61  rmat)...class_na
+00000480: 6d65 5a0d 6372 6561 7465 645f 636f 756e  meZ.created_coun
+00000490: 74a9 0072 0d00 0000 fa54 2f68 6f6d 652f  t..r.....T/home/
+000004a0: 6361 6d65 726f 6e2f 4465 762f 6b61 6e62  cameron/Dev/kanb
+000004b0: 616e 2d64 6576 2f64 6a61 6e67 6f2d 636f  an-dev/django-co
+000004c0: 6e6e 6563 7477 6973 652f 646a 636f 6e6e  nnectwise/djconn
+000004d0: 6563 7477 6973 652f 7465 7374 732f 7465  ectwise/tests/te
+000004e0: 7374 5f63 6f6d 6d61 6e64 732e 7079 da0c  st_commands.py..
+000004f0: 7379 6e63 5f73 756d 6d61 7279 0e00 0000  sync_summary....
+00000500: 7304 0000 0000 0104 0172 0f00 0000 6302  s........r....c.
+00000510: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00000520: 0000 0073 0c00 0000 6401 6a00 7c00 7c01  ...s....d.j.|.|.
+00000530: 8302 5300 2902 4e7a 357b 7d20 5379 6e63  ..S.).Nz5{} Sync
+00000540: 2053 756d 6d61 7279 202d 2043 7265 6174   Summary - Creat
+00000550: 6564 3a20 302c 2055 7064 6174 6564 3a20  ed: 0, Updated: 
+00000560: 302c 2044 656c 6574 6564 3a20 7b7d 2901  0, Deleted: {}).
+00000570: 720b 0000 0029 0272 0c00 0000 5a0d 6465  r....).r....Z.de
+00000580: 6c65 7465 645f 636f 756e 7472 0d00 0000  leted_countr....
+00000590: 720d 0000 0072 0e00 0000 da11 6675 6c6c  r....r......full
+000005a0: 5f73 796e 635f 7375 6d6d 6172 7914 0000  _sync_summary...
+000005b0: 0073 0400 0000 0001 0401 7210 0000 0063  .s........r....c
+000005c0: 0100 0000 0000 0000 0100 0000 0300 0000  ................
+000005d0: 4300 0000 7310 0000 007c 006a 0083 006a  C...s....|.j...j
+000005e0: 0164 0164 0283 0253 0029 034e da01 5ffa  .d.d...S.).N.._.
+000005f0: 0120 2902 da05 7469 746c 65da 0772 6570  . )...title..rep
+00000600: 6c61 6365 2901 da04 736c 7567 720d 0000  lace)...slugr...
+00000610: 0072 0d00 0000 720e 0000 00da 0d73 6c75  .r....r......slu
+00000620: 675f 746f 5f74 6974 6c65 1a00 0000 7302  g_to_title....s.
+00000630: 0000 0000 0172 1600 0000 6300 0000 0000  .....r....c.....
+00000640: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00000650: 2e00 0000 6500 5a01 6400 5a02 640b 6402  ....e.Z.d.Z.d.d.
+00000660: 6403 8401 5a03 6404 6405 8400 5a04 6406  d...Z.d.d...Z.d.
+00000670: 6407 8400 5a05 6408 6409 8400 5a06 640a  d...Z.d.d...Z.d.
+00000680: 5300 290c da14 4162 7374 7261 6374 4261  S.)...AbstractBa
+00000690: 7365 5379 6e63 5465 7374 4663 0500 0000  seSyncTestFc....
+000006a0: 0000 0000 0700 0000 0400 0000 4300 0000  ............C...
+000006b0: 7338 0000 007c 017c 0283 0101 0074 006a  s8...|.|.....t.j
+000006c0: 0183 007d 0564 017c 0367 027d 067c 0472  ...}.d.|.g.}.|.r
+000006d0: 267c 066a 0264 0283 0101 0074 037c 0664  &|.j.d.....t.|.d
+000006e0: 037c 0569 018e 0101 007c 0553 0029 044e  .|.i.....|.S.).N
+000006f0: da06 6377 7379 6e63 7a06 2d2d 6675 6c6c  ..cwsyncz.--full
+00000700: da06 7374 646f 7574 2904 da02 696f da08  ..stdout)...io..
+00000710: 5374 7269 6e67 494f da06 6170 7065 6e64  StringIO..append
+00000720: 7202 0000 0029 07da 0473 656c 66da 096d  r....)...self..m
+00000730: 6f63 6b5f 6361 6c6c da0c 7265 7475 726e  ock_call..return
+00000740: 5f76 616c 7565 da09 6377 5f6f 626a 6563  _value..cw_objec
+00000750: 74da 0b66 756c 6c5f 6f70 7469 6f6e da03  t..full_option..
+00000760: 6f75 74da 0461 7267 7372 0d00 0000 720d  out..argsr....r.
+00000770: 0000 0072 0e00 0000 da0a 5f74 6573 745f  ...r......_test_
+00000780: 7379 6e63 2000 0000 730e 0000 0000 0208  sync ...s.......
+00000790: 0108 0208 0104 010a 010e 017a 1f41 6273  ...........z.Abs
+000007a0: 7472 6163 7442 6173 6553 796e 6354 6573  tractBaseSyncTes
+000007b0: 742e 5f74 6573 745f 7379 6e63 6302 0000  t._test_syncc...
+000007c0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+000007d0: 0073 1000 0000 7c01 6a00 8300 6a01 6401  .s....|.j...j.d.
+000007e0: 6402 8302 5300 2903 4e72 1100 0000 7212  d...S.).Nr....r.
+000007f0: 0000 0029 0272 1300 0000 7214 0000 0029  ...).r....r....)
+00000800: 0272 1d00 0000 7220 0000 0072 0d00 0000  .r....r ...r....
+00000810: 720d 0000 0072 0e00 0000 da14 5f74 6974  r....r......_tit
+00000820: 6c65 5f66 6f72 5f63 775f 6f62 6a65 6374  le_for_cw_object
+00000830: 2b00 0000 7302 0000 0000 017a 2941 6273  +...s......z)Abs
+00000840: 7472 6163 7442 6173 6553 796e 6354 6573  tractBaseSyncTes
+00000850: 742e 5f74 6974 6c65 5f66 6f72 5f63 775f  t._title_for_cw_
+00000860: 6f62 6a65 6374 6301 0000 0000 0000 0003  objectc.........
+00000870: 0000 0003 0000 0043 0000 0073 3400 0000  .......C...s4...
+00000880: 7c00 6a00 7c00 6a01 8e00 7d01 7c00 6a02  |.j.|.j...}.|.j.
+00000890: 7c00 6a01 6402 1900 8301 7d02 7c00 6a03  |.j.d.....}.|.j.
+000008a0: 7c02 7c01 6a04 8300 6a05 8300 8302 0100  |.|.j...j.......
+000008b0: 6400 5300 2903 4e72 0500 0000 e9ff ffff  d.S.).Nr........
+000008c0: ff29 0672 2400 0000 7223 0000 0072 2500  .).r$...r#...r%.
+000008d0: 0000 da08 6173 7365 7274 496e da08 6765  ....assertIn..ge
+000008e0: 7476 616c 7565 da05 7374 7269 7029 0372  tvalue..strip).r
+000008f0: 1d00 0000 7222 0000 005a 096f 626a 5f74  ....r"...Z.obj_t
+00000900: 6974 6c65 720d 0000 0072 0d00 0000 720e  itler....r....r.
+00000910: 0000 00da 0974 6573 745f 7379 6e63 2e00  .....test_sync..
+00000920: 0000 7306 0000 0000 010c 0110 017a 1e41  ..s..........z.A
+00000930: 6273 7472 6163 7442 6173 6553 796e 6354  bstractBaseSyncT
+00000940: 6573 742e 7465 7374 5f73 796e 6363 0100  est.test_syncc..
+00000950: 0000 0000 0000 0900 0000 0400 0000 4300  ..............C.
+00000960: 0000 7364 0000 007c 006a 0083 0001 007c  ..sd...|.j.....|
+00000970: 006a 015c 037d 017d 027d 037c 0167 007c  .j.\.}.}.}.|.g.|
+00000980: 0367 037d 047c 006a 027c 0464 0164 0269  .g.}.|.j.|.d.d.i
+00000990: 018e 017d 057c 006a 037c 0383 017d 0664  ...}.|.j.|...}.d
+000009a0: 037d 077c 076a 047c 0674 057c 0283 0183  .}.|.j.|.t.|....
+000009b0: 027d 087c 006a 067c 087c 056a 0783 006a  .}.|.j.|.|.j...j
+000009c0: 0883 0083 0201 0064 0053 0029 044e 7221  .......d.S.).Nr!
+000009d0: 0000 0054 7a35 7b7d 2053 796e 6320 5375  ...Tz5{} Sync Su
+000009e0: 6d6d 6172 7920 2d20 4372 6561 7465 643a  mmary - Created:
+000009f0: 2030 2c20 5570 6461 7465 643a 2030 2c20   0, Updated: 0, 
+00000a00: 4465 6c65 7465 643a 207b 7d29 0972 2a00  Deleted: {}).r*.
+00000a10: 0000 7223 0000 0072 2400 0000 7225 0000  ..r#...r$...r%..
+00000a20: 0072 0b00 0000 da03 6c65 6eda 0b61 7373  .r......len..ass
+00000a30: 6572 7445 7175 616c 7228 0000 0072 2900  ertEqualr(...r).
+00000a40: 0000 2909 721d 0000 0072 1e00 0000 721f  ..).r....r....r.
+00000a50: 0000 0072 2000 0000 7223 0000 0072 2200  ...r ...r#...r".
+00000a60: 0000 5a09 6f62 6a5f 6c61 6265 6c5a 086d  ..Z.obj_labelZ.m
+00000a70: 7367 5f74 6d70 6cda 036d 7367 720d 0000  sg_tmpl..msgr...
+00000a80: 0072 0d00 0000 720e 0000 00da 0e74 6573  .r....r......tes
+00000a90: 745f 6675 6c6c 5f73 796e 6333 0000 0073  t_full_sync3...s
+00000aa0: 1400 0000 0001 0801 0c02 0201 0201 0603  ................
+00000ab0: 1001 0a01 0401 1001 7a23 4162 7374 7261  ........z#Abstra
+00000ac0: 6374 4261 7365 5379 6e63 5465 7374 2e74  ctBaseSyncTest.t
+00000ad0: 6573 745f 6675 6c6c 5f73 796e 634e 2901  est_full_syncN).
+00000ae0: 4629 07da 085f 5f6e 616d 655f 5fda 0a5f  F)...__name__.._
+00000af0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000b00: 6c6e 616d 655f 5f72 2400 0000 7225 0000  lname__r$...r%..
+00000b10: 0072 2a00 0000 722e 0000 0072 0d00 0000  .r*...r....r....
+00000b20: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00000b30: 1700 0000 1e00 0000 7308 0000 0008 030a  ........s.......
+00000b40: 0a08 0308 0572 1700 0000 6300 0000 0000  .....r....c.....
+00000b50: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00000b60: 1a00 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
+00000b70: 6505 6a06 6401 6603 5a07 6402 5300 2903  e.j.d.f.Z.d.S.).
+00000b80: da18 5465 7374 5379 6e63 4361 6c65 6e64  ..TestSyncCalend
+00000b90: 6172 7343 6f6d 6d61 6e64 da08 6361 6c65  arsCommand..cale
+00000ba0: 6e64 6172 4e29 0872 2f00 0000 7230 0000  ndarN).r/...r0..
+00000bb0: 0072 3100 0000 7206 0000 00da 1f73 6368  .r1...r......sch
+00000bc0: 6564 756c 655f 6170 695f 6765 745f 6361  edule_api_get_ca
+00000bd0: 6c65 6e64 6172 735f 6361 6c6c 7207 0000  lendars_callr...
+00000be0: 00da 1a41 5049 5f53 4348 4544 554c 455f  ...API_SCHEDULE_
+00000bf0: 4341 4c45 4e44 4152 5f4c 4953 5472 2300  CALENDAR_LISTr#.
+00000c00: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00000c10: 0072 0e00 0000 7232 0000 0043 0000 0073  .r....r2...C...s
+00000c20: 0600 0000 0802 0401 0401 7232 0000 0063  ..........r2...c
+00000c30: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000c40: 4000 0000 7322 0000 0065 005a 0164 005a  @...s"...e.Z.d.Z
+00000c50: 0265 036a 0465 056a 0664 0166 035a 0764  .e.j.e.j.d.f.Z.d
+00000c60: 0264 0384 005a 0864 0453 0029 05da 1654  .d...Z.d.S.)...T
+00000c70: 6573 7453 796e 6348 6f6c 6964 6179 436f  estSyncHolidayCo
+00000c80: 6d6d 616e 64da 0768 6f6c 6964 6179 6301  mmand..holidayc.
+00000c90: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00000ca0: 0000 0073 0c00 0000 7400 6a01 8300 0100  ...s....t.j.....
+00000cb0: 6400 5300 2901 4e29 0272 0800 0000 5a12  d.S.).N).r....Z.
+00000cc0: 696e 6974 5f68 6f6c 6964 6179 5f6c 6973  init_holiday_lis
+00000cd0: 7473 2901 721d 0000 0072 0d00 0000 720d  ts).r....r....r.
+00000ce0: 0000 0072 0e00 0000 da05 7365 7455 7052  ...r......setUpR
+00000cf0: 0000 0073 0200 0000 0001 7a1c 5465 7374  ...s......z.Test
+00000d00: 5379 6e63 486f 6c69 6461 7943 6f6d 6d61  SyncHolidayComma
+00000d10: 6e64 2e73 6574 5570 4e29 0972 2f00 0000  nd.setUpN).r/...
+00000d20: 7230 0000 0072 3100 0000 7206 0000 00da  r0...r1...r.....
+00000d30: 1e73 6368 6564 756c 655f 6170 695f 6765  .schedule_api_ge
+00000d40: 745f 686f 6c69 6461 7973 5f63 616c 6c72  t_holidays_callr
+00000d50: 0700 0000 da1f 4150 495f 5343 4845 4455  ......API_SCHEDU
+00000d60: 4c45 5f48 4f4c 4944 4159 5f4d 4f44 454c  LE_HOLIDAY_MODEL
+00000d70: 5f4c 4953 5472 2300 0000 7238 0000 0072  _LISTr#...r8...r
+00000d80: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+00000d90: 0000 0072 3600 0000 4b00 0000 7308 0000  ...r6...K...s...
+00000da0: 0008 0204 0104 0106 0372 3600 0000 6300  .........r6...c.
+00000db0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00000dc0: 0000 0073 1a00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000dd0: 6503 6a04 6505 6a06 6401 6603 5a07 6402  e.j.e.j.d.f.Z.d.
+00000de0: 5300 2903 da1a 5465 7374 5379 6e63 486f  S.)...TestSyncHo
+00000df0: 6c69 6461 794c 6973 7443 6f6d 6d61 6e64  lidayListCommand
+00000e00: da0c 686f 6c69 6461 795f 6c69 7374 4e29  ..holiday_listN)
+00000e10: 0872 2f00 0000 7230 0000 0072 3100 0000  .r/...r0...r1...
+00000e20: 7206 0000 00da 2373 6368 6564 756c 655f  r.....#schedule_
+00000e30: 6170 695f 6765 745f 686f 6c69 6461 795f  api_get_holiday_
+00000e40: 6c69 7374 735f 6361 6c6c 7207 0000 00da  lists_callr.....
+00000e50: 1e41 5049 5f53 4348 4544 554c 455f 484f  .API_SCHEDULE_HO
+00000e60: 4c49 4441 595f 4c49 5354 5f4c 4953 5472  LIDAY_LIST_LISTr
+00000e70: 2300 0000 720d 0000 0072 0d00 0000 720d  #...r....r....r.
+00000e80: 0000 0072 0e00 0000 723b 0000 0056 0000  ...r....r;...V..
+00000e90: 0073 0600 0000 0802 0401 0401 723b 0000  .s..........r;..
+00000ea0: 0063 0000 0000 0000 0000 0000 0000 0300  .c..............
+00000eb0: 0000 4000 0000 731a 0000 0065 005a 0164  ..@...s....e.Z.d
+00000ec0: 005a 0265 036a 0465 056a 0664 0166 035a  .Z.e.j.e.j.d.f.Z
+00000ed0: 0764 0253 0029 03da 1e54 6573 7453 796e  .d.S.)...TestSyn
+00000ee0: 6343 6f6d 7061 6e79 5374 6174 7573 6573  cCompanyStatuses
+00000ef0: 436f 6d6d 616e 64da 0e63 6f6d 7061 6e79  Command..company
+00000f00: 5f73 7461 7475 734e 2908 722f 0000 0072  _statusN).r/...r
+00000f10: 3000 0000 7231 0000 0072 0600 0000 da25  0...r1...r.....%
+00000f20: 636f 6d70 616e 795f 6170 695f 6765 745f  company_api_get_
+00000f30: 636f 6d70 616e 795f 7374 6174 7573 6573  company_statuses
+00000f40: 5f63 616c 6c72 0700 0000 da17 4150 495f  _callr......API_
+00000f50: 434f 4d50 414e 595f 5354 4154 5553 5f4c  COMPANY_STATUS_L
+00000f60: 4953 5472 2300 0000 720d 0000 0072 0d00  ISTr#...r....r..
+00000f70: 0000 720d 0000 0072 0e00 0000 723f 0000  ..r....r....r?..
+00000f80: 005e 0000 0073 0600 0000 0802 0401 0401  .^...s..........
+00000f90: 723f 0000 0063 0000 0000 0000 0000 0000  r?...c..........
+00000fa0: 0000 0300 0000 4000 0000 731a 0000 0065  ......@...s....e
+00000fb0: 005a 0164 005a 0265 036a 0465 056a 0664  .Z.d.Z.e.j.e.j.d
+00000fc0: 0166 035a 0764 0253 0029 03da 1a54 6573  .f.Z.d.S.)...Tes
+00000fd0: 7453 796e 6354 6572 7269 746f 7269 6573  tSyncTerritories
+00000fe0: 436f 6d6d 616e 64da 0974 6572 7269 746f  Command..territo
+00000ff0: 7279 4e29 0872 2f00 0000 7230 0000 0072  ryN).r/...r0...r
+00001000: 3100 0000 7206 0000 00da 1f73 7973 7465  1...r......syste
+00001010: 6d5f 6170 695f 6765 745f 7465 7272 6974  m_api_get_territ
+00001020: 6f72 6965 735f 6361 6c6c 7207 0000 00da  ories_callr.....
+00001030: 1941 5049 5f53 5953 5445 4d5f 5445 5252  .API_SYSTEM_TERR
+00001040: 4954 4f52 595f 4c49 5354 7223 0000 0072  ITORY_LISTr#...r
+00001050: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+00001060: 0000 0072 4300 0000 6600 0000 7306 0000  ...rC...f...s...
+00001070: 0008 0204 0104 0172 4300 0000 6300 0000  .......rC...c...
+00001080: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+00001090: 0073 2a00 0000 6500 5a01 6400 5a02 8700  .s*...e.Z.d.Z...
+000010a0: 6601 6401 6402 8408 5a03 6504 6a05 6506  f.d.d...Z.e.j.e.
+000010b0: 6a07 6403 6603 5a08 8700 0400 5a09 5300  j.d.f.Z.....Z.S.
+000010c0: 2904 da18 5465 7374 5379 6e63 436f 6d70  )...TestSyncComp
+000010d0: 616e 6965 7343 6f6d 6d61 6e64 6301 0000  aniesCommandc...
+000010e0: 0000 0000 0001 0000 0001 0000 0003 0000  ................
+000010f0: 0073 1600 0000 7400 8300 6a01 8300 0100  .s....t...j.....
+00001100: 7402 6a03 8300 0100 6400 5300 2901 4e29  t.j.....d.S.).N)
+00001110: 04da 0573 7570 6572 7238 0000 0072 0800  ...superr8...r..
+00001120: 0000 da10 696e 6974 5f74 6572 7269 746f  ....init_territo
+00001130: 7269 6573 2901 721d 0000 0029 01da 095f  ries).r....)..._
+00001140: 5f63 6c61 7373 5f5f 720d 0000 0072 0e00  _class__r....r..
+00001150: 0000 7238 0000 006f 0000 0073 0400 0000  ..r8...o...s....
+00001160: 0001 0a01 7a1e 5465 7374 5379 6e63 436f  ....z.TestSyncCo
+00001170: 6d70 616e 6965 7343 6f6d 6d61 6e64 2e73  mpaniesCommand.s
+00001180: 6574 5570 da07 636f 6d70 616e 7929 0a72  etUp..company).r
+00001190: 2f00 0000 7230 0000 0072 3100 0000 7238  /...r0...r1...r8
+000011a0: 0000 0072 0600 0000 da14 636f 6d70 616e  ...r......compan
+000011b0: 795f 6170 695f 6765 745f 6361 6c6c 7207  y_api_get_callr.
+000011c0: 0000 00da 1041 5049 5f43 4f4d 5041 4e59  .....API_COMPANY
+000011d0: 5f4c 4953 5472 2300 0000 da0d 5f5f 636c  _LISTr#.....__cl
+000011e0: 6173 7363 656c 6c5f 5f72 0d00 0000 720d  asscell__r....r.
+000011f0: 0000 0029 0172 4a00 0000 720e 0000 0072  ...).rJ...r....r
+00001200: 4700 0000 6e00 0000 7308 0000 0008 010c  G...n...s.......
+00001210: 0504 0104 0172 4700 0000 6300 0000 0000  .....rG...c.....
+00001220: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00001230: 1a00 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
+00001240: 6505 6a06 6401 6603 5a07 6402 5300 2903  e.j.d.f.Z.d.S.).
+00001250: da1b 5465 7374 5379 6e63 436f 6d70 616e  ..TestSyncCompan
+00001260: 7954 7970 6573 436f 6d6d 616e 64da 0c63  yTypesCommand..c
+00001270: 6f6d 7061 6e79 5f74 7970 654e 2908 722f  ompany_typeN).r/
+00001280: 0000 0072 3000 0000 7231 0000 0072 0600  ...r0...r1...r..
+00001290: 0000 da22 636f 6d70 616e 795f 6170 695f  ..."company_api_
+000012a0: 6765 745f 636f 6d70 616e 795f 7479 7065  get_company_type
+000012b0: 735f 6361 6c6c 7207 0000 00da 1641 5049  s_callr......API
+000012c0: 5f43 4f4d 5041 4e59 5f54 5950 4553 5f4c  _COMPANY_TYPES_L
+000012d0: 4953 5472 2300 0000 720d 0000 0072 0d00  ISTr#...r....r..
+000012e0: 0000 720d 0000 0072 0e00 0000 724f 0000  ..r....r....rO..
+000012f0: 007a 0000 0073 0600 0000 0802 0401 0401  .z...s..........
+00001300: 724f 0000 0063 0000 0000 0000 0000 0000  rO...c..........
+00001310: 0000 0300 0000 0000 0000 732a 0000 0065  ..........s*...e
+00001320: 005a 0164 005a 0265 036a 0465 056a 0664  .Z.d.Z.e.j.e.j.d
+00001330: 0166 035a 0787 0066 0164 0264 0384 085a  .f.Z...f.d.d...Z
+00001340: 0887 0004 005a 0953 0029 04da 1454 6573  .....Z.S.)...Tes
+00001350: 7453 796e 6354 6561 6d73 436f 6d6d 616e  tSyncTeamsComman
+00001360: 64da 0474 6561 6d63 0100 0000 0000 0000  d..teamc........
+00001370: 0100 0000 0100 0000 0300 0000 7316 0000  ............s...
+00001380: 0074 0083 006a 0183 0001 0074 026a 0383  .t...j.....t.j..
+00001390: 0001 0064 0053 0029 014e 2904 7248 0000  ...d.S.).N).rH..
+000013a0: 0072 3800 0000 7208 0000 00da 0b69 6e69  .r8...r......ini
+000013b0: 745f 626f 6172 6473 2901 721d 0000 0029  t_boards).r....)
+000013c0: 0172 4a00 0000 720d 0000 0072 0e00 0000  .rJ...r....r....
+000013d0: 7238 0000 0089 0000 0073 0400 0000 0001  r8.......s......
+000013e0: 0a01 7a1a 5465 7374 5379 6e63 5465 616d  ..z.TestSyncTeam
+000013f0: 7343 6f6d 6d61 6e64 2e73 6574 5570 290a  sCommand.setUp).
+00001400: 722f 0000 0072 3000 0000 7231 0000 0072  r/...r0...r1...r
+00001410: 0600 0000 da1a 7365 7276 6963 655f 6170  ......service_ap
+00001420: 695f 6765 745f 7465 616d 735f 6361 6c6c  i_get_teams_call
+00001430: 7207 0000 00da 1541 5049 5f53 4552 5649  r......API_SERVI
+00001440: 4345 5f54 4541 4d5f 4c49 5354 7223 0000  CE_TEAM_LISTr#..
+00001450: 0072 3800 0000 724e 0000 0072 0d00 0000  .r8...rN...r....
+00001460: 720d 0000 0029 0172 4a00 0000 720e 0000  r....).rJ...r...
+00001470: 0072 5300 0000 8200 0000 7308 0000 0008  .rS.......s.....
+00001480: 0204 0104 0106 0372 5300 0000 6300 0000  .......rS...c...
+00001490: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000014a0: 0073 1a00 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
+000014b0: 6a04 6505 6a06 6401 6603 5a07 6402 5300  j.e.j.d.f.Z.d.S.
+000014c0: 2903 da15 5465 7374 5379 6e63 426f 6172  )...TestSyncBoar
+000014d0: 6473 436f 6d6d 616e 64da 0562 6f61 7264  dsCommand..board
+000014e0: 4e29 0872 2f00 0000 7230 0000 0072 3100  N).r/...r0...r1.
+000014f0: 0000 7206 0000 00da 1b73 6572 7669 6365  ..r......service
+00001500: 5f61 7069 5f67 6574 5f62 6f61 7264 735f  _api_get_boards_
+00001510: 6361 6c6c 7207 0000 00da 0e41 5049 5f42  callr......API_B
+00001520: 4f41 5244 5f4c 4953 5472 2300 0000 720d  OARD_LISTr#...r.
+00001530: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00001540: 0000 7258 0000 008e 0000 0073 0600 0000  ..rX.......s....
+00001550: 0802 0401 0401 7258 0000 0063 0000 0000  ......rX...c....
+00001560: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00001570: 731a 0000 0065 005a 0164 005a 0265 036a  s....e.Z.d.Z.e.j
+00001580: 0465 056a 0664 0166 035a 0764 0253 0029  .e.j.d.f.Z.d.S.)
+00001590: 03da 1854 6573 7453 796e 634c 6f63 6174  ...TestSyncLocat
+000015a0: 696f 6e73 436f 6d6d 616e 64da 086c 6f63  ionsCommand..loc
+000015b0: 6174 696f 6e4e 2908 722f 0000 0072 3000  ationN).r/...r0.
+000015c0: 0000 7231 0000 0072 0600 0000 da1e 7365  ..r1...r......se
+000015d0: 7276 6963 655f 6170 695f 6765 745f 6c6f  rvice_api_get_lo
+000015e0: 6361 7469 6f6e 735f 6361 6c6c 7207 0000  cations_callr...
+000015f0: 00da 1941 5049 5f53 4552 5649 4345 5f4c  ...API_SERVICE_L
+00001600: 4f43 4154 494f 4e5f 4c49 5354 7223 0000  OCATION_LISTr#..
+00001610: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00001620: 720e 0000 0072 5c00 0000 9600 0000 7306  r....r\.......s.
+00001630: 0000 0008 0204 0104 0172 5c00 0000 6300  .........r\...c.
+00001640: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00001650: 0000 0073 2200 0000 6500 5a01 6400 5a02  ...s"...e.Z.d.Z.
+00001660: 6503 6a04 6505 6a06 6401 6603 5a07 6402  e.j.e.j.d.f.Z.d.
+00001670: 6403 8400 5a08 6404 5300 2905 da1d 5465  d...Z.d.S.)...Te
+00001680: 7374 5379 6e63 4d79 436f 6d70 616e 794f  stSyncMyCompanyO
+00001690: 7468 6572 436f 6d6d 616e 64da 0d63 6f6d  therCommand..com
+000016a0: 7061 6e79 5f6f 7468 6572 6301 0000 0000  pany_otherc.....
+000016b0: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
+000016c0: 0c00 0000 7400 6a01 8300 0100 6400 5300  ....t.j.....d.S.
+000016d0: 2901 4e29 0272 0800 0000 da0e 696e 6974  ).N).r......init
+000016e0: 5f63 616c 656e 6461 7273 2901 721d 0000  _calendars).r...
+000016f0: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+00001700: 7238 0000 00a5 0000 0073 0200 0000 0001  r8.......s......
+00001710: 7a23 5465 7374 5379 6e63 4d79 436f 6d70  z#TestSyncMyComp
+00001720: 616e 794f 7468 6572 436f 6d6d 616e 642e  anyOtherCommand.
+00001730: 7365 7455 704e 2909 722f 0000 0072 3000  setUpN).r/...r0.
+00001740: 0000 7231 0000 0072 0600 0000 da19 7379  ..r1...r......sy
+00001750: 7374 656d 5f61 7069 5f67 6574 5f6f 7468  stem_api_get_oth
+00001760: 6572 5f63 616c 6c72 0700 0000 da15 4150  er_callr......AP
+00001770: 495f 5359 5354 454d 5f4f 5448 4552 5f4c  I_SYSTEM_OTHER_L
+00001780: 4953 5472 2300 0000 7238 0000 0072 0d00  ISTr#...r8...r..
+00001790: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+000017a0: 0072 6000 0000 9e00 0000 7308 0000 0008  .r`.......s.....
+000017b0: 0204 0104 0106 0372 6000 0000 6300 0000  .......r`...c...
+000017c0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000017d0: 0073 1a00 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
+000017e0: 6a04 6505 6a06 6401 6603 5a07 6402 5300  j.e.j.d.f.Z.d.S.
+000017f0: 2903 da19 5465 7374 5379 6e63 5072 696f  )...TestSyncPrio
+00001800: 7269 7469 6573 436f 6d6d 616e 64da 0870  ritiesCommand..p
+00001810: 7269 6f72 6974 794e 2908 722f 0000 0072  riorityN).r/...r
+00001820: 3000 0000 7231 0000 0072 0600 0000 da1f  0...r1...r......
+00001830: 7365 7276 6963 655f 6170 695f 6765 745f  service_api_get_
+00001840: 7072 696f 7269 7469 6573 5f63 616c 6c72  priorities_callr
+00001850: 0700 0000 da19 4150 495f 5345 5256 4943  ......API_SERVIC
+00001860: 455f 5052 494f 5249 5459 5f4c 4953 5472  E_PRIORITY_LISTr
+00001870: 2300 0000 720d 0000 0072 0d00 0000 720d  #...r....r....r.
+00001880: 0000 0072 0e00 0000 7265 0000 00a9 0000  ...r....re......
+00001890: 0073 0600 0000 0803 0401 0401 7265 0000  .s..........re..
+000018a0: 0063 0000 0000 0000 0000 0000 0000 0300  .c..............
+000018b0: 0000 4000 0000 731a 0000 0065 005a 0164  ..@...s....e.Z.d
+000018c0: 005a 0265 036a 0465 056a 0664 0166 035a  .Z.e.j.e.j.d.f.Z
+000018d0: 0764 0253 0029 03da 1e54 6573 7453 796e  .d.S.)...TestSyn
+000018e0: 6350 726f 6a65 6374 5374 6174 7573 6573  cProjectStatuses
+000018f0: 436f 6d6d 616e 64da 0e70 726f 6a65 6374  Command..project
+00001900: 5f73 7461 7475 734e 2908 722f 0000 0072  _statusN).r/...r
+00001910: 3000 0000 7231 0000 0072 0600 0000 da26  0...r1...r.....&
+00001920: 7072 6f6a 6563 7473 5f61 7069 5f67 6574  projects_api_get
+00001930: 5f70 726f 6a65 6374 5f73 7461 7475 7365  _project_statuse
+00001940: 735f 6361 6c6c 7207 0000 00da 1441 5049  s_callr......API
+00001950: 5f50 524f 4a45 4354 5f53 5441 5455 5345  _PROJECT_STATUSE
+00001960: 5372 2300 0000 720d 0000 0072 0d00 0000  Sr#...r....r....
+00001970: 720d 0000 0072 0e00 0000 7269 0000 00b2  r....r....ri....
+00001980: 0000 0073 0600 0000 0802 0401 0401 7269  ...s..........ri
+00001990: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000019a0: 0300 0000 4000 0000 731a 0000 0065 005a  ....@...s....e.Z
+000019b0: 0164 005a 0265 036a 0465 056a 0664 0166  .d.Z.e.j.e.j.d.f
+000019c0: 035a 0764 0253 0029 03da 1b54 6573 7453  .Z.d.S.)...TestS
+000019d0: 796e 6350 726f 6a65 6374 5479 7065 7343  yncProjectTypesC
+000019e0: 6f6d 6d61 6e64 da0c 7072 6f6a 6563 745f  ommand..project_
+000019f0: 7479 7065 4e29 0872 2f00 0000 7230 0000  typeN).r/...r0..
+00001a00: 0072 3100 0000 7206 0000 00da 2370 726f  .r1...r.....#pro
+00001a10: 6a65 6374 735f 6170 695f 6765 745f 7072  jects_api_get_pr
+00001a20: 6f6a 6563 745f 7479 7065 735f 6361 6c6c  oject_types_call
+00001a30: 7207 0000 00da 1141 5049 5f50 524f 4a45  r......API_PROJE
+00001a40: 4354 5f54 5950 4553 7223 0000 0072 0d00  CT_TYPESr#...r..
+00001a50: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00001a60: 0072 6d00 0000 ba00 0000 7306 0000 0008  .rm.......s.....
+00001a70: 0204 0104 0172 6d00 0000 6300 0000 0000  .....rm...c.....
+00001a80: 0000 0000 0000 0003 0000 0000 0000 0073  ...............s
+00001a90: 2a00 0000 6500 5a01 6400 5a02 6503 6a04  *...e.Z.d.Z.e.j.
+00001aa0: 6505 6a06 6401 6603 5a07 8700 6601 6402  e.j.d.f.Z...f.d.
+00001ab0: 6403 8408 5a08 8700 0400 5a09 5300 2904  d...Z.....Z.S.).
+00001ac0: da17 5465 7374 5379 6e63 5072 6f6a 6563  ..TestSyncProjec
+00001ad0: 7473 436f 6d6d 616e 64da 0770 726f 6a65  tsCommand..proje
+00001ae0: 6374 6301 0000 0000 0000 0001 0000 0001  ctc.............
+00001af0: 0000 0003 0000 0073 1600 0000 7400 8300  .......s....t...
+00001b00: 6a01 8300 0100 7402 6a03 8300 0100 6400  j.....t.j.....d.
+00001b10: 5300 2901 4e29 0472 4800 0000 7238 0000  S.).N).rH...r8..
+00001b20: 0072 0800 0000 da15 696e 6974 5f70 726f  .r......init_pro
+00001b30: 6a65 6374 5f73 7461 7475 7365 7329 0172  ject_statuses).r
+00001b40: 1d00 0000 2901 724a 0000 0072 0d00 0000  ....).rJ...r....
+00001b50: 720e 0000 0072 3800 0000 c900 0000 7304  r....r8.......s.
+00001b60: 0000 0000 010a 017a 1d54 6573 7453 796e  .......z.TestSyn
+00001b70: 6350 726f 6a65 6374 7343 6f6d 6d61 6e64  cProjectsCommand
+00001b80: 2e73 6574 5570 290a 722f 0000 0072 3000  .setUp).r/...r0.
+00001b90: 0000 7231 0000 0072 0600 0000 da1d 7072  ..r1...r......pr
+00001ba0: 6f6a 6563 745f 6170 695f 6765 745f 7072  oject_api_get_pr
+00001bb0: 6f6a 6563 7473 5f63 616c 6c72 0700 0000  ojects_callr....
+00001bc0: da10 4150 495f 5052 4f4a 4543 545f 4c49  ..API_PROJECT_LI
+00001bd0: 5354 7223 0000 0072 3800 0000 724e 0000  STr#...r8...rN..
+00001be0: 0072 0d00 0000 720d 0000 0029 0172 4a00  .r....r....).rJ.
+00001bf0: 0000 720e 0000 0072 7100 0000 c200 0000  ..r....rq.......
+00001c00: 7308 0000 0008 0204 0104 0106 0372 7100  s............rq.
+00001c10: 0000 6300 0000 0000 0000 0000 0000 0003  ..c.............
+00001c20: 0000 0000 0000 0073 2a00 0000 6500 5a01  .......s*...e.Z.
+00001c30: 6400 5a02 6503 6a04 6505 6a06 6401 6603  d.Z.e.j.e.j.d.f.
+00001c40: 5a07 8700 6601 6402 6403 8408 5a08 8700  Z...f.d.d...Z...
+00001c50: 0400 5a09 5300 2904 da1b 5465 7374 5379  ..Z.S.)...TestSy
+00001c60: 6e63 5072 6f6a 6563 7450 6861 7365 436f  ncProjectPhaseCo
+00001c70: 6d6d 616e 64da 0d70 726f 6a65 6374 5f70  mmand..project_p
+00001c80: 6861 7365 6301 0000 0000 0000 0001 0000  hasec...........
+00001c90: 0001 0000 0003 0000 0073 1e00 0000 7400  .........s....t.
+00001ca0: 8300 6a01 8300 0100 7402 6a03 8300 0100  ..j.....t.j.....
+00001cb0: 7402 6a04 8300 0100 6400 5300 2901 4e29  t.j.....d.S.).N)
+00001cc0: 0572 4800 0000 7238 0000 0072 0800 0000  .rH...r8...r....
+00001cd0: da0d 696e 6974 5f70 726f 6a65 6374 735a  ..init_projectsZ
+00001ce0: 1369 6e69 745f 7072 6f6a 6563 745f 7068  .init_project_ph
+00001cf0: 6173 6573 2901 721d 0000 0029 0172 4a00  ases).r....).rJ.
+00001d00: 0000 720d 0000 0072 0e00 0000 7238 0000  ..r....r....r8..
+00001d10: 00d5 0000 0073 0600 0000 0001 0a01 0801  .....s..........
+00001d20: 7a21 5465 7374 5379 6e63 5072 6f6a 6563  z!TestSyncProjec
+00001d30: 7450 6861 7365 436f 6d6d 616e 642e 7365  tPhaseCommand.se
+00001d40: 7455 7029 0a72 2f00 0000 7230 0000 0072  tUp).r/...r0...r
+00001d50: 3100 0000 7206 0000 00da 2470 726f 6a65  1...r.....$proje
+00001d60: 6374 735f 6170 695f 6765 745f 7072 6f6a  cts_api_get_proj
+00001d70: 6563 745f 7068 6173 6573 5f63 616c 6c72  ect_phases_callr
+00001d80: 0700 0000 da16 4150 495f 5052 4f4a 4543  ......API_PROJEC
+00001d90: 545f 5048 4153 455f 4c49 5354 7223 0000  T_PHASE_LISTr#..
+00001da0: 0072 3800 0000 724e 0000 0072 0d00 0000  .r8...rN...r....
+00001db0: 720d 0000 0029 0172 4a00 0000 720e 0000  r....).rJ...r...
+00001dc0: 0072 7600 0000 ce00 0000 7308 0000 0008  .rv.......s.....
+00001dd0: 0204 0104 0106 0372 7600 0000 6300 0000  .......rv...c...
+00001de0: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+00001df0: 0073 2a00 0000 6500 5a01 6400 5a02 6503  .s*...e.Z.d.Z.e.
+00001e00: 6a04 6505 6a06 6401 6603 5a07 8700 6601  j.e.j.d.f.Z...f.
+00001e10: 6402 6403 8408 5a08 8700 0400 5a09 5300  d.d...Z.....Z.S.
+00001e20: 2904 da20 5465 7374 5379 6e63 5072 6f6a  ).. TestSyncProj
+00001e30: 6563 7454 6561 6d4d 656d 6265 7243 6f6d  ectTeamMemberCom
+00001e40: 6d61 6e64 da13 7072 6f6a 6563 745f 7465  mand..project_te
+00001e50: 616d 5f6d 656d 6265 7263 0100 0000 0000  am_memberc......
+00001e60: 0000 0100 0000 0300 0000 0300 0000 734a  ..............sJ
+00001e70: 0000 0074 0083 006a 0183 0001 0074 026a  ...t...j.....t.j
+00001e80: 0374 026a 0474 026a 0583 0066 0283 0101  .t.j.t.j...f....
+00001e90: 0074 066a 0783 0001 0074 066a 0883 0001  .t.j.....t.j....
+00001ea0: 0074 066a 0983 0001 0074 066a 0a83 0001  .t.j.....t.j....
+00001eb0: 0074 066a 0b83 0001 0064 0053 0029 014e  .t.j.....d.S.).N
+00001ec0: 290c 7248 0000 0072 3800 0000 7206 0000  ).rH...r8...r...
+00001ed0: 00da 2c73 7973 7465 6d5f 6170 695f 6765  ..,system_api_ge
+00001ee0: 745f 6d65 6d62 6572 5f69 6d61 6765 5f62  t_member_image_b
+00001ef0: 795f 7068 6f74 6f5f 6964 5f63 616c 6cda  y_photo_id_call.
+00001f00: 1843 575f 4d45 4d42 4552 5f49 4d41 4745  .CW_MEMBER_IMAGE
+00001f10: 5f46 494c 454e 414d 45da 1167 6574 5f6d  _FILENAME..get_m
+00001f20: 656d 6265 725f 6176 6174 6172 7208 0000  ember_avatarr...
+00001f30: 00da 0c69 6e69 745f 6d65 6d62 6572 73da  ...init_members.
+00001f40: 0f69 6e69 745f 776f 726b 5f72 6f6c 6573  .init_work_roles
+00001f50: 7273 0000 0072 7800 0000 5a19 696e 6974  rs...rx...Z.init
+00001f60: 5f70 726f 6a65 6374 5f74 6561 6d5f 6d65  _project_team_me
+00001f70: 6d62 6572 7329 0172 1d00 0000 2901 724a  mbers).r....).rJ
+00001f80: 0000 0072 0d00 0000 720e 0000 0072 3800  ...r....r....r8.
+00001f90: 0000 e200 0000 7310 0000 0000 010a 0104  ......s.........
+00001fa0: 0110 0108 0108 0108 0108 017a 2654 6573  ...........z&Tes
+00001fb0: 7453 796e 6350 726f 6a65 6374 5465 616d  tSyncProjectTeam
+00001fc0: 4d65 6d62 6572 436f 6d6d 616e 642e 7365  MemberCommand.se
+00001fd0: 7455 7029 0a72 2f00 0000 7230 0000 0072  tUp).r/...r0...r
+00001fe0: 3100 0000 7206 0000 00da 2170 726f 6a65  1...r.....!proje
+00001ff0: 6374 5f61 7069 5f67 6574 5f74 6561 6d5f  ct_api_get_team_
+00002000: 6d65 6d62 6572 735f 6361 6c6c 7207 0000  members_callr...
+00002010: 00da 1c41 5049 5f50 524f 4a45 4354 5f54  ...API_PROJECT_T
+00002020: 4541 4d5f 4d45 4d42 4552 5f4c 4953 5472  EAM_MEMBER_LISTr
+00002030: 2300 0000 7238 0000 0072 4e00 0000 720d  #...r8...rN...r.
+00002040: 0000 0072 0d00 0000 2901 724a 0000 0072  ...r....).rJ...r
+00002050: 0e00 0000 727b 0000 00db 0000 0073 0800  ....r{.......s..
+00002060: 0000 0802 0401 0401 0603 727b 0000 0063  ..........r{...c
+00002070: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00002080: 4000 0000 7322 0000 0065 005a 0164 005a  @...s"...e.Z.d.Z
+00002090: 0265 036a 0465 056a 0664 0166 035a 0764  .e.j.e.j.d.f.Z.d
+000020a0: 0264 0384 005a 0864 0453 0029 05da 1d54  .d...Z.d.S.)...T
+000020b0: 6573 7453 796e 6342 6f61 7264 7353 7461  estSyncBoardsSta
+000020c0: 7475 7365 7343 6f6d 6d61 6e64 da0c 626f  tusesCommand..bo
+000020d0: 6172 645f 7374 6174 7573 6301 0000 0000  ard_statusc.....
+000020e0: 0000 0004 0000 0002 0000 0043 0000 0073  ...........C...s
+000020f0: 3c00 0000 7400 6a01 8300 7d01 7402 6a03  <...t.j...}.t.j.
+00002100: 6a04 6a05 8300 6a06 8300 0100 7407 6a08  j.j...j.....t.j.
+00002110: 7409 6a0a 8301 5c02 7d02 7d03 7c01 6a00  t.j...\.}.}.|.j.
+00002120: 8300 0100 7c03 6a0b 8300 0100 6400 5300  ....|.j.....d.S.
+00002130: 2901 4e29 0c72 0a00 0000 5a11 426f 6172  ).N).r....Z.Boar
+00002140: 6453 796e 6368 726f 6e69 7a65 7272 0400  dSynchronizerr..
+00002150: 0000 da10 436f 6e6e 6563 7457 6973 6542  ....ConnectWiseB
+00002160: 6f61 7264 da07 6f62 6a65 6374 73da 0361  oard..objects..a
+00002170: 6c6c da06 6465 6c65 7465 7206 0000 0072  ll..deleter....r
+00002180: 5a00 0000 7207 0000 0072 5b00 0000 da04  Z...r....r[.....
+00002190: 7374 6f70 2904 721d 0000 005a 1262 6f61  stop).r....Z.boa
+000021a0: 7264 5f73 796e 6368 726f 6e69 7a65 7272  rd_synchronizerr
+000021b0: 1100 0000 da06 5f70 6174 6368 720d 0000  ......_patchr...
+000021c0: 0072 0d00 0000 720e 0000 0072 3800 0000  .r....r....r8...
+000021d0: f400 0000 730a 0000 0000 0108 0110 0110  ....s...........
+000021e0: 0108 017a 2354 6573 7453 796e 6342 6f61  ...z#TestSyncBoa
+000021f0: 7264 7353 7461 7475 7365 7343 6f6d 6d61  rdsStatusesComma
+00002200: 6e64 2e73 6574 5570 4e29 0972 2f00 0000  nd.setUpN).r/...
+00002210: 7230 0000 0072 3100 0000 7206 0000 00da  r0...r1...r.....
+00002220: 1d73 6572 7669 6365 5f61 7069 5f67 6574  .service_api_get
+00002230: 5f73 7461 7475 7365 735f 6361 6c6c 7207  _statuses_callr.
+00002240: 0000 00da 1541 5049 5f42 4f41 5244 5f53  .....API_BOARD_S
+00002250: 5441 5455 535f 4c49 5354 7223 0000 0072  TATUS_LISTr#...r
+00002260: 3800 0000 720d 0000 0072 0d00 0000 720d  8...r....r....r.
+00002270: 0000 0072 0e00 0000 7284 0000 00ed 0000  ...r....r.......
+00002280: 0073 0800 0000 0802 0401 0401 0603 7284  .s............r.
+00002290: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000022a0: 0300 0000 4000 0000 7322 0000 0065 005a  ....@...s"...e.Z
+000022b0: 0164 005a 0265 036a 0465 056a 0664 0166  .d.Z.e.j.e.j.d.f
+000022c0: 035a 0764 0264 0384 005a 0864 0453 0029  .Z.d.d...Z.d.S.)
+000022d0: 05da 1354 6573 7453 796e 6353 4c41 7343  ...TestSyncSLAsC
+000022e0: 6f6d 6d61 6e64 da03 736c 6163 0100 0000  ommand..slac....
+000022f0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00002300: 730c 0000 0074 006a 0183 0001 0064 0053  s....t.j.....d.S
+00002310: 0029 014e 2902 7208 0000 0072 6200 0000  .).N).r....rb...
+00002320: 2901 721d 0000 0072 0d00 0000 720d 0000  ).r....r....r...
+00002330: 0072 0e00 0000 7238 0000 0003 0100 0073  .r....r8.......s
+00002340: 0200 0000 0001 7a19 5465 7374 5379 6e63  ......z.TestSync
+00002350: 534c 4173 436f 6d6d 616e 642e 7365 7455  SLAsCommand.setU
+00002360: 704e 2909 722f 0000 0072 3000 0000 7231  pN).r/...r0...r1
+00002370: 0000 0072 0600 0000 da19 7365 7276 6963  ...r......servic
+00002380: 655f 6170 695f 6765 745f 736c 6173 5f63  e_api_get_slas_c
+00002390: 616c 6c72 0700 0000 da14 4150 495f 5345  allr......API_SE
+000023a0: 5256 4943 455f 534c 415f 4c49 5354 7223  RVICE_SLA_LISTr#
+000023b0: 0000 0072 3800 0000 720d 0000 0072 0d00  ...r8...r....r..
+000023c0: 0000 720d 0000 0072 0e00 0000 728e 0000  ..r....r....r...
+000023d0: 00fc 0000 0073 0800 0000 0802 0401 0401  .....s..........
+000023e0: 0603 728e 0000 0063 0000 0000 0000 0000  ..r....c........
+000023f0: 0000 0000 0300 0000 4000 0000 7322 0000  ........@...s"..
+00002400: 0065 005a 0164 005a 0265 036a 0465 056a  .e.Z.d.Z.e.j.e.j
+00002410: 0664 0166 035a 0764 0264 0384 005a 0864  .d.f.Z.d.d...Z.d
+00002420: 0453 0029 05da 1c54 6573 7453 796e 6353  .S.)...TestSyncS
+00002430: 4c41 5072 696f 7269 7469 6573 436f 6d6d  LAPrioritiesComm
+00002440: 616e 64da 0c73 6c61 5f70 7269 6f72 6974  and..sla_priorit
+00002450: 7963 0100 0000 0000 0000 0100 0000 0100  yc..............
+00002460: 0000 4300 0000 731c 0000 0074 006a 0183  ..C...s....t.j..
+00002470: 0001 0074 006a 0283 0001 0074 006a 0383  ...t.j.....t.j..
+00002480: 0001 0064 0053 0029 014e 2904 7208 0000  ...d.S.).N).r...
+00002490: 0072 6200 0000 5a09 696e 6974 5f73 6c61  .rb...Z.init_sla
+000024a0: 73da 0f69 6e69 745f 7072 696f 7269 7469  s..init_prioriti
+000024b0: 6573 2901 721d 0000 0072 0d00 0000 720d  es).r....r....r.
+000024c0: 0000 0072 0e00 0000 7238 0000 000e 0100  ...r....r8......
+000024d0: 0073 0600 0000 0001 0801 0801 7a22 5465  .s..........z"Te
+000024e0: 7374 5379 6e63 534c 4150 7269 6f72 6974  stSyncSLAPriorit
+000024f0: 6965 7343 6f6d 6d61 6e64 2e73 6574 5570  iesCommand.setUp
+00002500: 4e29 0972 2f00 0000 7230 0000 0072 3100  N).r/...r0...r1.
+00002510: 0000 7206 0000 00da 2373 6572 7669 6365  ..r.....#service
+00002520: 5f61 7069 5f67 6574 5f73 6c61 5f70 7269  _api_get_sla_pri
+00002530: 6f72 6974 6965 735f 6361 6c6c 7207 0000  orities_callr...
+00002540: 00da 1d41 5049 5f53 4552 5649 4345 5f53  ...API_SERVICE_S
+00002550: 4c41 5f50 5249 4f52 4954 595f 4c49 5354  LA_PRIORITY_LIST
+00002560: 7223 0000 0072 3800 0000 720d 0000 0072  r#...r8...r....r
+00002570: 0d00 0000 720d 0000 0072 0e00 0000 7292  ....r....r....r.
+00002580: 0000 0007 0100 0073 0800 0000 0802 0401  .......s........
+00002590: 0401 0603 7292 0000 0063 0000 0000 0000  ....r....c......
+000025a0: 0000 0000 0000 0300 0000 0000 0000 732a  ..............s*
+000025b0: 0000 0065 005a 0164 005a 0265 036a 0465  ...e.Z.d.Z.e.j.e
+000025c0: 056a 0664 0166 035a 0787 0066 0164 0264  .j.d.f.Z...f.d.d
+000025d0: 0384 085a 0887 0004 005a 0953 0029 04da  ...Z.....Z.S.)..
+000025e0: 1b54 6573 7453 796e 6353 6572 7669 6365  .TestSyncService
+000025f0: 4e6f 7465 7343 6f6d 6d61 6e64 da0c 7365  NotesCommand..se
+00002600: 7276 6963 655f 6e6f 7465 6301 0000 0000  rvice_notec.....
+00002610: 0000 0001 0000 0001 0000 0003 0000 0073  ...............s
+00002620: 4600 0000 7400 8300 6a01 8300 0100 7402  F...t...j.....t.
+00002630: 6a03 8300 0100 7402 6a04 8300 0100 7402  j.....t.j.....t.
+00002640: 6a05 8300 0100 7402 6a06 8300 0100 7402  j.....t.j.....t.
+00002650: 6a07 8300 0100 7402 6a08 8300 0100 7402  j.....t.j.....t.
+00002660: 6a09 8300 0100 6400 5300 2901 4e29 0a72  j.....d.S.).N).r
+00002670: 4800 0000 7238 0000 0072 0800 0000 5a12  H...r8...r....Z.
+00002680: 696e 6974 5f73 6572 7669 6365 5f6e 6f74  init_service_not
+00002690: 6573 7280 0000 0072 4900 0000 da0e 696e  esr....rI.....in
+000026a0: 6974 5f63 6f6d 7061 6e69 6573 7255 0000  it_companiesrU..
+000026b0: 00da 1369 6e69 745f 626f 6172 645f 7374  ...init_board_st
+000026c0: 6174 7573 6573 da0c 696e 6974 5f74 6963  atuses..init_tic
+000026d0: 6b65 7473 2901 721d 0000 0029 0172 4a00  kets).r....).rJ.
+000026e0: 0000 720d 0000 0072 0e00 0000 7238 0000  ..r....r....r8..
+000026f0: 001b 0100 0073 1000 0000 0001 0a01 0801  .....s..........
+00002700: 0801 0801 0801 0801 0801 7a21 5465 7374  ..........z!Test
+00002710: 5379 6e63 5365 7276 6963 654e 6f74 6573  SyncServiceNotes
+00002720: 436f 6d6d 616e 642e 7365 7455 7029 0a72  Command.setUp).r
+00002730: 2f00 0000 7230 0000 0072 3100 0000 7206  /...r0...r1...r.
+00002740: 0000 00da 1a73 6572 7669 6365 5f61 7069  .....service_api
+00002750: 5f67 6574 5f6e 6f74 6573 5f63 616c 6c72  _get_notes_callr
+00002760: 0700 0000 da15 4150 495f 5345 5256 4943  ......API_SERVIC
+00002770: 455f 4e4f 5445 5f4c 4953 5472 2300 0000  E_NOTE_LISTr#...
+00002780: 7238 0000 0072 4e00 0000 720d 0000 0072  r8...rN...r....r
+00002790: 0d00 0000 2901 724a 0000 0072 0e00 0000  ....).rJ...r....
+000027a0: 7297 0000 0014 0100 0073 0800 0000 0802  r........s......
+000027b0: 0401 0401 0603 7297 0000 0063 0000 0000  ......r....c....
+000027c0: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+000027d0: 732a 0000 0065 005a 0164 005a 0265 036a  s*...e.Z.d.Z.e.j
+000027e0: 0465 056a 0664 0166 035a 0787 0066 0164  .e.j.d.f.Z...f.d
+000027f0: 0264 0384 085a 0887 0004 005a 0953 0029  .d...Z.....Z.S.)
+00002800: 04da 1f54 6573 7453 796e 634f 7070 6f72  ...TestSyncOppor
+00002810: 7475 6e69 7479 4e6f 7465 7343 6f6d 6d61  tunityNotesComma
+00002820: 6e64 da10 6f70 706f 7274 756e 6974 795f  nd..opportunity_
+00002830: 6e6f 7465 6301 0000 0000 0000 0001 0000  notec...........
+00002840: 0001 0000 0003 0000 0073 3600 0000 7400  .........s6...t.
+00002850: 8300 6a01 8300 0100 7402 6a03 8300 0100  ..j.....t.j.....
+00002860: 7402 6a04 8300 0100 7402 6a05 8300 0100  t.j.....t.j.....
+00002870: 7402 6a06 8300 0100 7402 6a07 8300 0100  t.j.....t.j.....
+00002880: 6400 5300 2901 4e29 0872 4800 0000 7238  d.S.).N).rH...r8
+00002890: 0000 0072 0800 0000 da19 696e 6974 5f6f  ...r......init_o
+000028a0: 7070 6f72 7475 6e69 7479 5f73 7461 7475  pportunity_statu
+000028b0: 7365 73da 1769 6e69 745f 6f70 706f 7274  ses..init_opport
+000028c0: 756e 6974 795f 7374 6167 6573 da16 696e  unity_stages..in
+000028d0: 6974 5f6f 7070 6f72 7475 6e69 7479 5f74  it_opportunity_t
+000028e0: 7970 6573 da12 696e 6974 5f6f 7070 6f72  ypes..init_oppor
+000028f0: 7475 6e69 7469 6573 5a16 696e 6974 5f6f  tunitiesZ.init_o
+00002900: 7070 6f72 7475 6e69 7479 5f6e 6f74 6573  pportunity_notes
+00002910: 2901 721d 0000 0029 0172 4a00 0000 720d  ).r....).rJ...r.
+00002920: 0000 0072 0e00 0000 7238 0000 002d 0100  ...r....r8...-..
+00002930: 0073 0c00 0000 0001 0a01 0801 0801 0801  .s..............
+00002940: 0801 7a25 5465 7374 5379 6e63 4f70 706f  ..z%TestSyncOppo
+00002950: 7274 756e 6974 794e 6f74 6573 436f 6d6d  rtunityNotesComm
+00002960: 616e 642e 7365 7455 7029 0a72 2f00 0000  and.setUp).r/...
+00002970: 7230 0000 0072 3100 0000 7206 0000 00da  r0...r1...r.....
+00002980: 2473 616c 6573 5f61 7069 5f67 6574 5f6f  $sales_api_get_o
+00002990: 7070 6f72 7475 6e69 7479 5f6e 6f74 6573  pportunity_notes
+000029a0: 5f63 616c 6c72 0700 0000 da1f 4150 495f  _callr......API_
+000029b0: 5341 4c45 535f 4f50 504f 5254 554e 4954  SALES_OPPORTUNIT
+000029c0: 595f 4e4f 5445 5f4c 4953 5472 2300 0000  Y_NOTE_LISTr#...
+000029d0: 7238 0000 0072 4e00 0000 720d 0000 0072  r8...rN...r....r
+000029e0: 0d00 0000 2901 724a 0000 0072 0e00 0000  ....).rJ...r....
+000029f0: 729e 0000 0026 0100 0073 0800 0000 0802  r....&...s......
+00002a00: 0401 0401 0603 729e 0000 0063 0000 0000  ......r....c....
+00002a10: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00002a20: 732c 0000 0065 005a 0164 005a 0265 036a  s,...e.Z.d.Z.e.j
+00002a30: 0465 056a 0667 0164 0166 035a 0787 0066  .e.j.g.d.f.Z...f
+00002a40: 0164 0264 0384 085a 0887 0004 005a 0953  .d.d...Z.....Z.S
+00002a50: 0029 04da 1a54 6573 7453 796e 634f 7070  .)...TestSyncOpp
+00002a60: 6f72 7475 6e69 7479 436f 6d6d 616e 64da  ortunityCommand.
+00002a70: 0b6f 7070 6f72 7475 6e69 7479 6301 0000  .opportunityc...
+00002a80: 0000 0000 0001 0000 0001 0000 0003 0000  ................
+00002a90: 0073 3e00 0000 7400 8300 6a01 8300 0100  .s>...t...j.....
+00002aa0: 7402 6a03 8300 0100 7402 6a04 8300 0100  t.j.....t.j.....
+00002ab0: 7402 6a05 8300 0100 7402 6a06 8300 0100  t.j.....t.j.....
+00002ac0: 7402 6a07 8300 0100 7402 6a08 8300 0100  t.j.....t.j.....
+00002ad0: 6400 5300 2901 4e29 0972 4800 0000 7238  d.S.).N).rH...r8
+00002ae0: 0000 0072 0800 0000 7249 0000 0072 9900  ...r....rI...r..
+00002af0: 0000 7280 0000 0072 a000 0000 72a1 0000  ..r....r....r...
+00002b00: 0072 a200 0000 2901 721d 0000 0029 0172  .r....).r....).r
+00002b10: 4a00 0000 720d 0000 0072 0e00 0000 7238  J...r....r....r8
+00002b20: 0000 003d 0100 0073 0e00 0000 0001 0a01  ...=...s........
+00002b30: 0801 0801 0801 0801 0801 7a20 5465 7374  ..........z Test
+00002b40: 5379 6e63 4f70 706f 7274 756e 6974 7943  SyncOpportunityC
+00002b50: 6f6d 6d61 6e64 2e73 6574 5570 290a 722f  ommand.setUp).r/
+00002b60: 0000 0072 3000 0000 7231 0000 0072 0600  ...r0...r1...r..
+00002b70: 0000 da20 7361 6c65 735f 6170 695f 6765  ... sales_api_ge
+00002b80: 745f 6f70 706f 7274 756e 6974 6965 735f  t_opportunities_
+00002b90: 6361 6c6c 7207 0000 00da 1541 5049 5f53  callr......API_S
+00002ba0: 414c 4553 5f4f 5050 4f52 5455 4e49 5459  ALES_OPPORTUNITY
+00002bb0: 7223 0000 0072 3800 0000 724e 0000 0072  r#...r8...rN...r
+00002bc0: 0d00 0000 720d 0000 0029 0172 4a00 0000  ....r....).rJ...
+00002bd0: 720e 0000 0072 a600 0000 3601 0000 7308  r....r....6...s.
+00002be0: 0000 0008 0204 0106 0106 0372 a600 0000  ...........r....
+00002bf0: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
+00002c00: 0040 0000 0073 1a00 0000 6500 5a01 6400  .@...s....e.Z.d.
+00002c10: 5a02 6503 6a04 6505 6a06 6401 6603 5a07  Z.e.j.e.j.d.f.Z.
+00002c20: 6402 5300 2903 da20 5465 7374 5379 6e63  d.S.).. TestSync
+00002c30: 4f70 706f 7274 756e 6974 7953 7461 6765  OpportunityStage
+00002c40: 7343 6f6d 6d61 6e64 da11 6f70 706f 7274  sCommand..opport
+00002c50: 756e 6974 795f 7374 6167 654e 2908 722f  unity_stageN).r/
+00002c60: 0000 0072 3000 0000 7231 0000 0072 0600  ...r0...r1...r..
+00002c70: 0000 da25 7361 6c65 735f 6170 695f 6765  ...%sales_api_ge
+00002c80: 745f 6f70 706f 7274 756e 6974 795f 7374  t_opportunity_st
+00002c90: 6167 6573 5f63 616c 6c72 0700 0000 da1c  ages_callr......
+00002ca0: 4150 495f 5341 4c45 535f 4f50 504f 5254  API_SALES_OPPORT
+00002cb0: 554e 4954 595f 5354 4147 4553 7223 0000  UNITY_STAGESr#..
+00002cc0: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00002cd0: 720e 0000 0072 aa00 0000 4701 0000 7306  r....r....G...s.
+00002ce0: 0000 0008 0204 0104 0172 aa00 0000 6300  .........r....c.
+00002cf0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00002d00: 0000 0073 1a00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00002d10: 6503 6a04 6505 6a06 6401 6603 5a07 6402  e.j.e.j.d.f.Z.d.
+00002d20: 5300 2903 da22 5465 7374 5379 6e63 4f70  S.).."TestSyncOp
+00002d30: 706f 7274 756e 6974 7953 7461 7475 7365  portunityStatuse
+00002d40: 7343 6f6d 6d61 6e64 da12 6f70 706f 7274  sCommand..opport
+00002d50: 756e 6974 795f 7374 6174 7573 4e29 0872  unity_statusN).r
+00002d60: 2f00 0000 7230 0000 0072 3100 0000 7206  /...r0...r1...r.
+00002d70: 0000 00da 2773 616c 6573 5f61 7069 5f67  ....'sales_api_g
+00002d80: 6574 5f6f 7070 6f72 7475 6e69 7479 5f73  et_opportunity_s
+00002d90: 7461 7475 7365 735f 6361 6c6c 7207 0000  tatuses_callr...
+00002da0: 00da 1e41 5049 5f53 414c 4553 5f4f 5050  ...API_SALES_OPP
+00002db0: 4f52 5455 4e49 5459 5f53 5441 5455 5345  ORTUNITY_STATUSE
+00002dc0: 5372 2300 0000 720d 0000 0072 0d00 0000  Sr#...r....r....
+00002dd0: 720d 0000 0072 0e00 0000 72ae 0000 004f  r....r....r....O
+00002de0: 0100 0073 0600 0000 0802 0401 0401 72ae  ...s..........r.
+00002df0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002e00: 0300 0000 4000 0000 731a 0000 0065 005a  ....@...s....e.Z
+00002e10: 0164 005a 0265 036a 0465 056a 0664 0166  .d.Z.e.j.e.j.d.f
+00002e20: 035a 0764 0253 0029 03da 1f54 6573 7453  .Z.d.S.)...TestS
+00002e30: 796e 634f 7070 6f72 7475 6e69 7479 5479  yncOpportunityTy
+00002e40: 7065 7343 6f6d 6d61 6e64 da10 6f70 706f  pesCommand..oppo
+00002e50: 7274 756e 6974 795f 7479 7065 4e29 0872  rtunity_typeN).r
+00002e60: 2f00 0000 7230 0000 0072 3100 0000 7206  /...r0...r1...r.
+00002e70: 0000 00da 2473 616c 6573 5f61 7069 5f67  ....$sales_api_g
+00002e80: 6574 5f6f 7070 6f72 7475 6e69 7479 5f74  et_opportunity_t
+00002e90: 7970 6573 5f63 616c 6c72 0700 0000 da1b  ypes_callr......
+00002ea0: 4150 495f 5341 4c45 535f 4f50 504f 5254  API_SALES_OPPORT
+00002eb0: 554e 4954 595f 5459 5045 5372 2300 0000  UNITY_TYPESr#...
+00002ec0: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00002ed0: 0e00 0000 72b2 0000 0057 0100 0073 0600  ....r....W...s..
+00002ee0: 0000 0802 0401 0401 72b2 0000 0063 0000  ........r....c..
+00002ef0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+00002f00: 0000 731a 0000 0065 005a 0164 005a 0265  ..s....e.Z.d.Z.e
+00002f10: 036a 0465 056a 0664 0166 035a 0764 0253  .j.e.j.d.f.Z.d.S
+00002f20: 0029 03da 2154 6573 7453 796e 6353 616c  .)..!TestSyncSal
+00002f30: 6573 5072 6f62 6162 696c 6974 6965 7343  esProbabilitiesC
+00002f40: 6f6d 6d61 6e64 da11 7361 6c65 735f 7072  ommand..sales_pr
+00002f50: 6f62 6162 696c 6974 794e 2908 722f 0000  obabilityN).r/..
+00002f60: 0072 3000 0000 7231 0000 0072 0600 0000  .r0...r1...r....
+00002f70: da26 7361 6c65 735f 6170 695f 6765 745f  .&sales_api_get_
+00002f80: 7361 6c65 735f 7072 6f62 6162 696c 6974  sales_probabilit
+00002f90: 6965 735f 6361 6c6c 7207 0000 00da 1a41  ies_callr......A
+00002fa0: 5049 5f53 414c 4553 5f50 524f 4241 4249  PI_SALES_PROBABI
+00002fb0: 4c49 5459 5f4c 4953 5472 2300 0000 720d  LITY_LISTr#...r.
+00002fc0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00002fd0: 0000 72b6 0000 005f 0100 0073 0600 0000  ..r...._...s....
+00002fe0: 0802 0401 0401 72b6 0000 0063 0000 0000  ......r....c....
+00002ff0: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00003000: 732a 0000 0065 005a 0164 005a 0265 036a  s*...e.Z.d.Z.e.j
+00003010: 0465 056a 0664 0166 035a 0787 0066 0164  .e.j.d.f.Z...f.d
+00003020: 0264 0384 085a 0887 0004 005a 0953 0029  .d...Z.....Z.S.)
+00003030: 04da 1a54 6573 7453 796e 6354 696d 6545  ...TestSyncTimeE
+00003040: 6e74 7269 6573 436f 6d6d 616e 64da 0a74  ntriesCommand..t
+00003050: 696d 655f 656e 7472 7963 0100 0000 0000  ime_entryc......
+00003060: 0000 0100 0000 0100 0000 0300 0000 733e  ..............s>
+00003070: 0000 0074 0083 006a 0183 0001 0074 026a  ...t...j.....t.j
+00003080: 0383 0001 0074 026a 0483 0001 0074 026a  .....t.j.....t.j
+00003090: 0583 0001 0074 026a 0683 0001 0074 026a  .....t.j.....t.j
+000030a0: 0783 0001 0074 026a 0883 0001 0064 0053  .....t.j.....d.S
+000030b0: 0029 014e 2909 7248 0000 0072 3800 0000  .).N).rH...r8...
+000030c0: 7208 0000 0072 5500 0000 729a 0000 0072  r....rU...r....r
+000030d0: 9b00 0000 7249 0000 0072 9900 0000 7280  ....rI...r....r.
+000030e0: 0000 0029 0172 1d00 0000 2901 724a 0000  ...).r....).rJ..
+000030f0: 0072 0d00 0000 720e 0000 0072 3800 0000  .r....r....r8...
+00003100: 6e01 0000 730e 0000 0000 010a 0108 0108  n...s...........
+00003110: 0108 0108 0108 017a 2054 6573 7453 796e  .......z TestSyn
+00003120: 6354 696d 6545 6e74 7269 6573 436f 6d6d  cTimeEntriesComm
+00003130: 616e 642e 7365 7455 7029 0a72 2f00 0000  and.setUp).r/...
+00003140: 7230 0000 0072 3100 0000 7206 0000 00da  r0...r1...r.....
+00003150: 1e74 696d 655f 6170 695f 6765 745f 7469  .time_api_get_ti
+00003160: 6d65 5f65 6e74 7269 6573 5f63 616c 6c72  me_entries_callr
+00003170: 0700 0000 da13 4150 495f 5449 4d45 5f45  ......API_TIME_E
+00003180: 4e54 5259 5f4c 4953 5472 2300 0000 7238  NTRY_LISTr#...r8
+00003190: 0000 0072 4e00 0000 720d 0000 0072 0d00  ...rN...r....r..
+000031a0: 0000 2901 724a 0000 0072 0e00 0000 72ba  ..).rJ...r....r.
+000031b0: 0000 0067 0100 0073 0800 0000 0802 0401  ...g...s........
+000031c0: 0401 0603 72ba 0000 0063 0000 0000 0000  ....r....c......
+000031d0: 0000 0000 0000 0300 0000 0000 0000 732a  ..............s*
+000031e0: 0000 0065 005a 0164 005a 0265 036a 0465  ...e.Z.d.Z.e.j.e
+000031f0: 056a 0664 0166 035a 0787 0066 0164 0264  .j.d.f.Z...f.d.d
+00003200: 0384 085a 0887 0004 005a 0953 0029 04da  ...Z.....Z.S.)..
+00003210: 1e54 6573 7453 796e 6353 6368 6564 756c  .TestSyncSchedul
+00003220: 6545 6e74 7269 6573 436f 6d6d 616e 64da  eEntriesCommand.
+00003230: 0e73 6368 6564 756c 655f 656e 7472 7963  .schedule_entryc
+00003240: 0100 0000 0000 0000 0100 0000 0100 0000  ................
+00003250: 0300 0000 736e 0000 0074 0083 006a 0183  ....sn...t...j..
+00003260: 0001 0074 026a 0383 0001 0074 026a 0483  ...t.j.....t.j..
+00003270: 0001 0074 026a 0583 0001 0074 026a 0683  ...t.j.....t.j..
+00003280: 0001 0074 026a 0783 0001 0074 026a 0883  ...t.j.....t.j..
+00003290: 0001 0074 026a 0983 0001 0074 026a 0a83  ...t.j.....t.j..
+000032a0: 0001 0074 026a 0b83 0001 0074 026a 0c83  ...t.j.....t.j..
+000032b0: 0001 0074 026a 0d83 0001 0074 026a 0e83  ...t.j.....t.j..
+000032c0: 0001 0064 0053 0029 014e 290f 7248 0000  ...d.S.).N).rH..
+000032d0: 0072 3800 0000 7208 0000 0072 5500 0000  .r8...r....rU...
+000032e0: 729a 0000 0072 4900 0000 7299 0000 005a  r....rI...r....Z
+000032f0: 0e69 6e69 745f 6c6f 6361 7469 6f6e 73da  .init_locations.
+00003300: 0a69 6e69 745f 7465 616d 7372 8000 0000  .init_teamsr....
+00003310: 7294 0000 0072 7800 0000 5a13 696e 6974  r....rx...Z.init
+00003320: 5f73 6368 6564 756c 655f 7479 7065 735a  _schedule_typesZ
+00003330: 1669 6e69 745f 7363 6865 6475 6c65 5f73  .init_schedule_s
+00003340: 7461 7475 7365 7372 9b00 0000 2901 721d  tatusesr....).r.
+00003350: 0000 0029 0172 4a00 0000 720d 0000 0072  ...).rJ...r....r
+00003360: 0e00 0000 7238 0000 007f 0100 0073 1a00  ....r8.......s..
+00003370: 0000 0001 0a01 0801 0801 0801 0801 0801  ................
+00003380: 0801 0801 0801 0801 0801 0801 7a24 5465  ............z$Te
+00003390: 7374 5379 6e63 5363 6865 6475 6c65 456e  stSyncScheduleEn
+000033a0: 7472 6965 7343 6f6d 6d61 6e64 2e73 6574  triesCommand.set
+000033b0: 5570 290a 722f 0000 0072 3000 0000 7231  Up).r/...r0...r1
+000033c0: 0000 0072 0600 0000 da26 7363 6865 6475  ...r.....&schedu
+000033d0: 6c65 5f61 7069 5f67 6574 5f73 6368 6564  le_api_get_sched
+000033e0: 756c 655f 656e 7472 6965 735f 6361 6c6c  ule_entries_call
+000033f0: 7207 0000 00da 1441 5049 5f53 4348 4544  r......API_SCHED
+00003400: 554c 455f 454e 5452 4945 5372 2300 0000  ULE_ENTRIESr#...
+00003410: 7238 0000 0072 4e00 0000 720d 0000 0072  r8...rN...r....r
+00003420: 0d00 0000 2901 724a 0000 0072 0e00 0000  ....).rJ...r....
+00003430: 72be 0000 0078 0100 0073 0800 0000 0802  r....x...s......
+00003440: 0401 0401 0603 72be 0000 0063 0000 0000  ......r....c....
+00003450: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00003460: 731a 0000 0065 005a 0164 005a 0265 036a  s....e.Z.d.Z.e.j
+00003470: 0465 056a 0664 0166 035a 0764 0253 0029  .e.j.d.f.Z.d.S.)
+00003480: 03da 1c54 6573 7453 796e 6353 6368 6564  ...TestSyncSched
+00003490: 756c 6554 7970 6573 436f 6d6d 616e 64da  uleTypesCommand.
+000034a0: 0d73 6368 6564 756c 655f 7479 7065 4e29  .schedule_typeN)
+000034b0: 0872 2f00 0000 7230 0000 0072 3100 0000  .r/...r0...r1...
+000034c0: 7206 0000 00da 2473 6368 6564 756c 655f  r.....$schedule_
+000034d0: 6170 695f 6765 745f 7363 6865 6475 6c65  api_get_schedule
+000034e0: 5f74 7970 6573 5f63 616c 6c72 0700 0000  _types_callr....
+000034f0: da16 4150 495f 5343 4845 4455 4c45 5f54  ..API_SCHEDULE_T
+00003500: 5950 455f 4c49 5354 7223 0000 0072 0d00  YPE_LISTr#...r..
+00003510: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00003520: 0072 c300 0000 8f01 0000 7306 0000 0008  .r........s.....
+00003530: 0204 0104 0172 c300 0000 6300 0000 0000  .....r....c.....
+00003540: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00003550: 1a00 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
+00003560: 6505 6a06 6401 6603 5a07 6402 5300 2903  e.j.d.f.Z.d.S.).
+00003570: da1f 5465 7374 5379 6e63 5363 6865 6475  ..TestSyncSchedu
+00003580: 6c65 5374 6174 7573 6573 436f 6d6d 616e  leStatusesComman
+00003590: 64da 0f73 6368 6564 756c 655f 7374 6174  d..schedule_stat
+000035a0: 7573 4e29 0872 2f00 0000 7230 0000 0072  usN).r/...r0...r
+000035b0: 3100 0000 7206 0000 00da 2773 6368 6564  1...r.....'sched
+000035c0: 756c 655f 6170 695f 6765 745f 7363 6865  ule_api_get_sche
+000035d0: 6475 6c65 5f73 7461 7475 7365 735f 6361  dule_statuses_ca
+000035e0: 6c6c 7207 0000 00da 1841 5049 5f53 4348  llr......API_SCH
+000035f0: 4544 554c 455f 5354 4154 5553 5f4c 4953  EDULE_STATUS_LIS
+00003600: 5472 2300 0000 720d 0000 0072 0d00 0000  Tr#...r....r....
+00003610: 720d 0000 0072 0e00 0000 72c7 0000 0097  r....r....r.....
+00003620: 0100 0073 0600 0000 0802 0401 0401 72c7  ...s..........r.
+00003630: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00003640: 0300 0000 4000 0000 731a 0000 0065 005a  ....@...s....e.Z
+00003650: 0164 005a 0265 036a 0465 056a 0664 0166  .d.Z.e.j.e.j.d.f
+00003660: 035a 0764 0253 0029 03da 1f54 6573 7453  .Z.d.S.)...TestS
+00003670: 796e 6341 6374 6976 6974 7953 7461 7475  yncActivityStatu
+00003680: 7365 7343 6f6d 6d61 6e64 da0f 6163 7469  sesCommand..acti
+00003690: 7669 7479 5f73 7461 7475 734e 2908 722f  vity_statusN).r/
+000036a0: 0000 0072 3000 0000 7231 0000 0072 0600  ...r0...r1...r..
+000036b0: 0000 da26 7361 6c65 735f 6170 695f 6765  ...&sales_api_ge
+000036c0: 745f 6163 7469 7669 7469 6573 5f73 7461  t_activities_sta
+000036d0: 7475 7365 735f 6361 6c6c 7207 0000 00da  tuses_callr.....
+000036e0: 1b41 5049 5f53 414c 4553 5f41 4354 4956  .API_SALES_ACTIV
+000036f0: 4954 595f 5354 4154 5553 4553 7223 0000  ITY_STATUSESr#..
+00003700: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00003710: 720e 0000 0072 cb00 0000 9f01 0000 7306  r....r........s.
+00003720: 0000 0008 0204 0104 0172 cb00 0000 6300  .........r....c.
+00003730: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00003740: 0000 0073 1a00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00003750: 6503 6a04 6505 6a06 6401 6603 5a07 6402  e.j.e.j.d.f.Z.d.
+00003760: 5300 2903 da1c 5465 7374 5379 6e63 4163  S.)...TestSyncAc
+00003770: 7469 7669 7479 5479 7065 7343 6f6d 6d61  tivityTypesComma
+00003780: 6e64 da0d 6163 7469 7669 7479 5f74 7970  nd..activity_typ
+00003790: 654e 2908 722f 0000 0072 3000 0000 7231  eN).r/...r0...r1
+000037a0: 0000 0072 0600 0000 da23 7361 6c65 735f  ...r.....#sales_
+000037b0: 6170 695f 6765 745f 6163 7469 7669 7469  api_get_activiti
+000037c0: 6573 5f74 7970 6573 5f63 616c 6c72 0700  es_types_callr..
+000037d0: 0000 da18 4150 495f 5341 4c45 535f 4143  ....API_SALES_AC
+000037e0: 5449 5649 5459 5f54 5950 4553 7223 0000  TIVITY_TYPESr#..
+000037f0: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00003800: 720e 0000 0072 cf00 0000 a701 0000 7306  r....r........s.
+00003810: 0000 0008 0204 0104 0172 cf00 0000 6300  .........r....c.
+00003820: 0000 0000 0000 0000 0000 0003 0000 0000  ................
+00003830: 0000 0073 2a00 0000 6500 5a01 6400 5a02  ...s*...e.Z.d.Z.
+00003840: 6503 6a04 6505 6a06 6401 6603 5a07 8700  e.j.e.j.d.f.Z...
+00003850: 6601 6402 6403 8408 5a08 8700 0400 5a09  f.d.d...Z.....Z.
+00003860: 5300 2904 da17 5465 7374 5379 6e63 4163  S.)...TestSyncAc
+00003870: 7469 7669 7479 436f 6d6d 616e 64da 0861  tivityCommand..a
+00003880: 6374 6976 6974 7963 0100 0000 0000 0000  ctivityc........
+00003890: 0100 0000 0300 0000 0300 0000 736a 0000  ............sj..
+000038a0: 0074 0083 006a 0183 0001 0074 026a 0383  .t...j.....t.j..
+000038b0: 0001 0074 026a 0483 0001 0074 056a 0674  ...t.j.....t.j.t
+000038c0: 056a 0774 056a 0883 0066 0283 0101 0074  .j.t.j...f.....t
+000038d0: 026a 0983 0001 0074 026a 0a83 0001 0074  .j.....t.j.....t
+000038e0: 026a 0b83 0001 0074 026a 0c83 0001 0074  .j.....t.j.....t
+000038f0: 026a 0d83 0001 0074 026a 0e83 0001 0074  .j.....t.j.....t
+00003900: 026a 0f83 0001 0064 0053 0029 014e 2910  .j.....d.S.).N).
+00003910: 7248 0000 0072 3800 0000 7208 0000 0072  rH...r8...r....r
+00003920: 4900 0000 7299 0000 0072 0600 0000 727d  I...r....r....r}
+00003930: 0000 0072 7e00 0000 727f 0000 0072 8000  ...r~...r....r..
+00003940: 0000 72a0 0000 0072 a200 0000 72a3 0000  ..r....r....r...
+00003950: 0072 9b00 0000 729a 0000 005a 0f69 6e69  .r....r....Z.ini
+00003960: 745f 6163 7469 7669 7469 6573 2901 721d  t_activities).r.
+00003970: 0000 0029 0172 4a00 0000 720d 0000 0072  ...).rJ...r....r
+00003980: 0e00 0000 7238 0000 00b6 0100 0073 1800  ....r8.......s..
+00003990: 0000 0001 0a01 0801 0801 0401 1001 0801  ................
+000039a0: 0801 0801 0801 0801 0801 7a1d 5465 7374  ..........z.Test
+000039b0: 5379 6e63 4163 7469 7669 7479 436f 6d6d  SyncActivityComm
+000039c0: 616e 642e 7365 7455 7029 0a72 2f00 0000  and.setUp).r/...
+000039d0: 7230 0000 0072 3100 0000 7206 0000 00da  r0...r1...r.....
+000039e0: 1d73 616c 6573 5f61 7069 5f67 6574 5f61  .sales_api_get_a
+000039f0: 6374 6976 6974 6965 735f 6361 6c6c 7207  ctivities_callr.
+00003a00: 0000 00da 1441 5049 5f53 414c 4553 5f41  .....API_SALES_A
+00003a10: 4354 4956 4954 4945 5372 2300 0000 7238  CTIVITIESr#...r8
+00003a20: 0000 0072 4e00 0000 720d 0000 0072 0d00  ...rN...r....r..
+00003a30: 0000 2901 724a 0000 0072 0e00 0000 72d3  ..).rJ...r....r.
+00003a40: 0000 00af 0100 0073 0800 0000 0802 0401  .......s........
+00003a50: 0401 0603 72d3 0000 0063 0000 0000 0000  ....r....c......
+00003a60: 0000 0000 0000 0300 0000 0000 0000 732a  ..............s*
+00003a70: 0000 0065 005a 0164 005a 0287 0066 0164  ...e.Z.d.Z...f.d
+00003a80: 0164 0284 085a 0365 046a 0565 066a 0764  .d...Z.e.j.e.j.d
+00003a90: 0366 035a 0887 0004 005a 0953 0029 04da  .f.Z.....Z.S.)..
+00003aa0: 1354 6573 7453 796e 6354 7970 6543 6f6d  .TestSyncTypeCom
+00003ab0: 6d61 6e64 6301 0000 0000 0000 0001 0000  mandc...........
+00003ac0: 0001 0000 0003 0000 0073 1e00 0000 7400  .........s....t.
+00003ad0: 8300 6a01 8300 0100 7402 6a03 8300 0100  ..j.....t.j.....
+00003ae0: 7402 6a04 8300 0100 6400 5300 2901 4e29  t.j.....d.S.).N)
+00003af0: 0572 4800 0000 7238 0000 0072 0800 0000  .rH...r8...r....
+00003b00: da0a 696e 6974 5f74 7970 6573 7255 0000  ..init_typesrU..
+00003b10: 0029 0172 1d00 0000 2901 724a 0000 0072  .).r....).rJ...r
+00003b20: 0d00 0000 720e 0000 0072 3800 0000 c701  ....r....r8.....
+00003b30: 0000 7306 0000 0000 010a 0108 017a 1954  ..s..........z.T
+00003b40: 6573 7453 796e 6354 7970 6543 6f6d 6d61  estSyncTypeComma
+00003b50: 6e64 2e73 6574 5570 da04 7479 7065 290a  nd.setUp..type).
+00003b60: 722f 0000 0072 3000 0000 7231 0000 0072  r/...r0...r1...r
+00003b70: 3800 0000 7206 0000 00da 1a73 6572 7669  8...r......servi
+00003b80: 6365 5f61 7069 5f67 6574 5f74 7970 6573  ce_api_get_types
+00003b90: 5f63 616c 6c72 0700 0000 da0d 4150 495f  _callr......API_
+00003ba0: 5459 5045 5f4c 4953 5472 2300 0000 724e  TYPE_LISTr#...rN
+00003bb0: 0000 0072 0d00 0000 720d 0000 0029 0172  ...r....r....).r
+00003bc0: 4a00 0000 720e 0000 0072 d700 0000 c501  J...r....r......
+00003bd0: 0000 7308 0000 0008 020c 0604 0104 0172  ..s............r
+00003be0: d700 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00003bf0: 0003 0000 0000 0000 0073 2a00 0000 6500  .........s*...e.
+00003c00: 5a01 6400 5a02 8700 6601 6401 6402 8408  Z.d.Z...f.d.d...
+00003c10: 5a03 6504 6a05 6506 6a07 6403 6603 5a08  Z.e.j.e.j.d.f.Z.
+00003c20: 8700 0400 5a09 5300 2904 da16 5465 7374  ....Z.S.)...Test
+00003c30: 5379 6e63 5375 6254 7970 6543 6f6d 6d61  SyncSubTypeComma
+00003c40: 6e64 6301 0000 0000 0000 0001 0000 0001  ndc.............
+00003c50: 0000 0003 0000 0073 1e00 0000 7400 8300  .......s....t...
+00003c60: 6a01 8300 0100 7402 6a03 8300 0100 7402  j.....t.j.....t.
+00003c70: 6a04 8300 0100 6400 5300 2901 4e29 0572  j.....d.S.).N).r
+00003c80: 4800 0000 7238 0000 0072 0800 0000 72d8  H...r8...r....r.
+00003c90: 0000 0072 5500 0000 2901 721d 0000 0029  ...rU...).r....)
+00003ca0: 0172 4a00 0000 720d 0000 0072 0e00 0000  .rJ...r....r....
+00003cb0: 7238 0000 00d4 0100 0073 0600 0000 0001  r8.......s......
+00003cc0: 0a01 0801 7a1c 5465 7374 5379 6e63 5375  ....z.TestSyncSu
+00003cd0: 6254 7970 6543 6f6d 6d61 6e64 2e73 6574  bTypeCommand.set
+00003ce0: 5570 da08 7375 625f 7479 7065 290a 722f  Up..sub_type).r/
+00003cf0: 0000 0072 3000 0000 7231 0000 0072 3800  ...r0...r1...r8.
+00003d00: 0000 7206 0000 00da 1d73 6572 7669 6365  ..r......service
+00003d10: 5f61 7069 5f67 6574 5f73 7562 7479 7065  _api_get_subtype
+00003d20: 735f 6361 6c6c 7207 0000 00da 1041 5049  s_callr......API
+00003d30: 5f53 5542 5459 5045 5f4c 4953 5472 2300  _SUBTYPE_LISTr#.
+00003d40: 0000 724e 0000 0072 0d00 0000 720d 0000  ..rN...r....r...
+00003d50: 0029 0172 4a00 0000 720e 0000 0072 dc00  .).rJ...r....r..
+00003d60: 0000 d301 0000 7308 0000 0008 010c 0604  ......s.........
+00003d70: 0104 0172 dc00 0000 6300 0000 0000 0000  ...r....c.......
+00003d80: 0000 0000 0003 0000 0000 0000 0073 2a00  .............s*.
+00003d90: 0000 6500 5a01 6400 5a02 8700 6601 6401  ..e.Z.d.Z...f.d.
+00003da0: 6402 8408 5a03 6504 6a05 6506 6a07 6403  d...Z.e.j.e.j.d.
+00003db0: 6603 5a08 8700 0400 5a09 5300 2904 da13  f.Z.....Z.S.)...
+00003dc0: 5465 7374 5379 6e63 4974 656d 436f 6d6d  TestSyncItemComm
+00003dd0: 616e 6463 0100 0000 0000 0000 0100 0000  andc............
+00003de0: 0100 0000 0300 0000 731e 0000 0074 0083  ........s....t..
+00003df0: 006a 0183 0001 0074 026a 0383 0001 0074  .j.....t.j.....t
+00003e00: 026a 0483 0001 0064 0053 0029 014e 2905  .j.....d.S.).N).
+00003e10: 7248 0000 0072 3800 0000 7208 0000 0072  rH...r8...r....r
+00003e20: d800 0000 7255 0000 0029 0172 1d00 0000  ....rU...).r....
+00003e30: 2901 724a 0000 0072 0d00 0000 720e 0000  ).rJ...r....r...
+00003e40: 0072 3800 0000 e101 0000 7306 0000 0000  .r8.......s.....
+00003e50: 010a 0108 017a 1954 6573 7453 796e 6349  .....z.TestSyncI
+00003e60: 7465 6d43 6f6d 6d61 6e64 2e73 6574 5570  temCommand.setUp
+00003e70: da04 6974 656d 290a 722f 0000 0072 3000  ..item).r/...r0.
+00003e80: 0000 7231 0000 0072 3800 0000 7206 0000  ..r1...r8...r...
+00003e90: 00da 1a73 6572 7669 6365 5f61 7069 5f67  ...service_api_g
+00003ea0: 6574 5f69 7465 6d73 5f63 616c 6c72 0700  et_items_callr..
+00003eb0: 0000 da0d 4150 495f 4954 454d 5f4c 4953  ....API_ITEM_LIS
+00003ec0: 5472 2300 0000 724e 0000 0072 0d00 0000  Tr#...rN...r....
+00003ed0: 720d 0000 0029 0172 4a00 0000 720e 0000  r....).rJ...r...
+00003ee0: 0072 e000 0000 e001 0000 7308 0000 0008  .r........s.....
+00003ef0: 010c 0604 0104 0172 e000 0000 6300 0000  .......r....c...
+00003f00: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+00003f10: 0073 2a00 0000 6500 5a01 6400 5a02 8700  .s*...e.Z.d.Z...
+00003f20: 6601 6401 6402 8408 5a03 6504 6a05 6506  f.d.d...Z.e.j.e.
+00003f30: 6a07 6403 6603 5a08 8700 0400 5a09 5300  j.d.f.Z.....Z.S.
+00003f40: 2904 da17 5465 7374 5379 6e63 576f 726b  )...TestSyncWork
+00003f50: 5479 7065 436f 6d6d 616e 6463 0100 0000  TypeCommandc....
+00003f60: 0000 0000 0100 0000 0100 0000 0300 0000  ................
+00003f70: 7316 0000 0074 0083 006a 0183 0001 0074  s....t...j.....t
+00003f80: 026a 0383 0001 0064 0053 0029 014e 2904  .j.....d.S.).N).
+00003f90: 7248 0000 0072 3800 0000 7208 0000 005a  rH...r8...r....Z
+00003fa0: 0f69 6e69 745f 776f 726b 5f74 7970 6573  .init_work_types
+00003fb0: 2901 721d 0000 0029 0172 4a00 0000 720d  ).r....).rJ...r.
+00003fc0: 0000 0072 0e00 0000 7238 0000 00ee 0100  ...r....r8......
+00003fd0: 0073 0400 0000 0001 0a01 7a1d 5465 7374  .s........z.Test
+00003fe0: 5379 6e63 576f 726b 5479 7065 436f 6d6d  SyncWorkTypeComm
+00003ff0: 616e 642e 7365 7455 70da 0977 6f72 6b5f  and.setUp..work_
+00004000: 7479 7065 290a 722f 0000 0072 3000 0000  type).r/...r0...
+00004010: 7231 0000 0072 3800 0000 7206 0000 00da  r1...r8...r.....
+00004020: 1c74 696d 655f 6170 695f 6765 745f 776f  .time_api_get_wo
+00004030: 726b 5f74 7970 6573 5f63 616c 6c72 0700  rk_types_callr..
+00004040: 0000 da12 4150 495f 574f 524b 5f54 5950  ....API_WORK_TYP
+00004050: 455f 4c49 5354 7223 0000 0072 4e00 0000  E_LISTr#...rN...
+00004060: 720d 0000 0072 0d00 0000 2901 724a 0000  r....r....).rJ..
+00004070: 0072 0e00 0000 72e4 0000 00ed 0100 0073  .r....r........s
+00004080: 0800 0000 0801 0c05 0401 0401 72e4 0000  ............r...
+00004090: 0063 0000 0000 0000 0000 0000 0000 0300  .c..............
+000040a0: 0000 0000 0000 732a 0000 0065 005a 0164  ......s*...e.Z.d
+000040b0: 005a 0287 0066 0164 0164 0284 085a 0365  .Z...f.d.d...Z.e
+000040c0: 046a 0565 066a 0764 0366 035a 0887 0004  .j.e.j.d.f.Z....
+000040d0: 005a 0953 0029 04da 1754 6573 7453 796e  .Z.S.)...TestSyn
+000040e0: 6357 6f72 6b52 6f6c 6543 6f6d 6d61 6e64  cWorkRoleCommand
+000040f0: 6301 0000 0000 0000 0001 0000 0001 0000  c...............
+00004100: 0003 0000 0073 1600 0000 7400 8300 6a01  .....s....t...j.
+00004110: 8300 0100 7402 6a03 8300 0100 6400 5300  ....t.j.....d.S.
+00004120: 2901 4e29 0472 4800 0000 7238 0000 0072  ).N).rH...r8...r
+00004130: 0800 0000 7281 0000 0029 0172 1d00 0000  ....r....).r....
+00004140: 2901 724a 0000 0072 0d00 0000 720e 0000  ).rJ...r....r...
+00004150: 0072 3800 0000 fa01 0000 7304 0000 0000  .r8.......s.....
+00004160: 010a 017a 1d54 6573 7453 796e 6357 6f72  ...z.TestSyncWor
+00004170: 6b52 6f6c 6543 6f6d 6d61 6e64 2e73 6574  kRoleCommand.set
+00004180: 5570 da09 776f 726b 5f72 6f6c 6529 0a72  Up..work_role).r
+00004190: 2f00 0000 7230 0000 0072 3100 0000 7238  /...r0...r1...r8
+000041a0: 0000 0072 0600 0000 da1c 7469 6d65 5f61  ...r......time_a
+000041b0: 7069 5f67 6574 5f77 6f72 6b5f 726f 6c65  pi_get_work_role
+000041c0: 735f 6361 6c6c 7207 0000 00da 1241 5049  s_callr......API
+000041d0: 5f57 4f52 4b5f 524f 4c45 5f4c 4953 5472  _WORK_ROLE_LISTr
+000041e0: 2300 0000 724e 0000 0072 0d00 0000 720d  #...rN...r....r.
+000041f0: 0000 0029 0172 4a00 0000 720e 0000 0072  ...).rJ...r....r
+00004200: e800 0000 f901 0000 7308 0000 0008 010c  ........s.......
+00004210: 0504 0104 0172 e800 0000 6300 0000 0000  .....r....c.....
+00004220: 0000 0000 0000 0003 0000 0000 0000 0073  ...............s
+00004230: 2a00 0000 6500 5a01 6400 5a02 8700 6601  *...e.Z.d.Z...f.
+00004240: 6401 6402 8408 5a03 6504 6a05 6506 6a07  d.d...Z.e.j.e.j.
+00004250: 6403 6603 5a08 8700 0400 5a09 5300 2904  d.f.Z.....Z.S.).
+00004260: da18 5465 7374 5379 6e63 4167 7265 656d  ..TestSyncAgreem
+00004270: 656e 7443 6f6d 6d61 6e64 6301 0000 0000  entCommandc.....
+00004280: 0000 0001 0000 0001 0000 0003 0000 0073  ...............s
+00004290: 1600 0000 7400 8300 6a01 8300 0100 7402  ....t...j.....t.
+000042a0: 6a03 8300 0100 6400 5300 2901 4e29 0472  j.....d.S.).N).r
+000042b0: 4800 0000 7238 0000 0072 0800 0000 5a0f  H...r8...r....Z.
+000042c0: 696e 6974 5f61 6772 6565 6d65 6e74 7329  init_agreements)
+000042d0: 0172 1d00 0000 2901 724a 0000 0072 0d00  .r....).rJ...r..
+000042e0: 0000 720e 0000 0072 3800 0000 0602 0000  ..r....r8.......
+000042f0: 7304 0000 0000 010a 017a 1e54 6573 7453  s........z.TestS
+00004300: 796e 6341 6772 6565 6d65 6e74 436f 6d6d  yncAgreementComm
+00004310: 616e 642e 7365 7455 70da 0961 6772 6565  and.setUp..agree
+00004320: 6d65 6e74 290a 722f 0000 0072 3000 0000  ment).r/...r0...
+00004330: 7231 0000 0072 3800 0000 7206 0000 00da  r1...r8...r.....
+00004340: 1f66 696e 616e 6365 5f61 7069 5f67 6574  .finance_api_get
+00004350: 5f61 6772 6565 6d65 6e74 735f 6361 6c6c  _agreements_call
+00004360: 7207 0000 00da 1241 5049 5f41 4752 4545  r......API_AGREE
+00004370: 4d45 4e54 5f4c 4953 5472 2300 0000 724e  MENT_LISTr#...rN
+00004380: 0000 0072 0d00 0000 720d 0000 0029 0172  ...r....r....).r
+00004390: 4a00 0000 720e 0000 0072 ec00 0000 0502  J...r....r......
+000043a0: 0000 7308 0000 0008 010c 0504 0104 0172  ..s............r
+000043b0: ec00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+000043c0: 0003 0000 0000 0000 0073 2a00 0000 6500  .........s*...e.
+000043d0: 5a01 6400 5a02 8700 6601 6401 6402 8408  Z.d.Z...f.d.d...
+000043e0: 5a03 6504 6a05 6506 6a07 6403 6603 5a08  Z.e.j.e.j.d.f.Z.
+000043f0: 8700 0400 5a09 5300 2904 da1c 5465 7374  ....Z.S.)...Test
+00004400: 5379 6e63 5072 6f6a 6563 7454 6963 6b65  SyncProjectTicke
+00004410: 7443 6f6d 6d61 6e64 6301 0000 0000 0000  tCommandc.......
+00004420: 0001 0000 0003 0000 0003 0000 0073 3a00  .............s:.
+00004430: 0000 7400 8300 6a01 8300 0100 7402 6a03  ..t...j.....t.j.
+00004440: 7402 6a04 7402 6a05 8300 6602 8301 0100  t.j.t.j...f.....
+00004450: 7406 6a07 8300 0100 7406 6a08 8300 0100  t.j.....t.j.....
+00004460: 7406 6a09 8300 0100 6400 5300 2901 4e29  t.j.....d.S.).N)
+00004470: 0a72 4800 0000 7238 0000 0072 0600 0000  .rH...r8...r....
+00004480: 727d 0000 0072 7e00 0000 727f 0000 0072  r}...r~...r....r
+00004490: 0800 0000 7280 0000 0072 9a00 0000 5a14  ....r....r....Z.
+000044a0: 696e 6974 5f70 726f 6a65 6374 5f74 6963  init_project_tic
+000044b0: 6b65 7473 2901 721d 0000 0029 0172 4a00  kets).r....).rJ.
+000044c0: 0000 720d 0000 0072 0e00 0000 7238 0000  ..r....r....r8..
+000044d0: 0012 0200 0073 0c00 0000 0001 0a01 0401  .....s..........
+000044e0: 1001 0801 0801 7a22 5465 7374 5379 6e63  ......z"TestSync
+000044f0: 5072 6f6a 6563 7454 6963 6b65 7443 6f6d  ProjectTicketCom
+00004500: 6d61 6e64 2e73 6574 5570 5a0e 7072 6f6a  mand.setUpZ.proj
+00004510: 6563 745f 7469 636b 6574 290a 722f 0000  ect_ticket).r/..
+00004520: 0072 3000 0000 7231 0000 0072 3800 0000  .r0...r1...r8...
+00004530: 7206 0000 00da 2070 726f 6a65 6374 5f61  r..... project_a
+00004540: 7069 5f74 6963 6b65 7473 5f74 6573 745f  pi_tickets_test_
+00004550: 636f 6d6d 616e 6472 0700 0000 da17 4150  commandr......AP
+00004560: 495f 5052 4f4a 4543 545f 5449 434b 4554  I_PROJECT_TICKET
+00004570: 5f4c 4953 5472 2300 0000 724e 0000 0072  _LISTr#...rN...r
+00004580: 0d00 0000 720d 0000 0029 0172 4a00 0000  ....r....).rJ...
+00004590: 720e 0000 0072 f000 0000 1102 0000 7308  r....r........s.
+000045a0: 0000 0008 010c 0904 0104 0172 f000 0000  ...........r....
+000045b0: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
+000045c0: 0000 0000 0073 3600 0000 6500 5a01 6400  .....s6...e.Z.d.
+000045d0: 5a02 8700 6601 6401 6402 8408 5a03 640a  Z...f.d.d...Z.d.
+000045e0: 6404 6405 8401 5a04 6406 6407 8400 5a05  d.d...Z.d.d...Z.
+000045f0: 6408 6409 8400 5a06 8700 0400 5a07 5300  d.d...Z.....Z.S.
+00004600: 290b da12 5465 7374 5379 6e63 416c 6c43  )...TestSyncAllC
+00004610: 6f6d 6d61 6e64 6301 0000 0000 0000 0006  ommandc.........
+00004620: 0000 0028 0000 0003 0000 0073 ce00 0000  ...(.......s....
+00004630: 7400 8300 6a01 8300 0100 7402 6a03 7404  t...j.....t.j.t.
+00004640: 6a05 6701 8301 0100 7402 6a06 7402 6a07  j.g.....t.j.t.j.
+00004650: 7402 6a08 8300 6602 8301 0100 7402 6a09  t.j...f.....t.j.
+00004660: 7404 6a0a 8301 0100 7402 6a0b 8300 0100  t.j.....t.j.....
+00004670: 740c 740d 740e 740f 7410 7411 7412 7413  t.t.t.t.t.t.t.t.
+00004680: 7414 7415 7416 7417 7418 7419 741a 741b  t.t.t.t.t.t.t.t.
+00004690: 741c 741d 741e 741f 7420 7421 7422 7423  t.t.t.t.t t!t"t#
+000046a0: 7424 7425 7426 7427 7428 7429 742a 742b  t$t%t&t't(t)t*t+
+000046b0: 742c 742d 742e 742f 7430 7431 7432 7433  t,t-t.t/t0t1t2t3
+000046c0: 6728 7d01 6700 7c00 5f34 782e 7c01 4400  g(}.g.|._4x.|.D.
+000046d0: 5d26 7d02 7c00 6a34 6a35 7c02 6a36 8301  ]&}.|.j4j5|.j6..
+000046e0: 0100 7c02 6a36 5c03 7d03 7d04 7d05 7c03  ..|.j6\.}.}.}.|.
+000046f0: 7c04 8301 0100 71a0 5700 6400 5300 2901  |.....q.W.d.S.).
+00004700: 4e29 3772 4800 0000 7238 0000 0072 0600  N)7rH...r8...r..
+00004710: 0000 da1b 7379 7374 656d 5f61 7069 5f67  ....system_api_g
+00004720: 6574 5f6d 656d 6265 7273 5f63 616c 6c72  et_members_callr
+00004730: 0700 0000 da0a 4150 495f 4d45 4d42 4552  ......API_MEMBER
+00004740: 727d 0000 0072 7e00 0000 727f 0000 00da  r}...r~...r.....
+00004750: 1663 6f6d 7061 6e79 5f61 7069 5f62 795f  .company_api_by_
+00004760: 6964 5f63 616c 6cda 0b41 5049 5f43 4f4d  id_call..API_COM
+00004770: 5041 4e59 da18 7365 7276 6963 655f 6170  PANY..service_ap
+00004780: 695f 7469 636b 6574 735f 6361 6c6c 723f  i_tickets_callr?
+00004790: 0000 0072 4700 0000 724f 0000 0072 5c00  ...rG...rO...r\.
+000047a0: 0000 7265 0000 0072 7600 0000 7269 0000  ..re...rv...ri..
+000047b0: 0072 7100 0000 7253 0000 0072 8400 0000  .rq...rS...r....
+000047c0: 7258 0000 0072 9700 0000 729e 0000 0072  rX...r....r....r
+000047d0: ae00 0000 72aa 0000 0072 b200 0000 72a6  ....r....r....r.
+000047e0: 0000 0072 b600 0000 72cb 0000 0072 cf00  ...r....r....r..
+000047f0: 0000 72d3 0000 0072 c300 0000 72c7 0000  ..r....r....r...
+00004800: 0072 be00 0000 72ba 0000 0072 4300 0000  .r....r....rC...
+00004810: 728e 0000 0072 3200 0000 7292 0000 0072  r....r2...r....r
+00004820: 6000 0000 7236 0000 0072 3b00 0000 72d7  `...r6...r;...r.
+00004830: 0000 0072 dc00 0000 72e0 0000 0072 e400  ...r....r....r..
+00004840: 0000 72e8 0000 0072 ec00 0000 726d 0000  ..r....r....rm..
+00004850: 0072 7b00 0000 da09 7465 7374 5f61 7267  .r{.....test_arg
+00004860: 7372 1c00 0000 7223 0000 0029 0672 1d00  sr....r#...).r..
+00004870: 0000 5a0f 7379 6e63 5f74 6573 745f 6361  ..Z.sync_test_ca
+00004880: 7365 73da 0974 6573 745f 6361 7365 da07  ses..test_case..
+00004890: 6170 6963 616c 6cda 0766 6978 7475 7265  apicall..fixture
+000048a0: 7220 0000 0029 0172 4a00 0000 720d 0000  r ...).rJ...r...
+000048b0: 0072 0e00 0000 7238 0000 0023 0200 0073  .r....r8...#...s
+000048c0: 6600 0000 0001 0a01 0e01 0401 1001 0c01  f...............
+000048d0: 0802 0201 0201 0201 0201 0201 0201 0201  ................
+000048e0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+000048f0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00004900: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00004910: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00004920: 0603 0602 0a01 0e01 0c01 7a18 5465 7374  ..........z.Test
+00004930: 5379 6e63 416c 6c43 6f6d 6d61 6e64 2e73  SyncAllCommand.s
+00004940: 6574 5570 4663 0200 0000 0000 0000 0400  etUpFc..........
+00004950: 0000 0400 0000 4300 0000 7336 0000 0074  ......C...s6...t
+00004960: 006a 0183 007d 0264 0167 017d 037c 0172  .j...}.d.g.}.|.r
+00004970: 1c7c 036a 0264 0283 0101 0074 037c 0364  .|.j.d.....t.|.d
+00004980: 037c 0269 018e 0101 007c 026a 0483 006a  .|.i.....|.j...j
+00004990: 0583 0053 0029 044e 7218 0000 007a 062d  ...S.).Nr....z.-
+000049a0: 2d66 756c 6c72 1900 0000 2906 721a 0000  -fullr....).r...
+000049b0: 0072 1b00 0000 721c 0000 0072 0200 0000  .r....r....r....
+000049c0: 7228 0000 0072 2900 0000 2904 721d 0000  r(...r)...).r...
+000049d0: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
+000049e0: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
+000049f0: 1072 756e 5f73 796e 635f 636f 6d6d 616e  .run_sync_comman
+00004a00: 645c 0200 0073 0c00 0000 0001 0801 0602  d\...s..........
+00004a10: 0401 0a02 0e02 7a23 5465 7374 5379 6e63  ......z#TestSync
+00004a20: 416c 6c43 6f6d 6d61 6e64 2e72 756e 5f73  AllCommand.run_s
+00004a30: 796e 635f 636f 6d6d 616e 6463 0100 0000  ync_commandc....
+00004a40: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
+00004a50: 730e 0100 007c 006a 0083 007d 0178 327c  s....|.j...}.x2|
+00004a60: 006a 0144 005d 285c 037d 027d 037d 0474  .j.D.](\.}.}.}.t
+00004a70: 0274 037c 0483 0174 047c 0383 0183 027d  .t.|...t.|.....}
+00004a80: 057c 006a 057c 057c 0183 0201 0071 1057  .|.j.|.|.....q.W
+00004a90: 007c 006a 0674 076a 086a 096a 0a83 006a  .|.j.t.j.j.j...j
+00004aa0: 0b83 0074 0474 0c6a 0d83 0183 0201 007c  ...t.t.j.......|
+00004ab0: 006a 0674 076a 0e6a 096a 0a83 006a 0b83  .j.t.j.j.j...j..
+00004ac0: 0074 0474 0c6a 0f83 0183 0201 007c 006a  .t.t.j.......|.j
+00004ad0: 0674 076a 106a 096a 0a83 006a 0b83 0074  .t.j.j.j...j...t
+00004ae0: 0474 0c6a 1183 0183 0201 007c 006a 0674  .t.j.......|.j.t
+00004af0: 076a 126a 096a 0a83 006a 0b83 0074 0474  .j.j.j...j...t.t
+00004b00: 0c6a 1383 0183 0201 007c 006a 0674 076a  .j.......|.j.t.j
+00004b10: 146a 096a 0a83 006a 0b83 0074 0474 0c6a  .j.j...j...t.t.j
+00004b20: 1583 0183 0201 007c 006a 0674 076a 166a  .......|.j.t.j.j
+00004b30: 096a 0a83 006a 0b83 0064 0183 0201 007c  .j...j...d.....|
+00004b40: 006a 0674 076a 176a 096a 0a83 006a 0b83  .j.t.j.j.j...j..
+00004b50: 0074 0474 0c6a 1867 0183 0183 0201 0064  .t.t.j.g.......d
+00004b60: 0253 0029 037a 640a 2020 2020 2020 2020  .S.).zd.        
+00004b70: 5465 7374 2074 6865 2063 6f6d 6d61 6e64  Test the command
+00004b80: 2074 6f20 7275 6e20 6120 7379 6e63 206f   to run a sync o
+00004b90: 6620 616c 6c20 6f62 6a65 6374 7320 7769  f all objects wi
+00004ba0: 7468 6f75 740a 2020 2020 2020 2020 7468  thout.        th
+00004bb0: 6520 2d2d 6675 6c6c 2061 7267 756d 656e  e --full argumen
+00004bc0: 742e 0a20 2020 2020 2020 2072 0500 0000  t..        r....
+00004bd0: 4e29 1972 fd00 0000 72f9 0000 0072 0f00  N).r....r....r..
+00004be0: 0000 7216 0000 0072 2b00 0000 7227 0000  ..r....r+...r'..
+00004bf0: 0072 2c00 0000 7204 0000 00da 0454 6561  .r,...r......Tea
+00004c00: 6d72 8700 0000 7288 0000 00da 0563 6f75  mr....r......cou
+00004c10: 6e74 7207 0000 0072 5700 0000 da0d 436f  ntr....rW.....Co
+00004c20: 6d70 616e 7953 7461 7475 7372 4200 0000  mpanyStatusrB...
+00004c30: da0e 5469 636b 6574 5072 696f 7269 7479  ..TicketPriority
+00004c40: 7268 0000 0072 8600 0000 725b 0000 00da  rh...r....r[....
+00004c50: 0b42 6f61 7264 5374 6174 7573 728d 0000  .BoardStatusr...
+00004c60: 00da 084c 6f63 6174 696f 6eda 0654 6963  ...Location..Tic
+00004c70: 6b65 74da 1241 5049 5f53 4552 5649 4345  ket..API_SERVICE
+00004c80: 5f54 4943 4b45 5429 0672 1d00 0000 da06  _TICKET).r......
+00004c90: 6f75 7470 7574 72fb 0000 0072 fc00 0000  outputr....r....
+00004ca0: 7220 0000 00da 0773 756d 6d61 7279 720d  r .....summaryr.
+00004cb0: 0000 0072 0d00 0000 720e 0000 00da 1174  ...r....r......t
+00004cc0: 6573 745f 7061 7274 6961 6c5f 7379 6e63  est_partial_sync
+00004cd0: 6702 0000 7324 0000 0000 0508 0212 0112  g...s$..........
+00004ce0: 0110 0212 010c 0112 010c 0212 010c 0112  ................
+00004cf0: 010c 0112 010c 0112 0106 0212 017a 2454  .............z$T
+00004d00: 6573 7453 796e 6341 6c6c 436f 6d6d 616e  estSyncAllComman
+00004d10: 642e 7465 7374 5f70 6172 7469 616c 5f73  d.test_partial_s
+00004d20: 796e 6363 0100 0000 0000 0000 0b00 0000  yncc............
+00004d30: 2b00 0000 4300 0000 739e 0100 0074 006a  +...C...s....t.j
+00004d40: 0174 006a 0274 006a 0374 006a 0474 006a  .t.j.t.j.t.j.t.j
+00004d50: 0574 006a 0674 006a 0774 006a 0874 006a  .t.j.t.j.t.j.t.j
+00004d60: 0974 006a 0a74 006a 0b74 006a 0c74 006a  .t.j.t.j.t.j.t.j
+00004d70: 0d74 006a 0e74 006a 0f74 006a 1074 006a  .t.j.t.j.t.j.t.j
+00004d80: 1174 006a 1274 006a 1374 006a 1474 006a  .t.j.t.j.t.j.t.j
+00004d90: 1574 006a 1674 006a 1774 006a 1874 006a  .t.j.t.j.t.j.t.j
+00004da0: 1974 006a 1a74 006a 1b74 006a 1c74 006a  .t.j.t.j.t.j.t.j
+00004db0: 1d74 006a 1e74 006a 1f74 006a 2074 006a  .t.j.t.j.t.j t.j
+00004dc0: 2174 006a 2274 006a 2374 006a 2474 006a  !t.j"t.j#t.j$t.j
+00004dd0: 2574 006a 2674 006a 2774 006a 2874 006a  %t.j&t.j't.j(t.j
+00004de0: 2974 006a 2a64 019c 2a7d 017c 006a 2b83  )t.j*d..*}.|.j+.
+00004df0: 0001 0074 2c6a 2d83 0001 0074 2c6a 2e83  ...t,j-....t,j..
+00004e00: 0001 0074 2c6a 2f83 0001 0074 2c6a 3083  ...t,j/....t,j0.
+00004e10: 0001 0069 007d 0278 267c 016a 3183 0044  ...i.}.x&|.j1..D
+00004e20: 005d 1a5c 027d 037d 047c 046a 326a 3383  .].\.}.}.|.j2j3.
+00004e30: 006a 3483 007c 027c 033c 0071 e457 0074  .j4..|.|.<.q.W.t
+00004e40: 356a 3667 0083 0101 0074 356a 3767 0083  5j6g.....t5j7g..
+00004e50: 0101 0078 1e7c 006a 3844 005d 145c 037d  ...x.|.j8D.].\.}
+00004e60: 057d 067d 067c 0567 0083 0101 0090 0171  .}.}.|.g.......q
+00004e70: 1e57 007c 006a 2b64 0264 038d 017d 0778  .W.|.j+d.d...}.x
+00004e80: 567c 006a 3844 005d 4c5c 037d 057d 087d  V|.j8D.]L\.}.}.}
+00004e90: 097c 0964 0b6b 0690 0172 767c 006a 397c  .|.d.k...rv|.j9|
+00004ea0: 027c 0919 0064 0983 0201 0064 097c 027c  .|...d.....d.|.|
+00004eb0: 093c 0074 3a74 3b7c 0983 017c 027c 0919  .<.t:t;|...|.|..
+00004ec0: 0083 027d 0a7c 006a 3c7c 0a7c 0783 0201  ...}.|.j<|.|....
+00004ed0: 0090 0171 4a57 0064 0a53 0029 0c7a 3354  ...qJW.d.S.).z3T
+00004ee0: 6573 7420 7468 6520 636f 6d6d 616e 6420  est the command 
+00004ef0: 746f 2072 756e 2061 2066 756c 6c20 7379  to run a full sy
+00004f00: 6e63 206f 6620 616c 6c20 6f62 6a65 6374  nc of all object
+00004f10: 732e 292a da06 6d65 6d62 6572 7259 0000  s.)*..memberrY..
+00004f20: 0072 6600 0000 726a 0000 0072 7200 0000  .rf...rj...rr...
+00004f30: 7277 0000 0072 8500 0000 7244 0000 0072  rw...r....rD...r
+00004f40: 4000 0000 7250 0000 0072 5400 0000 725d  @...rP...rT...r]
+00004f50: 0000 00da 0674 6963 6b65 7472 9800 0000  .....ticketr....
+00004f60: 729f 0000 0072 4b00 0000 72a7 0000 0072  r....rK...r....r
+00004f70: af00 0000 72ab 0000 0072 b300 0000 72b7  ....r....r....r.
+00004f80: 0000 0072 cc00 0000 72d0 0000 0072 d400  ...r....r....r..
+00004f90: 0000 72bf 0000 0072 c400 0000 72c8 0000  ..r....r....r...
+00004fa0: 0072 bb00 0000 728f 0000 0072 3300 0000  .r....r....r3...
+00004fb0: 7293 0000 0072 6100 0000 7237 0000 0072  r....ra...r7...r
+00004fc0: 3c00 0000 72d9 0000 0072 dd00 0000 72e1  <...r....r....r.
+00004fd0: 0000 0072 e500 0000 72e9 0000 0072 ed00  ...r....r....r..
+00004fe0: 0000 726e 0000 0072 7c00 0000 5429 0172  ..rn...r|...T).r
+00004ff0: 2100 0000 7254 0000 0072 8500 0000 729f  !...rT...r....r.
+00005000: 0000 0072 9300 0000 7237 0000 0072 0100  ...r....r7...r..
+00005010: 0000 4e29 0572 5400 0000 7285 0000 0072  ..N).rT...r....r
+00005020: 9f00 0000 7293 0000 0072 3700 0000 293d  ....r....r7...)=
+00005030: 7204 0000 00da 064d 656d 6265 7272 8600  r......Memberr..
+00005040: 0000 7201 0100 00da 0d50 726f 6a65 6374  ..r......Project
+00005050: 5374 6174 7573 da07 5072 6f6a 6563 74da  Status..Project.
+00005060: 0c50 726f 6a65 6374 5068 6173 6572 0201  .ProjectPhaser..
+00005070: 0000 da09 5465 7272 6974 6f72 7972 0001  ....Territoryr..
+00005080: 0000 da0b 436f 6d70 616e 7954 7970 6572  ....CompanyTyper
+00005090: fe00 0000 7203 0100 0072 0401 0000 da0b  ....r....r......
+000050a0: 5365 7276 6963 654e 6f74 65da 0f4f 7070  ServiceNote..Opp
+000050b0: 6f72 7475 6e69 7479 4e6f 7465 da07 436f  ortunityNote..Co
+000050c0: 6d70 616e 79da 0b4f 7070 6f72 7475 6e69  mpany..Opportuni
+000050d0: 7479 da11 4f70 706f 7274 756e 6974 7953  ty..OpportunityS
+000050e0: 7461 7475 73da 104f 7070 6f72 7475 6e69  tatus..Opportuni
+000050f0: 7479 5374 6167 65da 0f4f 7070 6f72 7475  tyStage..Opportu
+00005100: 6e69 7479 5479 7065 da10 5361 6c65 7350  nityType..SalesP
+00005110: 726f 6261 6269 6c69 7479 da0e 4163 7469  robability..Acti
+00005120: 7669 7479 5374 6174 7573 da0c 4163 7469  vityStatus..Acti
+00005130: 7669 7479 5479 7065 da08 4163 7469 7669  vityType..Activi
+00005140: 7479 da0d 5363 6865 6475 6c65 456e 7472  ty..ScheduleEntr
+00005150: 79da 0c53 6368 6564 756c 6554 7970 65da  y..ScheduleType.
+00005160: 0e53 6368 6564 756c 6553 7461 7475 73da  .ScheduleStatus.
+00005170: 0954 696d 6545 6e74 7279 da03 536c 61da  .TimeEntry..Sla.
+00005180: 0843 616c 656e 6461 72da 0b53 6c61 5072  .Calendar..SlaPr
+00005190: 696f 7269 7479 da0e 4d79 436f 6d70 616e  iority..MyCompan
+000051a0: 794f 7468 6572 da07 486f 6c69 6461 79da  yOther..Holiday.
+000051b0: 0b48 6f6c 6964 6179 4c69 7374 da04 5479  .HolidayList..Ty
+000051c0: 7065 da07 5375 6254 7970 65da 0449 7465  pe..SubType..Ite
+000051d0: 6dda 0857 6f72 6b54 7970 65da 0857 6f72  m..WorkType..Wor
+000051e0: 6b52 6f6c 65da 0941 6772 6565 6d65 6e74  kRole..Agreement
+000051f0: da0b 5072 6f6a 6563 7454 7970 65da 1150  ..ProjectType..P
+00005200: 726f 6a65 6374 5465 616d 4d65 6d62 6572  rojectTeamMember
+00005210: 72fd 0000 0072 0800 0000 7278 0000 0072  r....r....rx...r
+00005220: 8000 0000 729a 0000 0072 c000 0000 da05  ....r....r......
+00005230: 6974 656d 7372 8700 0000 7288 0000 0072  itemsr....r....r
+00005240: ff00 0000 7206 0000 0072 f400 0000 72f6  ....r....r....r.
+00005250: 0000 0072 f900 0000 da0d 6173 7365 7274  ...r......assert
+00005260: 4772 6561 7465 7272 1000 0000 7216 0000  Greaterr....r...
+00005270: 0072 2700 0000 290b 721d 0000 005a 0d63  .r'...).r....Z.c
+00005280: 775f 6f62 6a65 6374 5f6d 6170 5a14 7072  w_object_mapZ.pr
+00005290: 655f 6675 6c6c 5f73 796e 635f 636f 756e  e_full_sync_coun
+000052a0: 7473 da03 6b65 79da 0b6d 6f64 656c 5f63  ts..key..model_c
+000052b0: 6c61 7373 72fb 0000 0072 1100 0000 7206  lassr....r....r.
+000052c0: 0100 0072 fc00 0000 7220 0000 0072 0701  ...r....r ...r..
+000052d0: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+000052e0: 0072 2e00 0000 8302 0000 7388 0000 0000  .r........s.....
+000052f0: 0304 0104 0104 0104 0104 0104 0104 0104  ................
+00005300: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+00005310: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+00005320: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+00005330: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+00005340: 0104 010a 0408 0208 0108 0108 0108 0204  ................
+00005350: 0212 0116 020a 010a 0212 010e 020c 0212  ................
+00005360: 0102 0100 0100 0100 0100 0108 0610 0108  ................
+00005370: 0102 0106 010a 027a 2154 6573 7453 796e  .......z!TestSyn
+00005380: 6341 6c6c 436f 6d6d 616e 642e 7465 7374  cAllCommand.test
+00005390: 5f66 756c 6c5f 7379 6e63 2901 4629 0872  _full_sync).F).r
+000053a0: 2f00 0000 7230 0000 0072 3100 0000 7238  /...r0...r1...r8
+000053b0: 0000 0072 fd00 0000 7208 0100 0072 2e00  ...r....r....r..
+000053c0: 0000 724e 0000 0072 0d00 0000 720d 0000  ..rN...r....r...
+000053d0: 0029 0172 4a00 0000 720e 0000 0072 f300  .).rJ...r....r..
+000053e0: 0000 2102 0000 7308 0000 0008 020c 390a  ..!...s.......9.
+000053f0: 0b08 1c72 f300 0000 6300 0000 0000 0000  ...r....c.......
+00005400: 0000 0000 0002 0000 0040 0000 0073 1400  .........@...s..
+00005410: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
+00005420: 5a03 6403 5300 2904 da14 5465 7374 4c69  Z.d.S.)...TestLi
+00005430: 7374 5573 6572 7343 6f6d 6d61 6e64 6301  stUsersCommandc.
+00005440: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00005450: 0000 0073 1400 0000 7c00 6a00 7401 6401  ...s....|.j.t.d.
+00005460: 8301 6400 8302 0100 6400 5300 2902 4e5a  ..d.....d.S.).NZ
+00005470: 0a6c 6973 745f 7573 6572 7329 0272 2c00  .list_users).r,.
+00005480: 0000 7202 0000 0029 0172 1d00 0000 720d  ..r....).r....r.
+00005490: 0000 0072 0d00 0000 720e 0000 00da 0c74  ...r....r......t
+000054a0: 6573 745f 636f 6d6d 616e 64dd 0200 0073  est_command....s
+000054b0: 0600 0000 0003 0401 0601 7a21 5465 7374  ..........z!Test
+000054c0: 4c69 7374 5573 6572 7343 6f6d 6d61 6e64  ListUsersCommand
+000054d0: 2e74 6573 745f 636f 6d6d 616e 644e 2904  .test_commandN).
+000054e0: 722f 0000 0072 3000 0000 7231 0000 0072  r/...r0...r1...r
+000054f0: 3301 0000 720d 0000 0072 0d00 0000 720d  3...r....r....r.
+00005500: 0000 0072 0e00 0000 7232 0100 00dc 0200  ...r....r2......
+00005510: 0073 0200 0000 0801 7232 0100 0029 3c72  .s......r2...)<r
+00005520: 1a00 0000 da16 646a 616e 676f 2e63 6f72  ......django.cor
+00005530: 652e 6d61 6e61 6765 6d65 6e74 7202 0000  e.managementr...
+00005540: 00da 0b64 6a61 6e67 6f2e 7465 7374 7203  ...django.testr.
+00005550: 0000 00da 0d64 6a63 6f6e 6e65 6374 7769  .....djconnectwi
+00005560: 7365 7204 0000 00da 0072 0600 0000 7207  ser......r....r.
+00005570: 0000 0072 0800 0000 720a 0000 0072 0f00  ...r....r....r..
+00005580: 0000 7210 0000 0072 1600 0000 da06 6f62  ..r....r......ob
+00005590: 6a65 6374 7217 0000 0072 3200 0000 7236  jectr....r2...r6
+000055a0: 0000 0072 3b00 0000 723f 0000 0072 4300  ...r;...r?...rC.
+000055b0: 0000 7247 0000 0072 4f00 0000 7253 0000  ..rG...rO...rS..
+000055c0: 0072 5800 0000 725c 0000 0072 6000 0000  .rX...r\...r`...
+000055d0: 7265 0000 0072 6900 0000 726d 0000 0072  re...ri...rm...r
+000055e0: 7100 0000 7276 0000 0072 7b00 0000 7284  q...rv...r{...r.
+000055f0: 0000 0072 8e00 0000 7292 0000 0072 9700  ...r....r....r..
+00005600: 0000 729e 0000 0072 a600 0000 72aa 0000  ..r....r....r...
+00005610: 0072 ae00 0000 72b2 0000 0072 b600 0000  .r....r....r....
+00005620: 72ba 0000 0072 be00 0000 72c3 0000 0072  r....r....r....r
+00005630: c700 0000 72cb 0000 0072 cf00 0000 72d3  ....r....r....r.
+00005640: 0000 0072 d700 0000 72dc 0000 0072 e000  ...r....r....r..
+00005650: 0000 72e4 0000 0072 e800 0000 72ec 0000  ..r....r....r...
+00005660: 0072 f000 0000 72f3 0000 0072 3201 0000  .r....r....r2...
+00005670: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00005680: 0e00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00005690: 0000 736e 0000 0008 020c 010c 020c 020c  ..sn............
+000056a0: 010c 010c 010c 0308 0608 0608 0410 2512  ..............%.
+000056b0: 0812 0b12 0812 0812 0812 0c12 0812 0c12  ................
+000056c0: 0812 0812 0b12 0912 0812 0812 0c12 0d12  ................
+000056d0: 1212 0f12 0b12 0d12 1212 1012 1112 0812  ................
+000056e0: 0812 0812 0812 1112 1712 0812 0812 0812  ................
+000056f0: 0812 1612 0e12 0d12 0d12 0c12 0c12 0c12  ................
+00005700: 1010 7f00 3c                             ....<
```

### Comparing `django-connectwise-0.3.98/djconnectwise/tests/__pycache__/test_views.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/tests/__pycache__/test_views.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,452 +1,417 @@
-00000000: 160d 0d0a a4b0 1f5d c81a 0000 e300 0000  .......]........
+00000000: 330d 0d0a 10ec da5c c81a 0000 e300 0000  3......\........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 e800 0000 6400 0064 0100 6c00 005a  .s....d..d..l..Z
-00000030: 0000 6400 0064 0100 6c01 005a 0100 6402  ..d..d..l..Z..d.
-00000040: 0064 0300 6c02 006d 0300 5a03 006d 0400  .d..l..m..Z..m..
-00000050: 5a04 006d 0500 5a05 0001 6400 0064 0400  Z..m..Z...d..d..
-00000060: 6c06 006d 0700 5a07 0001 6400 0064 0500  l..m..Z...d..d..
-00000070: 6c08 006d 0900 5a09 006d 0a00 5a0a 0001  l..m..Z..m..Z...
-00000080: 6400 0064 0600 6c0b 006d 0c00 5a0c 006d  d..d..l..m..Z..m
-00000090: 0d00 5a0d 006d 0e00 5a0e 0001 6400 0064  ..Z..m..Z...d..d
-000000a0: 0700 6c0f 006d 1000 5a10 006d 1100 5a11  ..l..m..Z..m..Z.
-000000b0: 0001 4764 0800 6409 0084 0000 6409 0065  ..Gd..d.....d..e
-000000c0: 0a00 8303 005a 1200 4764 0a00 640b 0084  .....Z..Gd..d...
-000000d0: 0000 640b 0065 1200 8303 005a 1300 4764  ..d..e.....Z..Gd
-000000e0: 0c00 640d 0084 0000 640d 0065 1200 8303  ..d.....d..e....
-000000f0: 005a 1400 4764 0e00 640f 0084 0000 640f  .Z..Gd..d.....d.
-00000100: 0065 1200 8303 005a 1500 6401 0053 2910  .e.....Z..d..S).
-00000110: e900 0000 004e e901 0000 0029 03da 0866  .....N.....)...f
-00000120: 6978 7475 7265 73da 0d66 6978 7475 7265  ixtures..fixture
-00000130: 5f75 7469 6c73 da05 6d6f 636b 7329 01da  _utils..mocks)..
-00000140: 0772 6576 6572 7365 2902 da06 436c 6965  .reverse)...Clie
-00000150: 6e74 da08 5465 7374 4361 7365 2903 da07  nt..TestCase)...
-00000160: 436f 6d70 616e 79da 0654 6963 6b65 74da  Company..Ticket.
-00000170: 0750 726f 6a65 6374 2902 da05 7669 6577  .Project)...view
-00000180: 73da 0361 7069 6300 0000 0000 0000 0000  s..apic.........
-00000190: 0000 0003 0000 0040 0000 0073 6400 0000  .......@...sd...
-000001a0: 6500 005a 0100 6400 005a 0200 6401 005a  e..Z..d..Z..d..Z
-000001b0: 0300 6402 0064 0300 8400 005a 0400 6404  ..d..d.....Z..d.
-000001c0: 0064 0500 8400 005a 0500 6401 0064 0600  .d.....Z..d..d..
-000001d0: 6407 0084 0100 5a06 0064 0800 6409 0084  d.....Z..d..d...
-000001e0: 0000 5a07 0064 0a00 640b 0084 0000 5a08  ..Z..d..d.....Z.
-000001f0: 0064 0c00 640d 0064 0e00 8401 005a 0900  .d..d..d.....Z..
-00000200: 6401 0053 290f da14 4261 7365 5465 7374  d..S)...BaseTest
-00000210: 4361 6c6c 4261 636b 5669 6577 4e63 0100  CallBackViewNc..
-00000220: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00000230: 0000 7322 0000 0074 0000 6a01 0083 0000  ..s"...t..j.....
-00000240: 0174 0000 6a02 0083 0000 0174 0000 6a03  .t..j......t..j.
-00000250: 0083 0000 0164 0000 5329 014e 2904 7204  .....d..S).N).r.
-00000260: 0000 00da 0b69 6e69 745f 626f 6172 6473  .....init_boards
-00000270: da13 696e 6974 5f62 6f61 7264 5f73 7461  ..init_board_sta
-00000280: 7475 7365 73da 0c69 6e69 745f 6d65 6d62  tuses..init_memb
-00000290: 6572 7329 01da 0473 656c 66a9 0072 1300  ers)...self..r..
-000002a0: 0000 fa5c 2f68 6f6d 652f 7361 6d2f 6769  ...\/home/sam/gi
-000002b0: 742f 4b61 6e62 616e 2f64 6a61 6e67 6f2d  t/Kanban/django-
-000002c0: 636f 6e6e 6563 7477 6973 652f 646a 616e  connectwise/djan
-000002d0: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
-000002e0: 6a63 6f6e 6e65 6374 7769 7365 2f74 6573  jconnectwise/tes
-000002f0: 7473 2f74 6573 745f 7669 6577 732e 7079  ts/test_views.py
-00000300: da05 7365 7455 700f 0000 0073 0600 0000  ..setUp....s....
-00000310: 0001 0a01 0a01 7a1a 4261 7365 5465 7374  ......z.BaseTest
-00000320: 4361 6c6c 4261 636b 5669 6577 2e73 6574  CallBackView.set
-00000330: 5570 6303 0000 0000 0000 0003 0000 0001  Upc.............
-00000340: 0000 0043 0000 0073 0a00 0000 7400 0082  ...C...s....t...
-00000350: 0100 6400 0053 2901 4e29 01da 134e 6f74  ..d..S).N)...Not
-00000360: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-00000370: 2903 7212 0000 00da 0869 6e73 7461 6e63  ).r......instanc
-00000380: 65da 0665 6e74 6974 7972 1300 0000 7213  e..entityr....r.
-00000390: 0000 0072 1400 0000 da0d 6173 7365 7274  ...r......assert
-000003a0: 5f66 6965 6c64 7314 0000 0073 0200 0000  _fields....s....
-000003b0: 0001 7a22 4261 7365 5465 7374 4361 6c6c  ..z"BaseTestCall
-000003c0: 4261 636b 5669 6577 2e61 7373 6572 745f  BackView.assert_
-000003d0: 6669 656c 6473 6305 0000 0000 0000 0008  fieldsc.........
-000003e0: 0000 0009 0000 0043 0000 0073 6700 0000  .......C...sg...
-000003f0: 7400 0083 0000 7d05 0064 0100 7c01 0064  t.....}..d..|..d
-00000400: 0200 7c02 0064 0300 7c03 0064 0400 7c04  ..|..d..|..d..|.
-00000410: 0072 3300 7401 006a 0200 7c04 0083 0100  .r3.t..j..|.....
-00000420: 6e03 0064 0000 6904 007d 0600 7401 006a  n..d..i..}..t..j
-00000430: 0200 7c06 0083 0100 7d07 007c 0500 6a03  ..|.....}..|..j.
-00000440: 0074 0400 6405 0083 0100 7c07 0064 0600  .t..d.....|..d..
-00000450: 6407 0083 0201 5329 084e da04 5479 7065  d.....S).N..Type
-00000460: da06 4163 7469 6f6e da02 4944 da06 456e  ..Action..ID..En
-00000470: 7469 7479 7a16 646a 636f 6e6e 6563 7477  tityz.djconnectw
-00000480: 6973 653a 6361 6c6c 6261 636b da0c 636f  ise:callback..co
-00000490: 6e74 656e 745f 7479 7065 7a10 6170 706c  ntent_typez.appl
-000004a0: 6963 6174 696f 6e2f 6a73 6f6e 2905 7207  ication/json).r.
-000004b0: 0000 00da 046a 736f 6eda 0564 756d 7073  .....json..dumps
-000004c0: da04 706f 7374 7206 0000 0029 0872 1200  ..postr....).r..
-000004d0: 0000 da0d 6361 6c6c 6261 636b 5f74 7970  ....callback_typ
-000004e0: 65da 0661 6374 696f 6eda 0965 6e74 6974  e..action..entit
-000004f0: 795f 6964 7218 0000 00da 0663 6c69 656e  y_idr......clien
-00000500: 74da 0462 6f64 795a 0962 6f64 795f 6a73  t..bodyZ.body_js
-00000510: 6f6e 7213 0000 0072 1300 0000 7214 0000  onr....r....r...
-00000520: 00da 0970 6f73 745f 6461 7461 1700 0000  ...post_data....
-00000530: 7314 0000 0000 0109 0206 0106 0106 0121  s..............!
-00000540: 020f 0206 0109 0106 017a 1e42 6173 6554  .........z.BaseT
-00000550: 6573 7443 616c 6c42 6163 6b56 6965 772e  estCallBackView.
-00000560: 706f 7374 5f64 6174 6163 0300 0000 0000  post_datac......
-00000570: 0000 0600 0000 0500 0000 4300 0000 7395  ..........C...s.
-00000580: 0000 007c 0000 6a00 007c 0100 7401 006a  ...|..j..|..t..j
-00000590: 0200 7c02 0064 0100 197c 0200 8304 007d  ..|..d...|.....}
-000005a0: 0300 7403 007c 0000 6a04 006a 0500 6a06  ..t..|..j..j..j.
-000005b0: 0083 0000 8301 007d 0400 7c04 0064 0200  .......}..|..d..
-000005c0: 197d 0500 7c00 006a 0700 7c05 007c 0200  .}..|..j..|..|..
-000005d0: 8302 0001 7c00 006a 0800 7c05 006a 0900  ....|..j..|..j..
-000005e0: 7c02 0064 0100 1983 0200 017c 0000 6a08  |..d.......|..j.
-000005f0: 0074 0a00 7c04 0083 0100 6403 0083 0200  .t..|.....d.....
-00000600: 017c 0000 6a08 007c 0300 6a0b 0064 0400  .|..j..|..j..d..
-00000610: 8302 0001 6400 0053 2905 4eda 0269 6472  ....d..S).N..idr
-00000620: 0100 0000 7202 0000 00e9 cc00 0000 290c  ....r.........).
-00000630: 7227 0000 0072 0c00 0000 5a0e 4341 4c4c  r'...r....Z.CALL
-00000640: 4241 434b 5f41 4444 4544 da04 6c69 7374  BACK_ADDED..list
-00000650: da0b 4d4f 4445 4c5f 434c 4153 53da 076f  ..MODEL_CLASS..o
-00000660: 626a 6563 7473 da03 616c 6c72 1900 0000  bjects..allr....
-00000670: da0b 6173 7365 7274 4571 7561 6c72 2800  ..assertEqualr(.
-00000680: 0000 da03 6c65 6eda 0b73 7461 7475 735f  ....len..status_
-00000690: 636f 6465 2906 7212 0000 0072 2200 0000  code).r....r"...
-000006a0: 7218 0000 00da 0872 6573 706f 6e73 65da  r......response.
-000006b0: 0969 6e73 7461 6e63 6573 7217 0000 0072  .instancesr....r
-000006c0: 1300 0000 7213 0000 0072 1400 0000 da0b  ....r....r......
-000006d0: 5f74 6573 745f 6164 6465 6427 0000 0073  _test_added'...s
-000006e0: 1600 0000 0001 0601 0301 0601 0701 0903  ................
-000006f0: 1801 0a02 1001 1701 1601 7a20 4261 7365  ..........z Base
-00000700: 5465 7374 4361 6c6c 4261 636b 5669 6577  TestCallBackView
-00000710: 2e5f 7465 7374 5f61 6464 6564 6303 0000  ._test_addedc...
-00000720: 0000 0000 0006 0000 0005 0000 0043 0000  .............C..
-00000730: 0073 9500 0000 7c00 006a 0000 7c01 0074  .s....|..j..|..t
-00000740: 0100 6a02 007c 0200 6401 0019 7c02 0083  ..j..|..d...|...
-00000750: 0400 7d03 0074 0300 7c00 006a 0400 6a05  ..}..t..|..j..j.
-00000760: 006a 0600 8300 0083 0100 7d04 007c 0400  .j........}..|..
-00000770: 6402 0019 7d05 007c 0000 6a07 007c 0500  d...}..|..j..|..
-00000780: 7c02 0083 0200 017c 0000 6a08 007c 0500  |......|..j..|..
-00000790: 6a09 007c 0200 6401 0019 8302 0001 7c00  j..|..d.......|.
-000007a0: 006a 0800 740a 007c 0400 8301 0064 0300  .j..t..|.....d..
-000007b0: 8302 0001 7c00 006a 0800 7c03 006a 0b00  ....|..j..|..j..
-000007c0: 6404 0083 0200 0164 0000 5329 054e 7228  d......d..S).Nr(
-000007d0: 0000 0072 0100 0000 7202 0000 0072 2900  ...r....r....r).
-000007e0: 0000 290c 7227 0000 0072 0c00 0000 5a10  ..).r'...r....Z.
-000007f0: 4341 4c4c 4241 434b 5f55 5044 4154 4544  CALLBACK_UPDATED
-00000800: 722a 0000 0072 2b00 0000 722c 0000 0072  r*...r+...r,...r
-00000810: 2d00 0000 7219 0000 0072 2e00 0000 7228  -...r....r....r(
-00000820: 0000 0072 2f00 0000 7230 0000 0029 0672  ...r/...r0...).r
-00000830: 1200 0000 7222 0000 0072 1800 0000 7231  ....r"...r....r1
-00000840: 0000 0072 3200 0000 7217 0000 0072 1300  ...r2...r....r..
-00000850: 0000 7213 0000 0072 1400 0000 da0c 5f74  ..r....r......_t
-00000860: 6573 745f 7570 6461 7465 3700 0000 7316  est_update7...s.
-00000870: 0000 0000 0106 0103 0106 0107 0109 0318  ................
-00000880: 010a 0210 0117 0116 017a 2142 6173 6554  .........z!BaseT
-00000890: 6573 7443 616c 6c42 6163 6b56 6965 772e  estCallBackView.
-000008a0: 5f74 6573 745f 7570 6461 7465 722c 0000  _test_updater,..
-000008b0: 0063 0400 0000 0000 0000 0700 0000 0400  .c..............
-000008c0: 0000 4300 0000 7369 0000 007c 0000 6a00  ..C...si...|..j.
-000008d0: 007c 0100 7401 006a 0200 7c02 0083 0300  .|..t..j..|.....
-000008e0: 7d04 0074 0300 7c00 006a 0400 7c03 0083  }..t..|..j..|...
-000008f0: 0200 7d05 0074 0500 7c05 006a 0600 8300  ..}..t..|..j....
-00000900: 0083 0100 7d06 007c 0000 6a07 007c 0400  ....}..|..j..|..
-00000910: 6a08 0064 0100 8302 0001 7c00 006a 0700  j..d......|..j..
-00000920: 7409 007c 0600 8301 0064 0200 8302 0001  t..|.....d......
-00000930: 6400 0053 2903 4e72 2900 0000 7201 0000  d..S).Nr)...r...
-00000940: 0029 0a72 2700 0000 720c 0000 005a 1043  .).r'...r....Z.C
-00000950: 414c 4c42 4143 4b5f 4445 4c45 5445 44da  ALLBACK_DELETED.
-00000960: 0767 6574 6174 7472 722b 0000 0072 2a00  .getattrr+...r*.
-00000970: 0000 722d 0000 0072 2e00 0000 7230 0000  ..r-...r....r0..
-00000980: 0072 2f00 0000 2907 7212 0000 0072 2200  .r/...).r....r".
-00000990: 0000 7224 0000 00da 076d 616e 6167 6572  ..r$.....manager
-000009a0: 7231 0000 005a 0d6d 6f64 656c 5f6d 616e  r1...Z.model_man
-000009b0: 6167 6572 7232 0000 0072 1300 0000 7213  agerr2...r....r.
-000009c0: 0000 0072 1400 0000 da0c 5f74 6573 745f  ...r......_test_
-000009d0: 6465 6c65 7465 4700 0000 7310 0000 0000  deleteG...s.....
-000009e0: 0106 0103 0106 0109 0612 0112 0113 017a  ...............z
-000009f0: 2142 6173 6554 6573 7443 616c 6c42 6163  !BaseTestCallBac
-00000a00: 6b56 6965 772e 5f74 6573 745f 6465 6c65  kView._test_dele
-00000a10: 7465 290a da08 5f5f 6e61 6d65 5f5f da0a  te)...__name__..
-00000a20: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000a30: 616c 6e61 6d65 5f5f 722b 0000 0072 1500  alname__r+...r..
-00000a40: 0000 7219 0000 0072 2700 0000 7233 0000  ..r....r'...r3..
-00000a50: 0072 3400 0000 7237 0000 0072 1300 0000  .r4...r7...r....
-00000a60: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00000a70: 0e00 0000 0c00 0000 730e 0000 000c 0106  ........s.......
-00000a80: 020c 050c 030f 100c 100c 1072 0e00 0000  ...........r....
-00000a90: 6300 0000 0000 0000 0000 0000 0002 0000  c...............
-00000aa0: 0040 0000 0073 4600 0000 6500 005a 0100  .@...sF...e..Z..
-00000ab0: 6400 005a 0200 6503 005a 0400 6401 0064  d..Z..e..Z..d..d
-00000ac0: 0200 8400 005a 0500 6403 0064 0400 8400  .....Z..d..d....
-00000ad0: 005a 0600 6405 0064 0600 8400 005a 0700  .Z..d..d.....Z..
-00000ae0: 6407 0064 0800 8400 005a 0800 6409 0053  d..d.....Z..d..S
-00000af0: 290a da16 5465 7374 5469 636b 6574 4361  )...TestTicketCa
-00000b00: 6c6c 4261 636b 5669 6577 6303 0000 0000  llBackViewc.....
-00000b10: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
-00000b20: 1b00 0000 7c00 006a 0000 7c01 006a 0100  ....|..j..|..j..
-00000b30: 7c02 0064 0100 1983 0200 0164 0000 5329  |..d.......d..S)
-00000b40: 024e da07 7375 6d6d 6172 7929 0272 2e00  .N..summary).r..
-00000b50: 0000 723c 0000 0029 0372 1200 0000 7217  ..r<...).r....r.
-00000b60: 0000 0072 1800 0000 7213 0000 0072 1300  ...r....r....r..
-00000b70: 0000 7214 0000 0072 1900 0000 5a00 0000  ..r....r....Z...
-00000b80: 7302 0000 0000 017a 2454 6573 7454 6963  s......z$TestTic
-00000b90: 6b65 7443 616c 6c42 6163 6b56 6965 772e  ketCallBackView.
-00000ba0: 6173 7365 7274 5f66 6965 6c64 7363 0100  assert_fieldsc..
-00000bb0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00000bc0: 0000 7376 0000 0074 0000 6a01 0083 0000  ..sv...t..j.....
-00000bd0: 0174 0000 6a02 0083 0000 0174 0000 6a03  .t..j......t..j.
-00000be0: 0083 0000 0174 0000 6a04 0083 0000 0174  .....t..j......t
-00000bf0: 0000 6a05 0083 0000 0174 0000 6a06 0083  ..j......t..j...
-00000c00: 0000 017c 0000 6a07 0074 0800 6a09 006a  ...|..j..t..j..j
-00000c10: 0a00 8300 0064 0100 8302 0001 740b 006a  .....d......t..j
-00000c20: 0c00 8300 0001 7c00 006a 0d00 6402 0074  ......|..j..d..t
-00000c30: 0e00 6a0f 0083 0200 0164 0000 5329 034e  ..j......d..S).N
-00000c40: 7201 0000 00da 0674 6963 6b65 7429 1072  r......ticket).r
-00000c50: 0400 0000 da0f 696e 6974 5f70 7269 6f72  ......init_prior
-00000c60: 6974 6965 73da 0d69 6e69 745f 7072 6f6a  ities..init_proj
-00000c70: 6563 7473 da0e 696e 6974 5f63 6f6d 7061  ects..init_compa
-00000c80: 6e69 6573 7210 0000 00da 0e69 6e69 745f  niesr......init_
-00000c90: 6c6f 6361 7469 6f6e 73da 0a69 6e69 745f  locations..init_
-00000ca0: 7465 616d 7372 2e00 0000 720a 0000 0072  teamsr....r....r
-00000cb0: 2c00 0000 da05 636f 756e 7472 0500 0000  ,.....countr....
-00000cc0: da1b 7365 7276 6963 655f 6170 695f 6765  ..service_api_ge
-00000cd0: 745f 7469 636b 6574 5f63 616c 6c72 3300  t_ticket_callr3.
-00000ce0: 0000 7203 0000 00da 1241 5049 5f53 4552  ..r......API_SER
-00000cf0: 5649 4345 5f54 4943 4b45 5429 0172 1200  VICE_TICKET).r..
-00000d00: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00000d10: 00da 0874 6573 745f 6164 645d 0000 0073  ...test_add]...s
-00000d20: 1200 0000 0001 0a01 0a01 0a01 0a01 0a01  ................
-00000d30: 0a01 1901 0a01 7a1f 5465 7374 5469 636b  ......z.TestTick
-00000d40: 6574 4361 6c6c 4261 636b 5669 6577 2e74  etCallBackView.t
-00000d50: 6573 745f 6164 6463 0100 0000 0000 0000  est_addc........
-00000d60: 0200 0000 0300 0000 4300 0000 73a8 0000  ........C...s...
-00000d70: 0074 0000 6a01 0083 0000 0174 0000 6a02  .t..j......t..j.
-00000d80: 0083 0000 0174 0000 6a03 0083 0000 0174  .....t..j......t
-00000d90: 0000 6a04 0083 0000 0174 0000 6a05 0083  ..j......t..j...
-00000da0: 0000 0174 0000 6a06 0083 0000 0174 0000  ...t..j......t..
-00000db0: 6a07 0083 0000 017c 0000 6a08 0074 0900  j......|..j..t..
-00000dc0: 6a0a 006a 0b00 8300 0064 0100 8302 0001  j..j.....d......
-00000dd0: 7409 006a 0a00 6a0c 0064 0200 6403 0083  t..j..j..d..d...
-00000de0: 0001 7d01 0064 0400 7c01 005f 0d00 7c01  ..}..d..|.._..|.
-00000df0: 006a 0e00 8300 0001 740f 006a 1000 8300  .j......t..j....
-00000e00: 0001 7c00 006a 1100 6405 0074 1200 6a13  ..|..j..d..t..j.
-00000e10: 0083 0200 0164 0000 5329 064e 7202 0000  .....d..S).Nr...
-00000e20: 0072 2800 0000 e945 0000 00da 0666 6f6f  .r(....E.....foo
-00000e30: 6261 7272 3d00 0000 2914 7204 0000 0072  barr=...).r....r
-00000e40: 3e00 0000 723f 0000 0072 4000 0000 7210  >...r?...r@...r.
-00000e50: 0000 0072 4100 0000 7242 0000 00da 0c69  ...rA...rB.....i
-00000e60: 6e69 745f 7469 636b 6574 7372 2e00 0000  nit_ticketsr....
-00000e70: 720a 0000 0072 2c00 0000 7243 0000 00da  r....r,...rC....
-00000e80: 0367 6574 723c 0000 00da 0473 6176 6572  .getr<.....saver
-00000e90: 0500 0000 7244 0000 0072 3400 0000 7203  ....rD...r4...r.
-00000ea0: 0000 0072 4500 0000 2902 7212 0000 00da  ...rE...).r.....
-00000eb0: 0174 7213 0000 0072 1300 0000 7214 0000  .tr....r....r...
-00000ec0: 00da 0b74 6573 745f 7570 6461 7465 6800  ...test_updateh.
-00000ed0: 0000 731a 0000 0000 010a 010a 010a 010a  ..s.............
-00000ee0: 010a 010a 010a 0119 0215 0109 010a 020a  ................
-00000ef0: 017a 2254 6573 7454 6963 6b65 7443 616c  .z"TestTicketCal
-00000f00: 6c42 6163 6b56 6965 772e 7465 7374 5f75  lBackView.test_u
-00000f10: 7064 6174 6563 0100 0000 0000 0000 0100  pdatec..........
-00000f20: 0000 0400 0000 4300 0000 7376 0000 0074  ......C...sv...t
-00000f30: 0000 6a01 0083 0000 0174 0000 6a02 0083  ..j......t..j...
-00000f40: 0000 0174 0000 6a03 0083 0000 0174 0000  ...t..j......t..
-00000f50: 6a04 0083 0000 0174 0000 6a05 0083 0000  j......t..j.....
-00000f60: 017c 0000 6a06 0074 0700 6a08 006a 0900  .|..j..t..j..j..
-00000f70: 8300 0064 0100 8302 0001 740a 006a 0b00  ...d......t..j..
-00000f80: 740c 006a 0d00 8301 0001 7c00 006a 0e00  t..j......|..j..
-00000f90: 6402 0074 0f00 6a10 0064 0300 1983 0200  d..t..j..d......
-00000fa0: 0164 0000 5329 044e 7202 0000 0072 3d00  .d..S).Nr....r=.
-00000fb0: 0000 7228 0000 0029 1172 0400 0000 7249  ..r(...).r....rI
-00000fc0: 0000 0072 3e00 0000 7240 0000 0072 4100  ...r>...r@...rA.
-00000fd0: 0000 7242 0000 0072 2e00 0000 720a 0000  ..rB...r....r...
-00000fe0: 0072 2c00 0000 7243 0000 0072 0500 0000  .r,...rC...r....
-00000ff0: 7244 0000 0072 0d00 0000 da1e 436f 6e6e  rD...r......Conn
-00001000: 6563 7457 6973 6552 6563 6f72 644e 6f74  ectWiseRecordNot
-00001010: 466f 756e 6445 7272 6f72 7237 0000 0072  FoundErrorr7...r
-00001020: 0300 0000 7245 0000 0029 0172 1200 0000  ....rE...).r....
-00001030: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-00001040: 0b74 6573 745f 6465 6c65 7465 7900 0000  .test_deletey...
-00001050: 7314 0000 0000 010a 010a 010a 010a 010a  s...............
-00001060: 0119 0210 0106 0103 017a 2254 6573 7454  .........z"TestT
-00001070: 6963 6b65 7443 616c 6c42 6163 6b56 6965  icketCallBackVie
-00001080: 772e 7465 7374 5f64 656c 6574 654e 2909  w.test_deleteN).
-00001090: 7238 0000 0072 3900 0000 723a 0000 0072  r8...r9...r:...r
-000010a0: 0a00 0000 722b 0000 0072 1900 0000 7246  ....r+...r....rF
-000010b0: 0000 0072 4d00 0000 724f 0000 0072 1300  ...rM...rO...r..
-000010c0: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
-000010d0: 0072 3b00 0000 5700 0000 730a 0000 000c  .r;...W...s.....
-000010e0: 0106 020c 030c 0b0c 1172 3b00 0000 6300  .........r;...c.
-000010f0: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
-00001100: 0000 0073 4600 0000 6500 005a 0100 6400  ...sF...e..Z..d.
-00001110: 005a 0200 6503 005a 0400 6401 0064 0200  .Z..e..Z..d..d..
-00001120: 8400 005a 0500 6403 0064 0400 8400 005a  ...Z..d..d.....Z
-00001130: 0600 6405 0064 0600 8400 005a 0700 6407  ..d..d.....Z..d.
-00001140: 0064 0800 8400 005a 0800 6409 0053 290a  .d.....Z..d..S).
-00001150: da17 5465 7374 5072 6f6a 6563 7443 616c  ..TestProjectCal
-00001160: 6c42 6163 6b56 6965 7763 0300 0000 0000  lBackViewc......
-00001170: 0000 0300 0000 0400 0000 4300 0000 731b  ..........C...s.
-00001180: 0000 007c 0000 6a00 007c 0100 6a01 007c  ...|..j..|..j..|
-00001190: 0200 6401 0019 8302 0001 6400 0053 2902  ..d.......d..S).
-000011a0: 4eda 046e 616d 6529 0272 2e00 0000 7251  N..name).r....rQ
-000011b0: 0000 0029 0372 1200 0000 7217 0000 0072  ...).r....r....r
-000011c0: 1800 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
-000011d0: 0000 0072 1900 0000 8b00 0000 7302 0000  ...r........s...
-000011e0: 0000 017a 2554 6573 7450 726f 6a65 6374  ...z%TestProject
-000011f0: 4361 6c6c 4261 636b 5669 6577 2e61 7373  CallBackView.ass
-00001200: 6572 745f 6669 656c 6473 6301 0000 0000  ert_fieldsc.....
-00001210: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-00001220: 4a00 0000 7400 006a 0100 8300 0001 7c00  J...t..j......|.
-00001230: 006a 0200 7403 006a 0400 6a05 0083 0000  .j..t..j..j.....
-00001240: 6401 0083 0200 0174 0600 6a07 0074 0800  d......t..j..t..
-00001250: 6a09 0083 0100 017c 0000 6a0a 0064 0200  j......|..j..d..
-00001260: 7408 006a 0900 8302 0001 6400 0053 2903  t..j......d..S).
-00001270: 4e72 0100 0000 da07 7072 6f6a 6563 7429  Nr......project)
-00001280: 0b72 0400 0000 da15 696e 6974 5f70 726f  .r......init_pro
-00001290: 6a65 6374 5f73 7461 7475 7365 7372 2e00  ject_statusesr..
-000012a0: 0000 720b 0000 0072 2c00 0000 7243 0000  ..r....r,...rC..
-000012b0: 0072 0500 0000 da1c 7072 6f6a 6563 745f  .r......project_
-000012c0: 6170 695f 6765 745f 7072 6f6a 6563 745f  api_get_project_
-000012d0: 6361 6c6c 7203 0000 00da 0b41 5049 5f50  callr......API_P
-000012e0: 524f 4a45 4354 7233 0000 0029 0172 1200  ROJECTr3...).r..
-000012f0: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00001300: 0072 4600 0000 8e00 0000 7308 0000 0000  .rF.......s.....
-00001310: 010a 0119 0110 017a 2054 6573 7450 726f  .......z TestPro
-00001320: 6a65 6374 4361 6c6c 4261 636b 5669 6577  jectCallBackView
-00001330: 2e74 6573 745f 6164 6463 0100 0000 0000  .test_addc......
-00001340: 0000 0200 0000 0300 0000 4300 0000 737c  ..........C...s|
-00001350: 0000 0074 0000 6a01 0083 0000 0174 0000  ...t..j......t..
-00001360: 6a02 0083 0000 017c 0000 6a03 0074 0400  j......|..j..t..
-00001370: 6a05 006a 0600 8300 0064 0100 8302 0001  j..j.....d......
-00001380: 7404 006a 0500 6a07 0064 0200 6403 0083  t..j..j..d..d...
-00001390: 0001 7d01 0064 0400 7c01 005f 0800 7c01  ..}..d..|.._..|.
-000013a0: 006a 0900 8300 0001 740a 006a 0b00 740c  .j......t..j..t.
-000013b0: 006a 0d00 8301 0001 7c00 006a 0e00 6405  .j......|..j..d.
-000013c0: 0074 0c00 6a0d 0083 0200 0164 0000 5329  .t..j......d..S)
-000013d0: 064e 7202 0000 0072 2800 0000 e905 0000  .Nr....r(.......
-000013e0: 0072 4800 0000 7252 0000 0029 0f72 0400  .rH...rR...).r..
-000013f0: 0000 7253 0000 0072 3f00 0000 722e 0000  ..rS...r?...r...
-00001400: 0072 0b00 0000 722c 0000 0072 4300 0000  .r....r,...rC...
-00001410: 724a 0000 0072 5100 0000 724b 0000 0072  rJ...rQ...rK...r
-00001420: 0500 0000 7254 0000 0072 0300 0000 7255  ....rT...r....rU
-00001430: 0000 0072 3400 0000 2902 7212 0000 00da  ...r4...).r.....
-00001440: 0170 7213 0000 0072 1300 0000 7214 0000  .pr....r....r...
-00001450: 0072 4d00 0000 9400 0000 7310 0000 0000  .rM.......s.....
-00001460: 010a 010a 0119 0215 0109 010a 0210 017a  ...............z
-00001470: 2354 6573 7450 726f 6a65 6374 4361 6c6c  #TestProjectCall
-00001480: 4261 636b 5669 6577 2e74 6573 745f 7570  BackView.test_up
-00001490: 6461 7465 6301 0000 0000 0000 0001 0000  datec...........
-000014a0: 0004 0000 0043 0000 0073 5e00 0000 7400  .....C...s^...t.
-000014b0: 006a 0100 8300 0001 7400 006a 0200 8300  .j......t..j....
-000014c0: 0001 7c00 006a 0300 7404 006a 0500 6a06  ..|..j..t..j..j.
-000014d0: 0083 0000 6401 0083 0200 0174 0700 6a08  ....d......t..j.
-000014e0: 0064 0000 6402 0074 0900 6a0a 0083 0101  .d..d..t..j.....
-000014f0: 017c 0000 6a0b 0064 0300 740c 006a 0d00  .|..j..d..t..j..
-00001500: 6404 0019 8302 0001 6400 0053 2905 4e72  d.......d..S).Nr
-00001510: 0200 0000 da06 7261 6973 6564 7252 0000  ......raisedrR..
-00001520: 0072 2800 0000 290e 7204 0000 0072 5300  .r(...).r....rS.
-00001530: 0000 723f 0000 0072 2e00 0000 720b 0000  ..r?...r....r...
-00001540: 0072 2c00 0000 7243 0000 0072 0500 0000  .r,...rC...r....
-00001550: 7254 0000 0072 0d00 0000 724e 0000 0072  rT...r....rN...r
-00001560: 3700 0000 7203 0000 0072 5500 0000 2901  7...r....rU...).
-00001570: 7212 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
-00001580: 1400 0000 724f 0000 00a0 0000 0073 1200  ....rO.......s..
-00001590: 0000 0001 0a01 0a01 1902 0601 0601 0a02  ................
-000015a0: 0601 0301 7a23 5465 7374 5072 6f6a 6563  ....z#TestProjec
-000015b0: 7443 616c 6c42 6163 6b56 6965 772e 7465  tCallBackView.te
-000015c0: 7374 5f64 656c 6574 654e 2909 7238 0000  st_deleteN).r8..
-000015d0: 0072 3900 0000 723a 0000 0072 0b00 0000  .r9...r:...r....
-000015e0: 722b 0000 0072 1900 0000 7246 0000 0072  r+...r....rF...r
-000015f0: 4d00 0000 724f 0000 0072 1300 0000 7213  M...rO...r....r.
-00001600: 0000 0072 1300 0000 7214 0000 0072 5000  ...r....r....rP.
-00001610: 0000 8800 0000 730a 0000 000c 0106 020c  ......s.........
-00001620: 030c 060c 0c72 5000 0000 6300 0000 0000  .....rP...c.....
-00001630: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
-00001640: 4600 0000 6500 005a 0100 6400 005a 0200  F...e..Z..d..Z..
-00001650: 6503 005a 0400 6401 0064 0200 8400 005a  e..Z..d..d.....Z
-00001660: 0500 6403 0064 0400 8400 005a 0600 6405  ..d..d.....Z..d.
-00001670: 0064 0600 8400 005a 0700 6407 0064 0800  .d.....Z..d..d..
-00001680: 8400 005a 0800 6409 0053 290a da17 5465  ...Z..d..S)...Te
-00001690: 7374 436f 6d70 616e 7943 616c 6c42 6163  stCompanyCallBac
-000016a0: 6b56 6965 7763 0300 0000 0000 0000 0300  kViewc..........
-000016b0: 0000 0400 0000 4300 0000 731b 0000 007c  ......C...s....|
-000016c0: 0000 6a00 007c 0100 6a01 007c 0200 6401  ..j..|..j..|..d.
-000016d0: 0019 8302 0001 6400 0053 2902 4e72 5100  ......d..S).NrQ.
-000016e0: 0000 2902 722e 0000 0072 5100 0000 2903  ..).r....rQ...).
-000016f0: 7212 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-00001700: 1300 0000 7213 0000 0072 1400 0000 7219  ....r....r....r.
-00001710: 0000 00b2 0000 0073 0200 0000 0001 7a25  .......s......z%
-00001720: 5465 7374 436f 6d70 616e 7943 616c 6c42  TestCompanyCallB
-00001730: 6163 6b56 6965 772e 6173 7365 7274 5f66  ackView.assert_f
-00001740: 6965 6c64 7363 0100 0000 0000 0000 0100  ieldsc..........
-00001750: 0000 0300 0000 4300 0000 7340 0000 007c  ......C...s@...|
-00001760: 0000 6a00 0074 0100 6a02 006a 0300 8300  ..j..t..j..j....
-00001770: 0064 0100 8302 0001 7404 006a 0500 7406  .d......t..j..t.
-00001780: 006a 0700 8301 0001 7c00 006a 0800 6402  .j......|..j..d.
-00001790: 0074 0600 6a07 0083 0200 0164 0000 5329  .t..j......d..S)
-000017a0: 034e 7201 0000 00da 0763 6f6d 7061 6e79  .Nr......company
-000017b0: 2909 722e 0000 0072 0900 0000 722c 0000  ).r....r....r,..
-000017c0: 0072 4300 0000 7205 0000 00da 1663 6f6d  .rC...r......com
-000017d0: 7061 6e79 5f61 7069 5f62 795f 6964 5f63  pany_api_by_id_c
-000017e0: 616c 6c72 0300 0000 da0b 4150 495f 434f  allr......API_CO
-000017f0: 4d50 414e 5972 3300 0000 2901 7212 0000  MPANYr3...).r...
-00001800: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
-00001810: 7246 0000 00b5 0000 0073 0600 0000 0001  rF.......s......
-00001820: 1901 1001 7a20 5465 7374 436f 6d70 616e  ....z TestCompan
-00001830: 7943 616c 6c42 6163 6b56 6965 772e 7465  yCallBackView.te
-00001840: 7374 5f61 6464 6301 0000 0000 0000 0002  st_addc.........
-00001850: 0000 0003 0000 0043 0000 0073 7200 0000  .......C...sr...
-00001860: 7400 006a 0100 8300 0001 7c00 006a 0200  t..j......|..j..
-00001870: 7403 006a 0400 6a05 0083 0000 6401 0083  t..j..j.....d...
-00001880: 0200 0174 0300 6a04 006a 0600 6402 0064  ...t..j..j..d..d
-00001890: 0300 8300 017d 0100 6404 007c 0100 5f07  .....}..d..|.._.
-000018a0: 007c 0100 6a08 0083 0000 0174 0900 6a0a  .|..j......t..j.
-000018b0: 0074 0b00 6a0c 0083 0100 017c 0000 6a0d  .t..j......|..j.
-000018c0: 0064 0500 740b 006a 0c00 8302 0001 6400  .d..t..j......d.
-000018d0: 0053 2906 4e72 0200 0000 7228 0000 00e9  .S).Nr....r(....
-000018e0: 0200 0000 7248 0000 0072 5a00 0000 290e  ....rH...rZ...).
-000018f0: 7204 0000 0072 4000 0000 722e 0000 0072  r....r@...r....r
-00001900: 0900 0000 722c 0000 0072 4300 0000 724a  ....r,...rC...rJ
-00001910: 0000 0072 5100 0000 724b 0000 0072 0500  ...rQ...rK...r..
-00001920: 0000 725b 0000 0072 0300 0000 725c 0000  ..r[...r....r\..
-00001930: 0072 3400 0000 2902 7212 0000 00da 0163  .r4...).r......c
-00001940: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00001950: 4d00 0000 ba00 0000 730e 0000 0000 010a  M.......s.......
-00001960: 0119 0215 0109 010a 0210 017a 2354 6573  ...........z#Tes
-00001970: 7443 6f6d 7061 6e79 4361 6c6c 4261 636b  tCompanyCallBack
-00001980: 5669 6577 2e74 6573 745f 7570 6461 7465  View.test_update
-00001990: 6301 0000 0000 0000 0002 0000 0005 0000  c...............
-000019a0: 0043 0000 0073 6a00 0000 7400 006a 0100  .C...sj...t..j..
-000019b0: 8300 0001 7c00 006a 0200 7403 006a 0400  ....|..j..t..j..
-000019c0: 6a05 0083 0000 6401 0083 0200 0174 0600  j.....d......t..
-000019d0: 6a07 0074 0800 6a09 0083 0100 7d01 0064  j..t..j.....}..d
-000019e0: 0200 7c01 0064 0300 3c74 0a00 6a0b 007c  ..|..d..<t..j..|
-000019f0: 0100 8301 0001 7c00 006a 0c00 6404 007c  ......|..j..d..|
-00001a00: 0100 6405 0019 6406 0064 0700 8302 0101  ..d...d..d......
-00001a10: 6400 0053 2908 4e72 0200 0000 54da 0b64  d..S).Nr....T..d
-00001a20: 656c 6574 6564 466c 6167 725a 0000 0072  eletedFlagrZ...r
-00001a30: 2800 0000 7236 0000 00da 1161 7661 696c  (...r6.....avail
-00001a40: 6162 6c65 5f6f 626a 6563 7473 290d 7204  able_objects).r.
-00001a50: 0000 0072 4000 0000 722e 0000 0072 0900  ...r@...r....r..
-00001a60: 0000 722c 0000 0072 4300 0000 da04 636f  ..r,...rC.....co
-00001a70: 7079 da08 6465 6570 636f 7079 7203 0000  py..deepcopyr...
-00001a80: 0072 5c00 0000 7205 0000 0072 5b00 0000  .r\...r....r[...
-00001a90: 7237 0000 0029 0272 1200 0000 5a0f 636f  r7...).r....Z.co
-00001aa0: 6d70 616e 795f 6669 7874 7572 6572 1300  mpany_fixturer..
-00001ab0: 0000 7213 0000 0072 1400 0000 724f 0000  ..r....r....rO..
-00001ac0: 00c5 0000 0073 1200 0000 0001 0a01 1904  .....s..........
-00001ad0: 1201 0a01 0d01 0601 0301 0a01 7a23 5465  ............z#Te
-00001ae0: 7374 436f 6d70 616e 7943 616c 6c42 6163  stCompanyCallBac
-00001af0: 6b56 6965 772e 7465 7374 5f64 656c 6574  kView.test_delet
-00001b00: 654e 2909 7238 0000 0072 3900 0000 723a  eN).r8...r9...r:
-00001b10: 0000 0072 0900 0000 722b 0000 0072 1900  ...r....r+...r..
-00001b20: 0000 7246 0000 0072 4d00 0000 724f 0000  ..rF...rM...rO..
-00001b30: 0072 1300 0000 7213 0000 0072 1300 0000  .r....r....r....
-00001b40: 7214 0000 0072 5900 0000 af00 0000 730a  r....rY.......s.
-00001b50: 0000 000c 0106 020c 030c 050c 0b72 5900  .............rY.
-00001b60: 0000 2916 721f 0000 0072 6100 0000 da00  ..).r....ra.....
-00001b70: 7203 0000 0072 0400 0000 7205 0000 00da  r....r....r.....
-00001b80: 0b64 6a61 6e67 6f2e 7572 6c73 7206 0000  .django.urlsr...
-00001b90: 00da 0b64 6a61 6e67 6f2e 7465 7374 7207  ...django.testr.
-00001ba0: 0000 0072 0800 0000 5a14 646a 636f 6e6e  ...r....Z.djconn
-00001bb0: 6563 7477 6973 652e 6d6f 6465 6c73 7209  ectwise.modelsr.
-00001bc0: 0000 0072 0a00 0000 720b 0000 00da 0d64  ...r....r......d
-00001bd0: 6a63 6f6e 6e65 6374 7769 7365 720c 0000  jconnectwiser...
-00001be0: 0072 0d00 0000 720e 0000 0072 3b00 0000  .r....r....r;...
-00001bf0: 7250 0000 0072 5900 0000 7213 0000 0072  rP...rY...r....r
-00001c00: 1300 0000 7213 0000 0072 1400 0000 da08  ....r....r......
-00001c10: 3c6d 6f64 756c 653e 0100 0000 7314 0000  <module>....s...
-00001c20: 000c 010c 011c 0210 0116 021c 0116 0316  ................
-00001c30: 4b16 3116 27                             K.1.'
+00000020: 0073 a800 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
+00000030: 6401 6c01 5a01 6402 6403 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
+00000040: 6d04 5a04 6d05 5a05 0100 6400 6404 6c06  m.Z.m.Z...d.d.l.
+00000050: 6d07 5a07 0100 6400 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
+00000060: 6d0a 5a0a 0100 6400 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
+00000070: 6d0d 5a0d 6d0e 5a0e 0100 6400 6407 6c0f  m.Z.m.Z...d.d.l.
+00000080: 6d10 5a10 6d11 5a11 0100 4700 6408 6409  m.Z.m.Z...G.d.d.
+00000090: 8400 6409 650a 8303 5a12 4700 640a 640b  ..d.e...Z.G.d.d.
+000000a0: 8400 640b 6512 8303 5a13 4700 640c 640d  ..d.e...Z.G.d.d.
+000000b0: 8400 640d 6512 8303 5a14 4700 640e 640f  ..d.e...Z.G.d.d.
+000000c0: 8400 640f 6512 8303 5a15 6401 5300 2910  ..d.e...Z.d.S.).
+000000d0: e900 0000 004e e901 0000 0029 03da 0866  .....N.....)...f
+000000e0: 6978 7475 7265 73da 0d66 6978 7475 7265  ixtures..fixture
+000000f0: 5f75 7469 6c73 da05 6d6f 636b 7329 01da  _utils..mocks)..
+00000100: 0772 6576 6572 7365 2902 da06 436c 6965  .reverse)...Clie
+00000110: 6e74 da08 5465 7374 4361 7365 2903 da07  nt..TestCase)...
+00000120: 436f 6d70 616e 79da 0654 6963 6b65 74da  Company..Ticket.
+00000130: 0750 726f 6a65 6374 2902 da05 7669 6577  .Project)...view
+00000140: 73da 0361 7069 6300 0000 0000 0000 0000  s..apic.........
+00000150: 0000 0003 0000 0040 0000 0073 4400 0000  .......@...sD...
+00000160: 6500 5a01 6400 5a02 6401 5a03 6402 6403  e.Z.d.Z.d.Z.d.d.
+00000170: 8400 5a04 6404 6405 8400 5a05 640f 6406  ..Z.d.d...Z.d.d.
+00000180: 6407 8401 5a06 6408 6409 8400 5a07 640a  d...Z.d.d...Z.d.
+00000190: 640b 8400 5a08 6410 640d 640e 8401 5a09  d...Z.d.d.d...Z.
+000001a0: 6401 5300 2911 da14 4261 7365 5465 7374  d.S.)...BaseTest
+000001b0: 4361 6c6c 4261 636b 5669 6577 4e63 0100  CallBackViewNc..
+000001c0: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+000001d0: 0000 731c 0000 0074 006a 0183 0001 0074  ..s....t.j.....t
+000001e0: 006a 0283 0001 0074 006a 0383 0001 0064  .j.....t.j.....d
+000001f0: 0053 0029 014e 2904 7204 0000 00da 0b69  .S.).N).r......i
+00000200: 6e69 745f 626f 6172 6473 da13 696e 6974  nit_boards..init
+00000210: 5f62 6f61 7264 5f73 7461 7475 7365 73da  _board_statuses.
+00000220: 0c69 6e69 745f 6d65 6d62 6572 7329 01da  .init_members)..
+00000230: 0473 656c 66a9 0072 1300 0000 fa51 2f68  .self..r.....Q/h
+00000240: 6f6d 652f 6361 6d65 726f 6e2f 4465 762f  ome/cameron/Dev/
+00000250: 6b61 6e62 616e 2d64 6576 2f64 6a61 6e67  kanban-dev/djang
+00000260: 6f2d 636f 6e6e 6563 7477 6973 652f 646a  o-connectwise/dj
+00000270: 636f 6e6e 6563 7477 6973 652f 7465 7374  connectwise/test
+00000280: 732f 7465 7374 5f76 6965 7773 2e70 79da  s/test_views.py.
+00000290: 0573 6574 5570 0f00 0000 7306 0000 0000  .setUp....s.....
+000002a0: 0108 0108 017a 1a42 6173 6554 6573 7443  .....z.BaseTestC
+000002b0: 616c 6c42 6163 6b56 6965 772e 7365 7455  allBackView.setU
+000002c0: 7063 0300 0000 0000 0000 0300 0000 0100  pc..............
+000002d0: 0000 4300 0000 7308 0000 0074 0082 0164  ..C...s....t...d
+000002e0: 0053 0029 014e 2901 da13 4e6f 7449 6d70  .S.).N)...NotImp
+000002f0: 6c65 6d65 6e74 6564 4572 726f 7229 0372  lementedError).r
+00000300: 1200 0000 da08 696e 7374 616e 6365 da06  ......instance..
+00000310: 656e 7469 7479 7213 0000 0072 1300 0000  entityr....r....
+00000320: 7214 0000 00da 0d61 7373 6572 745f 6669  r......assert_fi
+00000330: 656c 6473 1400 0000 7302 0000 0000 017a  elds....s......z
+00000340: 2242 6173 6554 6573 7443 616c 6c42 6163  "BaseTestCallBac
+00000350: 6b56 6965 772e 6173 7365 7274 5f66 6965  kView.assert_fie
+00000360: 6c64 7363 0500 0000 0000 0000 0800 0000  ldsc............
+00000370: 0500 0000 4300 0000 7340 0000 0074 0083  ....C...s@...t..
+00000380: 007d 057c 017c 027c 037c 0472 1a74 016a  .}.|.|.|.|.r.t.j
+00000390: 027c 0483 016e 0264 0064 019c 047d 0674  .|...n.d.d...}.t
+000003a0: 016a 027c 0683 017d 077c 056a 0374 0464  .j.|...}.|.j.t.d
+000003b0: 0283 017c 0764 0364 048d 0353 0029 054e  ...|.d.d...S.).N
+000003c0: 2904 da04 5479 7065 da06 4163 7469 6f6e  )...Type..Action
+000003d0: da02 4944 da06 456e 7469 7479 7a16 646a  ..ID..Entityz.dj
+000003e0: 636f 6e6e 6563 7477 6973 653a 6361 6c6c  connectwise:call
+000003f0: 6261 636b 7a10 6170 706c 6963 6174 696f  backz.applicatio
+00000400: 6e2f 6a73 6f6e 2901 da0c 636f 6e74 656e  n/json)...conten
+00000410: 745f 7479 7065 2905 7207 0000 00da 046a  t_type).r......j
+00000420: 736f 6eda 0564 756d 7073 da04 706f 7374  son..dumps..post
+00000430: 7206 0000 0029 0872 1200 0000 da0d 6361  r....).r......ca
+00000440: 6c6c 6261 636b 5f74 7970 65da 0661 6374  llback_type..act
+00000450: 696f 6eda 0965 6e74 6974 795f 6964 7218  ion..entity_idr.
+00000460: 0000 00da 0663 6c69 656e 74da 0462 6f64  .....client..bod
+00000470: 795a 0962 6f64 795f 6a73 6f6e 7213 0000  yZ.body_jsonr...
+00000480: 0072 1300 0000 7214 0000 00da 0970 6f73  .r....r......pos
+00000490: 745f 6461 7461 1700 0000 7314 0000 0000  t_data....s.....
+000004a0: 0106 0202 0102 0102 0116 020a 0204 0106  ................
+000004b0: 0102 017a 1e42 6173 6554 6573 7443 616c  ...z.BaseTestCal
+000004c0: 6c42 6163 6b56 6965 772e 706f 7374 5f64  lBackView.post_d
+000004d0: 6174 6163 0300 0000 0000 0000 0600 0000  atac............
+000004e0: 0500 0000 4300 0000 736e 0000 007c 006a  ....C...sn...|.j
+000004f0: 007c 0174 016a 027c 0264 0119 007c 0283  .|.t.j.|.d...|..
+00000500: 047d 0374 037c 006a 046a 056a 0683 0083  .}.t.|.j.j.j....
+00000510: 017d 047c 0464 0219 007d 057c 006a 077c  .}.|.d...}.|.j.|
+00000520: 057c 0283 0201 007c 006a 087c 056a 097c  .|.....|.j.|.j.|
+00000530: 0264 0119 0083 0201 007c 006a 0874 0a7c  .d.......|.j.t.|
+00000540: 0483 0164 0383 0201 007c 006a 087c 036a  ...d.....|.j.|.j
+00000550: 0b64 0483 0201 0064 0053 0029 054e da02  .d.....d.S.).N..
+00000560: 6964 7201 0000 0072 0200 0000 e9cc 0000  idr....r........
+00000570: 0029 0c72 2700 0000 720c 0000 005a 0e43  .).r'...r....Z.C
+00000580: 414c 4c42 4143 4b5f 4144 4445 44da 046c  ALLBACK_ADDED..l
+00000590: 6973 74da 0b4d 4f44 454c 5f43 4c41 5353  ist..MODEL_CLASS
+000005a0: da07 6f62 6a65 6374 73da 0361 6c6c 7219  ..objects..allr.
+000005b0: 0000 00da 0b61 7373 6572 7445 7175 616c  .....assertEqual
+000005c0: 7228 0000 00da 036c 656e da0b 7374 6174  r(.....len..stat
+000005d0: 7573 5f63 6f64 6529 0672 1200 0000 7222  us_code).r....r"
+000005e0: 0000 0072 1800 0000 da08 7265 7370 6f6e  ...r......respon
+000005f0: 7365 da09 696e 7374 616e 6365 7372 1700  se..instancesr..
+00000600: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00000610: 00da 0b5f 7465 7374 5f61 6464 6564 2700  ..._test_added'.
+00000620: 0000 7316 0000 0000 0104 0102 0104 0106  ..s.............
+00000630: 0106 0310 0108 020c 0112 0110 017a 2042  .............z B
+00000640: 6173 6554 6573 7443 616c 6c42 6163 6b56  aseTestCallBackV
+00000650: 6965 772e 5f74 6573 745f 6164 6465 6463  iew._test_addedc
+00000660: 0300 0000 0000 0000 0600 0000 0500 0000  ................
+00000670: 4300 0000 736e 0000 007c 006a 007c 0174  C...sn...|.j.|.t
+00000680: 016a 027c 0264 0119 007c 0283 047d 0374  .j.|.d...|...}.t
+00000690: 037c 006a 046a 056a 0683 0083 017d 047c  .|.j.j.j.....}.|
+000006a0: 0464 0219 007d 057c 006a 077c 057c 0283  .d...}.|.j.|.|..
+000006b0: 0201 007c 006a 087c 056a 097c 0264 0119  ...|.j.|.j.|.d..
+000006c0: 0083 0201 007c 006a 0874 0a7c 0483 0164  .....|.j.t.|...d
+000006d0: 0383 0201 007c 006a 087c 036a 0b64 0483  .....|.j.|.j.d..
+000006e0: 0201 0064 0053 0029 054e 7228 0000 0072  ...d.S.).Nr(...r
+000006f0: 0100 0000 7202 0000 0072 2900 0000 290c  ....r....r)...).
+00000700: 7227 0000 0072 0c00 0000 5a10 4341 4c4c  r'...r....Z.CALL
+00000710: 4241 434b 5f55 5044 4154 4544 722a 0000  BACK_UPDATEDr*..
+00000720: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
+00000730: 7219 0000 0072 2e00 0000 7228 0000 0072  r....r....r(...r
+00000740: 2f00 0000 7230 0000 0029 0672 1200 0000  /...r0...).r....
+00000750: 7222 0000 0072 1800 0000 7231 0000 0072  r"...r....r1...r
+00000760: 3200 0000 7217 0000 0072 1300 0000 7213  2...r....r....r.
+00000770: 0000 0072 1400 0000 da0c 5f74 6573 745f  ...r......_test_
+00000780: 7570 6461 7465 3700 0000 7316 0000 0000  update7...s.....
+00000790: 0104 0102 0104 0106 0106 0310 0108 020c  ................
+000007a0: 0112 0110 017a 2142 6173 6554 6573 7443  .....z!BaseTestC
+000007b0: 616c 6c42 6163 6b56 6965 772e 5f74 6573  allBackView._tes
+000007c0: 745f 7570 6461 7465 722c 0000 0063 0400  t_updater,...c..
+000007d0: 0000 0000 0000 0700 0000 0400 0000 4300  ..............C.
+000007e0: 0000 734a 0000 007c 006a 007c 0174 016a  ..sJ...|.j.|.t.j
+000007f0: 027c 0283 037d 0474 037c 006a 047c 0383  .|...}.t.|.j.|..
+00000800: 027d 0574 057c 056a 0683 0083 017d 067c  .}.t.|.j.....}.|
+00000810: 006a 077c 046a 0864 0183 0201 007c 006a  .j.|.j.d.....|.j
+00000820: 0774 097c 0683 0164 0283 0201 0064 0053  .t.|...d.....d.S
+00000830: 0029 034e 7229 0000 0072 0100 0000 290a  .).Nr)...r....).
+00000840: 7227 0000 0072 0c00 0000 5a10 4341 4c4c  r'...r....Z.CALL
+00000850: 4241 434b 5f44 454c 4554 4544 da07 6765  BACK_DELETED..ge
+00000860: 7461 7474 7272 2b00 0000 722a 0000 0072  tattrr+...r*...r
+00000870: 2d00 0000 722e 0000 0072 3000 0000 722f  -...r....r0...r/
+00000880: 0000 0029 0772 1200 0000 7222 0000 0072  ...).r....r"...r
+00000890: 2400 0000 da07 6d61 6e61 6765 7272 3100  $.....managerr1.
+000008a0: 0000 5a0d 6d6f 6465 6c5f 6d61 6e61 6765  ..Z.model_manage
+000008b0: 7272 3200 0000 7213 0000 0072 1300 0000  rr2...r....r....
+000008c0: 7214 0000 00da 0c5f 7465 7374 5f64 656c  r......_test_del
+000008d0: 6574 6547 0000 0073 1000 0000 0001 0401  eteG...s........
+000008e0: 0201 0401 0606 0c01 0c01 0e01 7a21 4261  ............z!Ba
+000008f0: 7365 5465 7374 4361 6c6c 4261 636b 5669  seTestCallBackVi
+00000900: 6577 2e5f 7465 7374 5f64 656c 6574 6529  ew._test_delete)
+00000910: 014e 2901 722c 0000 0029 0ada 085f 5f6e  .N).r,...)...__n
+00000920: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000930: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+00000940: 2b00 0000 7215 0000 0072 1900 0000 7227  +...r....r....r'
+00000950: 0000 0072 3300 0000 7234 0000 0072 3700  ...r3...r4...r7.
+00000960: 0000 7213 0000 0072 1300 0000 7213 0000  ..r....r....r...
+00000970: 0072 1400 0000 720e 0000 000c 0000 0073  .r....r........s
+00000980: 0e00 0000 0801 0402 0805 0803 0a10 0810  ................
+00000990: 0810 720e 0000 0063 0000 0000 0000 0000  ..r....c........
+000009a0: 0000 0000 0200 0000 4000 0000 7330 0000  ........@...s0..
+000009b0: 0065 005a 0164 005a 0265 035a 0464 0164  .e.Z.d.Z.e.Z.d.d
+000009c0: 0284 005a 0564 0364 0484 005a 0664 0564  ...Z.d.d...Z.d.d
+000009d0: 0684 005a 0764 0764 0884 005a 0864 0953  ...Z.d.d...Z.d.S
+000009e0: 0029 0ada 1654 6573 7454 6963 6b65 7443  .)...TestTicketC
+000009f0: 616c 6c42 6163 6b56 6965 7763 0300 0000  allBackViewc....
+00000a00: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
+00000a10: 7316 0000 007c 006a 007c 016a 017c 0264  s....|.j.|.j.|.d
+00000a20: 0119 0083 0201 0064 0053 0029 024e da07  .......d.S.).N..
+00000a30: 7375 6d6d 6172 7929 0272 2e00 0000 723c  summary).r....r<
+00000a40: 0000 0029 0372 1200 0000 7217 0000 0072  ...).r....r....r
+00000a50: 1800 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
+00000a60: 0000 0072 1900 0000 5a00 0000 7302 0000  ...r....Z...s...
+00000a70: 0000 017a 2454 6573 7454 6963 6b65 7443  ...z$TestTicketC
+00000a80: 616c 6c42 6163 6b56 6965 772e 6173 7365  allBackView.asse
+00000a90: 7274 5f66 6965 6c64 7363 0100 0000 0000  rt_fieldsc......
+00000aa0: 0000 0100 0000 0300 0000 4300 0000 735c  ..........C...s\
+00000ab0: 0000 0074 006a 0183 0001 0074 006a 0283  ...t.j.....t.j..
+00000ac0: 0001 0074 006a 0383 0001 0074 006a 0483  ...t.j.....t.j..
+00000ad0: 0001 0074 006a 0583 0001 0074 006a 0683  ...t.j.....t.j..
+00000ae0: 0001 007c 006a 0774 086a 096a 0a83 0064  ...|.j.t.j.j...d
+00000af0: 0183 0201 0074 0b6a 0c83 0001 007c 006a  .....t.j.....|.j
+00000b00: 0d64 0274 0e6a 0f83 0201 0064 0053 0029  .d.t.j.....d.S.)
+00000b10: 034e 7201 0000 00da 0674 6963 6b65 7429  .Nr......ticket)
+00000b20: 1072 0400 0000 da0f 696e 6974 5f70 7269  .r......init_pri
+00000b30: 6f72 6974 6965 73da 0d69 6e69 745f 7072  orities..init_pr
+00000b40: 6f6a 6563 7473 da0e 696e 6974 5f63 6f6d  ojects..init_com
+00000b50: 7061 6e69 6573 7210 0000 00da 0e69 6e69  paniesr......ini
+00000b60: 745f 6c6f 6361 7469 6f6e 73da 0a69 6e69  t_locations..ini
+00000b70: 745f 7465 616d 7372 2e00 0000 720a 0000  t_teamsr....r...
+00000b80: 0072 2c00 0000 da05 636f 756e 7472 0500  .r,.....countr..
+00000b90: 0000 da1b 7365 7276 6963 655f 6170 695f  ....service_api_
+00000ba0: 6765 745f 7469 636b 6574 5f63 616c 6c72  get_ticket_callr
+00000bb0: 3300 0000 7203 0000 00da 1241 5049 5f53  3...r......API_S
+00000bc0: 4552 5649 4345 5f54 4943 4b45 5429 0172  ERVICE_TICKET).r
+00000bd0: 1200 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
+00000be0: 0000 00da 0874 6573 745f 6164 645d 0000  .....test_add]..
+00000bf0: 0073 1200 0000 0001 0801 0801 0801 0801  .s..............
+00000c00: 0801 0801 1201 0801 7a1f 5465 7374 5469  ........z.TestTi
+00000c10: 636b 6574 4361 6c6c 4261 636b 5669 6577  cketCallBackView
+00000c20: 2e74 6573 745f 6164 6463 0100 0000 0000  .test_addc......
+00000c30: 0000 0200 0000 0300 0000 4300 0000 7380  ..........C...s.
+00000c40: 0000 0074 006a 0183 0001 0074 006a 0283  ...t.j.....t.j..
+00000c50: 0001 0074 006a 0383 0001 0074 006a 0483  ...t.j.....t.j..
+00000c60: 0001 0074 006a 0583 0001 0074 006a 0683  ...t.j.....t.j..
+00000c70: 0001 0074 006a 0783 0001 007c 006a 0874  ...t.j.....|.j.t
+00000c80: 096a 0a6a 0b83 0064 0183 0201 0074 096a  .j.j...d.....t.j
+00000c90: 0a6a 0c64 0264 038d 017d 0164 047c 015f  .j.d.d...}.d.|._
+00000ca0: 0d7c 016a 0e83 0001 0074 0f6a 1083 0001  .|.j.....t.j....
+00000cb0: 007c 006a 1164 0574 126a 1383 0201 0064  .|.j.d.t.j.....d
+00000cc0: 0053 0029 064e 7202 0000 00e9 4500 0000  .S.).Nr.....E...
+00000cd0: 2901 7228 0000 00da 0666 6f6f 6261 7272  ).r(.....foobarr
+00000ce0: 3d00 0000 2914 7204 0000 0072 3e00 0000  =...).r....r>...
+00000cf0: 723f 0000 0072 4000 0000 7210 0000 0072  r?...r@...r....r
+00000d00: 4100 0000 7242 0000 00da 0c69 6e69 745f  A...rB.....init_
+00000d10: 7469 636b 6574 7372 2e00 0000 720a 0000  ticketsr....r...
+00000d20: 0072 2c00 0000 7243 0000 00da 0367 6574  .r,...rC.....get
+00000d30: 723c 0000 00da 0473 6176 6572 0500 0000  r<.....saver....
+00000d40: 7244 0000 0072 3400 0000 7203 0000 0072  rD...r4...r....r
+00000d50: 4500 0000 2902 7212 0000 00da 0174 7213  E...).r......tr.
+00000d60: 0000 0072 1300 0000 7214 0000 00da 0b74  ...r....r......t
+00000d70: 6573 745f 7570 6461 7465 6800 0000 731a  est_updateh...s.
+00000d80: 0000 0000 0108 0108 0108 0108 0108 0108  ................
+00000d90: 0108 0112 020e 0106 0108 0208 017a 2254  .............z"T
+00000da0: 6573 7454 6963 6b65 7443 616c 6c42 6163  estTicketCallBac
+00000db0: 6b56 6965 772e 7465 7374 5f75 7064 6174  kView.test_updat
+00000dc0: 6563 0100 0000 0000 0000 0100 0000 0400  ec..............
+00000dd0: 0000 4300 0000 735c 0000 0074 006a 0183  ..C...s\...t.j..
+00000de0: 0001 0074 006a 0283 0001 0074 006a 0383  ...t.j.....t.j..
+00000df0: 0001 0074 006a 0483 0001 0074 006a 0583  ...t.j.....t.j..
+00000e00: 0001 007c 006a 0674 076a 086a 0983 0064  ...|.j.t.j.j...d
+00000e10: 0183 0201 0074 0a6a 0b74 0c6a 0d83 0101  .....t.j.t.j....
+00000e20: 007c 006a 0e64 0274 0f6a 1064 0319 0083  .|.j.d.t.j.d....
+00000e30: 0201 0064 0053 0029 044e 7202 0000 0072  ...d.S.).Nr....r
+00000e40: 3d00 0000 7228 0000 0029 1172 0400 0000  =...r(...).r....
+00000e50: 7249 0000 0072 3e00 0000 7240 0000 0072  rI...r>...r@...r
+00000e60: 4100 0000 7242 0000 0072 2e00 0000 720a  A...rB...r....r.
+00000e70: 0000 0072 2c00 0000 7243 0000 0072 0500  ...r,...rC...r..
+00000e80: 0000 7244 0000 0072 0d00 0000 da1e 436f  ..rD...r......Co
+00000e90: 6e6e 6563 7457 6973 6552 6563 6f72 644e  nnectWiseRecordN
+00000ea0: 6f74 466f 756e 6445 7272 6f72 7237 0000  otFoundErrorr7..
+00000eb0: 0072 0300 0000 7245 0000 0029 0172 1200  .r....rE...).r..
+00000ec0: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00000ed0: 00da 0b74 6573 745f 6465 6c65 7465 7900  ...test_deletey.
+00000ee0: 0000 7314 0000 0000 0108 0108 0108 0108  ..s.............
+00000ef0: 0108 0112 020c 0104 0102 017a 2254 6573  ...........z"Tes
+00000f00: 7454 6963 6b65 7443 616c 6c42 6163 6b56  tTicketCallBackV
+00000f10: 6965 772e 7465 7374 5f64 656c 6574 654e  iew.test_deleteN
+00000f20: 2909 7238 0000 0072 3900 0000 723a 0000  ).r8...r9...r:..
+00000f30: 0072 0a00 0000 722b 0000 0072 1900 0000  .r....r+...r....
+00000f40: 7246 0000 0072 4d00 0000 724f 0000 0072  rF...rM...rO...r
+00000f50: 1300 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
+00000f60: 0000 0072 3b00 0000 5700 0000 730a 0000  ...r;...W...s...
+00000f70: 0008 0104 0208 0308 0b08 1172 3b00 0000  ...........r;...
+00000f80: 6300 0000 0000 0000 0000 0000 0002 0000  c...............
+00000f90: 0040 0000 0073 3000 0000 6500 5a01 6400  .@...s0...e.Z.d.
+00000fa0: 5a02 6503 5a04 6401 6402 8400 5a05 6403  Z.e.Z.d.d...Z.d.
+00000fb0: 6404 8400 5a06 6405 6406 8400 5a07 6407  d...Z.d.d...Z.d.
+00000fc0: 6408 8400 5a08 6409 5300 290a da17 5465  d...Z.d.S.)...Te
+00000fd0: 7374 5072 6f6a 6563 7443 616c 6c42 6163  stProjectCallBac
+00000fe0: 6b56 6965 7763 0300 0000 0000 0000 0300  kViewc..........
+00000ff0: 0000 0400 0000 4300 0000 7316 0000 007c  ......C...s....|
+00001000: 006a 007c 016a 017c 0264 0119 0083 0201  .j.|.j.|.d......
+00001010: 0064 0053 0029 024e da04 6e61 6d65 2902  .d.S.).N..name).
+00001020: 722e 0000 0072 5100 0000 2903 7212 0000  r....rQ...).r...
+00001030: 0072 1700 0000 7218 0000 0072 1300 0000  .r....r....r....
+00001040: 7213 0000 0072 1400 0000 7219 0000 008b  r....r....r.....
+00001050: 0000 0073 0200 0000 0001 7a25 5465 7374  ...s......z%Test
+00001060: 5072 6f6a 6563 7443 616c 6c42 6163 6b56  ProjectCallBackV
+00001070: 6965 772e 6173 7365 7274 5f66 6965 6c64  iew.assert_field
+00001080: 7363 0100 0000 0000 0000 0100 0000 0300  sc..............
+00001090: 0000 4300 0000 7338 0000 0074 006a 0183  ..C...s8...t.j..
+000010a0: 0001 007c 006a 0274 036a 046a 0583 0064  ...|.j.t.j.j...d
+000010b0: 0183 0201 0074 066a 0774 086a 0983 0101  .....t.j.t.j....
+000010c0: 007c 006a 0a64 0274 086a 0983 0201 0064  .|.j.d.t.j.....d
+000010d0: 0053 0029 034e 7201 0000 00da 0770 726f  .S.).Nr......pro
+000010e0: 6a65 6374 290b 7204 0000 00da 1569 6e69  ject).r......ini
+000010f0: 745f 7072 6f6a 6563 745f 7374 6174 7573  t_project_status
+00001100: 6573 722e 0000 0072 0b00 0000 722c 0000  esr....r....r,..
+00001110: 0072 4300 0000 7205 0000 00da 1c70 726f  .rC...r......pro
+00001120: 6a65 6374 5f61 7069 5f67 6574 5f70 726f  ject_api_get_pro
+00001130: 6a65 6374 5f63 616c 6c72 0300 0000 da0b  ject_callr......
+00001140: 4150 495f 5052 4f4a 4543 5472 3300 0000  API_PROJECTr3...
+00001150: 2901 7212 0000 0072 1300 0000 7213 0000  ).r....r....r...
+00001160: 0072 1400 0000 7246 0000 008e 0000 0073  .r....rF.......s
+00001170: 0800 0000 0001 0801 1201 0c01 7a20 5465  ............z Te
+00001180: 7374 5072 6f6a 6563 7443 616c 6c42 6163  stProjectCallBac
+00001190: 6b56 6965 772e 7465 7374 5f61 6464 6301  kView.test_addc.
+000011a0: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+000011b0: 0000 0073 5c00 0000 7400 6a01 8300 0100  ...s\...t.j.....
+000011c0: 7400 6a02 8300 0100 7c00 6a03 7404 6a05  t.j.....|.j.t.j.
+000011d0: 6a06 8300 6401 8302 0100 7404 6a05 6a07  j...d.....t.j.j.
+000011e0: 6402 6403 8d01 7d01 6404 7c01 5f08 7c01  d.d...}.d.|._.|.
+000011f0: 6a09 8300 0100 740a 6a0b 740c 6a0d 8301  j.....t.j.t.j...
+00001200: 0100 7c00 6a0e 6405 740c 6a0d 8302 0100  ..|.j.d.t.j.....
+00001210: 6400 5300 2906 4e72 0200 0000 e905 0000  d.S.).Nr........
+00001220: 0029 0172 2800 0000 7248 0000 0072 5200  .).r(...rH...rR.
+00001230: 0000 290f 7204 0000 0072 5300 0000 723f  ..).r....rS...r?
+00001240: 0000 0072 2e00 0000 720b 0000 0072 2c00  ...r....r....r,.
+00001250: 0000 7243 0000 0072 4a00 0000 7251 0000  ..rC...rJ...rQ..
+00001260: 0072 4b00 0000 7205 0000 0072 5400 0000  .rK...r....rT...
+00001270: 7203 0000 0072 5500 0000 7234 0000 0029  r....rU...r4...)
+00001280: 0272 1200 0000 da01 7072 1300 0000 7213  .r......pr....r.
+00001290: 0000 0072 1400 0000 724d 0000 0094 0000  ...r....rM......
+000012a0: 0073 1000 0000 0001 0801 0801 1202 0e01  .s..............
+000012b0: 0601 0802 0c01 7a23 5465 7374 5072 6f6a  ......z#TestProj
+000012c0: 6563 7443 616c 6c42 6163 6b56 6965 772e  ectCallBackView.
+000012d0: 7465 7374 5f75 7064 6174 6563 0100 0000  test_updatec....
+000012e0: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
+000012f0: 7348 0000 0074 006a 0183 0001 0074 006a  sH...t.j.....t.j
+00001300: 0283 0001 007c 006a 0374 046a 056a 0683  .....|.j.t.j.j..
+00001310: 0064 0183 0201 0074 076a 0864 0074 096a  .d.....t.j.d.t.j
+00001320: 0a64 028d 0201 007c 006a 0b64 0374 0c6a  .d.....|.j.d.t.j
+00001330: 0d64 0419 0083 0201 0064 0053 0029 054e  .d.......d.S.).N
+00001340: 7202 0000 0029 01da 0672 6169 7365 6472  r....)...raisedr
+00001350: 5200 0000 7228 0000 0029 0e72 0400 0000  R...r(...).r....
+00001360: 7253 0000 0072 3f00 0000 722e 0000 0072  rS...r?...r....r
+00001370: 0b00 0000 722c 0000 0072 4300 0000 7205  ....r,...rC...r.
+00001380: 0000 0072 5400 0000 720d 0000 0072 4e00  ...rT...r....rN.
+00001390: 0000 7237 0000 0072 0300 0000 7255 0000  ..r7...r....rU..
+000013a0: 0029 0172 1200 0000 7213 0000 0072 1300  .).r....r....r..
+000013b0: 0000 7214 0000 0072 4f00 0000 a000 0000  ..r....rO.......
+000013c0: 7312 0000 0000 0108 0108 0112 0204 0102  s...............
+000013d0: 010a 0204 0102 017a 2354 6573 7450 726f  .......z#TestPro
+000013e0: 6a65 6374 4361 6c6c 4261 636b 5669 6577  jectCallBackView
+000013f0: 2e74 6573 745f 6465 6c65 7465 4e29 0972  .test_deleteN).r
+00001400: 3800 0000 7239 0000 0072 3a00 0000 720b  8...r9...r:...r.
+00001410: 0000 0072 2b00 0000 7219 0000 0072 4600  ...r+...r....rF.
+00001420: 0000 724d 0000 0072 4f00 0000 7213 0000  ..rM...rO...r...
+00001430: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
+00001440: 7250 0000 0088 0000 0073 0a00 0000 0801  rP.......s......
+00001450: 0402 0803 0806 080c 7250 0000 0063 0000  ........rP...c..
+00001460: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00001470: 0000 7330 0000 0065 005a 0164 005a 0265  ..s0...e.Z.d.Z.e
+00001480: 035a 0464 0164 0284 005a 0564 0364 0484  .Z.d.d...Z.d.d..
+00001490: 005a 0664 0564 0684 005a 0764 0764 0884  .Z.d.d...Z.d.d..
+000014a0: 005a 0864 0953 0029 0ada 1754 6573 7443  .Z.d.S.)...TestC
+000014b0: 6f6d 7061 6e79 4361 6c6c 4261 636b 5669  ompanyCallBackVi
+000014c0: 6577 6303 0000 0000 0000 0003 0000 0004  ewc.............
+000014d0: 0000 0043 0000 0073 1600 0000 7c00 6a00  ...C...s....|.j.
+000014e0: 7c01 6a01 7c02 6401 1900 8302 0100 6400  |.j.|.d.......d.
+000014f0: 5300 2902 4e72 5100 0000 2902 722e 0000  S.).NrQ...).r...
+00001500: 0072 5100 0000 2903 7212 0000 0072 1700  .rQ...).r....r..
+00001510: 0000 7218 0000 0072 1300 0000 7213 0000  ..r....r....r...
+00001520: 0072 1400 0000 7219 0000 00b2 0000 0073  .r....r........s
+00001530: 0200 0000 0001 7a25 5465 7374 436f 6d70  ......z%TestComp
+00001540: 616e 7943 616c 6c42 6163 6b56 6965 772e  anyCallBackView.
+00001550: 6173 7365 7274 5f66 6965 6c64 7363 0100  assert_fieldsc..
+00001560: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00001570: 0000 7330 0000 007c 006a 0074 016a 026a  ..s0...|.j.t.j.j
+00001580: 0383 0064 0183 0201 0074 046a 0574 066a  ...d.....t.j.t.j
+00001590: 0783 0101 007c 006a 0864 0274 066a 0783  .....|.j.d.t.j..
+000015a0: 0201 0064 0053 0029 034e 7201 0000 00da  ...d.S.).Nr.....
+000015b0: 0763 6f6d 7061 6e79 2909 722e 0000 0072  .company).r....r
+000015c0: 0900 0000 722c 0000 0072 4300 0000 7205  ....r,...rC...r.
+000015d0: 0000 00da 1663 6f6d 7061 6e79 5f61 7069  .....company_api
+000015e0: 5f62 795f 6964 5f63 616c 6c72 0300 0000  _by_id_callr....
+000015f0: da0b 4150 495f 434f 4d50 414e 5972 3300  ..API_COMPANYr3.
+00001600: 0000 2901 7212 0000 0072 1300 0000 7213  ..).r....r....r.
+00001610: 0000 0072 1400 0000 7246 0000 00b5 0000  ...r....rF......
+00001620: 0073 0600 0000 0001 1201 0c01 7a20 5465  .s..........z Te
+00001630: 7374 436f 6d70 616e 7943 616c 6c42 6163  stCompanyCallBac
+00001640: 6b56 6965 772e 7465 7374 5f61 6464 6301  kView.test_addc.
+00001650: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00001660: 0000 0073 5400 0000 7400 6a01 8300 0100  ...sT...t.j.....
+00001670: 7c00 6a02 7403 6a04 6a05 8300 6401 8302  |.j.t.j.j...d...
+00001680: 0100 7403 6a04 6a06 6402 6403 8d01 7d01  ..t.j.j.d.d...}.
+00001690: 6404 7c01 5f07 7c01 6a08 8300 0100 7409  d.|._.|.j.....t.
+000016a0: 6a0a 740b 6a0c 8301 0100 7c00 6a0d 6405  j.t.j.....|.j.d.
+000016b0: 740b 6a0c 8302 0100 6400 5300 2906 4e72  t.j.....d.S.).Nr
+000016c0: 0200 0000 e902 0000 0029 0172 2800 0000  .........).r(...
+000016d0: 7248 0000 0072 5a00 0000 290e 7204 0000  rH...rZ...).r...
+000016e0: 0072 4000 0000 722e 0000 0072 0900 0000  .r@...r....r....
+000016f0: 722c 0000 0072 4300 0000 724a 0000 0072  r,...rC...rJ...r
+00001700: 5100 0000 724b 0000 0072 0500 0000 725b  Q...rK...r....r[
+00001710: 0000 0072 0300 0000 725c 0000 0072 3400  ...r....r\...r4.
+00001720: 0000 2902 7212 0000 00da 0163 7213 0000  ..).r......cr...
+00001730: 0072 1300 0000 7214 0000 0072 4d00 0000  .r....r....rM...
+00001740: ba00 0000 730e 0000 0000 0108 0112 020e  ....s...........
+00001750: 0106 0108 020c 017a 2354 6573 7443 6f6d  .......z#TestCom
+00001760: 7061 6e79 4361 6c6c 4261 636b 5669 6577  panyCallBackView
+00001770: 2e74 6573 745f 7570 6461 7465 6301 0000  .test_updatec...
+00001780: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
+00001790: 0073 5000 0000 7400 6a01 8300 0100 7c00  .sP...t.j.....|.
+000017a0: 6a02 7403 6a04 6a05 8300 6401 8302 0100  j.t.j.j...d.....
+000017b0: 7406 6a07 7408 6a09 8301 7d01 6402 7c01  t.j.t.j...}.d.|.
+000017c0: 6403 3c00 740a 6a0b 7c01 8301 0100 7c00  d.<.t.j.|.....|.
+000017d0: 6a0c 6404 7c01 6405 1900 6406 6407 8d03  j.d.|.d...d.d...
+000017e0: 0100 6400 5300 2908 4e72 0200 0000 54da  ..d.S.).Nr....T.
+000017f0: 0b64 656c 6574 6564 466c 6167 725a 0000  .deletedFlagrZ..
+00001800: 0072 2800 0000 da11 6176 6169 6c61 626c  .r(.....availabl
+00001810: 655f 6f62 6a65 6374 7329 0172 3600 0000  e_objects).r6...
+00001820: 290d 7204 0000 0072 4000 0000 722e 0000  ).r....r@...r...
+00001830: 0072 0900 0000 722c 0000 0072 4300 0000  .r....r,...rC...
+00001840: da04 636f 7079 da08 6465 6570 636f 7079  ..copy..deepcopy
+00001850: 7203 0000 0072 5c00 0000 7205 0000 0072  r....r\...r....r
+00001860: 5b00 0000 7237 0000 0029 0272 1200 0000  [...r7...).r....
+00001870: 5a0f 636f 6d70 616e 795f 6669 7874 7572  Z.company_fixtur
+00001880: 6572 1300 0000 7213 0000 0072 1400 0000  er....r....r....
+00001890: 724f 0000 00c5 0000 0073 1200 0000 0001  rO.......s......
+000018a0: 0801 1204 0c01 0801 0a01 0401 0201 0601  ................
+000018b0: 7a23 5465 7374 436f 6d70 616e 7943 616c  z#TestCompanyCal
+000018c0: 6c42 6163 6b56 6965 772e 7465 7374 5f64  lBackView.test_d
+000018d0: 656c 6574 654e 2909 7238 0000 0072 3900  eleteN).r8...r9.
+000018e0: 0000 723a 0000 0072 0900 0000 722b 0000  ..r:...r....r+..
+000018f0: 0072 1900 0000 7246 0000 0072 4d00 0000  .r....rF...rM...
+00001900: 724f 0000 0072 1300 0000 7213 0000 0072  rO...r....r....r
+00001910: 1300 0000 7214 0000 0072 5900 0000 af00  ....r....rY.....
+00001920: 0000 730a 0000 0008 0104 0208 0308 0508  ..s.............
+00001930: 0b72 5900 0000 2916 721f 0000 0072 6100  .rY...).r....ra.
+00001940: 0000 da00 7203 0000 0072 0400 0000 7205  ....r....r....r.
+00001950: 0000 00da 0b64 6a61 6e67 6f2e 7572 6c73  .....django.urls
+00001960: 7206 0000 00da 0b64 6a61 6e67 6f2e 7465  r......django.te
+00001970: 7374 7207 0000 0072 0800 0000 5a14 646a  str....r....Z.dj
+00001980: 636f 6e6e 6563 7477 6973 652e 6d6f 6465  connectwise.mode
+00001990: 6c73 7209 0000 0072 0a00 0000 720b 0000  lsr....r....r...
+000019a0: 00da 0d64 6a63 6f6e 6e65 6374 7769 7365  ...djconnectwise
+000019b0: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+000019c0: 3b00 0000 7250 0000 0072 5900 0000 7213  ;...rP...rY...r.
+000019d0: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+000019e0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000019f0: 7314 0000 0008 0108 0114 020c 0110 0214  s...............
+00001a00: 0110 0310 4b10 3110 27                   ....K.1.'
```

### Comparing `django-connectwise-0.3.98/djconnectwise/tests/test_utils.py` & `django-connectwise-0.3.99/djconnectwise/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/tests/test_commands.py` & `django-connectwise-0.3.99/djconnectwise/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/tests/mocks.py` & `django-connectwise-0.3.99/djconnectwise/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/tests/test_sync.py` & `django-connectwise-0.3.99/djconnectwise/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/tests/test_callback.py` & `django-connectwise-0.3.99/djconnectwise/tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/tests/mommy_recipes.py` & `django-connectwise-0.3.99/djconnectwise/tests/mommy_recipes.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/tests/fixture_utils.py` & `django-connectwise-0.3.99/djconnectwise/tests/fixture_utils.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/tests/test_views.py` & `django-connectwise-0.3.99/djconnectwise/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/tests/test_models.py` & `django-connectwise-0.3.99/djconnectwise/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/admin.py` & `django-connectwise-0.3.99/djconnectwise/admin.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/sync.py` & `django-connectwise-0.3.99/djconnectwise/sync.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/signals.py` & `django-connectwise-0.3.99/djconnectwise/signals.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/management/commands/list_users.py` & `django-connectwise-0.3.99/djconnectwise/management/commands/list_users.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/management/commands/__pycache__/list_users.cpython-35.pyc` & `django-connectwise-0.3.99/djconnectwise/management/commands/__pycache__/list_users.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,53 @@
-00000000: 160d 0d0a f859 f25e 2f02 0000 e300 0000  .....Y.^/.......
+00000000: 330d 0d0a 8740 f55e 2f02 0000 e300 0000  3....@.^/.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3a00 0000 6400 0064 0100 6c00 006d  .s:...d..d..l..m
-00000030: 0100 5a01 0001 6400 0064 0200 6c02 006d  ..Z...d..d..l..m
-00000040: 0300 5a03 0001 4764 0300 6404 0084 0000  ..Z...Gd..d.....
-00000050: 6404 0065 0100 8303 005a 0400 6405 0053  d..e.....Z..d..S
-00000060: 2906 e900 0000 0029 01da 0b42 6173 6543  )......)...BaseC
-00000070: 6f6d 6d61 6e64 2901 da06 4d65 6d62 6572  ommand)...Member
-00000080: 6300 0000 0000 0000 0000 0000 0002 0000  c...............
-00000090: 0040 0000 0073 2200 0000 6500 005a 0100  .@...s"...e..Z..
-000000a0: 6400 005a 0200 6401 005a 0300 6402 0064  d..Z..d..Z..d..d
-000000b0: 0300 8400 005a 0400 6404 0053 2905 da07  .....Z..d..S)...
-000000c0: 436f 6d6d 616e 647a 2e4c 6973 7420 6163  Commandz.List ac
-000000d0: 7469 7665 2c20 6675 6c6c 2d6c 6963 656e  tive, full-licen
-000000e0: 7365 2043 6f6e 6e65 6374 5769 7365 206d  se ConnectWise m
-000000f0: 656d 6265 7273 2e63 0100 0000 0000 0000  embers.c........
-00000100: 0400 0000 0600 0000 4f00 0000 7364 0000  ........O...sd..
-00000110: 0078 5d00 7400 006a 0100 6a02 0064 0100  .x].t..j..j..d..
-00000120: 6402 0064 0300 6404 0083 0002 445d 4000  d..d..d.....D]@.
-00000130: 7d03 007c 0000 6a03 006a 0400 6405 006a  }..|..j..j..d..j
-00000140: 0500 7c03 006a 0600 7c03 006a 0700 8300  ..|..j..|..j....
-00000150: 007c 0300 6a08 0072 5200 7c03 006a 0800  .|..j..rR.|..j..
-00000160: 6e03 0064 0600 8303 0083 0100 0171 1c00  n..d.........q..
-00000170: 5764 0000 5329 074e da08 696e 6163 7469  Wd..S).N..inacti
-00000180: 7665 46da 0d6c 6963 656e 7365 5f63 6c61  veF..license_cla
-00000190: 7373 da01 467a 117b 3a31 357d 207b 3a32  ss..Fz.{:15} {:2
-000001a0: 307d 207b 3a34 337d da00 2909 7203 0000  0} {:43}..).r...
-000001b0: 00da 076f 626a 6563 7473 da06 6669 6c74  ...objects..filt
-000001c0: 6572 da06 7374 646f 7574 da05 7772 6974  er..stdout..writ
-000001d0: 65da 0666 6f72 6d61 74da 0a69 6465 6e74  e..format..ident
-000001e0: 6966 6965 72da 075f 5f73 7472 5f5f da0c  ifier..__str__..
-000001f0: 6f66 6669 6365 5f65 6d61 696c 2904 da04  office_email)...
-00000200: 7365 6c66 da04 6172 6773 da07 6f70 7469  self..args..opti
-00000210: 6f6e 73da 066d 656d 6265 72a9 0072 1500  ons..member..r..
-00000220: 0000 fa6a 2f68 6f6d 652f 7361 6d2f 6769  ...j/home/sam/gi
-00000230: 742f 4b61 6e62 616e 2f64 6a61 6e67 6f2d  t/Kanban/django-
-00000240: 636f 6e6e 6563 7477 6973 652f 646a 616e  connectwise/djan
-00000250: 676f 2d63 6f6e 6e65 6374 7769 7365 2f64  go-connectwise/d
-00000260: 6a63 6f6e 6e65 6374 7769 7365 2f6d 616e  jconnectwise/man
-00000270: 6167 656d 656e 742f 636f 6d6d 616e 6473  agement/commands
-00000280: 2f6c 6973 745f 7573 6572 732e 7079 da06  /list_users.py..
-00000290: 6861 6e64 6c65 0800 0000 730c 0000 0000  handle....s.....
-000002a0: 0122 0109 0106 0106 0109 017a 0e43 6f6d  .".........z.Com
-000002b0: 6d61 6e64 2e68 616e 646c 654e 2905 da08  mand.handleN)...
-000002c0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000002d0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000002e0: 5f5f da04 6865 6c70 7217 0000 0072 1500  __..helpr....r..
-000002f0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000300: 0072 0400 0000 0500 0000 7304 0000 000c  .r........s.....
-00000310: 0106 0272 0400 0000 4e29 05da 1b64 6a61  ...r....N)...dja
-00000320: 6e67 6f2e 636f 7265 2e6d 616e 6167 656d  ngo.core.managem
-00000330: 656e 742e 6261 7365 7202 0000 005a 1464  ent.baser....Z.d
-00000340: 6a63 6f6e 6e65 6374 7769 7365 2e6d 6f64  jconnectwise.mod
-00000350: 656c 7372 0300 0000 7204 0000 0072 1500  elsr....r....r..
-00000360: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000370: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000380: 0400 0000 1001 1003                      ........
+00000020: 0073 2c00 0000 6400 6401 6c00 6d01 5a01  .s,...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 0100 4700  ..d.d.l.m.Z...G.
+00000040: 6403 6404 8400 6404 6501 8303 5a04 6405  d.d...d.e...Z.d.
+00000050: 5300 2906 e900 0000 0029 01da 0b42 6173  S.)......)...Bas
+00000060: 6543 6f6d 6d61 6e64 2901 da06 4d65 6d62  eCommand)...Memb
+00000070: 6572 6300 0000 0000 0000 0000 0000 0002  erc.............
+00000080: 0000 0040 0000 0073 1800 0000 6500 5a01  ...@...s....e.Z.
+00000090: 6400 5a02 6401 5a03 6402 6403 8400 5a04  d.Z.d.Z.d.d...Z.
+000000a0: 6404 5300 2905 da07 436f 6d6d 616e 647a  d.S.)...Commandz
+000000b0: 2e4c 6973 7420 6163 7469 7665 2c20 6675  .List active, fu
+000000c0: 6c6c 2d6c 6963 656e 7365 2043 6f6e 6e65  ll-license Conne
+000000d0: 6374 5769 7365 206d 656d 6265 7273 2e63  ctWise members.c
+000000e0: 0100 0000 0000 0000 0400 0000 0600 0000  ................
+000000f0: 4f00 0000 7346 0000 0078 4074 006a 016a  O...sF...x@t.j.j
+00000100: 0264 0164 0264 038d 0244 005d 2c7d 037c  .d.d.d...D.],}.|
+00000110: 006a 036a 0464 046a 057c 036a 067c 036a  .j.j.d.j.|.j.|.j
+00000120: 0783 007c 036a 0872 367c 036a 086e 0264  ...|.j.r6|.j.n.d
+00000130: 0583 0383 0101 0071 1257 0064 0053 0029  .......q.W.d.S.)
+00000140: 064e 46da 0146 2902 da08 696e 6163 7469  .NF..F)...inacti
+00000150: 7665 da0d 6c69 6365 6e73 655f 636c 6173  ve..license_clas
+00000160: 737a 117b 3a31 357d 207b 3a32 307d 207b  sz.{:15} {:20} {
+00000170: 3a34 337d da00 2909 7203 0000 00da 076f  :43}..).r......o
+00000180: 626a 6563 7473 da06 6669 6c74 6572 da06  bjects..filter..
+00000190: 7374 646f 7574 da05 7772 6974 65da 0666  stdout..write..f
+000001a0: 6f72 6d61 74da 0a69 6465 6e74 6966 6965  ormat..identifie
+000001b0: 72da 075f 5f73 7472 5f5f da0c 6f66 6669  r..__str__..offi
+000001c0: 6365 5f65 6d61 696c 2904 da04 7365 6c66  ce_email)...self
+000001d0: da04 6172 6773 da07 6f70 7469 6f6e 73da  ..args..options.
+000001e0: 066d 656d 6265 72a9 0072 1500 0000 fa5f  .member..r....._
+000001f0: 2f68 6f6d 652f 6361 6d65 726f 6e2f 4465  /home/cameron/De
+00000200: 762f 6b61 6e62 616e 2d64 6576 2f64 6a61  v/kanban-dev/dja
+00000210: 6e67 6f2d 636f 6e6e 6563 7477 6973 652f  ngo-connectwise/
+00000220: 646a 636f 6e6e 6563 7477 6973 652f 6d61  djconnectwise/ma
+00000230: 6e61 6765 6d65 6e74 2f63 6f6d 6d61 6e64  nagement/command
+00000240: 732f 6c69 7374 5f75 7365 7273 2e70 79da  s/list_users.py.
+00000250: 0668 616e 646c 6508 0000 0073 0c00 0000  .handle....s....
+00000260: 0001 1601 0601 0401 0401 0601 7a0e 436f  ............z.Co
+00000270: 6d6d 616e 642e 6861 6e64 6c65 4e29 05da  mmand.handleN)..
+00000280: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000290: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000002a0: 655f 5fda 0468 656c 7072 1700 0000 7215  e__..helpr....r.
+000002b0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+000002c0: 0000 7204 0000 0005 0000 0073 0400 0000  ..r........s....
+000002d0: 0801 0402 7204 0000 004e 2905 da1b 646a  ....r....N)...dj
+000002e0: 616e 676f 2e63 6f72 652e 6d61 6e61 6765  ango.core.manage
+000002f0: 6d65 6e74 2e62 6173 6572 0200 0000 5a14  ment.baser....Z.
+00000300: 646a 636f 6e6e 6563 7477 6973 652e 6d6f  djconnectwise.mo
+00000310: 6465 6c73 7203 0000 0072 0400 0000 7215  delsr....r....r.
+00000320: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00000330: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000340: 7304 0000 000c 010c 03                   s........
```

### Comparing `django-connectwise-0.3.98/djconnectwise/management/commands/cwclearoldsyncjobs.py` & `django-connectwise-0.3.99/djconnectwise/management/commands/cwclearoldsyncjobs.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/management/commands/cwsync.py` & `django-connectwise-0.3.99/djconnectwise/management/commands/cwsync.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/management/commands/list_callbacks.py` & `django-connectwise-0.3.99/djconnectwise/management/commands/list_callbacks.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/management/commands/updateslaexpiretimes.py` & `django-connectwise-0.3.99/djconnectwise/management/commands/updateslaexpiretimes.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/utils.py` & `django-connectwise-0.3.99/djconnectwise/utils.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/djconnectwise/api.py` & `django-connectwise-0.3.99/djconnectwise/api.py`

 * *Files identical despite different names*

### Comparing `django-connectwise-0.3.98/PKG-INFO` & `django-connectwise-0.3.99/django_connectwise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-connectwise
-Version: 0.3.98
+Version: 0.3.99
 Summary: Django app for working with ConnectWise. Defines models (tickets, members, companies, etc.) and callbacks.
 Home-page: https://github.com/KerkhoffTechnologies/django-connectwise
 Author: Kerkhoff Technologies Inc.
 Author-email: matt@kerkhofftech.ca
 License: MIT
 Description: # django-connectwise
```

### Comparing `django-connectwise-0.3.98/django_connectwise.egg-info/SOURCES.txt` & `django-connectwise-0.3.99/django_connectwise.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,37 +14,37 @@
 djconnectwise/callbacks.py
 djconnectwise/models.py
 djconnectwise/signals.py
 djconnectwise/sync.py
 djconnectwise/urls.py
 djconnectwise/utils.py
 djconnectwise/views.py
-djconnectwise/__pycache__/__init__.cpython-35.pyc
-djconnectwise/__pycache__/api.cpython-35.pyc
-djconnectwise/__pycache__/apps.cpython-35.pyc
-djconnectwise/__pycache__/callbacks.cpython-35.pyc
-djconnectwise/__pycache__/models.cpython-35.pyc
-djconnectwise/__pycache__/signals.cpython-35.pyc
-djconnectwise/__pycache__/sync.cpython-35.pyc
-djconnectwise/__pycache__/urls.cpython-35.pyc
-djconnectwise/__pycache__/utils.cpython-35.pyc
-djconnectwise/__pycache__/views.cpython-35.pyc
+djconnectwise/__pycache__/__init__.cpython-36.pyc
+djconnectwise/__pycache__/api.cpython-36.pyc
+djconnectwise/__pycache__/apps.cpython-36.pyc
+djconnectwise/__pycache__/callbacks.cpython-36.pyc
+djconnectwise/__pycache__/models.cpython-36.pyc
+djconnectwise/__pycache__/signals.cpython-36.pyc
+djconnectwise/__pycache__/sync.cpython-36.pyc
+djconnectwise/__pycache__/urls.cpython-36.pyc
+djconnectwise/__pycache__/utils.cpython-36.pyc
+djconnectwise/__pycache__/views.cpython-36.pyc
 djconnectwise/management/__init__.py
-djconnectwise/management/__pycache__/__init__.cpython-35.pyc
+djconnectwise/management/__pycache__/__init__.cpython-36.pyc
 djconnectwise/management/commands/__init__.py
 djconnectwise/management/commands/callbacks_deleted.py
 djconnectwise/management/commands/callbacks_registered.py
 djconnectwise/management/commands/cwclearoldsyncjobs.py
 djconnectwise/management/commands/cwsync.py
 djconnectwise/management/commands/list_callbacks.py
 djconnectwise/management/commands/list_users.py
 djconnectwise/management/commands/updateslaexpiretimes.py
-djconnectwise/management/commands/__pycache__/__init__.cpython-35.pyc
-djconnectwise/management/commands/__pycache__/cwsync.cpython-35.pyc
-djconnectwise/management/commands/__pycache__/list_users.cpython-35.pyc
+djconnectwise/management/commands/__pycache__/__init__.cpython-36.pyc
+djconnectwise/management/commands/__pycache__/cwsync.cpython-36.pyc
+djconnectwise/management/commands/__pycache__/list_users.cpython-36.pyc
 djconnectwise/migrations/0001_initial.py
 djconnectwise/migrations/0002_auto_20170223_2143.py
 djconnectwise/migrations/0003_auto_20170223_2233.py
 djconnectwise/migrations/0004_auto_20170224_1853.py
 djconnectwise/migrations/0005_auto_20170225_0101.py
 djconnectwise/migrations/0006_auto_20170303_1242.py
 djconnectwise/migrations/0007_auto_20170311_1415.py
@@ -173,170 +173,170 @@
 djconnectwise/migrations/0115_agreement_agreement_status.py
 djconnectwise/migrations/0116_auto_20200522_1107.py
 djconnectwise/migrations/0117_auto_20200609_1514.py
 djconnectwise/migrations/0118_auto_20200623_1016.py
 djconnectwise/migrations/0119_auto_20200624_1028.py
 djconnectwise/migrations/0120_auto_20200721_1617.py
 djconnectwise/migrations/__init__.py
-djconnectwise/migrations/__pycache__/0001_initial.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0002_auto_20170223_2143.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0003_auto_20170223_2233.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0004_auto_20170224_1853.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0005_auto_20170225_0101.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0006_auto_20170303_1242.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0007_auto_20170311_1415.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0008_project_status_name.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0009_member_license_class.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0010_remove_project_project_href.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0011_company_deleted_flag.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0012_auto_20170320_1057.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0013_auto_20170403_1203.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0014_company_status.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0015_auto_20170404_1504.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0016_auto_20170404_1504.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0017_auto_20170504_2054.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0018_auto_20170505_1531.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0019_syncjob_entity_name.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0019_ticket_owner.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0020_merge.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0020_ticket_customer_updated.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0021_merge.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0022_opportunitystatus.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0023_auto_20170605_0705.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0024_opportunitystage.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0025_opportunity.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0025_opportunitypriority.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0026_merge.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0027_auto_20170605_1534.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0028_merge.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0028_remove_company_company_alias.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0029_auto_20170607_1147.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0029_merge.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0030_merge.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0031_auto_20170607_2234.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0032_auto_20170616_1144.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0033_auto_20170616_1251.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0034_auto_20170727_1243.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0035_activity.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0036_auto_20170823_1417.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0037_auto_20170920_0959.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0038_auto_20170920_1138.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0039_auto_20170925_1418.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0040_auto_20170926_2145.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0041_auto_20171030_1047.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0042_auto_20171115_1131.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0043_projectstatus.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0044_auto_20171222_1700.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0045_auto_20171222_1725.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0046_auto_20180104_1504.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0047_syncjob_sync_type.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0048_project_manager.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0049_auto_20180205_1122.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0050_auto_20180417_1620.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0050_servicenote.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0050_timeentry.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0051_merge.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0051_opportunitynote.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0052_merge.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0053_merge.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0054_auto_20180501_1009.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0055_auto_20180501_1022.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0056_auto_20180504_0744.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0057_auto_20180511_1440.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0058_auto_20180516_1052.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0059_auto_20180518_0811.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0060_auto_20180605_0840.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0061_auto_20180605_1208.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0061_auto_20180607_1210.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0062_auto_20180606_1117.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0063_merge_20180611_0905.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0064_auto_20180808_1214.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0065_auto_20180809_1124.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0066_auto_20180814_1046.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0066_slapriority.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0067_auto_20180813_1355.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0068_merge_20180814_1104.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0069_auto_20180815_1116.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0070_mycompanyother.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0071_auto_20180822_1300.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0072_remove_callbackentry_member.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0073_auto_20180824_1446.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0074_auto_20180827_1241.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0075_auto_20180910_1629.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0076_auto_20180925_1618.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0077_item_subtype_type.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0078_auto_20181203_1017.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0079_auto_20181203_1606.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0080_auto_20181210_0930.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0081_auto_20181220_0917.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0082_auto_20190125_1109.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0083_delete_callbackentry.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0084_auto_20190404_1532.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0085_auto_20190430_1004.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0085_auto_20190506_1028.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0086_merge_20190507_1402.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0087_auto_20190705_1015.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0087_auto_20190709_0836.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0088_auto_20190710_0953.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0089_merge_20190711_1100.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0090_auto_20190711_1114.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0091_workrole.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0091_worktype_bill_time.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0092_remove_ticket_work_type.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0093_auto_20190716_1630.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0093_merge_20190716_1459.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0094_connectwiseboard_work_role.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0095_connectwiseboard_work_type.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0096_agreement.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0096_merge_20190718_1102.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0097_merge_20190718_1325.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0098_auto_20190718_1406.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0099_timeentry_agreement.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0100_auto_20190718_1417.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0101_agreement_company.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0102_auto_20190719_1058.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0103_activitystatus_activitytype.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0104_auto_20190722_1232.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0105_auto_20190722_1444.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0106_auto_20190722_1524.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0107_auto_20190729_1352.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0108_projectphase.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0109_ticket_phase.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0110_project_company.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0111_auto_20191204_0838.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0112_syncjob_synchronizer_class.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0113_auto_20200204_1054.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0114_auto_20200219_1515.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0115_agreement_agreement_status.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0116_auto_20200522_1107.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0117_auto_20200609_1514.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0118_auto_20200623_1016.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0119_auto_20200624_1028.cpython-35.pyc
-djconnectwise/migrations/__pycache__/0120_auto_20200721_1617.cpython-35.pyc
-djconnectwise/migrations/__pycache__/__init__.cpython-35.pyc
+djconnectwise/migrations/__pycache__/0001_initial.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0002_auto_20170223_2143.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0003_auto_20170223_2233.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0004_auto_20170224_1853.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0005_auto_20170225_0101.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0006_auto_20170303_1242.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0007_auto_20170311_1415.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0008_project_status_name.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0009_member_license_class.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0010_remove_project_project_href.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0011_company_deleted_flag.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0012_auto_20170320_1057.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0013_auto_20170403_1203.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0014_company_status.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0015_auto_20170404_1504.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0016_auto_20170404_1504.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0017_auto_20170504_2054.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0018_auto_20170505_1531.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0019_syncjob_entity_name.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0019_ticket_owner.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0020_merge.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0020_ticket_customer_updated.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0021_merge.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0022_opportunitystatus.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0023_auto_20170605_0705.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0024_opportunitystage.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0025_opportunity.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0025_opportunitypriority.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0026_merge.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0027_auto_20170605_1534.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0028_merge.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0028_remove_company_company_alias.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0029_auto_20170607_1147.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0029_merge.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0030_merge.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0031_auto_20170607_2234.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0032_auto_20170616_1144.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0033_auto_20170616_1251.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0034_auto_20170727_1243.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0035_activity.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0036_auto_20170823_1417.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0037_auto_20170920_0959.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0038_auto_20170920_1138.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0039_auto_20170925_1418.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0040_auto_20170926_2145.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0041_auto_20171030_1047.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0042_auto_20171115_1131.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0043_projectstatus.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0044_auto_20171222_1700.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0045_auto_20171222_1725.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0046_auto_20180104_1504.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0047_syncjob_sync_type.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0048_project_manager.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0049_auto_20180205_1122.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0050_auto_20180417_1620.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0050_servicenote.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0050_timeentry.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0051_merge.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0051_opportunitynote.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0052_merge.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0053_merge.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0054_auto_20180501_1009.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0055_auto_20180501_1022.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0056_auto_20180504_0744.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0057_auto_20180511_1440.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0058_auto_20180516_1052.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0059_auto_20180518_0811.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0060_auto_20180605_0840.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0061_auto_20180605_1208.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0061_auto_20180607_1210.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0062_auto_20180606_1117.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0063_merge_20180611_0905.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0064_auto_20180808_1214.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0065_auto_20180809_1124.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0066_auto_20180814_1046.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0066_slapriority.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0067_auto_20180813_1355.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0068_merge_20180814_1104.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0069_auto_20180815_1116.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0070_mycompanyother.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0071_auto_20180822_1300.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0072_remove_callbackentry_member.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0073_auto_20180824_1446.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0074_auto_20180827_1241.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0075_auto_20180910_1629.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0076_auto_20180925_1618.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0077_item_subtype_type.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0078_auto_20181203_1017.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0079_auto_20181203_1606.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0080_auto_20181210_0930.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0081_auto_20181220_0917.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0082_auto_20190125_1109.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0083_delete_callbackentry.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0084_auto_20190404_1532.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0085_auto_20190430_1004.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0085_auto_20190506_1028.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0086_merge_20190507_1402.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0087_auto_20190705_1015.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0087_auto_20190709_0836.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0088_auto_20190710_0953.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0089_merge_20190711_1100.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0090_auto_20190711_1114.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0091_workrole.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0091_worktype_bill_time.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0092_remove_ticket_work_type.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0093_auto_20190716_1630.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0093_merge_20190716_1459.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0094_connectwiseboard_work_role.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0095_connectwiseboard_work_type.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0096_agreement.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0096_merge_20190718_1102.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0097_merge_20190718_1325.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0098_auto_20190718_1406.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0099_timeentry_agreement.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0100_auto_20190718_1417.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0101_agreement_company.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0102_auto_20190719_1058.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0103_activitystatus_activitytype.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0104_auto_20190722_1232.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0105_auto_20190722_1444.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0106_auto_20190722_1524.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0107_auto_20190729_1352.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0108_projectphase.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0109_ticket_phase.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0110_project_company.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0111_auto_20191204_0838.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0112_syncjob_synchronizer_class.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0113_auto_20200204_1054.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0114_auto_20200219_1515.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0115_agreement_agreement_status.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0116_auto_20200522_1107.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0117_auto_20200609_1514.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0118_auto_20200623_1016.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0119_auto_20200624_1028.cpython-36.pyc
+djconnectwise/migrations/__pycache__/0120_auto_20200721_1617.cpython-36.pyc
+djconnectwise/migrations/__pycache__/__init__.cpython-36.pyc
 djconnectwise/tests/AnonymousMember.png
 djconnectwise/tests/__init__.py
 djconnectwise/tests/fixture_utils.py
 djconnectwise/tests/fixtures.py
 djconnectwise/tests/mocks.py
 djconnectwise/tests/mommy_recipes.py
 djconnectwise/tests/test_api.py
 djconnectwise/tests/test_callback.py
 djconnectwise/tests/test_commands.py
 djconnectwise/tests/test_models.py
 djconnectwise/tests/test_sync.py
 djconnectwise/tests/test_utils.py
 djconnectwise/tests/test_views.py
 djconnectwise/tests/urls.py
-djconnectwise/tests/__pycache__/__init__.cpython-35.pyc
-djconnectwise/tests/__pycache__/fixture_utils.cpython-35.pyc
-djconnectwise/tests/__pycache__/fixtures.cpython-35.pyc
-djconnectwise/tests/__pycache__/mocks.cpython-35.pyc
-djconnectwise/tests/__pycache__/mommy_recipes.cpython-35.pyc
-djconnectwise/tests/__pycache__/test_api.cpython-35.pyc
-djconnectwise/tests/__pycache__/test_callback.cpython-35.pyc
-djconnectwise/tests/__pycache__/test_commands.cpython-35.pyc
-djconnectwise/tests/__pycache__/test_models.cpython-35.pyc
-djconnectwise/tests/__pycache__/test_sync.cpython-35.pyc
-djconnectwise/tests/__pycache__/test_utils.cpython-35.pyc
-djconnectwise/tests/__pycache__/test_views.cpython-35.pyc
-djconnectwise/tests/__pycache__/urls.cpython-35.pyc
+djconnectwise/tests/__pycache__/__init__.cpython-36.pyc
+djconnectwise/tests/__pycache__/fixture_utils.cpython-36.pyc
+djconnectwise/tests/__pycache__/fixtures.cpython-36.pyc
+djconnectwise/tests/__pycache__/mocks.cpython-36.pyc
+djconnectwise/tests/__pycache__/mommy_recipes.cpython-36.pyc
+djconnectwise/tests/__pycache__/test_api.cpython-36.pyc
+djconnectwise/tests/__pycache__/test_callback.cpython-36.pyc
+djconnectwise/tests/__pycache__/test_commands.cpython-36.pyc
+djconnectwise/tests/__pycache__/test_models.cpython-36.pyc
+djconnectwise/tests/__pycache__/test_sync.cpython-36.pyc
+djconnectwise/tests/__pycache__/test_utils.cpython-36.pyc
+djconnectwise/tests/__pycache__/test_views.cpython-36.pyc
+djconnectwise/tests/__pycache__/urls.cpython-36.pyc
```

### Comparing `django-connectwise-0.3.98/django_connectwise.egg-info/PKG-INFO` & `django-connectwise-0.3.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-connectwise
-Version: 0.3.98
+Version: 0.3.99
 Summary: Django app for working with ConnectWise. Defines models (tickets, members, companies, etc.) and callbacks.
 Home-page: https://github.com/KerkhoffTechnologies/django-connectwise
 Author: Kerkhoff Technologies Inc.
 Author-email: matt@kerkhofftech.ca
 License: MIT
 Description: # django-connectwise
```

### Comparing `django-connectwise-0.3.98/README.md` & `django-connectwise-0.3.99/README.md`

 * *Files identical despite different names*

