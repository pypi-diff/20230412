# Comparing `tmp/simeon-0.0.8.tar.gz` & `tmp/simeon-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simeon-0.0.8.tar", last modified: Wed Oct 27 13:48:25 2021, max compression
+gzip compressed data, was "simeon-0.0.9.tar", last modified: Wed Oct 27 14:57:07 2021, max compression
```

## Comparing `simeon-0.0.8.tar` & `simeon-0.0.9.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 13:48:25.339949 simeon-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-10-27 13:48:11.000000 simeon-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-10-27 13:48:11.000000 simeon-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14764 2021-10-27 13:48:25.339949 simeon-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13733 2021-10-27 13:48:11.000000 simeon-0.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-27 13:48:25.339949 simeon-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2068 2021-10-27 13:48:11.000000 simeon-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 13:48:25.327949 simeon-0.0.8/simeon/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 13:48:25.327949 simeon-0.0.8/simeon/download/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6020 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/download/aws.py
--rw-r--r--   0 runner    (1001) docker     (121)     4011 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/download/emails.py
--rw-r--r--   0 runner    (1001) docker     (121)    12896 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/download/logs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7202 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/download/sqls.py
--rw-r--r--   0 runner    (1001) docker     (121)    18593 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/download/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 13:48:25.327949 simeon-0.0.8/simeon/exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)     1769 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 13:48:25.327949 simeon-0.0.8/simeon/report/
--rw-r--r--   0 runner    (1001) docker     (121)      418 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 13:48:25.331949 simeon-0.0.8/simeon/report/queries/
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/chapter_grades.sql
--rw-r--r--   0 runner    (1001) docker     (121)    18496 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/course_item.sql
--rw-r--r--   0 runner    (1001) docker     (121)      681 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/course_modal_ip.sql
--rw-r--r--   0 runner    (1001) docker     (121)      634 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/course_modal_language.sql
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/course_problem.sql
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/enrollday_all.sql
--rw-r--r--   0 runner    (1001) docker     (121)      790 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/enrollment_events.sql
--rw-r--r--   0 runner    (1001) docker     (121)     4970 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/forum_events.sql
--rw-r--r--   0 runner    (1001) docker     (121)     4537 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/forum_person.sql
--rw-r--r--   0 runner    (1001) docker     (121)     5210 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/forum_posts.sql
--rw-r--r--   0 runner    (1001) docker     (121)      875 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/language_multi_transcripts.sql
--rw-r--r--   0 runner    (1001) docker     (121)     3728 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/ora_events.sql
--rw-r--r--   0 runner    (1001) docker     (121)      356 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/pc_day_ip_counts.sql
--rw-r--r--   0 runner    (1001) docker     (121)      744 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/pc_day_totals.sql
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/pc_day_trlang.sql
--rw-r--r--   0 runner    (1001) docker     (121)      412 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/pc_forum.sql
--rw-r--r--   0 runner    (1001) docker     (121)      221 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/pc_nchapters.sql
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/pc_video_watched.sql
--rw-r--r--   0 runner    (1001) docker     (121)     4497 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/person_course.sql
--rw-r--r--   0 runner    (1001) docker     (121)    13181 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/person_course_day.sql
--rw-r--r--   0 runner    (1001) docker     (121)      412 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/person_enrollment_verified.sql
--rw-r--r--   0 runner    (1001) docker     (121)      699 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/person_item.sql
--rw-r--r--   0 runner    (1001) docker     (121)      469 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/person_problem.sql
--rw-r--r--   0 runner    (1001) docker     (121)      504 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/problem_grades.sql
--rw-r--r--   0 runner    (1001) docker     (121)      336 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/show_answer.sql
--rw-r--r--   0 runner    (1001) docker     (121)    11196 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/show_answer_stats_by_course.sql
--rw-r--r--   0 runner    (1001) docker     (121)     3033 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/show_answer_stats_by_user.sql
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/time_on_asset_daily.sql
--rw-r--r--   0 runner    (1001) docker     (121)     2431 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/time_on_asset_totals.sql
--rw-r--r--   0 runner    (1001) docker     (121)     7660 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/time_on_task.sql
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/time_on_task_totals.sql
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/video_axis.sql
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/queries/video_stats_day.sql
--rw-r--r--   0 runner    (1001) docker     (121)    56286 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/report/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 13:48:25.331949 simeon-0.0.8/simeon/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 13:48:25.331949 simeon-0.0.8/simeon/scripts/data/
--rw-r--r--   0 runner    (1001) docker     (121)    18016 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/scripts/data/geographic_regions_by_country.csv
--rw-r--r--   0 runner    (1001) docker     (121)    14608 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/scripts/geoip.py
--rw-r--r--   0 runner    (1001) docker     (121)    54931 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/scripts/simeon.py
--rw-r--r--   0 runner    (1001) docker     (121)    25405 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/scripts/utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    14832 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/scripts/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 13:48:25.331949 simeon-0.0.8/simeon/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17604 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/tests/test_download_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     6135 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     7774 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/tests/test_report_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     3366 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/tests/test_upload_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 13:48:25.331949 simeon-0.0.8/simeon/upload/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13795 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 13:48:25.335949 simeon-0.0.8/simeon/upload/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_chapter_grades.json
--rw-r--r--   0 runner    (1001) docker     (121)    45300 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_combined_course_summary_stats.json
--rw-r--r--   0 runner    (1001) docker     (121)      792 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_content_stats.json
--rw-r--r--   0 runner    (1001) docker     (121)     5523 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_course_axis.json
--rw-r--r--   0 runner    (1001) docker     (121)     7870 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_course_item.json
--rw-r--r--   0 runner    (1001) docker     (121)    13178 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_course_listing_and_metainfo.json
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_course_listings.json
--rw-r--r--   0 runner    (1001) docker     (121)      401 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_course_metainfo.json
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_course_modal_ip.json
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_course_modal_language.json
--rw-r--r--   0 runner    (1001) docker     (121)     2857 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_course_problem.json
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_email_opt_in.json
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_enrollday_all.json
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_enrollment_events.json
--rw-r--r--   0 runner    (1001) docker     (121)     4035 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_forum.json
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_forum_events.json
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_forum_person.json
--rw-r--r--   0 runner    (1001) docker     (121)     2153 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_forum_posts.json
--rw-r--r--   0 runner    (1001) docker     (121)     2944 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_geoip.json
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_grades_persistent.json
--rw-r--r--   0 runner    (1001) docker     (121)     2942 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_grades_persistent_subsection.json
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_grading_policy.json
--rw-r--r--   0 runner    (1001) docker     (121)     2136 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_language_multi_transcripts.json
--rw-r--r--   0 runner    (1001) docker     (121)     4453 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_mitx_course.json
--rw-r--r--   0 runner    (1001) docker     (121)     3052 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_ora_events.json
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_pc_day_ip_counts.json
--rw-r--r--   0 runner    (1001) docker     (121)     4476 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_pc_day_totals.json
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_pc_day_trlang.json
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_pc_forum.json
--rw-r--r--   0 runner    (1001) docker     (121)      610 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_pc_nchapters.json
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_pc_video_watched.json
--rw-r--r--   0 runner    (1001) docker     (121)    15646 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_person_course.json
--rw-r--r--   0 runner    (1001) docker     (121)     7923 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_person_course_day.json
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_person_enrollment_verified.json
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_person_item.json
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_person_problem.json
--rw-r--r--   0 runner    (1001) docker     (121)     2778 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_problem_analysis.json
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_problem_grades.json
--rw-r--r--   0 runner    (1001) docker     (121)     3111 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_roles.json
--rw-r--r--   0 runner    (1001) docker     (121)      982 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_show_answer.json
--rw-r--r--   0 runner    (1001) docker     (121)    13311 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_show_answer_stats_by_course.json
--rw-r--r--   0 runner    (1001) docker     (121)     4832 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_show_answer_stats_by_user.json
--rw-r--r--   0 runner    (1001) docker     (121)      627 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_staff.json
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_studentmodule.json
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_time_on_asset_daily.json
--rw-r--r--   0 runner    (1001) docker     (121)     3572 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_time_on_asset_totals.json
--rw-r--r--   0 runner    (1001) docker     (121)     3822 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_time_on_task.json
--rw-r--r--   0 runner    (1001) docker     (121)     3708 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_time_on_task_totals.json
--rw-r--r--   0 runner    (1001) docker     (121)    16795 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_tracking_log.json
--rw-r--r--   0 runner    (1001) docker     (121)     8330 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_user_info_combo.json
--rw-r--r--   0 runner    (1001) docker     (121)      729 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_user_partitions.json
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_video_axis.json
--rw-r--r--   0 runner    (1001) docker     (121)      742 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_video_stats_day.json
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schema_youtube.json
--rw-r--r--   0 runner    (1001) docker     (121)    49273 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/schemas/schemas.json
--rw-r--r--   0 runner    (1001) docker     (121)    12218 2021-10-27 13:48:11.000000 simeon-0.0.8/simeon/upload/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 13:48:25.327949 simeon-0.0.8/simeon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14764 2021-10-27 13:48:25.000000 simeon-0.0.8/simeon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5029 2021-10-27 13:48:25.000000 simeon-0.0.8/simeon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-27 13:48:25.000000 simeon-0.0.8/simeon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-10-27 13:48:25.000000 simeon-0.0.8/simeon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-10-27 13:48:25.000000 simeon-0.0.8/simeon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-27 13:48:25.000000 simeon-0.0.8/simeon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 14:57:07.241747 simeon-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-10-27 14:56:57.000000 simeon-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2021-10-27 14:56:57.000000 simeon-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    14764 2021-10-27 14:57:07.241747 simeon-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    13733 2021-10-27 14:56:57.000000 simeon-0.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-27 14:57:07.241747 simeon-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2068 2021-10-27 14:56:57.000000 simeon-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 14:57:07.225747 simeon-0.0.9/simeon/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 14:57:07.225747 simeon-0.0.9/simeon/download/
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6020 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/download/aws.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4011 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/download/emails.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12896 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/download/logs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7202 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/download/sqls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18593 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/download/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 14:57:07.225747 simeon-0.0.9/simeon/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (121)     1769 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 14:57:07.225747 simeon-0.0.9/simeon/report/
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 14:57:07.229747 simeon-0.0.9/simeon/report/queries/
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/chapter_grades.sql
+-rw-r--r--   0 runner    (1001) docker     (121)    18496 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/course_item.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/course_modal_ip.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/course_modal_language.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/course_problem.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     1708 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/enrollday_all.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/enrollment_events.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     4970 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/forum_events.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     4537 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/forum_person.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     5210 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/forum_posts.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      875 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/language_multi_transcripts.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     3728 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/ora_events.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/pc_day_ip_counts.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      744 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/pc_day_totals.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     2991 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/pc_day_trlang.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/pc_forum.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/pc_nchapters.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/pc_video_watched.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     4497 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/person_course.sql
+-rw-r--r--   0 runner    (1001) docker     (121)    13181 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/person_course_day.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/person_enrollment_verified.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      699 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/person_item.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/person_problem.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/problem_grades.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/show_answer.sql
+-rw-r--r--   0 runner    (1001) docker     (121)    11196 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/show_answer_stats_by_course.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     3033 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/show_answer_stats_by_user.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     1987 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/time_on_asset_daily.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     2431 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/time_on_asset_totals.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     7660 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/time_on_task.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     1528 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/time_on_task_totals.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     1359 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/video_axis.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/queries/video_stats_day.sql
+-rw-r--r--   0 runner    (1001) docker     (121)    56286 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/report/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 14:57:07.233747 simeon-0.0.9/simeon/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 14:57:07.233747 simeon-0.0.9/simeon/scripts/data/
+-rw-r--r--   0 runner    (1001) docker     (121)    18016 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/scripts/data/geographic_regions_by_country.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    14608 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/scripts/geoip.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54931 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/scripts/simeon.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25405 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/scripts/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14832 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/scripts/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 14:57:07.233747 simeon-0.0.9/simeon/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17604 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/tests/test_download_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6135 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7774 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/tests/test_report_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3366 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/tests/test_upload_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 14:57:07.233747 simeon-0.0.9/simeon/upload/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14009 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 14:57:07.237747 simeon-0.0.9/simeon/upload/schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)     1811 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_chapter_grades.json
+-rw-r--r--   0 runner    (1001) docker     (121)    45300 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_combined_course_summary_stats.json
+-rw-r--r--   0 runner    (1001) docker     (121)      792 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_content_stats.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5523 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_course_axis.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7870 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_course_item.json
+-rw-r--r--   0 runner    (1001) docker     (121)    13178 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_course_listing_and_metainfo.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1533 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_course_listings.json
+-rw-r--r--   0 runner    (1001) docker     (121)      401 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_course_metainfo.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_course_modal_ip.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1746 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_course_modal_language.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2857 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_course_problem.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1375 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_email_opt_in.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2017 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_enrollday_all.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2157 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_enrollment_events.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4035 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_forum.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1788 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_forum_events.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3257 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_forum_person.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2153 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_forum_posts.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2944 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_geoip.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2260 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_grades_persistent.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2942 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_grades_persistent_subsection.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2210 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_grading_policy.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2136 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_language_multi_transcripts.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4453 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_mitx_course.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3052 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_ora_events.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_pc_day_ip_counts.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4476 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_pc_day_totals.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1925 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_pc_day_trlang.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1494 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_pc_forum.json
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_pc_nchapters.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1439 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_pc_video_watched.json
+-rw-r--r--   0 runner    (1001) docker     (121)    15646 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_person_course.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7923 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_person_course_day.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1113 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_person_enrollment_verified.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1790 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_person_item.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1786 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_person_problem.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2778 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_problem_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_problem_grades.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3111 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_roles.json
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_show_answer.json
+-rw-r--r--   0 runner    (1001) docker     (121)    13311 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_show_answer_stats_by_course.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4832 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_show_answer_stats_by_user.json
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_staff.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2053 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_studentmodule.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1374 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_time_on_asset_daily.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3572 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_time_on_asset_totals.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3822 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_time_on_task.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3708 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_time_on_task_totals.json
+-rw-r--r--   0 runner    (1001) docker     (121)    16795 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_tracking_log.json
+-rw-r--r--   0 runner    (1001) docker     (121)     8330 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_user_info_combo.json
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_user_partitions.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1466 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_video_axis.json
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_video_stats_day.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1403 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schema_youtube.json
+-rw-r--r--   0 runner    (1001) docker     (121)    49273 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/schemas/schemas.json
+-rw-r--r--   0 runner    (1001) docker     (121)    12218 2021-10-27 14:56:57.000000 simeon-0.0.9/simeon/upload/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 14:57:07.225747 simeon-0.0.9/simeon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    14764 2021-10-27 14:57:07.000000 simeon-0.0.9/simeon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5029 2021-10-27 14:57:07.000000 simeon-0.0.9/simeon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-27 14:57:07.000000 simeon-0.0.9/simeon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2021-10-27 14:57:07.000000 simeon-0.0.9/simeon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-10-27 14:57:07.000000 simeon-0.0.9/simeon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-27 14:57:07.000000 simeon-0.0.9/simeon.egg-info/top_level.txt
```

### Comparing `simeon-0.0.8/LICENSE` & `simeon-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/PKG-INFO` & `simeon-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simeon
-Version: 0.0.8
+Version: 0.0.9
 Summary: A CLI tool to help process research data from edX
 Home-page: https://github.com/MIT-IR/simeon
 Author: MIT Institutional Research
 Author-email: irx@mit.edu
 License: MIT LICENSE
 Keywords: edx research data,mitx,edx,MOOC,education,online learning
 Platform: UNKNOWN
```

### Comparing `simeon-0.0.8/README.rst` & `simeon-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/setup.py` & `simeon-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 # Get the value of __version__ from the library's __init__.py file
 exec(open(os.path.join('simeon', '__init__.py')).read())
 
 setup(
     name='simeon',
-    version=globals().get('__version__', '0.0.8'),
+    version=globals().get('__version__', '0.0.9'),
     author='MIT Institutional Research',
     author_email='irx@mit.edu',
     packages=find_packages(exclude=('docs',)),
     url='https://github.com/MIT-IR/simeon',
     license='MIT LICENSE',
     keywords=[
         'edx research data', 'mitx', 'edx',
```

### Comparing `simeon-0.0.8/simeon/download/aws.py` & `simeon-0.0.9/simeon/download/aws.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/download/emails.py` & `simeon-0.0.9/simeon/download/emails.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/download/logs.py` & `simeon-0.0.9/simeon/download/logs.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/download/sqls.py` & `simeon-0.0.9/simeon/download/sqls.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/download/utilities.py` & `simeon-0.0.9/simeon/download/utilities.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/exceptions/__init__.py` & `simeon-0.0.9/simeon/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/chapter_grades.sql` & `simeon-0.0.9/simeon/report/queries/chapter_grades.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/course_item.sql` & `simeon-0.0.9/simeon/report/queries/course_item.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/course_modal_ip.sql` & `simeon-0.0.9/simeon/report/queries/course_modal_ip.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/course_modal_language.sql` & `simeon-0.0.9/simeon/report/queries/course_modal_language.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/course_problem.sql` & `simeon-0.0.9/simeon/report/queries/course_problem.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/enrollday_all.sql` & `simeon-0.0.9/simeon/report/queries/enrollday_all.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/enrollment_events.sql` & `simeon-0.0.9/simeon/report/queries/enrollment_events.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/forum_events.sql` & `simeon-0.0.9/simeon/report/queries/forum_events.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/forum_person.sql` & `simeon-0.0.9/simeon/report/queries/forum_person.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/forum_posts.sql` & `simeon-0.0.9/simeon/report/queries/forum_posts.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/language_multi_transcripts.sql` & `simeon-0.0.9/simeon/report/queries/language_multi_transcripts.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/ora_events.sql` & `simeon-0.0.9/simeon/report/queries/ora_events.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/pc_day_totals.sql` & `simeon-0.0.9/simeon/report/queries/pc_day_totals.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/pc_day_trlang.sql` & `simeon-0.0.9/simeon/report/queries/pc_day_trlang.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/pc_video_watched.sql` & `simeon-0.0.9/simeon/report/queries/pc_video_watched.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/person_course.sql` & `simeon-0.0.9/simeon/report/queries/person_course.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/person_course_day.sql` & `simeon-0.0.9/simeon/report/queries/person_course_day.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/person_item.sql` & `simeon-0.0.9/simeon/report/queries/person_item.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/show_answer_stats_by_course.sql` & `simeon-0.0.9/simeon/report/queries/show_answer_stats_by_course.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/show_answer_stats_by_user.sql` & `simeon-0.0.9/simeon/report/queries/show_answer_stats_by_user.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/time_on_asset_daily.sql` & `simeon-0.0.9/simeon/report/queries/time_on_asset_daily.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/time_on_asset_totals.sql` & `simeon-0.0.9/simeon/report/queries/time_on_asset_totals.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/time_on_task.sql` & `simeon-0.0.9/simeon/report/queries/time_on_task.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/time_on_task_totals.sql` & `simeon-0.0.9/simeon/report/queries/time_on_task_totals.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/video_axis.sql` & `simeon-0.0.9/simeon/report/queries/video_axis.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/queries/video_stats_day.sql` & `simeon-0.0.9/simeon/report/queries/video_stats_day.sql`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/report/utilities.py` & `simeon-0.0.9/simeon/report/utilities.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/scripts/data/geographic_regions_by_country.csv` & `simeon-0.0.9/simeon/scripts/data/geographic_regions_by_country.csv`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/scripts/geoip.py` & `simeon-0.0.9/simeon/scripts/geoip.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/scripts/simeon.py` & `simeon-0.0.9/simeon/scripts/simeon.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/scripts/utilities.py` & `simeon-0.0.9/simeon/scripts/utilities.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/scripts/youtube.py` & `simeon-0.0.9/simeon/scripts/youtube.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/tests/test_download_utilities.py` & `simeon-0.0.9/simeon/tests/test_download_utilities.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/tests/test_integration.py` & `simeon-0.0.9/simeon/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/tests/test_report_utilities.py` & `simeon-0.0.9/simeon/tests/test_report_utilities.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/tests/test_upload_utilities.py` & `simeon-0.0.9/simeon/tests/test_upload_utilities.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/gcp.py` & `simeon-0.0.9/simeon/upload/gcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Utilities functions and classes to help with loading data to Google Cloud
 """
 import glob
 import gzip
 import os
+import uuid
 from datetime import datetime
 from typing import List
 
 from google.cloud import (
     bigquery, exceptions as gcp_exceptions, storage
 )
 
@@ -255,15 +256,20 @@
         :raises: Propagates everything from the underlying package
         """
         schema_dir = schema_dir or SCHEMA_DIR
         if len(table.split('.')) < 3:
             table = '{p}.{t}'.format(p=self.project, t=table)
         dataset = table.rsplit('.', 1)[0]
         bqtable = bigquery.Table.from_string(table)
-        temp_table = bigquery.Table.from_string(table + '_temp')
+        temp_table_name = '{t}_{d}_{u}_temp'.format(
+            t=table,
+            d=datetime.now().strftime('%Y%m%d%H%M%S%f'),
+            u=uuid.uuid4().replace('-', '').replace('.', '')
+        )
+        temp_table = bigquery.Table.from_string(temp_table_name)
         schema, desc = uputils.get_bq_schema(table, schema_dir=schema_dir)
         bqtable.schema = schema
         bqtable.description = desc
         temp_table.schema = schema
         if patch:
             # Update the destination table's description.
             # Catch the error raised when the destination table
@@ -295,15 +301,15 @@
         rutils.wait_for_bq_job_ids([job.job_id], self)
         if job.errors:
             msg = 'Merge job failed with: {e}'
             raise LoadJobException(msg.format(
                 e='\n'.join(self.extract_error_messages(job.errors))
             ))
         query = MERGE_DDL.format(
-            first=table, second=table + '_temp', column=col,
+            first=table, second=temp_table_name, column=col,
         )
         qjob = self.query(query)
         rutils.wait_for_bq_job_ids([qjob.job_id], self)
         if qjob.errors:
             msg = 'Merge job failed with: {e}'
             raise LoadJobException(msg.format(
                 e='\n'.join(self.extract_error_messages(job.errors))
```

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_chapter_grades.json` & `simeon-0.0.9/simeon/upload/schemas/schema_chapter_grades.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_combined_course_summary_stats.json` & `simeon-0.0.9/simeon/upload/schemas/schema_combined_course_summary_stats.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_content_stats.json` & `simeon-0.0.9/simeon/upload/schemas/schema_content_stats.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_course_axis.json` & `simeon-0.0.9/simeon/upload/schemas/schema_course_axis.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_course_item.json` & `simeon-0.0.9/simeon/upload/schemas/schema_course_item.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_course_listing_and_metainfo.json` & `simeon-0.0.9/simeon/upload/schemas/schema_course_listing_and_metainfo.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_course_listings.json` & `simeon-0.0.9/simeon/upload/schemas/schema_course_listings.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_course_modal_ip.json` & `simeon-0.0.9/simeon/upload/schemas/schema_course_modal_ip.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_course_modal_language.json` & `simeon-0.0.9/simeon/upload/schemas/schema_course_modal_language.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_course_problem.json` & `simeon-0.0.9/simeon/upload/schemas/schema_course_problem.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_email_opt_in.json` & `simeon-0.0.9/simeon/upload/schemas/schema_email_opt_in.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_enrollday_all.json` & `simeon-0.0.9/simeon/upload/schemas/schema_enrollday_all.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_enrollment_events.json` & `simeon-0.0.9/simeon/upload/schemas/schema_enrollment_events.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_forum.json` & `simeon-0.0.9/simeon/upload/schemas/schema_forum.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_forum_events.json` & `simeon-0.0.9/simeon/upload/schemas/schema_forum_events.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_forum_person.json` & `simeon-0.0.9/simeon/upload/schemas/schema_forum_person.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_forum_posts.json` & `simeon-0.0.9/simeon/upload/schemas/schema_forum_posts.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_geoip.json` & `simeon-0.0.9/simeon/upload/schemas/schema_geoip.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_grades_persistent.json` & `simeon-0.0.9/simeon/upload/schemas/schema_grades_persistent.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_grades_persistent_subsection.json` & `simeon-0.0.9/simeon/upload/schemas/schema_grades_persistent_subsection.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_grading_policy.json` & `simeon-0.0.9/simeon/upload/schemas/schema_grading_policy.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_language_multi_transcripts.json` & `simeon-0.0.9/simeon/upload/schemas/schema_language_multi_transcripts.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_mitx_course.json` & `simeon-0.0.9/simeon/upload/schemas/schema_mitx_course.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_ora_events.json` & `simeon-0.0.9/simeon/upload/schemas/schema_ora_events.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_pc_day_ip_counts.json` & `simeon-0.0.9/simeon/upload/schemas/schema_pc_day_ip_counts.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_pc_day_totals.json` & `simeon-0.0.9/simeon/upload/schemas/schema_pc_day_totals.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_pc_day_trlang.json` & `simeon-0.0.9/simeon/upload/schemas/schema_pc_day_trlang.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_pc_forum.json` & `simeon-0.0.9/simeon/upload/schemas/schema_pc_forum.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_pc_nchapters.json` & `simeon-0.0.9/simeon/upload/schemas/schema_pc_nchapters.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_pc_video_watched.json` & `simeon-0.0.9/simeon/upload/schemas/schema_pc_video_watched.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_person_course.json` & `simeon-0.0.9/simeon/upload/schemas/schema_person_course.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_person_course_day.json` & `simeon-0.0.9/simeon/upload/schemas/schema_person_course_day.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_person_enrollment_verified.json` & `simeon-0.0.9/simeon/upload/schemas/schema_person_enrollment_verified.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_person_item.json` & `simeon-0.0.9/simeon/upload/schemas/schema_person_item.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_person_problem.json` & `simeon-0.0.9/simeon/upload/schemas/schema_person_problem.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_problem_analysis.json` & `simeon-0.0.9/simeon/upload/schemas/schema_problem_analysis.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_problem_grades.json` & `simeon-0.0.9/simeon/upload/schemas/schema_problem_grades.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_roles.json` & `simeon-0.0.9/simeon/upload/schemas/schema_roles.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_show_answer.json` & `simeon-0.0.9/simeon/upload/schemas/schema_show_answer.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_show_answer_stats_by_course.json` & `simeon-0.0.9/simeon/upload/schemas/schema_show_answer_stats_by_course.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_show_answer_stats_by_user.json` & `simeon-0.0.9/simeon/upload/schemas/schema_show_answer_stats_by_user.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_staff.json` & `simeon-0.0.9/simeon/upload/schemas/schema_staff.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_studentmodule.json` & `simeon-0.0.9/simeon/upload/schemas/schema_studentmodule.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_time_on_asset_daily.json` & `simeon-0.0.9/simeon/upload/schemas/schema_time_on_asset_daily.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_time_on_asset_totals.json` & `simeon-0.0.9/simeon/upload/schemas/schema_time_on_asset_totals.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_time_on_task.json` & `simeon-0.0.9/simeon/upload/schemas/schema_time_on_task.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_time_on_task_totals.json` & `simeon-0.0.9/simeon/upload/schemas/schema_time_on_task_totals.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_tracking_log.json` & `simeon-0.0.9/simeon/upload/schemas/schema_tracking_log.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_user_info_combo.json` & `simeon-0.0.9/simeon/upload/schemas/schema_user_info_combo.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_user_partitions.json` & `simeon-0.0.9/simeon/upload/schemas/schema_user_partitions.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_video_axis.json` & `simeon-0.0.9/simeon/upload/schemas/schema_video_axis.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_video_stats_day.json` & `simeon-0.0.9/simeon/upload/schemas/schema_video_stats_day.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schema_youtube.json` & `simeon-0.0.9/simeon/upload/schemas/schema_youtube.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/schemas/schemas.json` & `simeon-0.0.9/simeon/upload/schemas/schemas.json`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon/upload/utilities.py` & `simeon-0.0.9/simeon/upload/utilities.py`

 * *Files identical despite different names*

### Comparing `simeon-0.0.8/simeon.egg-info/PKG-INFO` & `simeon-0.0.9/simeon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simeon
-Version: 0.0.8
+Version: 0.0.9
 Summary: A CLI tool to help process research data from edX
 Home-page: https://github.com/MIT-IR/simeon
 Author: MIT Institutional Research
 Author-email: irx@mit.edu
 License: MIT LICENSE
 Keywords: edx research data,mitx,edx,MOOC,education,online learning
 Platform: UNKNOWN
```

### Comparing `simeon-0.0.8/simeon.egg-info/SOURCES.txt` & `simeon-0.0.9/simeon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

