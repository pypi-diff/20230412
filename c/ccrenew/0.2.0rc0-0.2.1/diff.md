# Comparing `tmp/ccrenew-0.2.0rc0.tar.gz` & `tmp/ccrenew-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccrenew-0.2.0rc0.tar", last modified: Fri Feb 24 21:40:21 2023, max compression
+gzip compressed data, was "ccrenew-0.2.1.tar", last modified: Wed Apr 12 16:26:02 2023, max compression
```

## Comparing `ccrenew-0.2.0rc0.tar` & `ccrenew-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-02-24 21:40:21.324762 ccrenew-0.2.0rc0/
--rw-rw-rw-   0        0        0     1100 2022-11-09 21:01:48.000000 ccrenew-0.2.0rc0/LICENSE
--rw-rw-rw-   0        0        0      352 2023-02-24 21:40:21.323762 ccrenew-0.2.0rc0/PKG-INFO
--rw-rw-rw-   0        0        0      615 2022-11-11 15:45:04.000000 ccrenew-0.2.0rc0/README.md
--rw-rw-rw-   0        0        0       42 2023-02-24 21:40:21.324762 ccrenew-0.2.0rc0/setup.cfg
--rw-rw-rw-   0        0        0      437 2023-02-14 20:58:01.000000 ccrenew-0.2.0rc0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-24 21:40:21.238181 ccrenew-0.2.0rc0/src/
-drwxrwxrwx   0        0        0        0 2023-02-24 21:40:21.255404 ccrenew-0.2.0rc0/src/ccrenew/
--rw-rw-rw-   0        0        0       85 2023-02-24 21:40:15.000000 ccrenew-0.2.0rc0/src/ccrenew/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 21:40:21.289405 ccrenew-0.2.0rc0/src/ccrenew/dashboard/
--rw-rw-rw-   0        0        0     1530 2023-02-14 20:58:01.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 21:40:21.313403 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/
--rw-rw-rw-   0        0        0     5137 2022-10-18 20:46:55.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/BV_pp_deg.py
--rw-rw-rw-   0        0        0    11591 2023-02-22 12:26:14.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Bluesky_weather_fucntions_v01.py
--rw-rw-rw-   0        0        0     7163 2023-02-14 20:58:01.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/CCR.py
--rw-rw-rw-   0        0        0    18123 2023-02-14 20:58:01.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_IS6.py
--rw-rw-rw-   0        0        0    15404 2022-12-01 19:51:33.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_smartercheck.py
--rw-rw-rw-   0        0        0    15151 2022-12-01 19:51:33.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Correct_POI_data_v01.py
--rw-rw-rw-   0        0        0    12986 2022-11-08 16:31:40.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Performance_Guarantees_v01.py
--rw-rw-rw-   0        0        0    18698 2023-01-18 18:36:56.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Plant_Availability_v16_bbsc.py
--rw-rw-rw-   0        0        0    15852 2023-01-18 18:36:56.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Rate_Structure_Python_with_DST_v07.py
--rw-rw-rw-   0        0        0     4249 2022-10-27 19:54:24.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Table_by_Rate_Schedule_v01.py
--rw-rw-rw-   0        0        0        0 2022-10-27 20:52:08.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/__init__.py
--rw-rw-rw-   0        0        0     6493 2023-02-14 20:58:01.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/batch_process.py
--rw-rw-rw-   0        0        0     8666 2022-10-27 19:55:09.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/battery_deg.py
--rw-rw-rw-   0        0        0     7749 2023-02-23 13:34:02.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/data_determination.py
--rw-rw-rw-   0        0        0     6078 2022-12-12 13:52:10.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/snow_loss_functions_v3.py
--rw-rw-rw-   0        0        0     4286 2023-02-14 20:58:01.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/solcats_API.py
--rw-rw-rw-   0        0        0    11006 2022-10-27 19:54:38.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/weather_adjusted_functions_v03.py
-drwxrwxrwx   0        0        0        0 2023-02-24 21:40:21.316404 ccrenew-0.2.0rc0/src/ccrenew/dashboard/plotting/
--rw-rw-rw-   0        0        0        0 2022-10-27 20:51:43.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/plotting/__init__.py
--rw-rw-rw-   0        0        0    52557 2023-02-24 21:36:35.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/plotting/plots.py
--rw-rw-rw-   0        0        0   161779 2023-02-24 16:20:52.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/project.py
--rw-rw-rw-   0        0        0    61131 2023-02-21 19:44:23.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/session.py
-drwxrwxrwx   0        0        0        0 2023-02-24 21:40:21.322758 ccrenew-0.2.0rc0/src/ccrenew/dashboard/utils/
--rw-rw-rw-   0        0        0        0 2022-10-27 20:52:31.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/utils/__init__.py
--rw-rw-rw-   0        0        0    10749 2023-02-14 20:58:01.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/utils/dashboard_utils.py
--rw-rw-rw-   0        0        0     1623 2023-02-01 16:17:23.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/utils/df_tools.py
--rw-rw-rw-   0        0        0     1265 2022-09-22 19:52:54.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/utils/logging_conf.py
--rw-rw-rw-   0        0        0     7074 2023-02-15 16:56:05.000000 ccrenew-0.2.0rc0/src/ccrenew/dashboard/utils/project_neighbors.py
-drwxrwxrwx   0        0        0        0 2023-02-24 21:40:21.285402 ccrenew-0.2.0rc0/src/ccrenew.egg-info/
--rw-rw-rw-   0        0        0      352 2023-02-24 21:40:21.000000 ccrenew-0.2.0rc0/src/ccrenew.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1655 2023-02-24 21:40:21.000000 ccrenew-0.2.0rc0/src/ccrenew.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-24 21:40:21.000000 ccrenew-0.2.0rc0/src/ccrenew.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-02-24 21:40:21.000000 ccrenew-0.2.0rc0/src/ccrenew.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.681366 ccrenew-0.2.1/
+-rw-rw-rw-   0        0        0     1100 2022-11-09 21:01:48.000000 ccrenew-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      349 2023-04-12 16:26:02.680365 ccrenew-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2022-11-11 15:45:04.000000 ccrenew-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 16:26:02.681366 ccrenew-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      437 2023-02-14 20:58:01.000000 ccrenew-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.610365 ccrenew-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.629367 ccrenew-0.2.1/src/ccrenew/
+-rw-rw-rw-   0        0        0     1120 2023-04-12 16:25:08.000000 ccrenew-0.2.1/src/ccrenew/__init__.py
+-rw-rw-rw-   0        0        0     6869 2023-03-30 20:00:56.000000 ccrenew-0.2.1/src/ccrenew/ccr.py
+-rw-rw-rw-   0        0        0     8021 2023-04-05 21:36:13.000000 ccrenew-0.2.1/src/ccrenew/cloud_data.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.648368 ccrenew-0.2.1/src/ccrenew/dashboard/
+-rw-rw-rw-   0        0        0     2463 2023-03-30 18:52:35.000000 ccrenew-0.2.1/src/ccrenew/dashboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.667365 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/
+-rw-rw-rw-   0        0        0     1783 2023-03-30 17:14:14.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/BV_pp_deg.py
+-rw-rw-rw-   0        0        0    18089 2023-03-17 12:55:19.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_IS6.py
+-rw-rw-rw-   0        0        0    15346 2023-03-17 13:06:23.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_smartercheck.py
+-rw-rw-rw-   0        0        0    15095 2023-03-17 13:06:04.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Correct_POI_data_v01.py
+-rw-rw-rw-   0        0        0    13086 2023-03-30 17:22:42.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Performance_Guarantees_v01.py
+-rw-rw-rw-   0        0        0    18643 2023-04-11 19:13:49.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Plant_Availability_v16_bbsc.py
+-rw-rw-rw-   0        0        0    16011 2023-03-30 17:25:57.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Rate_Structure_Python_with_DST_v07.py
+-rw-rw-rw-   0        0        0     4195 2023-03-17 13:10:53.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Table_by_Rate_Schedule_v01.py
+-rw-rw-rw-   0        0        0        0 2022-10-27 20:52:08.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-03-13 14:27:41.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/_project_processing.py
+-rw-rw-rw-   0        0        0     6645 2023-03-31 19:10:24.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/batch_process.py
+-rw-rw-rw-   0        0        0     8608 2023-03-17 13:08:51.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/battery_deg.py
+-rw-rw-rw-   0        0        0     6026 2023-03-17 13:11:08.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/snow_loss_functions_v3.py
+-rw-rw-rw-   0        0        0     3668 2023-03-16 14:56:45.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/solcats_API.py
+-rw-rw-rw-   0        0        0    10948 2023-03-17 13:13:01.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/weather_adjusted_functions_v03.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.669366 ccrenew-0.2.1/src/ccrenew/dashboard/plotting/
+-rw-rw-rw-   0        0        0        0 2022-10-27 20:51:43.000000 ccrenew-0.2.1/src/ccrenew/dashboard/plotting/__init__.py
+-rw-rw-rw-   0        0        0    60141 2023-04-12 12:56:15.000000 ccrenew-0.2.1/src/ccrenew/dashboard/plotting/plots.py
+-rw-rw-rw-   0        0        0   176836 2023-04-11 21:18:09.000000 ccrenew-0.2.1/src/ccrenew/dashboard/project.py
+-rw-rw-rw-   0        0        0    65313 2023-04-11 18:39:34.000000 ccrenew-0.2.1/src/ccrenew/dashboard/session.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.676380 ccrenew-0.2.1/src/ccrenew/dashboard/utils/
+-rw-rw-rw-   0        0        0        0 2022-10-27 20:52:31.000000 ccrenew-0.2.1/src/ccrenew/dashboard/utils/__init__.py
+-rw-rw-rw-   0        0        0     5468 2023-03-30 17:24:26.000000 ccrenew-0.2.1/src/ccrenew/dashboard/utils/dashboard_utils.py
+-rw-rw-rw-   0        0        0     1623 2023-02-01 16:17:23.000000 ccrenew-0.2.1/src/ccrenew/dashboard/utils/df_tools.py
+-rw-rw-rw-   0        0        0     1265 2022-09-22 19:52:54.000000 ccrenew-0.2.1/src/ccrenew/dashboard/utils/logging_conf.py
+-rw-rw-rw-   0        0        0     7281 2023-03-16 14:57:33.000000 ccrenew-0.2.1/src/ccrenew/dashboard/utils/project_neighbors.py
+-rw-rw-rw-   0        0        0    12778 2023-04-11 17:07:28.000000 ccrenew-0.2.1/src/ccrenew/data_determination.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.679366 ccrenew-0.2.1/src/ccrenew/pvmodel/
+-rw-rw-rw-   0        0        0       54 2023-03-09 21:59:00.000000 ccrenew-0.2.1/src/ccrenew/pvmodel/__init__.py
+-rw-rw-rw-   0        0        0    11379 2023-04-12 15:52:36.000000 ccrenew-0.2.1/src/ccrenew/pvmodel/project_model.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.644366 ccrenew-0.2.1/src/ccrenew.egg-info/
+-rw-rw-rw-   0        0        0      349 2023-04-12 16:26:02.000000 ccrenew-0.2.1/src/ccrenew.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1688 2023-04-12 16:26:02.000000 ccrenew-0.2.1/src/ccrenew.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 16:26:02.000000 ccrenew-0.2.1/src/ccrenew.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-12 16:26:02.000000 ccrenew-0.2.1/src/ccrenew.egg-info/top_level.txt
```

### Comparing `ccrenew-0.2.0rc0/LICENSE` & `ccrenew-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.0rc0/README.md` & `ccrenew-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/CCR.py` & `ccrenew-0.2.1/src/ccrenew/ccr.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,15 @@
 
 import numpy as np
 import os
 import pandas as pd
 import re
 import smartsheet
 from sqlalchemy import create_engine
-from time import time
 
-"""
-Imports above docstring to exclude from Sphinx AutoAPI
-Created on Wed Aug 16 09:38:55 2017
-
-@author: Kevin Anderson
-"""
 
 username = os.path.split(os.path.expanduser("~"))[1]
 if username == 'Kevin Anderson':
     # back in my day, C drives were good enough for anyone
     file_project = os.path.join(r'C:\Users', username, r'Box Sync\Cypress Creek Renewables\Asset Management\8) Production Data\_Dashboard_Project')
 elif username == 'blumenthal':
     file_project = r'C:\Users\blumenthal\Cypress Creek Renewables\AM-Performance - _Dashboard_Project'
@@ -30,15 +23,14 @@
     file_project = r'C:\Users\MartinWaters\Box Sync\Cypress Creek Renewables\Asset Management\8) Production Data\_Dashboard_Project'
     
 elif username == 'EricFitch':
     # RIP
     file_project = r'C:\Users\EricFitch\Box Sync\Cypress Creek Renewables\Asset Management\8) Production Data\_Dashboard_Project'
     
 elif username == 'ChristopherDowns':
-    #file_project = r'D:\Cypress Creek Renewables\AM-Performance - Documents\_Dashboard_Project'
     file_project=r'C:\Users\ChristopherDowns\Cypress Creek Renewables\AM-Performance - Documents\_Dashboard_Project'
     
 elif username == 'PerfEng':
     file_project = r'C:\Users\PerfEng\Cypress Creek Renewables\AM-Performance - Documents\_Dashboard_Project'
     
 elif username == 'corey.pullium':
     file_project = r'C:\Users\corey.pullium\Cypress Creek Renewables\AM-Performance - Documents\_Dashboard_Project'
@@ -57,28 +49,26 @@
 
 elif username == 'LukeSain':
     file_project = r'C:\Users\LukeSain\OneDrive - Cypress Creek Renewables\Documents - AM-Performance\_Dashboard_Project'
 
 elif username == 'AndrewCurthoys':
     file_project = r'C:\Users\AndrewCurthoys\Cypress Creek Renewables\AM-Performance - Documents\_Dashboard_Project'
 
-
 else:
     # saurabh because he likes the D drive better. 
     # Wait...why do I have to be the 'else'. I demand to be the 'if'
     # dude you put yourself there, idk what you're complaining about
     # malarky! there is a plot against me. and I don't mean one of the dashboard variety.
     # typical asset-management performance engineer, playing the victim when he tilted the POA himself
     # RIP
     file_project = r'D:\Box Sync\Cypress Creek Renewables\Asset Management\8) Production Data\_Dashboard_Project'
 
 file_production_data = os.path.split(file_project)[0]
     
 def get_sql_engine():
-
     sql_username = os.environ['BARTERTOWN_USERNAME']
     sql_password = os.environ['BARTERTOWN_PASSWORD']
     encoding_dict = {
         ':': '%3A',
         '/': '%2F',
         '?': '%3F',
         '#': '%23',
@@ -108,19 +98,15 @@
     
     url = 'postgresql+psycopg2://{}:{}@{}:{}/{}'
     url = url.format(sql_username, sql_password, host, port, db)
     
     engine = create_engine(url,pool_pre_ping=True)
     return engine
 
-
 def get_ss_as_df(sheet_id, drop_col_1=True, start_col=None, index_col=None):
-    # helper function to query the data in a SS and put it into a dataframe
-    start = time()
-
     # API_TOKEN is user-specific, so SS will block you from accessing 
     # sheets that you don't have permissions for
     API_TOKEN = os.environ['SMARTSHEET_TOKEN']
 
     # Initialize API client
     ss_client = smartsheet.Smartsheet(API_TOKEN)
 
@@ -139,16 +125,16 @@
     elif isinstance(index_col, str):
         for col in cols.result:
             if col.title == index_col:
                 index_col_id, index_colname = col.id, col.title
 
     # Add index column to the col list if present
     try:
-        col_ids = (index_col_id,) + col_ids
-        colnames = (index_colname,) + colnames
+        col_ids = (index_col_id,) + col_ids # type: ignore
+        colnames = (index_colname,) + colnames # type: ignore
     except NameError:
         pass
         
     # Get sheet
     sheet = ss_client.Sheets.get_sheet(sheet_id, column_ids=list(col_ids))
     
     # extract out the cell values into a df
@@ -160,30 +146,29 @@
     # Fill empty values with np.nan
     df = df.fillna(np.nan)
     
     # df has the data, but the column names are just numbers
     df.columns = list(colnames)
 
     # bring the index over
-    df.index = range(len(df))
+    df.index = range(len(df)) # type: ignore
     if drop_col_1:
         del df['Column1']
     
     # Set index if provided
     if index_col:
-        df = df.set_index(index_colname)
+        df = df.set_index(index_colname) # type: ignore
 
     return df
 
-
 def get_df_keys(retired=False):
     # df_keys SS ID
     sheet_id = '8659171076794244'
     all_df_keys = get_ss_as_df(sheet_id)
-    all_df_keys.index = all_df_keys['Project']
+    all_df_keys = all_df_keys.set_index('Project')
     for col in ['PIS', 'FC']:
         all_df_keys[col] = pd.to_datetime(all_df_keys[col])
         
     if not retired:
         df_keys = all_df_keys.loc[all_df_keys['Retired'] != True, :]
     else:
         df_keys = all_df_keys
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_IS6.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_IS6.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,8 @@
 # -*- coding: utf-8 -*-
-
-import pandas as pd
-import numpy as np
-import datetime as dt
-import os
-
 """
 Imports above docstring to exclude from Sphinx AutoAPI
 Created on Wed Sep 28 15:45:14 2016
 
 @author: SEBASTIAN
 
 
@@ -16,14 +10,18 @@
 There is a case that some meters are off, but inverters are on.  When the meter is back
 online there is an increment in energy. 
 Code corrects this issue.
 
 See Boseman Solar Center  month: MARCH
 """
 
+import pandas as pd
+import numpy as np
+
+
 def list_pairs(lis):
     #find pairs that are at least 2 hours in duration
     beg = []
     end = []
     
     start_time = 0
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_smartercheck.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_smartercheck.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # -*- coding: utf-8 -*-
-
-import pandas as pd
-import numpy as np
-
 """
-Imports above docstring to exclude from Sphinx AutoAPI
 Created on Wed Sep 28 15:45:14 2016
 
 @author: SEBASTIAN
 
 
 Code to correct meter data.  Meter data is calculated as a sum of different meters.
 There is a case that some meters are off, but inverters are on.  When the meter is back
 online there is an increment in energy. 
 Code corrects this issue.
 
 See Boseman Solar Center  month: MARCH
 """
 
+import pandas as pd
+import numpy as np
+
 
 def list_pairs(lis):
     #find pairs that are at least 2 hours in duration
     beg = []
     end = []
     
     start_time = 0
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Correct_POI_data_v01.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Correct_POI_data_v01.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # -*- coding: utf-8 -*-
 
-import pandas as pd
-import numpy as np
-
 """
-Imports above docstring to exclude from Sphinx AutoAPI
 Created on 12/12/17
 
 -v1: normal meter correction at POI based on PVsyst data
 
 
 @author: RB + KA
 """
 
+import pandas as pd
+import numpy as np
+
 def list_pairs(lis):
     #find pairs that are at least 2 hours in duration
     beg = []
     end = []
     
     start_time = 0
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Performance_Guarantees_v01.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Performance_Guarantees_v01.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 
+"""
+Created on Wed Apr 12 15:00:08 2017
+
+@author: Kevin Anderson
+"""
+
 import pandas as pd
 import numpy as np
 import datetime as datetime
 import os
+from pathlib import Path
 
-from ccrenew.dashboard import ccr
+from ccrenew import ccr
 file_project = ccr.file_project
 
-"""
-Imports above docstring to exclude from Sphinx AutoAPI
-Created on Wed Apr 12 15:00:08 2017
-
-@author: Kevin Anderson
-"""
 
 def USB1_performance_guarantee(df, length, df_Pvsyst, PIS_date, guarantee_input, df_perf):
     if PIS_date.month != 12 or PIS_date.year != 2014:
         raise RuntimeError("Guarantee assumptions not met")
     n_years = df.index[-1].year - 2015
     
     # calculate how much each month contributes to yearly POA
@@ -193,19 +194,24 @@
     df_perf['Guar_freq'] = 'Monthly'
     df_perf['Gaur_range'] = ['{} - {}'.format(s.strftime('%m/%d'), e.strftime('%m/%d')) for s,e in zip(month_start, result.index.tolist())]
     
     return df_perf, result.tolist()
 
 
 #added by SPA on 11/28/18
-def SCEG_performance_guarantee(project_name, df, df_Pvsyst, PIS_date, df_perf):    
+def SCEG_performance_guarantee(project_name, df, df_Pvsyst, PIS_date, df_perf, data_platform):    
     
     #read in Net Energy and REC Delivery Requirements - One large Excel file for all the SCEG sites taking different tabs
     #df_attachement = pd.read_excel(r'D:\Box Sync\Cypress Creek Renewables\Asset Management\8) Production Data\_Dashboard_Project\Python_Functions\Other Scripts\Testing - SCEG Performance Guarantees\SCEG_Perf Gaur_Contract_Quantity.xlsx', sheet_name=project_name) #NEED TO PUT THIS EXCEL FILE IN CENTRAL LOCATION AND RENAME
-    df_attachement = pd.read_excel(os.path.join(file_project, 'Python_Functions\Other Scripts\Performance Guarantee Inputs\SCEG\SCEG_Perf Gaur_Contract_Quantity.xlsx'), sheet_name=project_name) #NEED TO PUT THIS EXCEL FILE IN CENTRAL LOCATION AND RENAME
+        
+    filepath = Path(file_project) / 'Python_Functions\Other Scripts\Performance Guarantee Inputs\SCEG\SCEG_Perf Gaur_Contract_Quantity.xlsx'
+    if data_platform == 's3':
+        filepath = filepath.as_posix().replace('s3:/', 's3://')
+
+    df_attachment = pd.read_excel(filepath, sheet_name=project_name) #NEED TO PUT THIS EXCEL FILE IN CENTRAL LOCATION AND RENAME
 
     #get start year to test if we are in year 2 or not
     perf_guar_start_year = PIS_date.year
     
     #determine reporting year 
     reporting_year = df.index.year[-1]    
 
@@ -222,15 +228,15 @@
         monthly_fractions = df['POA_avg'].resample("M").count() / df_Pvsyst['POA (W/m2)'].resample("M").count()
         monthly_fractions = monthly_fractions.fillna(0)
         proration = (monthly_weights * monthly_fractions).sum()
         ########################################################################################################
 
         #get contract_year and performance guarentee value
         contract_year = (reporting_year - perf_guar_start_year) + 1 #note the +1 as year 0 is actually contract year 1, so adding 1.
-        net_energy = df_attachement.loc[df_attachement['Contract Year']==contract_year, 'Net Energy (kWh)'].item()
+        net_energy = df_attachment.loc[df_attachment['Contract Year']==contract_year, 'Net Energy (kWh)'].item()
 
         #find out lost kWh due to grid outages TO subtract out of the Net Energy value which we compare on
         #   contract states 'provided that the Contract Quantity for Net Energy shall be reduced on an equitable basisa 
         grid_loss = df['Meter_&_ava_&_grid'].sum() - df['Meter_&_ava'].sum()
         
         #subtract grid loss from net_energy given contractual language, then with that value, derive the 85% target value
         net_energy_adj = net_energy - grid_loss
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Plant_Availability_v16_bbsc.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Plant_Availability_v16_bbsc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # -*- coding: utf-8 -*-
-
-import pandas as pd
-import numpy as np
-
 """
-Imports above docstring to exclude from Sphinx AutoAPI
 Created on Thu Jul 28 16:08:53 2016
 
 @author: SEBASTIAN
 
 LOG:
 
 1) 2016-09-25  Inverter Cum Meter.  See Boseman, month of August.  
         Meter gets corrected with Inverter data, but needs cum meter
 """
 
+import pandas as pd
+import numpy as np
+
+
 def calculate_inverter_availability_and_loss(df , df_Pvsyst, P_exp): 
     #
     table_P = pd.pivot_table(df_Pvsyst, values = 'Year 0 Actual Production (kWh)', index =['Month'], columns ='Hour', aggfunc = np.mean)
 
     #  Find position of Inverter data        
     pos_Inv = [s for s in df.columns if 'Inv_kw_' in s]
     n_inv = len(pos_Inv)
     #    
     pos_Meter = [s for s in df.columns if 'Meter_kw_' in s]
-    pos_Meter_cum = [s for s in df.columns if 'Meter_kwnet' in s]
+    pos_Meter_cum = [s for s in df.columns if 'Meter_kwhnet' in s]
     #
     ava = pd.DataFrame()
     ava[pos_Meter + pos_Meter_cum + pos_Inv] = df[pos_Meter + pos_Meter_cum + pos_Inv]
     #  Inveter cum meter   
     
     pos_Inv_cum = [s for s in df.columns if 'Inv_kwnet' in s]
     ava[pos_Inv_cum] = df[pos_Inv_cum]
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Rate_Structure_Python_with_DST_v07.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Rate_Structure_Python_with_DST_v07.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 # -*- coding: utf-8 -*-
 
-import pandas as pd
-
-import numpy as np
-import datetime as dt
-import os
-from holidays import UnitedStates
-import calendar
-
 """
-Imports above docstring to exclude from Sphinx AutoAPI
 Created on Wed Jun 22 14:16:25 2016
 
 @author: SEBASTIAN
 
 Change log:
 
 - 2016/07/24 -> Added code to make sure that days 1/1 , 7/4 and 12/25 are holidays.  
 - 2017/07/01 -> Fixed DST not working. DST start and end were read from config instead of being calculated
 - 2017/07/13 -> Speed up code to run on peak hours for energy and capacity. 
 - 2017/08/09 -> Add line-loss adjustment
 TODO: read holiday list from config file
 
 """
 
-from pandas.tseries.holiday import AbstractHolidayCalendar, Holiday, nearest_workday, \
-    USMartinLutherKingJr, USPresidentsDay, GoodFriday, USMemorialDay, \
-    USLaborDay, USThanksgivingDay, TH, FR, SA, next_monday
+import calendar
+import datetime as dt
+from holidays import UnitedStates
+import numpy as np
+import os
+import pandas as pd
+from pathlib import Path
+
+
+from pandas.tseries.holiday import (
+    AbstractHolidayCalendar,
+    Holiday,
+    nearest_workday,
+    USMartinLutherKingJr,
+    USPresidentsDay,
+    GoodFriday,
+    USMemorialDay,
+    USLaborDay,
+    USThanksgivingDay,
+    TH,
+    FR,
+    SA,
+    next_monday
+)
 
 class USTradingCalendar(AbstractHolidayCalendar):
     rules = [
         Holiday('NewYearsDay', month=1, day=1, observance=nearest_workday),
         #USMartinLutherKingJr,
         #USPresidentsDay,
         GoodFriday,
@@ -137,15 +149,15 @@
     
     aux = pd.DataFrame(np.zeros([len(df),len(filler)]), index = df.index, columns = filler)
     
     export = pd.concat([aux,df], axis = 1)
     
     return export
 
-def generate_Rate_column (project_name, file_input, shift_DST, year):
+def generate_Rate_column (project_name, file_input, shift_DST, year, data_platform):
 
     def generate_rate(df_t1, df_t2, normal_rate_flag, year, shift_DST):
         #  Create DataFrame with Columns of Interest
         #
         #   Read all variables defined on Table 1
         #
         # year =  df_t1[df_t1['Name'] == 'Current Year']['Value'].values[0]
@@ -335,17 +347,22 @@
         df_t2 = pd.read_excel(file_input, sheet_name = 'Table_2', index_col=0).fillna(0)
         normal_rate_flag = True
     except:
         #rate calc not in config file, redirect to yearly rates file
         normal_rate_flag = False
 
         #read new file - only use specific year's worth of data
-        path, config = os.path.split(file_input)
-        read_file = os.path.join(path, project_name + '_YearlyRates.csv')
-        df = pd.read_csv(read_file, index_col = 'IND', usecols= ['IND', np.str(year)])
+        filedir = Path(file_input).parent
+        filename = project_name + '_YearlyRates.csv'
+        filepath = filedir / filename
+
+        if data_platform == 's3':
+            filepath = filepath.as_posix().replace('s3:/', 's3://')
+
+        df = pd.read_csv(filepath, index_col = 'IND', usecols= ['IND', np.str(year)])
 
         if not shift_DST:
             df_1 = yearly8760(df.copy(), project_name, year, shift_DST=True)
             df_2 = yearly8760(df.copy(), project_name, year, shift_DST=False)
 
             return df_1, normal_rate_flag, df_2, normal_rate_flag
         else:
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/Table_by_Rate_Schedule_v01.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Table_by_Rate_Schedule_v01.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 
-import pandas as pd
-import numpy as np
-
 """
-Imports above docstring to exclude from Sphinx AutoAPI
 Created on Fri Jul 29 09:34:27 2016
 
 @author: SEBASTIAN
 """
 
+import pandas as pd
+import numpy as np
+
+
 def generate_table_variable_by_rev_schedule(rates_year_i, df_h, var_t,df_Pvsyst_2, var_pvsyst, df_config, df_month_2, df_Pvsyst_2_month):
     df_aux = pd.DataFrame()
     df_aux['rates'] = rates_year_i
     df_aux['month'] = df_aux.index.month
     df_aux[var_t] = df_h[var_t]
     table = pd.pivot_table(df_aux,  columns = 'rates', index=['month'], aggfunc=np.sum).fillna(0)
     #
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/batch_process.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/batch_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from concurrent.futures import (
     as_completed,
     ProcessPoolExecutor)
 from functools import partial
 import os
 import time
+import traceback
 
 
 def process_pool(kwargslist):
 
     # We'll use half of the available processors for the machine to not completely bog it down.
     max_workers = int(os.cpu_count()/2)
 
@@ -43,23 +44,25 @@
     project_start = time.time()
 
     # Collect kwargs
     session = kwargs.get('session')
     data_source = kwargs.get('data_source')
     project_name = kwargs.get('project_name')
     reprocess = kwargs.get('reprocess')
+    data_sub = kwargs.get('data_sub')
+    use_solcast = kwargs.get('use_solcast')
     project_num = kwargs.get('project_num')
     project_total = kwargs.get('project_total')
     batch_start = kwargs.get('batch_start')
 
     # Initialize new session
     session = session(data_source=data_source)
 
     # Process project
-    project = session.process_project(project_name=project_name, reprocess=reprocess)
+    project = session.process_project(project_name=project_name, reprocess=reprocess, data_sub=data_sub, use_solcast=use_solcast)
     project_time = time.time()-project_start
     batch_time = time.time()-batch_start
 
     # Return dict for parsing the results
     return {'project_list': session.project_list.items(),
             'project_name': project_name,
             'project_num': project_num,
@@ -120,16 +123,16 @@
     # Initialize new session
     session = session(data_source=data_source)
 
     # Process project
     error_info = ''
     try:
         session.export_project(project_name=project_name, **func_args)
-    except Exception as e:
-        error_info = e
+    except:
+        error_info = traceback.format_exc()
 
     project_time = time.time()-project_start
     batch_time = time.time()-batch_start
 
     # Return dict for parsing the results
     return {'project_list': session.project_list.items(),
             'project_name': project_name,
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/battery_deg.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/battery_deg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #!/usr/bin/env python
 
+"""
+API for modelling solar+storage dispatch over shorter timer periods.
+"""
+
 __author__ = "Allen Lawrence"
 __credits__ = "Brian Knowles", "Michael Baker"
 __version__ = "0.1.0"
 __maintainer__ = "Allen Lawrence"
 __email__ = "allen.lawrence@ccrenew.com"
 __status__ = "Development"
 
 
-"""
-Imports above docstring to exclude from Sphinx AutoAPI
-API for modelling solar+storage dispatch over shorter timer periods.
-"""
-
-
 import numpy as np
 
 ### BINARY LOGIC ###
 def binDischarge(cue, batt_power, soc, inp, lim, discharge_eff):
     """
     Calculates battery discharge for a single time step.
     Adapted from Brian Knowles's (CCR) battery model.
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/snow_loss_functions_v3.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/snow_loss_functions_v3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # -*- coding: utf-8 -*-
+
+"""
+Created on Fri May 26 11:43:57 2017
+
+-v3: adding conditions around interp. If outside the mesh, return nan and use nearest reporting site data
+
+@author: BLUMENTHAL
+"""
+
 import pandas as pd
 import numpy as np
 import scipy.interpolate
 import datetime
 import math
 import s3fs
 import shapely.geometry as gs
 
 from ccrenew.dashboard.utils.project_neighbors import haversine
 
-"""
-Imports above docstring to exclude from Sphinx AutoAPI
-Created on Fri May 26 11:43:57 2017
-
--v3: adding conditions around interp. If outside the mesh, return nan and use nearest reporting site data
-
-@author: BLUMENTHAL
-"""
 
 def timeseries(raw_snow_df, project_df_index, project_lat, project_lon):
 
     X, Y = np.meshgrid([project_lon],[project_lat])
     df = raw_snow_df.copy()
     
     #Z = []
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/solcats_API.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/solcats_API.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,31 +2,22 @@
 """
 Created on Mon Dec 13 15:25:27 2021
 
 @author: Chris Downs
 """
 
 import boto3
+from io import StringIO
 from multiprocessing.pool import ThreadPool
-from numpy import *
+import os
 import pandas as pd
 import requests
 import s3fs
 
-from ccrenew.dashboard import (
-    ccr,
-    all_df_keys
-)
-
-
-# Python 2 compatibility
-try:
-    from StringIO import StringIO
-except ImportError:
-    from io import StringIO
+from ccrenew import all_df_keys
 
 
 s3_config = boto3.client('s3')
 bucket = 'perfdatadev.ccrenew.com'
 bucket_prefix_satellite = "5min_archive/Solcats/"
 bucket_prefix_measured = "5min_archive/PF/"
 
@@ -38,15 +29,14 @@
 def make_satellite_key(CCR_ID, date):
     return bucket_prefix_satellite + CCR_ID + "/" + "sat_weather_" + date.strftime('%Y-%m-%d') + ".csv"
 
 def make_measured_key(CCR_ID, date):
     return bucket_prefix_measured + CCR_ID + "/" + "main_" + date.strftime('%Y-%m-%d') + ".csv"
 
 def retrieve_df(key):
-    
     fs = s3fs.S3FileSystem(anon=False)
     path = "s3://{b}/{k}".format(b=bucket, k=key)
     try:
         with fs.open(path, 'rb') as f:
             df = pd.read_csv(f, index_col = 0, parse_dates = True)
             df = df.loc[~df.index.duplicated(), :]
     except FileNotFoundError:
@@ -57,31 +47,27 @@
     fileobj = StringIO()
     df.to_csv(fileobj)
     fileobj.seek(0)
     s3_config.upload_fileobj(fileobj, bucket, s3_key)
 
 def get_cat_files(site):
     s3=boto3.resource('s3')
-    mybucket=s3.Bucket(bucket)
-    lis1=[]
+    mybucket=s3.Bucket(bucket) # type: ignore
+    files = []
     for cat_file in mybucket.objects.filter(Delimiter='/', Prefix=(bucket_prefix_satellite +'{}/'.format(site))):
-        lis1.append((cat_file.key))
-    #print lis1
-    return lis1
+        files.append((cat_file.key))
+
+    return files
 
 def get_solcats(site): #yes solCATS. because typos that last forever are funny
     
-    PRIMARY_KEY = "Q771UVOj2Px5w9F6k3A6PGY6WVd58jjI"
-
-    #API_URL2 = "https://api.solcast.com.au/world_radiation/estimated_actuals?latitude=-33.86882&longitude=151.209295&hours=168"
-    #new API =  "https://api.solcast.com.au/data/live/radiation_and_weather?latitude=-33.86882&longitude=151.209295&format=json"
-    API_URL="https://api.solcast.com.au/"
+    PRIMARY_KEY = os.environ['SOLCAST_PRIMARY_KEY']
+    API_URL = "https://api.solcast.com.au/"
     
     hours=168
-    #print 'Sunshine and Lollipops' 
     if site == 'NC-000166':
         lat=df_keys.GPS_Lat.loc[df_keys.CCR_ID==site][0]
         lon=df_keys.GPS_Long.loc[df_keys.CCR_ID==site][0]
         tz='US/'+str(df_keys.Timezone.loc[df_keys.CCR_ID==site][0])
     else:
         lat=df_keys.GPS_Lat.loc[df_keys.CCR_ID==site].item()
         lon=df_keys.GPS_Long.loc[df_keys.CCR_ID==site].item()
@@ -91,27 +77,24 @@
     lat_url='&latitude={}'.format(lat)
     long_url='&longitude={}'.format(lon)
     hour_url='&hours={}'.format(hours)
     format_url='&format=json'
     period_url='&period=PT5M'
     params_url='&output_parameters=air_temp,clearsky_dhi,clearsky_dni,clearsky_ghi,cloud_opacity,dhi,dni,ghi,precipitable_water,precipitation_rate,snow_water,wind_speed_10m'
     
-    #url=API_URL+"world_radiation/estimated_actuals?"+key_url+lat_url+long_url+hour_url+format_url    #OLD URL
     url=API_URL+"data/live/radiation_and_weather?"+key_url+lat_url+long_url+hour_url+format_url+period_url+params_url   #new URL
     response=requests.get(url)
     if response.status_code==200:
         df_cats=pd.DataFrame(response.json()['estimated_actuals'])
     
-    
         #fix the timestamp and make it localized to the site. i.e we want the ghi here to line up exactly with the ghi from PF or AE
         df_cats['time']=df_cats.period_end #period end is solcast's column for the timestamp. I believe it is hour end UTC
         df_cats['time']=pd.to_datetime(df_cats['time'])
-        df_cats.index=df_cats['time']
+        df_cats.set_index(df_cats['time'])
         df_cats.index.name=None
         df_cats=df_cats.sort_index() #actually order the dataframe because the original df is all out of order
         df_cats=df_cats.tz_localize('Etc/GMT').tz_convert(tz).tz_localize(None)#uses gmt+1 to switch from hour end to start
-        #df_cats=df_cats[['cloud_opacity','dhi','dni','ebh','ghi']]
     
         return response.status_code,df_cats
     else:
         return response.status_code,None
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/data_processing/weather_adjusted_functions_v03.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/weather_adjusted_functions_v03.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # -*- coding: utf-8 -*-
-
-import pandas as pd
-import numpy as np
-import statsmodels.api as sm
-
 """
-Imports above docstring to exclude from Sphinx AutoAPI
 Created on Wed Jul 27 08:25:53 2016
 
 @author: SEBASTIAN
 """
 
+import pandas as pd
+import numpy as np
+import statsmodels.api as sm
+
 def generate_Tcell(POA,Tamb,wind_speed, a,b, Delta_Tcnd):
     #  based on NREL formulas.
     Ref_Irrad = 1000.0
     Tmod = Tamb + POA *np.exp( a+ b*wind_speed)
     #Temp_drop = 3.0
     Tcell = Tmod + (POA / Ref_Irrad)*Delta_Tcnd
     return Tcell
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/plotting/plots.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/plotting/plots.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,84 +1,212 @@
 from __future__ import annotations
 
 import calendar
 from collections import namedtuple
+from datetime import (
+    datetime,
+    timedelta)
+from dateutil import parser
+from dateutil.parser import ParserError
 from functools import partial
 import logging
-from numbers import Number
-from os import pathsep
-import numpy as np
 from matplotlib import (
+    lines as mlines,
     patches as mpatches,
     pyplot as plt,
     rcParams)
-from matplotlib.collections import PatchCollection, PolyCollection
+from matplotlib.collections import (
+    PatchCollection,
+    PathCollection
+)
 from matplotlib.figure import Figure
+from matplotlib.legend import Legend
+import os
+import numpy as np
 import pandas as pd
 from PyQt5.QtGui import QGuiApplication
+from typing import TYPE_CHECKING
 import warnings
 
-from ccrenew.dashboard.data_processing.data_determination import daylight
+from ccrenew import Numeric
+from ccrenew.dashboard import daylight
+
+# Conditional import for typechecking
+if TYPE_CHECKING:
+    from ccrenew.dashboard import Project
 
 plt.ion()  # turn on interactive plots
 plt.style.use('ggplot')
 
 # Create logger
 # logger = logging.getLogger(__name__)
 
 # Create namedtuple for storing plots
 Plot = namedtuple('Plot', 'fig ax')
+    
+# Create dict for interactive legend
+legend_type_dict = {mlines.Line2D: 'lines',
+                    mpatches.Rectangle: 'backgrounds',
+                    PathCollection: 'markers'}
 
-def picker(event, fig, path_dict):
+def picker(event, fig, plot_paths):
     # Assign the legend line that was clicked
     legend_icon = event.artist
-    print(f"legend_icon = {legend_icon}")
-    # print(f"path_dict: {path_dict}")
-    
-    # Find the plot line based on the legend line name
-    plot_artist = path_dict[legend_icon][0]
-    print(f"plot_artist: {plot_artist}")
-    path_type = path_dict[legend_icon][1]
-    print(f"path type: {path_type}")
-
-    if path_type != 'background':
-        # Get visibility of the line & swap it
-        visible = plot_artist.get_visible()
-        plot_artist.set_visible(not visible)
-
-        # Make inactive lines mostly transparent in the legend
-        legend_icon.set_alpha(0.2 if visible else 1.0)
-    else:
-        # Loop through all patches & change visibility
-        visible = plot_artist[0].get_visible()
-        for patch in plot_artist:
-            patch.set_visible(not visible)
 
-        # Make inactive background color invisible on legend
-        legend_icon.set_alpha(0 if visible else 0.3)
+    if type(legend_icon) != Legend:
+        legend_label = legend_icon._label
+        path_type = legend_type_dict[type(legend_icon)]
+
+        # Find the plot line based on the legend line name
+        plot_artists = plot_paths[legend_label][path_type]
+
+        # Get visibility of the lines/markers/backgrounds & swap it
+        visible = True
+        for artist in plot_artists:
+            visible = artist.get_visible()
+            artist.set_visible(not visible)
+
+        if path_type != 'backgrounds':
+            # Make inactive lines mostly transparent in the legend
+            legend_icon.set_alpha(0.2 if visible else 1.0)
+        else:
+            # Make inactive background color invisible on legend
+            legend_icon.set_alpha(0 if visible else 0.3)
+
+        fig.canvas.draw_idle()
+        fig.canvas.flush_events()
 
-    fig.canvas.draw_idle()
-    fig.canvas.flush_events()
 
 class Plotter:
-    def __init__(self, project: str, neighbor_sensors: dict):
+    def __init__(self, project:Project, neighbor_sensor_data:dict = {}):
         self.project = project
-        self.neighbor_sensors = neighbor_sensors
+        self.neighbor_sensor_data = neighbor_sensor_data
         self.plot_list = {}
 
     def __repr__(self):
         return 'Plotter object for {}'.format(self.project.project_name)
 
     def __str__(self):
         return 'Plotter object for {}'.format(self.project.project_name)
 
 
-    def _update_plotter_data(self, project: Project, neighbor_sensors: dict):
-        self.project = project
-        self.neighbor_sensors = neighbor_sensors
+    def _update_plotter_neighbors(self, neighbor_sensor_data: dict):
+        self.neighbor_sensor_data = neighbor_sensor_data
+
+
+    def draw_plots(self, plot_order: list|str, *args, **kwargs):
+        """
+        Private method to orchestrate drawing of plots
+
+        Args:
+            plotter (Plotter): [Plotter][ccrenew.dashboard.plotting.plots.Plotter] to use to draw plots for analysis
+            plot_order (list): Order of plots to draw.
+        """
+        mth = kwargs.get('mth', None)
+        close_plots = kwargs.get('close_plots', True)
+        min_date = kwargs.get('min_date', None)
+        max_date = kwargs.get('max_date', None)
+        poa_onboarding = kwargs.get('poa_onboarding', False)
+        open_folder = kwargs.get('open_folder', False)
+        fullscreen = kwargs.get('fullscreen', True)
+        persist = kwargs.get('persist', False)
+            
+        # Close all existing plots if requested
+        if close_plots:
+            self.close_plots(close_plots)
+
+        # Default month to a month previous to today
+        if not mth:
+            mth = datetime.now().month - 1
+            
+        def parse_date(dt, direction, days=None):
+            if isinstance(dt, Numeric):
+                if direction == 'backward':
+                    dt = datetime.today() - timedelta(days=abs(dt))
+                else:
+                    dt = datetime.today() + timedelta(days=abs(dt))
+            else:
+                try:
+                    dt = parser.parse(dt)
+                except (ValueError, ParserError):
+                    if direction == 'backward':
+                        days = 45 if not days else days
+                        dt = datetime.today() - timedelta(days)
+                    else:
+                        days = 4 if not days else days
+                        dt = datetime.today() + timedelta(days)
+                except TypeError:
+                    pass
+
+            return dt
+
+        # Set min & max dates for plots
+        # If no min_date supplied we'll just leave it as None to show the whole plot
+        if min_date:
+            min_date = parse_date(min_date, 'backward')
+
+        # Default max_date to 4 days from today to give some padding to the right side of the plot
+        if max_date:
+            max_date = parse_date(max_date, 'forward', 0)
+        else:
+            max_date = parse_date(datetime.today(), 'forward')
+
+        # Set default date format parameters
+        rcParams["date.autoformatter.day"] = "%#m/%#d/%Y"
+        rcParams["date.autoformatter.hour"] = "%#m/%#d %H:%M"
+        rcParams['figure.titlesize'] = 'xx-large'
+        rcParams['figure.titleweight'] = 'bold'
+
+        plot_params = {'mth': mth,
+                       'min_date': min_date,
+                       'max_date': max_date,
+                       'poa_onboarding': poa_onboarding,
+                       'fullscreen': fullscreen}
+
+        # Display plots
+        if not plot_order:
+            plot_order = [
+                'xplot_pwr_poa',
+                'xplot_temp',
+                'temps',
+                'inv',
+                'pr',
+                '8760',
+                'weather',
+                'mtr_corrected',
+                'mtr_dif',
+                'poas',
+                'pwr_poa',
+                'ghi',
+                'irrad',
+                'tz',
+                'losses',
+                'poa_corr',
+            ]
+        
+            if self.project.Battery_AC_site:
+                plot_order.append('battery')
+            if self.project.Tracker_site:
+                plot_order.append('tracker')
+
+        if isinstance(plot_order, str):
+            plot_order = [plot_order]
+
+        for plot_name in plot_order:
+            self.plot_list[plot_name] = self._draw_plot(plot_name, plot_params, **kwargs)
+
+        if persist:
+            plt.show(block=True)
+        else:
+            plt.show()
+
+        if open_folder:
+            os.startfile(os.path.join(self.project.dashboard_dir,
+                                      self.project.project_directory,
+                                      self.project.project_name))
 
 
     def _draw_plot(self, plot_name, plot_params, **kwargs):
         # Assign parameters
         mth = plot_params['mth']
         min_date = plot_params['min_date']
         max_date = plot_params['max_date']
@@ -97,22 +225,21 @@
             for df, ax in zip(dfs, axs):
                 try:
                     df.plot(ax=ax)
                     ax.set_xlim(left=min_date, right=max_date)
 
                     # Create interactive legend
                     legend = ax.legend()
-                    lines =  [line for line in ax.get_lines()]
-                    path_dict = {}
+                    legend.set_draggable(True)
+                    plot_paths = {line._label: {'lines': [line]} for line in ax.get_lines()}
 
-                    for leg_line, plot_line in zip(legend.get_lines(), lines):
-                        leg_line.set_picker(5)
-                        path_dict[leg_line] = plot_line
+                    for legend_handle in legend.legendHandles:
+                        legend_handle.set_picker(5)
 
-                    on_pick = partial(picker, fig=fig, path_dict=path_dict)
+                    on_pick = partial(picker, fig=fig, plot_paths=plot_paths)
                     fig.canvas.mpl_connect('pick_event', on_pick)
                 except TypeError:
                     continue
 
 
         if plot_name.replace(' ', '_').lower() == 'xplot_pwr_poa':
             # Power vs POA Crossplot
@@ -152,18 +279,18 @@
             y_orig_meter.name = 'Original'
             y_meter_corrected = self.project.df.loc[:, 'Meter_Corrected_2']
             y_meter_corrected.name = 'Meter Corrected'
             y_inv_sum = self.project.ava.loc[:, 'Inv_sum']
             y_inv_sum.name = 'Inv Sum'
             y_poa = self.project.df.loc[:, 'POA_avg']
             y_poa.name = 'POA Avg'
-            mc_max = y_meter_corrected.max()
-            meter_corrected_ylim = [-0.05*mc_max, mc_max/0.9]
-            poa_max = y_poa.max()
-            poa_ylim = [-0.05*poa_max, poa_max/0.9]
+            mc_max:float = y_meter_corrected.max()
+            meter_corrected_ylim = (-0.05*mc_max, mc_max/0.9)
+            poa_max:float = y_poa.max()
+            poa_ylim = (-0.05*poa_max, poa_max/0.9)
 
             fig, ax = plt.subplots(num='Power & POA - {}'.format(self.project.project_name))
             fig.suptitle(self.project.project_name)
             ax_power = ax
             ax_poa = ax_power.twinx()
 
             if self.project.Battery_DC_site:
@@ -182,22 +309,21 @@
             y_poa.plot(ax=ax_poa, color='grey')
             ax_power.set_xlim(left=min_date, right=max_date)
             ax_power.set_ylim(meter_corrected_ylim)
             ax_poa.set_ylim(poa_ylim)
 
             # Create interactive legend
             legend = fig.legend()
-            lines =  [line for line in ax_power.get_lines()] + [line for line in ax_poa.get_lines()]
-            path_dict = {}
+            legend.set_draggable(True)
+            plot_paths = {line.get_label(): {'lines': [line]} for line in list(ax_power.get_lines()) + list(ax_poa.get_lines())}
 
-            for leg_line, plot_line in zip(legend.get_lines(), lines):
-                leg_line.set_picker(5)
-                path_dict[leg_line] = plot_line
+            for legend_handle in legend.legendHandles:
+                legend_handle.set_picker(5)
 
-            on_pick = partial(picker, fig=fig, path_dict=path_dict)
+            on_pick = partial(picker, fig=fig, plot_paths=plot_paths)
             fig.canvas.mpl_connect('pick_event', on_pick)
 
 
         elif plot_name.replace(' ', '_').lower() == 'mtr_corrected':
             # Meter Corrections
             y_orig_meter = self.project.df_Meter_ORIGINAL.loc[:,self.project.pos_Meter_ORIGINAL].sum(axis=1)
             y_orig_meter.name = 'Original'
@@ -222,21 +348,22 @@
                 title = 'Power Meter Correction\nBattery DC Site'
             elif self.project.Battery_AC_site:
                 title = 'Power Meter Correction\nBattery AC Site'
             elif self.project.df_proj_keys['Fund'] == 'USB 1':
                 title = 'Power Meter Correction\n***NOTE: USB site - will need a utility invoice for meter data***'
             else:
                 title = ' Power Meter Correction'
+
             ax_power.set_title(title)
             y_orig_meter.plot(ax=ax_power)
             y_meter_corrected.plot(ax=ax_power, linestyle=':',linewidth=5)
             y_inv_sum.plot(ax=ax_power, linestyle='-.')
             ax_power.axhline(y = self.project.MWAC * 1000, color = 'r', linestyle = '--', label='Clipping Limit')
             ax_power.set_xlim(left=min_date, right=max_date)
-            ax_power.set_ylim([-100, self.project.MWAC * 1.3 * 1000])
+            ax_power.set_ylim((-100, self.project.MWAC * 1.3 * 1000))
             ax_power.legend()
 
             ax_cum.set_title('Cumulative Energy Meter Correction')
             y_cum_orig.plot(ax=ax_cum)
             y_cum_corrected.plot(ax=ax_cum)
             y_cum_inv.plot(ax=ax_cum, linestyle='-.')
             ax_cum.set_xlim(left=min_date, right=max_date)
@@ -245,21 +372,24 @@
             # We'll turn the x-axis labels back on for the top plot because pyplot disables those by default when you share an axis
             ax_power.xaxis.set_tick_params(labelbottom=True, which='both')
 
 
         elif plot_name.replace(' ', '_').lower() == 'poas':
             # POA sensors
             y_poa = self.project.df.loc[:, self.project.pos_POA]
-            y_poa_solcast = self.project.df_solcast.loc[:, 'POA_avg']
-            y_poa_solcast.index.name = None
-            y_poa_solcast.name = 'Solcast'
+            y_poa_solcast = self.project.df_bluesky.loc[:, 'sat_poa']
+            y_poa_solcast.name = 'Satellite'
+            y_poa_tran_ghi = self.project.df_bluesky.loc[:, 'proj_ghi_poa']
+            y_poa_tran_ghi.name = 'Trans GHI'
+            # y_poa_solcast.index.name = None
+            # y_poa_solcast.name = 'Solcast'
             y_poa_avg = self.project.df.loc[:, 'POA_avg']
             y_poa_avg.name = 'POA Avg'
             y_neighbors = pd.DataFrame()
-            for neighbor_name, neighbor_df in self.neighbor_sensors.items():
+            for neighbor_name, neighbor_df in self.neighbor_sensor_data.items():
                 if self.project.neighbor_list[neighbor_name]:
                     y_neighbors[neighbor_name] = neighbor_df.loc[:, 'POA_avg']
             racking = self.project.df_proj_keys.get('Racking')
             
             fig, ax = plt.subplots(num='POAs - {}'.format(self.project.project_name))
             fig.suptitle(self.project.project_name)
 
@@ -267,153 +397,177 @@
             if self.project.df_proj_keys['Fund'] == 'Soltage Landfill':
                 title = 'Irradiance - Racking: {}\n***NOTE: POAs might be off tilt from each other due to site geography. The average may still be acceptable.***'.format(racking)
             ax.set_title(title)
 
             # We'll use the default colormap but remove '#FBC15E' to use as the Solcast color
             cmap = plt.rcParams['axes.prop_cycle'].by_key()['color']
             solcast_color = '#FBC15E'
+            tran_ghi_color = '#CE7E00'
             cmap.remove(solcast_color)
             ax.set_prop_cycle(color=cmap)
 
             # Plot data
             y_poa.plot(ax=ax)
             if not y_neighbors.empty:
                 y_neighbors.plot(ax=ax)
             y_poa_solcast.plot(ax=ax, linestyle='--', color=solcast_color)
+            y_poa_tran_ghi.plot(ax=ax, linestyle='-.', color=tran_ghi_color)
 
             ax.set_xlim(left=min_date, right=max_date)
 
-            # Plot data sources used for POA_avg as scatter markers
+            # Initialize dictionary for interactive legend
+            plot_paths = {line.get_label(): {'lines': [line]} for line in ax.get_lines()}
+
+            # Group POA_avg data sources to plot as scatter markers
             poa_source_df_dict = self.project.df[['POA_avg', 'POA_source']].groupby('POA_source').groups
 
             # Order sources to show Native, Config, Solcast followed by others
             poa_source_df_dict_sorted = {}
-            poa_source_list = ['Native', 'Config', 'Config MT', 'Solcast', 'Solcast MT']
+            poa_source_list = ['Native', 'Config', 'Config MT', 'Satellite', 'Satellite MT', 'Trans GHI', 'Trans GHI MT']
             for source in poa_source_list:
                 try:
                     poa_source_df_dict_sorted[source] = poa_source_df_dict.pop(source)
                 except KeyError:
                     continue
 
             # Sort the neighbors to show as closest first in order to farthest
             # (project.neighbor_list is already in this order, we'll use that as a key for the sorted function)
             neighbors_sorted = list(self.project.neighbor_list.keys())
-
             for neighbor in neighbors_sorted:
                 # Add neighbors
                 try:
                     poa_source_df_dict_sorted[neighbor] = poa_source_df_dict.pop(neighbor)
                 except KeyError:
                     pass
                 try:
                     poa_source_df_dict_sorted[neighbor + ' MT'] = poa_source_df_dict.pop(neighbor + ' MT')
                 except KeyError:
                     continue
 
-            marker_dict = {'Native': 'o', 'Config': '$c$', 'Config MT': '$c$', 'Solcast': '*', 'Solcast MT': '*'}
-            neighbor_markers = ['x', '+', 'd', '^', '2', '<', 's', 'p', '>', 'h', 'H', 'D', 'P', 'v', (6,2,90)]
-            background_color_dict = {'Native': 'dodgerblue', 'Config': 'palegreen', 'Config MT': 'palegreen', 'Solcast': 'gold', 'Solcast MT': 'gold'}
+            # Custom markers for data source type
+            marker_dict = {'Native': 'o', 'Config': '$c$', 'Config MT': '$c$',
+                           'Satellite': '*', 'Satellite MT': '*', 'Trans GHI': '^', 'Trans GHI MT': '^'}
+            neighbor_markers = ['x', '+', 'd', '2', '<', 's', 'p', '>', 'h', 'H', 'D', 'P', 'v', (6,2,90), '^']
+            background_color_dict = {'Native': 'dodgerblue', 'Config': 'palegreen', 'Config MT': 'palegreen',
+                                     'Satellite': 'gold', 'Satellite MT': 'gold', 'Trans GHI': 'orange', 'Trans GHI MT': 'orange'}
             for i, neighbor in enumerate(neighbors_sorted):
                 marker_dict[neighbor] = neighbor_markers[i]
                 marker_dict[neighbor + ' MT'] = neighbor_markers[i]
 
             # Plot the data source points
-            plot_markers = {}
-            plot_backgrounds = {}
-            background_labels = []
             background_handles = []
             for i, (source, idx) in enumerate(poa_source_df_dict_sorted.items()):
                 # There's a weird bug in the ax.scatter method that errors out if there's only one x-axis Pandas datetime point
                 # So when there's only one point we'll just add itself to the index & carry on
                 if len(idx) == 1:
                     idx = idx.append(idx)
                 if ' MT' in source:
                     color = 'black'
                 else:
                     color = 'red'
                 markers = ax.scatter(x=idx, y=y_poa_avg[idx], marker=marker_dict[source], label=source, color=color)
-                plot_markers[markers] = 'markers'
+                try:
+                    plot_paths[source]['markers'] = [markers]
+                except KeyError:
+                    plot_paths[source] = {'markers': [markers]}
 
                 # Add background color
-                source_diff = idx.to_series().diff()
-                source_gaps = source_diff != pd.Timedelta(hours=1)
-                source_spans = source_gaps[source_gaps.diff(-1).fillna(True)]
-                span_starts = source_spans[source_spans].index
-                span_ends = source_spans[~source_spans].index
+                source_spans = pd.DataFrame({'data': idx})
+                source_spans['span_starts'] = source_spans['data'].diff() != pd.Timedelta(hours=1)
+                source_spans['span_ends'] = source_spans['data'].diff(-1) != pd.Timedelta(days=-1, hours=23)
+                span_starts = source_spans['data'][source_spans['span_starts']]
+                span_ends = source_spans['data'][source_spans['span_ends']] + pd.Timedelta(hours=1)
 
+                # Standard colors for Native/Config/Solcast, violet for neighbors
                 try:
                     background_color = background_color_dict[source]
                 except KeyError:
                     background_color = 'violet'
 
-                background_spans = []
+                # Create patch collection for each data source
+                patches = []
                 for start, end in zip(span_starts, span_ends):
                     xmin, xmax = start, end
                     ymin, ymax = 0, 1
+
+                    # Convert from dates to floats
                     (xmin, xmax), = ax._process_unit_info([('x', [xmin, xmax])])
+
                     verts = [(xmin, ymin), (xmin, ymax), (xmax, ymax), (xmax, ymin)]
                     p = mpatches.Polygon(verts, color=background_color, alpha=0.3, label=source)
-                    p.set_transform(ax.get_xaxis_transform(which="grid"))
-                    p.get_path()._interpolation_steps = 100
-                    p = ax.add_patch(p)
-                    background_spans.append(p)
-                
-                # Since Matplot lib (version 3.5.2) doesn't allow for creation of a legend entry for patches
-                # We'll just choose one patch to represent the collection in the legend
-                label_stripped = source.replace(' MT', '')
-                if label_stripped not in background_labels:
-                    background_labels.append(label_stripped)
-                    background_handles.append(p)
 
-                try:    
-                    plot_backgrounds[label_stripped].extend(background_spans)
+                    patches.append(p)
+                    
+                patch_collection = PatchCollection(
+                        patches,
+                        facecolors=background_color,
+                        edgecolors=background_color,
+                        alpha=0.3,
+                        label=source)
+
+                # We need to first add the collection to the axes then apply the transform lest everything get all wonky
+                ax.add_collection(patch_collection)
+                background = ax.collections[-1]
+                background.set_transform(ax.get_xaxis_transform(which='grid'))
+
+                # Update plot_paths with the background
+                label_stripped = source.replace(' MT', '')
+                try:
+                    plot_paths[label_stripped]['backgrounds'].append(background)
                 except KeyError:
-                    plot_backgrounds[label_stripped] = background_spans
+                    plot_paths[label_stripped]['backgrounds'] = [background]
+                    background_handles.append(p)
 
             # Create interactive legend
-            plot_lines = {line: 'line' for line in ax.get_lines()}
-
-            legend_handles = list(plot_lines.keys()) + list(plot_markers.keys()) + background_handles
-            plot_paths = {**plot_lines, **plot_markers, **plot_backgrounds}
+            # We'll need to exclude the background PatchCollections then add the individual patches in the next step due to the issue above
+            legend_handles = [plot_artist[0] for artist_dict in plot_paths.values() for plot_type, plot_artist in artist_dict.items() if plot_type != 'backgrounds']
+            legend_handles.extend(background_handles)
             visible_lines = self.project.col_ref['POA_cols'] + list(poa_source_df_dict_sorted)
             
             legend = ax.legend(handles=legend_handles)
+            legend.set_draggable(True)
+
             # Add Solcast to the list of visible lines if it's only been added due to mistracking
-            if 'Solcast MT' in visible_lines and 'Solcast' not in visible_lines:
-                visible_lines.append('Solcast')
+            if 'Satellite MT' in visible_lines and 'Satellite' not in visible_lines:
+                visible_lines.append('Satellite')
+            if 'Tran GHI MT' in visible_lines and 'Tran GHI' not in visible_lines:
+                visible_lines.append('Tran GHI')
             path_dict = {}
 
-            for legend_icon, plot_path in zip(legend.legendHandles, plot_paths.items()):
+            for legend_handle in legend.legendHandles:
+                source = legend_handle._label
+                path_dict = plot_paths[source]
+                legend_handle.set_picker(True)
+
                 # For line-type legend icons we'll add some padding around the line so you don't have to click exactly on the line
-                # Line buffer in pixels
-                path = plot_path[0]
-                path_type = plot_path[1]
-                line_buffer = 5
-                legend_icon.set_picker(True)
-                if path_type == 'line':
-                    path_label = path.get_label()
-                    legend_icon.set_picker(line_buffer)
-                    # Turn line off if not used for data sub
-                    if path_label not in visible_lines:
-                        path.set_visible(False)
-                        legend_icon.set_alpha(0.2)
-                elif path_type == 'markers':
-                    path_label = path.get_label()
-                    # Bring marker points in front of all lines
-                    path.set_zorder(100)
-                else:
-                    # Send the background patches to the back
-                    path = path_type
-                    for patch in path:
-                        patch.set_zorder(0)
-                    path_type = 'background'
+                # Line padding in pixels
+                line_padding = 5
+
+                for path_type, paths in path_dict.items():
+                    if path_type == 'lines':
+                        legend_handle.set_picker(line_padding)
+
+                        # Turn line off if not used for data sub
+                        if source not in visible_lines:
+                            for path in paths:
+                                path.set_visible(False)
+                            legend_handle.set_alpha(0.2)
+
+                    elif path_type == 'markers':
+                        # Bring marker points in front of all lines
+                        for path in paths:
+                            path.set_zorder(100)
+
+                    else:
+                        # Push backgrounds to the back of the pot
+                        for path in paths:
+                            path.set_zorder(0)
 
-                path_dict[legend_icon] = (path, path_type)
 
-            on_pick = partial(picker, fig=fig, path_dict=path_dict)
+            on_pick = partial(picker, fig=fig, plot_paths=plot_paths)
             fig.canvas.mpl_connect('pick_event', on_pick)
 
 
         elif plot_name.replace(' ', '_').lower() == 'poa_corr':
             # POA Correlations
             if len(self.project.pos_POA) > 1:
                 if poa_onboarding:
@@ -454,17 +608,17 @@
 
         elif plot_name.replace(' ', '_').lower() == 'xplot_poa_sol':
             # POA sensors
             poa_cols = self.project.col_ref['POA_cols']
             if not min_date:
                 min_date = self.project.df.index[0]
             df_poa = self.project.df.query("index>=@min_date and index<@max_date").reindex(columns=poa_cols)
-            df_poa = daylight(lambda **kwargs: kwargs['df'])(df=df_poa, project=self.project)
+            df_poa = daylight(lambda **kwargs: kwargs['df'])(df=df_poa, pv_model = self.project.pv_model)
             native_poa_cols = df_poa.columns
-            df_poa['Solcast'] = self.project.df_solcast.loc[:, 'POA_avg']
+            df_poa['Solcast'] = self.project.df_bluesky.loc[:, 'POA_avg']
             x = df_poa.loc[:, 'Solcast']
             y = df_poa.loc[:, native_poa_cols]
 
             racking = self.project.df_proj_keys.get('Racking')
             
             fig, ax = plt.subplots(num='POA vs Solcast - {}'.format(self.project.project_name))
             fig.suptitle(self.project.project_name)
@@ -515,25 +669,23 @@
 
             ax.set_title('Inverter KW')
             y.plot(ax=ax)
             ax.set_xlim(left=min_date, right=max_date)
 
             # Create interactive legend
             legend = ax.legend()
-            lines =  [line for line in ax.get_lines()]
-            path_dict = {}
+            legend.set_draggable(True)
+            plot_paths = {line._label: {'lines': [line]} for line in ax.get_lines()}
 
-            for leg_line, plot_line in zip(legend.get_lines(), lines):
-                leg_line.set_picker(5)
-                path_dict[leg_line] = plot_line
+            for legend_handle in legend.legendHandles:
+                legend_handle.set_picker(5)
 
-            on_pick = partial(picker, fig=fig, path_dict=path_dict)
+            on_pick = partial(picker, fig=fig, plot_paths=plot_paths)
             fig.canvas.mpl_connect('pick_event', on_pick)
-            
-            
+
             # TODO: is this for determining inverter outages?
             def list_pairs(lis):
                 #find pairs that are at least 2 hours in duration
                 beg = []
                 end = []
                             
                 start_time = 0
@@ -551,14 +703,60 @@
                 
             beg, end = list_pairs(list(self.project.df.loc[self.project.df['Meter_&_ava'] > self.project.df['Meter_Corrected_2'], :].index) )
 
             for beg,end in zip(beg,end):
                 ax.axvspan(beg, end, facecolor='#2ca02c', alpha=0.5)
 
 
+        elif plot_name.replace(' ', '_').lower() == 'inv_cum':
+            # Inverters
+            y_inv = self.project.df.loc[:, self.project.pos_Inv]
+            y_inv_cum = self.project.df.loc[:, self.project.pos_Inv_cum]
+            min_inv_cum = y_inv_cum[(y_inv_cum > 0)].min().min()
+            
+            # Check for nans
+            if min_inv_cum != min_inv_cum:
+                min_inv_cum = None
+
+            fig, axs = plt.subplots(2, sharex=True, num='Inverters - {}'.format(self.project.project_name))
+            fig.suptitle(self.project.project_name)
+            ax_inv = axs[0]
+            ax_inv.set_title('Inverter Power')
+            ax_inv_cum = axs[1]
+            ax_inv_cum.set_title('Inverter Energy')
+
+            draw_multiple_axes([y_inv, y_inv_cum], axs, min_date, max_date)
+            ax_inv_cum.set_ylim(bottom=min_inv_cum)
+
+            # TODO: is this for determining inverter outages?
+            def list_pairs(lis):
+                #find pairs that are at least 2 hours in duration
+                beg = []
+                end = []
+                            
+                start_time = 0
+                
+                while start_time < len(lis):
+                    end_time = start_time+1
+                    while end_time < len(lis) and lis[end_time] - lis[end_time-1] == pd.Timedelta('1h'):
+                        end_time = end_time+1
+                    # end_time overshoots by one hour, so adjust to make sure it's longer than 1 hr
+                    if (end_time-1) - start_time >= 1:
+                        beg.append(lis[start_time])
+                        end.append(lis[end_time-1])
+                    start_time = end_time
+                return beg, end
+                
+            beg, end = list_pairs(list(self.project.df.loc[self.project.df['Meter_&_ava'] > self.project.df['Meter_Corrected_2'], :].index) )
+
+            for beg,end in zip(beg,end):
+                ax_inv.axvspan(beg, end, facecolor='#2ca02c', alpha=0.5)
+                ax_inv_cum.axvspan(beg, end, facecolor='#2ca02c', alpha=0.5)
+
+
         elif plot_name.replace(' ', '_').lower() == 'pr':
             # Hourly PR
             freq = 'h'
             top = self.project.df.loc[:, 'Gen_NO_Clipping'].resample(freq).sum()
             bottom = self.project.df.loc[:, 'DC_corrected_PR'].resample(freq).sum()
             y = top.div(bottom)
             y_avg = y.dropna().rolling(48).mean()
@@ -573,24 +771,23 @@
             except Exception as e:
                 print('Skipped adding PR line for {}'.format(self.project.project_name))
                 # logger.warn('{} error plotting PR rolling avg for {}'.format(e, self.project.project_name))
             ax.set_xlim(left=min_date, right=max_date)
             
             # Create interactive legend
             legend = ax.legend()
-            lines =  [line for line in ax.get_lines()]
-            path_dict = {}
+            legend.set_draggable(True)
+            plot_paths = {line._label: {'lines': [line]} for line in ax.get_lines()}
 
-            for leg_line, plot_line in zip(legend.get_lines(), lines):
-                leg_line.set_picker(5)
-                path_dict[leg_line] = plot_line
+            for legend_handle in legend.legendHandles:
+                legend_handle.set_picker(5)
 
-            on_pick = partial(picker, fig=fig, path_dict=path_dict)
+            on_pick = partial(picker, fig=fig, plot_paths=plot_paths)
             fig.canvas.mpl_connect('pick_event', on_pick)
-
+        
 
         elif plot_name.replace(' ', '_').lower() == 'losses':
             # Losses
             y_losses = self.project.losses
 
             # If single inverter site, remove losses where meter_corrected_2 > 0
             if len(self.project.pos_Inv) == 1:
@@ -633,59 +830,53 @@
             y_fahr.plot(ax=ax_fahr, style='None', grid=False)
             ax_cels.set_ylabel('Temperature (C)')
             ax_fahr.set_ylabel('Temperature (F)')
             ax_cels.set_xlim(left=min_date, right=max_date)
 
             # Create interactive legend
             legend = ax_cels.legend()
-            lines =  [line for line in ax_cels.get_lines()]
-            path_dict = {}
+            legend.set_draggable(True)
+            plot_paths = {line._label: {'lines': [line]} for line in ax_cels.get_lines()}
 
-            for leg_line, plot_line in zip(legend.get_lines(), lines):
-                leg_line.set_picker(5)
-                path_dict[leg_line] = plot_line
+            for legend_handle in legend.legendHandles:
+                legend_handle.set_picker(5)
 
-            on_pick = partial(picker, fig=fig, path_dict=path_dict)
+            on_pick = partial(picker, fig=fig, plot_paths=plot_paths)
             fig.canvas.mpl_connect('pick_event', on_pick)
 
             ax_fahr.legend().set_visible(False)
 
 
         elif plot_name.replace(' ', '_').lower() == 'weather':
             # Weather Sensors
             y_poa = self.project.df['POA_avg']
-            y_temp = self.project.df['Tamb_avg']
+            y_tamb = self.project.df['Tamb_avg']
+            y_tmod = self.project.df['Tmod_avg']
             y_wind = self.project.df['Wind_speed']
 
-            fig, axs = plt.subplots(3, num='Weather Sensors - {}'.format(self.project.project_name), sharex=True)
+            fig, axs = plt.subplots(4, num='Weather Sensors - {}'.format(self.project.project_name), sharex=True)
             fig.suptitle(self.project.project_name)
             ax_poa = axs[0]
-            ax_temp = axs[1]
-            ax_wind = axs[2]
+            ax_tamb = axs[1]
+            ax_tmod = axs[2]
+            ax_wind = axs[3]
 
             ax_poa.set_title('Irradiance')
             y_poa.plot(ax=ax_poa, label='POA Avg')
-            ax_temp.set_title('Ambient Temperature')
-            y_temp.plot(ax=ax_temp, label='Tamb Avg')
+            ax_tamb.set_title('Ambient Temperature')
+            y_tamb.plot(ax=ax_tamb, label='Tamb Avg')
+            ax_tmod.set_title('Module Temperature')
+            y_tmod.plot(ax=ax_tmod, label='Tmod Avg')
             ax_wind.set_title('Wind Speed')
             y_wind.plot(ax=ax_wind, label='Wind Speed')
             for ax in axs:
                 ax.set_xlim(left=min_date, right=max_date)
                 
                 # Create interactive legend
                 legend = ax.legend()
-                lines =  [line for line in ax.get_lines()]
-                path_dict = {}
-
-                for leg_line, plot_line in zip(legend.get_lines(), lines):
-                    leg_line.set_picker(5)
-                    path_dict[leg_line] = plot_line
-
-                on_pick = partial(picker, fig=fig, path_dict=path_dict)
-                fig.canvas.mpl_connect('pick_event', on_pick)
 
 
         elif plot_name.replace(' ', '_').lower() == 'ghi':
             #GHI plot
             if len(self.project.pos_GHI) > 0:
                 y_ghi = self.project.df.loc[:, self.project.pos_GHI]
                 y_ghi_avg = self.project.df.loc[:, 'GHI_avg']
@@ -699,22 +890,21 @@
                     ax.set_title('GHI Sensors')
                     y_ghi.plot(ax=ax)
                     y_ghi_avg.plot(ax=ax, style='o', label='GHI Avg')
                     ax.set_xlim(left=min_date, right=max_date)
                     
                     # Create interactive legend
                     legend = ax.legend()
-                    lines =  [line for line in ax.get_lines()]
-                    path_dict = {}
+                    legend.set_draggable(True)
+                    plot_paths = {line._label: {'lines': [line]} for line in ax.get_lines()}
 
-                    for leg_line, plot_line in zip(legend.get_lines(), lines):
-                        leg_line.set_picker(5)
-                        path_dict[leg_line] = plot_line
+                    for legend_handle in legend.legendHandles:
+                        legend_handle.set_picker(5)
 
-                    on_pick = partial(picker, fig=fig, path_dict=path_dict)
+                    on_pick = partial(picker, fig=fig, plot_paths=plot_paths)
                     fig.canvas.mpl_connect('pick_event', on_pick)
 
                 except:
                     print("Couldn't make GHI_avg plot")
                     fig, ax = 'GHI plot error', 'GHI plot error'
             else:
                 print("No GHI sensors to build the GHI plots")
@@ -741,24 +931,23 @@
                 y_ghi_avg.plot(ax=ax, label='GHI Avg', style='-.')
                 y_poa.plot(ax=ax)
                 y_poa_avg.plot(ax=ax, label='POA Avg', style=':')                               
                 ax.set_xlim(left=min_date, right=max_date)
                 
                 # Create interactive legend
                 legend = ax.legend()
-                lines =  [line for line in ax.get_lines()]
-                path_dict = {}
+                legend.set_draggable(True)
+                plot_paths = {line._label: {'lines': [line]} for line in ax.get_lines()}
 
-                for leg_line, plot_line in zip(legend.get_lines(), lines):
-                    leg_line.set_picker(5)
-                    path_dict[leg_line] = plot_line
+                for legend_handle in legend.legendHandles:
+                    legend_handle.set_picker(5)
 
-                on_pick = partial(picker, fig=fig, path_dict=path_dict)
+                on_pick = partial(picker, fig=fig, plot_paths=plot_paths)
                 fig.canvas.mpl_connect('pick_event', on_pick)
-                
+
             except Exception as e:
                 print("Couldn't make POA vs GHI plot. Exception: {}".format(e))
                 fig, ax = 'POA vs GHI plot error', 'POA vs GHI plot error'
             
 
         elif plot_name.replace(' ', '_').lower() == 'tz':
             #Timezone plot and night check
@@ -815,22 +1004,21 @@
 
             ax.set_title('Measured/8760 Generation Comparison')
             y_8760.plot(ax=ax, label='8760', c='blue')
             y_meter_corrected.plot(ax=ax, label='Meter Corrected', c='red')
             
             # Create interactive legend
             legend = ax.legend()
-            lines =  [line for line in ax.get_lines()]
-            path_dict = {}
+            legend.set_draggable(True)
+            plot_paths = {line._label: {'lines': [line]} for line in ax.get_lines()}
 
-            for leg_line, plot_line in zip(legend.get_lines(), lines):
-                leg_line.set_picker(5)
-                path_dict[leg_line] = plot_line
+            for legend_handle in legend.legendHandles:
+                legend_handle.set_picker(5)
 
-            on_pick = partial(picker, fig=fig, path_dict=path_dict)
+            on_pick = partial(picker, fig=fig, plot_paths=plot_paths)
             fig.canvas.mpl_connect('pick_event', on_pick)
             
 
         elif plot_name.replace(' ', '_').lower() == 'xplot_temp':
             # Power vs POA by Temperature
             x = self.project.df.loc[:, 'POA_avg']
             y = self.project.df.loc[:, 'Meter_Corrected_2']
@@ -882,18 +1070,20 @@
 
             draw_multiple_axes([poa, ghi, tamb, tmod, wind], axs, min_date, max_date)
 
 
         elif plot_name.replace(' ', '_').lower() == 'meters':
             fig_list = []
             for i in range(len(self.project.pos_Meter)):
+                meter_name = self.project.pos_Meter[i]
                 y_meter_orig = self.project.df_Meter_ORIGINAL.iloc[:,i]
-                y_meter_corr = self.project.df[self.project.pos_Meter[i]]
+                y_meter_corr = self.project.df[meter_name]
                 y_cum_orig = self.project.df_Meter_ORIGINAL.iloc[:,[i+len(self.project.pos_Meter)]]
-                y_cum_corr = self.project.df[[self.project.pos_Meter[i]]].cumsum()
+                y_cum_corr = self.project.df[[meter_name]].cumsum()
+                y_cum_corr = y_cum_corr.rename(columns = {meter_name: meter_name.replace('_kw_', '_kwhnet_')})
                 
                 # Add in a vertical offset if the original & corrected cum meters don't match up
                 condition = y_cum_orig.loc[(y_cum_orig[y_cum_orig.columns[0]] > 0), :].index
                 offset = np.mean(y_cum_orig.loc[condition, :].values - y_cum_corr.loc[condition, :].values)
                 y_cum_corr = y_cum_corr.add(offset)
 
                 fig, axs = plt.subplots(2, num='Meter {} - {}'.format(i+1, self.project.project_name), sharex=True)
@@ -908,33 +1098,26 @@
 
                 y_cum_orig.plot(ax=ax_cum)
                 y_cum_corr.plot(ax=ax_cum)
                 ax_cum.set_xlim(left=min_date, right=max_date)
 
                 # Create interactive legend
                 meter_legend = ax_meter.legend(['Original', 'Corrected'])
-                meter_lines =  [line for line in ax_meter.get_lines()]
-                meter_path_dict = {}
+                meter_legend.set_draggable(True)
 
                 cum_legend = ax_cum.legend(['Original', 'Corrected'])
-                cum_lines =  [line for line in ax_cum.get_lines()]
-                cum_path_dict = {}
+                cum_legend.set_draggable(True)
 
-                for leg_data in [(meter_legend, meter_lines, meter_path_dict),
-                                 (cum_legend, cum_lines, cum_path_dict)]:
-                    legend = leg_data[0]
-                    lines = leg_data[1]
-                    path_dict = leg_data[2]
-
-                    for leg_line, plot_line in zip(legend.get_lines(), lines):
-                        leg_line.set_picker(5)
-                        path_dict[leg_line] = plot_line
+                plot_paths = {line._label: {'lines': [line]} for line in list(ax_meter.get_lines()) + list(ax_cum.get_lines())}
 
-                    on_pick = partial(picker, fig=fig, path_dict=path_dict)
-                    fig.canvas.mpl_connect('pick_event', on_pick)
+                for legend_handle in list(meter_legend.legendHandles) + list(cum_legend.legendHandles):
+                    legend_handle.set_picker(5)
+
+                on_pick = partial(picker, fig=fig, plot_paths=plot_paths)
+                fig.canvas.mpl_connect('pick_event', on_pick)
 
                 fig_list.append(fig)
 
 
         elif plot_name.replace(' ', '_').lower() == 'snow':
             # Snow Plots
             y_snow_data = self.project.snow_data['snow']
@@ -943,24 +1126,24 @@
             fig, ax = plt.subplots(num='Snow Data - {}'.format(self.project.project_name))
             fig.suptitle(self.project.project_name)
 
             ax.set_title('Snow Data')
             y_snow_data.plot(ax=ax, label='Snowfall', c='blue')
             y_snow_coverage.plot(ax=ax, label='Coverage', c='red')
             
+            
             # Create interactive legend
             legend = ax.legend()
-            lines =  [line for line in ax.get_lines()]
-            path_dict = {}
+            legend.set_draggable(True)
+            plot_paths = {line._label: {'lines': [line]} for line in ax.get_lines()}
 
-            for leg_line, plot_line in zip(legend.get_lines(), lines):
-                leg_line.set_picker(5)
-                path_dict[leg_line] = plot_line
+            for legend_handle in legend.legendHandles:
+                legend_handle.set_picker(5)
 
-            on_pick = partial(picker, fig=fig, path_dict=path_dict)
+            on_pick = partial(picker, fig=fig, plot_paths=plot_paths)
             fig.canvas.mpl_connect('pick_event', on_pick)
 
 
         elif plot_name.replace(' ', '_').lower() == 'battery':
             if self.project.Battery_AC_site:
                 # Battery Discharge
                 poi_cols = [s for s in self.project.df_POI_ORIGINAL.columns if 'POI_kw_' in s]
@@ -1012,25 +1195,26 @@
                 ax_cum_correction.set_title('POI Energy Correction')
                 ax_cum_correction.plot(y_poi_cum_original, label='Original')
                 ax_cum_correction.plot(y_poi_cum_corrected, label='Corrected')
                 ax_cum_correction.legend()
             
 
         elif plot_name.replace(' ', '_').lower() == 'tracker':
-            if self.project.Tracker_site:
+            if self.project.pos_Tracker:
                 y = self.project.df[self.project.pos_Tracker]
 
                 fig, ax = plt.subplots(num='Tracker Angles - {}'.format(self.project.project_name))
                 fig.suptitle(self.project.project_name)
 
                 ax.set_title('Tracker Angles')
                 y.plot(ax=ax)
                 ax.set_xlim(left=min_date, right=max_date)
                 ax.set_ylim(-60,60)
-        
+            else:
+                print(f"No `pos_Tracker` found for {self.project.project_name}, tracker plot will not be drawn.") 
         else:
             print('`{}` is not a valid plot name. See documentation for valid names & try again'.format(plot_name))
             fig, ax = 'Invalid plot_name', 'Invalid plot_name'
 
 
         # If we have multiple subplots we'll overwrite `ax` with the list of subplots stored in `axs`
         if not ax:
@@ -1061,15 +1245,15 @@
         tight_layout = kwargs.get('tight_layout', None)
         default_tool = kwargs.get('default_tool', None)
 
         if isinstance(fig, Figure):
             try:
                 # Move plots to the selected screen
                 if screen:
-                    if isinstance(screen, Number):
+                    if isinstance(screen, Numeric):
                         try:
                             screen = screen-1
                             screens = QGuiApplication.screens()
                             top_left = screens[screen].availableGeometry().topLeft()
                             fig.canvas.manager.window.move(top_left)
                         except IndexError:
                             warnings.warn('`screen` index out of range. Please supply a number less than or equal to the number of screens you have.')
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/project.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,88 @@
 # -*- coding: utf-8 -*-
+"""
+Module to store and process data related to CCRenew solar projects.
+"""
+from __future__ import annotations
 
-import csv
-import awswrangler as wr
-from calendar import c
-from collections import namedtuple
+import boto3
 from datetime import datetime
 from dateutil.parser import parse
-from inspect import ArgSpec
 import io
+from IPython.display import HTML
 import itertools
 import logging
 import logging.config
-from numbers import Number
+import matplotlib.pyplot as plt
 import numpy as np
 import os
 import pandas as pd
-from pandas import DataFrame
 from pathlib import Path
 import pickle
+import s3fs
 import scipy.stats as sct
 import shutil
 from sqlalchemy import (
     delete,
     MetaData,
     Table
 )
 from sqlalchemy.sql import extract
 import sys
+import traceback
 from typing import Iterable, Union
 import xlsxwriter
+import xlsxwriter.utility
 
-from ccrenew import __version__
-from ccrenew.dashboard import (
+from ccrenew import (
+    __version__,
     ccr,
     DateLike,
-    func_timer
+    Numeric,
+    FileNotFoundError,
+    FileOpenError
 )
+from ccrenew.dashboard import (
+    Colmap,
+    S3FilePath,
+    func_timer,
+    get_modified_time,
+    make_s3_filepath,
+    Plotter
+)
+
+import ccrenew.data_determination as det
+
 import ccrenew.dashboard.data_processing.BV_pp_deg as batt
 import ccrenew.dashboard.data_processing.Correct_POI_data_v01 as poi
 import ccrenew.dashboard.data_processing.Correct_Meter_data_v08_smartercheck as meter_correct
-import ccrenew.dashboard.data_processing.data_determination as det
 import ccrenew.dashboard.data_processing.Performance_Guarantees_v01 as perf
 import ccrenew.dashboard.data_processing.Plant_Availability_v16_bbsc as plant_ava
 import ccrenew.dashboard.data_processing.Rate_Structure_Python_with_DST_v07 as rates
 import ccrenew.dashboard.data_processing.snow_loss_functions_v3 as snow
 import ccrenew.dashboard.data_processing.Table_by_Rate_Schedule_v01 as rate_table
 import ccrenew.dashboard.data_processing.weather_adjusted_functions_v03 as weather
 
-from ccrenew.dashboard.plotting.plots import Plotter
-
-from ccrenew.dashboard.utils.dashboard_utils import (
-    FileNotFoundError,
-    FileOpenError
-)
 import ccrenew.dashboard.utils.dashboard_utils as utils
 import ccrenew.dashboard.utils.df_tools as df_tools
 import ccrenew.dashboard.utils.project_neighbors as neighbs
 
-# Python 2 compatibility
-if sys.version_info.major == 3:
-    unicode = str
+from ccrenew.pvmodel.project_model import ProjectModel
+
+
+# Create boto s3 client
+s3_client = boto3.client('s3')
 
 # suppress warnings about "A value is trying to be set on a copy of a slice from a DataFrame."
-pd.options.mode.chained_assignment = None
+pd.set_option('mode.chained_assignment', None)
 
 # Create logger
 # logger = logging.getLogger(__name__)
 # logger = logging.getLogger(__name__)
 
-Colmap = namedtuple('Colmap', ['col_list', 'col_avg'])
 
 class PowertrackFileException(Exception):
     pass
 
 class Project:
     """An object representing a project (i.e. site). This should never be initialized\
         outside of a [DashboardSession][ccrenew.dashboard.session.DashboardSession] instance,
@@ -80,109 +90,123 @@
 
     Args:
         proj_init_dict (dict): A dictionary of metadata to pass to the `Project` for initialization.
     """
     
     # Initialize class variables
     Gstc:int = 1000
+    report_type_map = {'monthly': 'Monthly', 'ul': 'UL Monthly', 'weekly': 'Weekly'}
+
+    def __init__(self, proj_init_dict:dict):
 
-    def __init__(self, proj_init_dict: dict):
+        # Initialize Project name
+        self.project_name = proj_init_dict['project_name']
 
         # Store the version for checking when loading a pickle
         self.__version__ = __version__
 
         # Processed flag that we'll turn to true once we process the data
         self.processed = False
 
+        # Processed flag that we'll update when processing if we use datasub or not
+        self.datasub = False
+
         # Errored flag that will warn us when a project has encountered an error in processing
         self.errored = False
 
-        # Error info for a project than encounters an error
-        self.error_info = None
-
-        # Plotter object to store dashboard plots
-        self.plotter = None
+        # Error info for a project that encounters an error
+        self.error_info = proj_init_dict.get('error_info', dict())
+        if self.error_info:
+            print(f"{self.project_name} Errored. Error details: {self.error_info}")
+            self.errored = True
+            return
 
         # List to note neighbor sensors once we've added them
-        self.neighbor_sensors = set()
+        self.config_neighbor_sensors = set()
         
         # Project properties passed from DashboardSession
-        self.project_name = proj_init_dict['project_name']
         self.df_proj_keys = proj_init_dict['df_proj_keys']
         self.df_proj_ss_comments = proj_init_dict['df_proj_ss_comments']
         self.dashboard_dir = proj_init_dict['dashboard_dir']
         self.data_cutoff_date = proj_init_dict['data_cutoff_date']
+        self.data_platform = proj_init_dict['data_platform']
+        self.data_platform_dirs = proj_init_dict['data_platform_dirs']
         self.data_source = proj_init_dict['data_source']
+        self.report_type = proj_init_dict['report_type']
         self.Battery_AC_site = proj_init_dict['Battery_AC_site']
         self.Battery_DC_site = proj_init_dict['Battery_DC_site']
         self.Tracker_site = proj_init_dict['Tracker_site']
         self.raw_snow_df = proj_init_dict['raw_snow_df']
         self.snow_file = proj_init_dict['snow_file']
         self.neighbor_list = proj_init_dict['neighbor_list']
 
         # Project year based on `data_source`
-        if self.data_source == 'AE_data_':
-            self.year = datetime.now().year
-        else:
-            self.year = int(self.data_source.split('_')[0])
+        self.year = int(self.data_source.split('_')[0])
 
         # Get information for the project from DF keys
         # `self.df_proj_keys` is the appropriate row from `df_keys` as a dictionary
         self.project_directory = self.df_proj_keys['Folder']
         self.lat = self.df_proj_keys['GPS_Lat']
         self.lon = self.df_proj_keys['GPS_Long']
+        self.tz = f"US/{self.df_proj_keys['Timezone']}"
         self.MWAC = self.df_proj_keys['MWAC']
         try:
             self.publish_date = parse(self.df_proj_keys['PerfData_Publish_Date']).date()
         except:
             self.publish_date = datetime(2023, 1, 1).date()
 
+        # PV model object for pvlib functionality
+        self.pv_model = ProjectModel(self.project_name)    
+
         # Build filename for config file
         self.config_filepath = self._find_config_file()     
 
         # Get last update time for config file - we will use this to check if config file has been updated
-        self.last_update_config = 0.0
+        self.last_update_config = datetime.fromtimestamp(0)
 
         # Build filename for bool file
         self.bool_filepath = self._find_bool_file()     
 
         # Get last update time for bool file, will use it the same as config
-        self.last_update_bool = 0.0
+        self.last_update_bool = datetime.fromtimestamp(0)
 
         # Build filename for Powertrack file
         self.powertrack_filepath, self.powertrack_csv = self._find_powertrack_file()
 
         # Initialize powertrack update time, will use it the same as config
-        self.last_update_powertrack = 0.0
+        self.last_update_powertrack = datetime.fromtimestamp(0)
 
         # Check for pickle jar folder & create if it doesn't exist
         self.pickle_jar = self._find_pickle_jar()
         
         # Initialize other instance variables
-        self.config_sheets = None
-        self.config_column_map = None
-        self.colnames_ccr = None
-        self.colnames_das = None
+        self.config_sheets = {}
+        self.config_column_map = pd.Series()
+        self.colnames_ccr = []
+        self.colnames_das = []
         self.df = pd.DataFrame()
         self.df_Pvsyst = pd.DataFrame()
         self.df_sensor_ON = pd.DataFrame()
         self.df_bool = pd.DataFrame()
         self.df_sensors = pd.DataFrame()
         self.df_sensors_native_avg = pd.DataFrame()
-        self.df_solcast = pd.DataFrame()
+        self.df_bluesky = pd.DataFrame()
 
         # Finish initializing project
         # FIXME: update error handling when can't find config file
         self._parse_config_file()
         self._load_bool_file()
         self._map_columns()
-        self._find_neighbor_sensors()
+        self._find_config_neighbor_sensors()
         self.__get_project_parameters()
         self.__read_degradation_profile()
 
+        # Plotter object to store dashboard plots
+        self.plotter = Plotter(self)
+
 
         # Type annotations & docstrings for documentation
         self.project_name: str
         """The string representation of the [Project][ccrenew.dashboard.project.Project] name.
             This should match the 'Project' field in [df_keys][ccrenew.dashboard.session.DashboardSession.df_keys]."""
         self.proj_init_dict: dict
         """Metadata related to the project generated by the [DashboardSession][ccrenew.dashboard.session.DashboardSession]
@@ -190,49 +214,53 @@
         self.df_proj_keys: dict
         """The subset of [df_keys][ccrenew.dashboard.session.DashboardSession.df_keys]
             corresponding to the [Project][ccrenew.dashboard.project.Project] instance."""
         self.df_proj_ss_comments: dict
         """The comments entered into the Dashboard Startup Notes Smartsheet"""
         self.processed: bool
         """Flag to denote if the Project has been processed."""
+        self.datasub: bool
+        """Flag to denote if the Project was processed with the datasub algorithm."""
         self.errored: bool
         """Flag to denote if the Project has errored out during processing."""
-        self.error_info: dict
+        self.error_info: str
         """Information on the error that caused the Project to error during processing."""
         self.project_directory: str
         """Folder in the Dashboard file structure where the project data lives."""
         self.pickle_jar: str
         """Directory where the Project's pickle files are stored."""
         self.config_filepath: str
         """Filepath for the Project's config file."""
-        self.last_update_config: float
+        self.last_update_config: datetime
         """Timestamp of the last update to the config file. This is used to
             check if it needs to be re-loaded from the filesystem."""
         self.bool_filepath: str
         """Filepath for the Project's bool file based on the year."""
-        self.last_update_bool: float
+        self.last_update_bool: datetime
         """Timestamp of the last update to the bool file. This is used to
             check if it needs to be re-loaded from the filesystem."""
         self.powertrack_filepath: str
         """Filepath for the Project's Powertrack file."""
-        self.last_update_powertrack: float
+        self.last_update_powertrack: datetime
         """Timestamp of the last update to the powertrack file. This is used to
             check if it needs to be re-loaded from the filesystem."""
         self.config_sheets: dict
-        """Dictionary of `DataFrame`s for each sheet in the config file"""
+        """Dictionary of `DataFrame`s for each sheet in the config file."""
         self.colnames_ccr: list
         """CCR standard column names for data fields."""
         self.colnames_das: list
-        """Original column names from the DAS"""
-        self.plotter: object
+        """Original column names from the DAS."""
+        self.pv_model: ProjectModel
+        """A model for the project based on the `pvlib` package."""
+        self.plotter: Plotter
         """An object to store dashboard plots"""
-        self.neighbor_sensors: list
+        self.config_neighbor_sensors: set
         """A list of neighbor sensors that are available to the project.
         These are set with the `Get_Sensor` keyword on the `data` tab of the config file"""
-        self.neighbor_list: list
+        self.neighbor_list: dict
         """List of neighbors that meet the criteria for data substitution.
         
         * Default Criteria:
             * Distance: $<=$ 10 miles
             * Same racking OEM
             * Fixed tilt:
                 * Same module tilt
@@ -249,53 +277,56 @@
         """Boolean table to specify if a meter or sensor should be used or ignored."""
         self.df_bool: pd.DataFrame
         """Boolean table generated from bool file in project's config folder."""
         self.df_sensors: pd.DataFrame
         """Native sensors for the project."""
         self.df_sensors_native_avg: pd.DataFrame
         """Average of the native sensors for the project."""
-        self.df_solcast: pd.DataFrame
+        self.df_bluesky: pd.DataFrame
         """Solcast data for the project."""
         self.snow_data: pd.DataFrame
         """Calculated snowfall inches by day for the project."""
         self.snow_coverage: pd.Series
         """Snow coverage for the project."""
         self.lat: float
         """Project latitude."""
         self.lon: float
         """Project longitude."""
+        self.tz: str
+        """Project timezone from the Olson timezone database."""
         self.MWAC: float
         """Nameplate AC rating of the project."""
         self.Battery_AC_site: bool
         """Flag denoting a project with AC battery storage"""
         self.Battery_DC_site: bool
         """Flag denoting a project with DC battery storage"""
         self.Tracker_site: bool
         """Flag denoting a project with tracker-type racking"""
 
 
     def __repr__(self):
-        return 'Project object for {}'.format(self.project_name)
+        return f'{self.report_type_map[self.report_type]} Project object for {self.project_name}'
 
     
     def __str__(self):
-        return 'Project object for {}'.format(self.project_name)
+        return f'{self.report_type_map[self.report_type]} Project object for {self.project_name}'
 
 
     def _parse_config_file(self):
         """Reads data from config file & parses each sheet into a dataframe"""
         # Read variables from Plant Configuration File
         # `self.config_sheets` will store all the sheets from the config file as a dictionary
-        if self.last_update_config == os.path.getmtime(self.config_filepath):
+        if self.last_update_config == get_modified_time(self.config_filepath, self.data_platform, 'file'):
             return
+
         try:
             print("Loading config file for {}".format(self.project_name))
             self.config_sheets = pd.read_excel(self.config_filepath, sheet_name=None)
         except Exception:
-            error_num = sys.exc_info()[1].errno
+            error_num = sys.exc_info()[1].errno # type: ignore
             if error_num == 2:
                 error_msg = 'Config file not found for {}. Please verify the following file exists and try again: {}'.format(self.project_name, self.config_filepath)
                 # logger.error(error_msg)
                 raise FileNotFoundError(error_msg)
             elif error_num == 13:
                 error_msg = 'Config file is open for {}. Please close the file and try again'.format(self.project_name)
                 # logger.error(error_msg)
@@ -315,29 +346,37 @@
         ############# `Column_ID` tab #############
         # `colnames_ccr` is a list of the CCR column names
         # `colnames_das` is a list of the original column names from the project's DAS
         col_id_sheet = self.config_sheets['Column_ID']
 
         # Python 2 compatibility - old versions of Pandas would read the first column as the index, with new versions we have to set it explicitly
         if col_id_sheet.index.inferred_type == 'integer':
-            col_id_sheet.set_index(col_id_sheet.columns[0], inplace=True)
+            col_id_sheet = col_id_sheet.set_index(col_id_sheet.columns[0])
 
         self.config_column_map = col_id_sheet.iloc[2,:]
         self.colnames_ccr = self.config_column_map.index.tolist()
-        self.colnames_das = self.config_column_map.values.tolist()
+        self.colnames_das = self.config_column_map.values.tolist() # type: ignore
         self.non_error_cols = [col for col in self.colnames_ccr if 'ERROR' not in col]
 
         ########## `Sensor_Offline` tab ###########
         self.sensor_OFF = self.config_sheets['Sensor_Offline'].reset_index()
 
         ############## `Unit_Tab` tab #############
         self.Convert_Units = self.config_sheets['Unit_Tab']
 
         ################ `8760` tab ###############
-        self.df_Pvsyst = self.config_sheets['8760'].fillna(0)
+        # Only run UL or weekly for CCR owned projects
+        if self.df_proj_keys['Owner'] != 'CCR':
+            self.report_type = 'monthly'
+
+        # Option to run UL or weekly reports
+        if self.report_type.lower() == 'monthly':
+            self.df_Pvsyst = self.config_sheets['8760'].fillna(0)
+        else:
+            self.df_Pvsyst = self.config_sheets['UL_8760'].fillna(0)
         self.df_Pvsyst.loc[self.df_Pvsyst['Year 0 Actual Production (kWh)'] < 0, 'Year 0 Actual Production (kWh)'] = 0
 
         # Create date index from date column
         try:
             self.df_Pvsyst.loc[:, 'date'] = pd.to_datetime(self.df_Pvsyst.loc[:, 'date'])
             self.df_Pvsyst.set_index('date', inplace=True)
         except KeyError:
@@ -346,43 +385,48 @@
         # Get capacity & neighbor sensor params
         self.OFF_PEAK = self.config_dict['OFF_PEAK']
         self.CAPACITY_ON_PEAK_SUMMER = self.config_dict['CAPACITY_ON_PEAK_SUMMER']
         self.CAPACITY_ON_PEAK_NON_SUMMER = self.config_dict['CAPACITY_ON_PEAK_NON_SUMMER']
         self.Get_Sensor = self.df_config.loc[(self.df_config['Name'].str.lower() == 'get_sensor'), :]
         
         # Update last config update timestamp
-        self.last_update_config = os.path.getmtime(self.config_filepath)
+        self.last_update_config = get_modified_time(self.config_filepath, self.data_platform, 'file')
 
 
     def _load_bool_file(self):
         try:
-            if self.last_update_bool != os.path.getmtime(self.bool_filepath):
+            if self.last_update_bool != get_modified_time(self.bool_filepath, self.data_platform, 'file'):
                 self.df_bool = pd.read_csv(self.bool_filepath, index_col=0, parse_dates=True)
-                self.last_update_bool = os.path.getmtime(self.bool_filepath)
+                self.last_update_bool = get_modified_time(self.bool_filepath, self.data_platform, 'file')
         except:
             pass
 
 
     def _map_columns(self):
 
-        def get_col_locs(df_cols, colref):
+        def get_colnames(df_cols, colref):
             col_locs = [col for col in df_cols if colref in col]
             return col_locs
 
         # Read in column names from powertrack csv file - we won't read any rows since we just need the column names.
-        raw_df = pd.read_csv(self.powertrack_csv, index_col=0, nrows=0)
+        try:
+            raw_df = pd.read_csv(self.powertrack_csv, index_col=0, nrows=0)
+        except:
+            self.load_production_data()
+            raw_df = pd.read_csv(self.powertrack_csv, index_col=0, nrows=0)
+
 
         # Create column mappings based on sensor type
         raw_df_cols = raw_df.columns
-        tamb_cols = get_col_locs(raw_df_cols, 'Tamb')
-        tmod_cols = get_col_locs(raw_df_cols, 'Tmod')
-        wind_cols = get_col_locs(raw_df_cols, 'Wind_speed')
+        tamb_cols = get_colnames(raw_df_cols, 'Tamb')
+        tmod_cols = get_colnames(raw_df_cols, 'Tmod')
+        wind_cols = get_colnames(raw_df_cols, 'Wind_speed')
         temp_cols = tamb_cols + tmod_cols
         weather_cols = temp_cols + wind_cols
-        poa_cols = get_col_locs(raw_df_cols, 'POA')
+        poa_cols = get_colnames(raw_df_cols, 'POA')
 
         self.col_ref = {'Tamb_cols': tamb_cols,
                         'Tmod_cols': tmod_cols,
                         'Wind_cols': wind_cols,
                         'Temp_cols': temp_cols,
                         'Weather_cols': weather_cols,
                         'POA_cols': poa_cols,
@@ -390,20 +434,20 @@
 
         self.sensor_colmap = [Colmap(self.col_ref['Tamb_cols'], 'Tamb_avg'),
                               Colmap(self.col_ref['Tmod_cols'], 'Tmod_avg'),
                               Colmap(self.col_ref['Wind_cols'], 'Wind_speed'),
                               Colmap(self.col_ref['POA_cols'], 'POA_avg')]
 
     
-    def _find_neighbor_sensors(self):
+    def _find_config_neighbor_sensors(self):
         """Loops through all neighbor sensors listed in the config file and adds the
         `Project` to `neighbor_sensors`"""
         # TODO: check here if project already exists in DashboardSession & load it if not
         for neighbor_name in self.Get_Sensor['Source'].unique().tolist():
-            self.neighbor_sensors.add(neighbor_name)
+            self.config_neighbor_sensors.add(neighbor_name)
             
             
     def __get_project_parameters(self):
         """Checks that base parameters are present in `df_keys` & pulls the parameters from the config file if not"""
         params = [self.df_proj_keys['MWDC'], 
                   self.df_proj_keys['Delta_Tcnd'],
                   self.df_proj_keys['Temp_Coeff_Pmax'],
@@ -492,70 +536,124 @@
             self.Deg['Capacity'] = 1
             print('*** Degradation profile failed for {} ***'.format(self.project_name))
 
         # Fix year index to properly to 0.0, 0.5, 1.5 index steps per Jeff Webber spreadsheet
         self.Deg.set_index(np.append([0], np.arange(0.5, 40.5, 1)), inplace=True)
 
 
-    def _find_config_file(self):
+    def _find_config_file(self) -> str:
         # Build filename for config file
         config_filename = self.project_name + r'_Plant_Config_MACRO.xlsm'
         config_filepath = os.path.join(self.dashboard_dir,
                                         self.project_directory,
                                         self.project_name,
                                        'Plant_Config_File',
                                         config_filename)
 
-        if not os.path.isfile(config_filepath):
-            raise RuntimeError("*** No config file found for {}, skipping project. Check that filepath exists: {}".format(self.project_name, config_filepath))
+        config_filepath = Path(config_filepath)
+
+        if self.data_platform == 's3':
+            # Convert Windows-type filepath to use forwards slashes like a normal
+            config_filepath = config_filepath.as_posix().replace('s3:/', 's3://')
+            s3_filepath = make_s3_filepath(config_filepath, obj_type='file')
+            try:
+                s3_client.get_object(Bucket=s3_filepath.bucket, Key=s3_filepath.key)
+            except:
+                error_msg = f"*** No config file on S3 found for {self.project_name}, skipping project. Check that filepath exists: {config_filepath}"
+                raise RuntimeError(error_msg)
+            
+        else:
+            if not config_filepath.is_file():
+                error_msg = f"*** No config file on Sharepoint found for {self.project_name}, skipping project. Check that filepath exists: {config_filepath}"
+                raise RuntimeError(error_msg)
+
+            config_filepath = str(config_filepath)
 
         return config_filepath
 
 
     def _find_bool_file(self):
         # Build filename for bool file
         bool_filename = f"{self.year}_{self.project_name}_BOOL.csv"
         bool_filepath = os.path.join(self.dashboard_dir,
                                      self.project_directory,
                                      self.project_name,
                                      'Plant_Config_File',
                                      bool_filename)
 
+        bool_filepath = Path(bool_filepath)
+
+        if self.data_platform == 's3':
+            # Convert Windows-type filepath to use forwards slashes like a normal
+            bool_filepath = bool_filepath.as_posix().replace('s3:/', 's3://')
+        else:
+            bool_filepath = str(bool_filepath)
+
         return bool_filepath
 
 
     def _find_powertrack_file(self):
         # Find Powertrack folder
         self.data_AE_dir = os.path.join(self.dashboard_dir,
                                         self.project_directory,
                                         self.project_name,
                                         'Powertrack_data')
-        self.data_AE_all_files = [f for f in os.listdir(self.data_AE_dir) if os.path.isfile(os.path.join(self.data_AE_dir, f))]
-        data_AE = [s for s in self.data_AE_all_files if self.data_source in s]
+        
+        if self.data_platform == 's3':
+            s3_filepath = make_s3_filepath(self.data_AE_dir, obj_type='folder')
+            all_pt_files = s3_client.list_objects(Bucket=s3_filepath.bucket, Prefix=s3_filepath.key)
+            powertrack_filename = [f['Key'] for f in all_pt_files['Contents'] if self.data_source in f['Key']][0]
+            powertrack_filename = Path(powertrack_filename).name
+        else:
+            self.data_AE_all_files = [f for f in os.listdir(self.data_AE_dir) if os.path.isfile(os.path.join(self.data_AE_dir, f))]
+            powertrack_filename = [s for s in self.data_AE_all_files if self.data_source in s][0]
 
         # TODO: check on error handling here if we can't find the Powertrack file
-        if len(data_AE) == 0:
+        if len(powertrack_filename) == 0:
             raise PowertrackFileException("*** No Powertrack file found for {}, skipping project".format(self.project_name))
 
         # Build filename for Powertrack file
-        powertrack_filepath = os.path.join(self.dashboard_dir, self.project_directory, self.project_name, 'Powertrack_data', data_AE[0])
+        powertrack_filepath = Path(self.dashboard_dir) / self.project_directory / self.project_name / 'Powertrack_data' / powertrack_filename
         powertrack_csv = Path(powertrack_filepath).parent / f"{self.year}_hourly_{self.project_name}.csv"
 
+        if self.data_platform == 's3':
+            # Convert Windows-type filepath to use forwards slashes like a normal
+            powertrack_filepath = powertrack_filepath.as_posix().replace('s3:/', 's3://')
+            powertrack_csv = powertrack_csv.as_posix().replace('s3:/', 's3://')
+        else:
+            powertrack_filepath = str(powertrack_filepath)
+            powertrack_csv = str(powertrack_csv)
+        
         return powertrack_filepath, powertrack_csv
 
 
     def _find_pickle_jar(self):
         # Check for pickle jar folder & create if it doesn't exist
         pickle_jar = os.path.join(self.dashboard_dir,
                                        self.project_directory,
                                        self.project_name,
                                        'Pickle_Jar')
 
-        if not os.path.isdir(pickle_jar):
-            os.makedirs(pickle_jar)
+        pickle_jar = Path(pickle_jar)
+
+        if self.data_platform == 's3':
+            # Check that Pickle Jar exists & create folder if not
+            s3_filepath = make_s3_filepath(pickle_jar, obj_type='folder')
+            try:
+                s3_client.get_object(Bucket=s3_filepath.bucket, Key=s3_filepath.key)
+            except:
+                s3_client.put_object(Bucket=s3_filepath.bucket, Key=s3_filepath.key)
+
+            # Convert Windows-type filepath to use forwards slashes like a normal
+            pickle_jar = pickle_jar.as_posix().replace('s3:/', 's3://')
+        else:
+            if not pickle_jar.is_dir():
+                pickle_jar.mkdir()
+
+            pickle_jar = str(pickle_jar)
         
         return pickle_jar
 
 
     def load_production_data(self):
         """Loads production data from the Project's Powertrack file.
         If file has already been loaded, it will check
@@ -565,69 +663,72 @@
         """
 
         # Read Powertrack data
         # If the powertrack file has been updated since we last loaded production
         # we'll read the data from Excel & store a copy in df_powertrack
         # If it hasn't been updated we'll just use the powertrack copy we loaded previously
         try:
-            last_update_powertrack_file = os.path.getmtime(self.powertrack_filepath)
+            last_update_powertrack_file = get_modified_time(self.powertrack_filepath, self.data_platform, 'file')
         except:
             self.powertrack_filepath, self.powertrack_csv = self._find_powertrack_file()
-            last_update_powertrack_file = os.path.getmtime(self.powertrack_filepath)
+            last_update_powertrack_file = get_modified_time(self.powertrack_filepath, self.data_platform, 'file')
         
         if self.last_update_powertrack != last_update_powertrack_file:
             self.__load_from_source(self.powertrack_filepath)
         else:
             # If we try to load from `df_powertrack` and it doesn't exist we'll need to load from source
             try:
                 self.df = self.df_powertrack.copy()
+                self.df.set_index(pd.to_datetime(self.df.index))
                 print('Using previously loaded Powertrack file for {}'.format(self.project_name))
             except AttributeError:
                 self.__load_from_source(self.powertrack_filepath)
             
         # Find native sensors, used to find DAS_ON instead of all sensors.
         # Avoids using Get_Sensor data from another site
         val = ['Meter_kw_', 'POA', 'GHI', 'Wind_speed', 'Inv_kw_', 'Inv_kwnet', 'Tmod', 'Tamb']
         self.pos_Native = [s for s in self.df.columns if any([x in s for x in val])]
 
         # Convert production data to hourly values
+        # Replace any blank strings with NaN
+        self.df = self.df.replace(r'^\s*$', np.nan, regex=True)
         self.df = self.df.resample('h').mean()
 
         # Initialize & populate sensor_ON dataframe
-        self.df_sensor_ON = pd.DataFrame(columns=self.df.columns.tolist(), index=self.df.index).fillna(True).astype(object)
+        self.df_sensor_ON = pd.DataFrame(columns=self.df.columns.tolist(), index=self.df.index).fillna(True).astype(bool)
 
-        # Disable any faulty sensors defined in the config file
+        # Initialize POA_source column & disable any faulty sensors defined in the config file
+        self.df.loc[:, 'POA_source'] = 'Native'
         self._config_disable_sensors()
 
 
     def __load_from_source(self, filepath):
         print('Loading Powertrack data for {}'.format(self.project_name))
         # Load data from Excel
         try:
             self.df = pd.read_excel(filepath, sheet_name='Sheet1', skiprows=0, index_col=0)
         except IOError as e:
-            error_num = e[0]
+            error_num = e.errno
             if error_num == 2:
                 error_msg = 'Powertrack file not found for {}. Please verify the following file exists and try again: {}'.format(self.project_name, self.config_filepath)
                 # logger.error(error_msg)
                 raise FileNotFoundError(error_msg)
             elif error_num == 13:
                 error_msg = 'Powertrack file is open for {}. Please close the file and try again'.format(self.project_name)
                 # logger.error(error_msg)
                 raise FileOpenError(error_msg)
             else:
-                error_msg = e
-                raise Exception(error_msg)
+                raise Exception(traceback.format_exc())
 
         # Curtail date to max of `data_cutoff_date`
         self.df = self.df.loc[self.df.index < self.data_cutoff_date, :]
 
         # Apply CCR column names to df
         self.colnames_ccr = self.config_column_map.index.tolist()
-        self.colnames_das = self.config_column_map.values.tolist()
+        self.colnames_das = self.config_column_map.values.tolist() # type: ignore
         self.non_error_cols = [col for col in self.colnames_ccr if 'ERROR' not in col]
 
         # This top case happens if some columns are removed from the
         # Powertrack file after the COLUMN_ID tab has been set up in the config file
         if len(self.df.columns) < len(self.colnames_ccr):
             list1 = self.df.columns.tolist()
             list2 = self.colnames_das
@@ -642,76 +743,71 @@
 
         # Remove error columns
         self.df = self.df.reindex(columns=self.non_error_cols)
 
         # Copy columns if necessary - most commonly used to map inverters to meters
         # at sites where we don't have standalone meters & use the inverters as a proxy
         Copy_Sensor = self.df_config.loc[(self.df_config['Name'].str.lower() == 'copy_sensor'), :]
-        Copy_from = Copy_Sensor['Value'].values.tolist()
-        Copy_to = Copy_Sensor['Source'].values.tolist()
+        Copy_from = Copy_Sensor['Value'].values.tolist() # type: ignore
+        Copy_to = Copy_Sensor['Source'].values.tolist() # type: ignore
         for _from, _to in zip(Copy_from, Copy_to):
             self.df[_to] = self.df[_from]
             self.colnames_ccr = self.colnames_ccr + [_to]
 
         # Locate columns
         self._locate_column_positions()
 
         # Perform any unit conversions needed
         self._convert_sensor_units()
 
         # Update the last updated date for the powertrack file
-        self.last_update_powertrack = os.path.getmtime(self.powertrack_filepath)
+        self.last_update_powertrack = get_modified_time(self.powertrack_filepath, self.data_platform, 'file')
         self.df_powertrack = self.df.copy()
 
         # Write to csv
         self.df.to_csv(self.powertrack_csv)
 
 
-    def _fetch_solcast_data(self):
-        if self.df_solcast.empty:
-            print(f"Fetching solcast data for {self.project_name}")
+    def _fetch_bluesky_data(self):
+        # If solcast data hasn't been loaded from AWS or the indexes of the main df & df_bluesky don't match - load data
+        if self.df_bluesky.empty or self.df_bluesky.index[0] != self.df.index[0] or self.df_bluesky.index[-1] != self.df.index[-1]:
             start_date = self.df.index[0]
             end_date = self.df.index[-1]
-            df_solcast = self.run_bluesky(start=start_date, end=end_date, plot=False)
-
-            # Drop ghi column as it's not needed anymore
-            df_solcast = df_solcast.drop(columns='ghi')
 
-            # Attempt to pull transposed GHI if available
-            try:
-                tran_ghi = df_solcast['sites_ghi_poa']
+            fetch_ghi = False
+            if self.pos_GHI:
+                fetch_ghi = True
+            df_bluesky = self.pv_model.run_bluesky(start_date, end_date, resample=True, fetch_ghi=fetch_ghi) # type: ignore
+            # df_bluesky = df_bluesky.fillna(0)
 
-                # Pass transposed GHI column through daylight zeroes filter to make sure the data is good
-                # (the filter returns True where there are daylight zeroes so we need to invert it)
-                tran_ghi_bool = ~det.daylight_zeroes(df=tran_ghi, project=self)
+            # # (the filter returns True where there are daylight zeroes so we need to invert it)
+            # proj_ghi_poa = df_project_ghi.join(project_poa['poa_global'])
+            # proj_ghi_bool = ~det.daylight_zeroes(df=proj_ghi_poa, pv_model=self)
 
-                # Convert all False values (bad data) to np.inf so we can replace with NaN after reindexing in the next step
-                tran_ghi_bool = tran_ghi_bool.replace(False, np.inf)
+            # # Convert all False values (bad data) to np.inf so we can replace with NaN after reindexing in the next step
+            # proj_ghi_bool = proj_ghi_bool.replace(False, np.inf)
 
-                # Reindex to add nighttime rows back in & set them to False so they don't change the data in the original df
-                tran_ghi_bool = tran_ghi_bool.reindex(index=tran_ghi.index).fillna(False)
+            # # Reindex to add nighttime rows back in & set them to False so they don't change the data in the original df
+            # proj_ghi_bool = proj_ghi_bool.reindex(index=proj_ghi_poa.index).fillna(False)
 
-                # Replace np.inf with np.nan (we used np.inf to demarcate bad data so it wouldn't be overwritten in the step above)
-                tran_ghi_bool = tran_ghi_bool.replace(np.inf, np.nan)
+            # # Replace np.inf with np.nan (we used np.inf to demarcate bad data so it wouldn't be overwritten in the step above)
+            # proj_ghi_bool = proj_ghi_bool.replace(np.inf, np.nan)
 
-                # Filter out bad data
-                tran_ghi = tran_ghi*tran_ghi_bool
+            # # Filter out bad data
+            # proj_ghi_poa = (proj_ghi_poa*proj_ghi_bool).astype(float)
 
-                # Fill in any NaNs with satellite POA
-                tran_ghi = tran_ghi.fillna(df_solcast['poa'])
+            # # Fill in any NaNs with satellite data
+            # proj_ghi_poa = proj_ghi_poa.fillna({'proj_ghi': df_bluesky['sat_ghi'], 'poa_global': df_bluesky['sat_poa']})
 
-                # Rename & drop column `sites_ghi_poa` column to match sites with no GHI
-                df_solcast['poa'] = tran_ghi
-                df_solcast = df_solcast.drop(columns='sites_ghi_poa')
-            except KeyError:
-                # No `sites_ghi_poa` column, use satellite POA instead
-                pass
+            # # Rename & drop column `sites_ghi_poa` column to match sites with no GHI
+            # df_bluesky[['ghi', 'poa']] = proj_ghi_poa[['proj_ghi', 'poa_global']]
 
             # Rename to match sensor avg columns & replace NaNs
-            self.df_solcast = df_solcast.rename(columns={'Tamb': 'Tamb_avg', 'Tmod': 'Tmod_avg', 'poa': 'POA_avg'})
+            self.df_bluesky = df_bluesky.rename(columns={'Tamb': 'Tamb_avg', 'Tmod': 'Tmod_avg',
+                                                         'poa': 'POA_avg', 'ghi': 'GHI_avg'})
 
   
     def _locate_column_positions(self):
         # Find Meters
         self.pos_Meter = [s for s in self.df.columns if 'Meter_kw_' in s]
         # Find CUM Meters
         self.pos_Meter_Cum = [s for s in self.df.columns if 'Meter_kwhnet_' in s]
@@ -737,61 +833,93 @@
         #  Battery site cols
         self.pos_BatteryAC = [s for s in self.df.columns if 'BatteryAC_kw_' in s]
         self.pos_BatteryAC_del = [s for s in self.df.columns if 'BatteryAC_kwhdel_' in s]
         self.pos_BatteryAC_rec = [s for s in self.df.columns if 'BatteryAC_kwhrec_' in s]
 
         # Find all tracker position sensors
         self.pos_Tracker = [s for s in self.df.columns if 'Tracker_position' in s]
-        # self.Tracker_site = not (self.pos_Tracker == [])
         
 
     def _convert_sensor_units(self):
         """
 
         """
         # Perform unit conversions that are found in the configuration file
         if np.any(['Convert_Multiply' in s for s in list(self.Convert_Units.columns)]):
             Convert_custom = self.Convert_Units.loc[~self.Convert_Units['Convert_Multiply'].isnull(), ['Var_ID', 'Convert_Multiply']]
             for index, row in Convert_custom.iterrows():
                 self.df[row['Var_ID']] = self.df[row['Var_ID']] * row['Convert_Multiply']
 
         # Convert sensor units
-        Convert_Temperature = self.Convert_Units.loc[self.Convert_Units['Convert_Farenheit_to_Celcius'] == True, 'Var_ID'].values.tolist()
+        Convert_Temperature = self.Convert_Units.loc[self.Convert_Units['Convert_Farenheit_to_Celcius'] == True, 'Var_ID'].values.tolist() # type: ignore
         for t_sensor in Convert_Temperature:
             self.df[t_sensor] = (self.df[t_sensor] - 32.0) * 5.0 / 9.0
 
-        Convert_wind = self.Convert_Units.loc[self.Convert_Units['Convert_mph_to_mps'] == True, 'Var_ID'].values.tolist()
+        Convert_wind = self.Convert_Units.loc[self.Convert_Units['Convert_mph_to_mps'] == True, 'Var_ID'].values.tolist() # type: ignore
         for wind in Convert_wind:
             self.df[wind] = self.df[wind] * 0.44704
 
 
     def get_columns(self):
         """Prints out CCR column names with their location in the Project's
         Powertrack file and a map to its DAS column name.
         """
         intake = self.pos_Meter + self.pos_Meter_Cum + self.pos_Inv + self.pos_Inv_cum
-        columns_df=DataFrame(data={'Column':[],'Position':[],'OG Name':[]})
+        columns_df=pd.DataFrame(data={'Column':[],'Position':[],'OG Name':[]})
         #lists out the column names and index for the lists. 
         for x in intake: 
             try:
                 column=x
                 position=xlsxwriter.utility.xl_col_to_name(self.colnames_ccr.index(x)+1)
                 og=self.colnames_das[self.colnames_ccr.index(x)]
-                temp=DataFrame(data={'Column':[column],'Position':[position],'OG Name':[og]})
+                temp=pd.DataFrame(data={'Column':[column],'Position':[position],'OG Name':[og]})
                 columns_df=columns_df.append(temp)
             except IndexError:
                 continue
 
         print('\n')
         print('Column locations for {}:'.format(self.project_name))
         print(columns_df[['Column','Position','OG Name']])
         print('\n')
 
 
-    def get_ss_comments(self, num_comments: int=None):
+    def get_sensors(self):
+        """Prints out the location of POA & weather sensors in a Project's
+        Powertrack file and a map to its DAS column name.
+        """
+        columns_df=pd.DataFrame(data={'Column':[],'Position':[],'OG Name':[]})
+        for x in self.pos_POA: #lists out the column names and index for the lists.
+            if len(x) < 7:
+                column=x
+                position=xlsxwriter.utility.xl_col_to_name(self.colnames_ccr.index(x)+1)
+                og=self.colnames_das[self.colnames_ccr.index(x)]
+                temp=pd.DataFrame(data={'Column':[column],'Position':[position],'OG Name':[og]})
+                columns_df=columns_df.append(temp)
+        for x in self.pos_Temperature: #lists out the column names and index for the lists.
+            if len(x) < 7:
+                column=x
+                position=xlsxwriter.utility.xl_col_to_name(self.colnames_ccr.index(x)+1)
+                og=self.colnames_das[self.colnames_ccr.index(x)]
+                temp=pd.DataFrame(data={'Column':[column],'Position':[position],'OG Name':[og]})
+                columns_df=columns_df.append(temp)
+        for x in self.pos_Wind: #lists out the column names and index for the lists.
+            if len(x) < 13:
+                column=x
+                position=xlsxwriter.utility.xl_col_to_name(self.colnames_ccr.index(x)+1)
+                og=self.colnames_das[self.colnames_ccr.index(x)]
+                temp=pd.DataFrame(data={'Column':[column],'Position':[position],'OG Name':[og]})
+                columns_df=columns_df.append(temp)
+        columns_df = columns_df.set_index('Column')
+        print('\n')
+        print('Sensor locations for {}:'.format(self.project_name))
+        print(columns_df[['Position','OG Name']])
+        print('\n')
+
+
+    def get_ss_comments(self, num_comments: int|None=None):
         """Prints Smartsheet comments for the Project
 
         Args:
             num_comments (int): Number of comments to show, starting from the
                 most recent. Defaults to None, which will show all comments.
         """
         
@@ -806,48 +934,45 @@
             comment_list = list(self.df_proj_ss_comments.items())[-num_comments:]
         else:
             comment_list = list(self.df_proj_ss_comments.items())
         for dt, comment in comment_list:
             print(dt + ': ', comment)
     
 
-    def get_sensors(project):
-        """Prints out the location of POA & weather sensors in a Project's
-        Powertrack file and a map to its DAS column name.
+    def get_datasub_stats(self, add_sparklines:bool = True) -> pd.DataFrame|HTML:
+        """Returns statistics from a daily linear regression on Solcast POA & GHI values.
+
+        Returns:
+            pd.DataFrame: Linear regression statistics for each day the analysis was run.
+                <ul>
+                    <li>`rPOA`: The R-value in relation to the Solcast POA</li>
+                    <li>`mPOA`: The slope in relation to the Solcast POA</li>
+                    <li>`rGHI`: The R-value in relation to the Solcast GHI</li>
+                    <li>`mGHI`: The slope in relation to the Solcast GHI</li>
+                </ul>
         """
-        columns_df=DataFrame(data={'Column':[],'Position':[],'OG Name':[]})
-        for x in project.pos_POA: #lists out the column names and index for the lists.
-            if len(x) < 7:
-                column=x
-                position=xlsxwriter.utility.xl_col_to_name(project.colnames_ccr.index(x)+1)
-                og=project.colnames_das[project.colnames_ccr.index(x)]
-                temp=DataFrame(data={'Column':[column],'Position':[position],'OG Name':[og]})
-                columns_df=columns_df.append(temp)
-        for x in project.pos_Temperature: #lists out the column names and index for the lists.
-            if len(x) < 7:
-                column=x
-                position=xlsxwriter.utility.xl_col_to_name(project.colnames_ccr.index(x)+1)
-                og=project.colnames_das[project.colnames_ccr.index(x)]
-                temp=DataFrame(data={'Column':[column],'Position':[position],'OG Name':[og]})
-                columns_df=columns_df.append(temp)
-        for x in project.pos_Wind: #lists out the column names and index for the lists.
-            if len(x) < 13:
-                column=x
-                position=xlsxwriter.utility.xl_col_to_name(project.colnames_ccr.index(x)+1)
-                og=project.colnames_das[project.colnames_ccr.index(x)]
-                temp=DataFrame(data={'Column':[column],'Position':[position],'OG Name':[og]})
-                columns_df=columns_df.append(temp)
-        columns_df = columns_df.set_index('Column')
-        print('\n')
-        print('Sensor locations for {}:'.format(project.project_name))
-        print(columns_df[['Position','OG Name']])
-        print('\n')
 
+        poa_cols = self.col_ref['POA_cols']
+        df_poa = self.df[poa_cols]
+        df_poa_w_bs = df_poa.join(self.df_bluesky[['sat_ghi', 'sat_poa', 'proj_ghi', 'proj_ghi_poa']])
+        df_poa_w_bs = df_poa_w_bs.rename(columns={'sat_ghi': 'Satellite GHI',
+                                                  'sat_poa': 'Satellite POA',
+                                                  'proj_ghi': 'Project GHI',
+                                                  'proj_ghi_poa': 'Trans POA'})
 
-    def find_nearby_projects(self, dist:int=10, print_data:bool=True, include_retired:bool=False, df:DataFrame=None) -> DataFrame:
+        # Find trackers that aren't tracking
+        tracker_poa, datasub_stats = det.daylight_poa_mistracking(df=df_poa_w_bs, pv_model=self.pv_model, add_sparklines=add_sparklines, degree=8) # type: ignore
+        if add_sparklines:
+            # _repr_html_ escapes HTML so manually handle the rendering
+            datasub_stats = HTML(datasub_stats.to_html(escape=False))
+
+        return datasub_stats
+
+
+    def find_nearby_projects(self, dist:int = 10, print_data:bool = True, include_retired:bool = False, df:pd.DataFrame = pd.DataFrame()) -> pd.DataFrame:
         """Creates a list of Projects within a certain distance of the reference Project.
 
         Args:
             dist (int): Number of miles to search around the reference Project`
             print_data (bool): Option to print the data in the console. If False,
                 the DataFrame will be returned without printing out the contents.
             include_retired (bool): Option to include retired Projects in the search.
@@ -858,15 +983,15 @@
         Returns:
             Information about all Projects within the specified distance from the reference Project.
         """
         ns = neighbs.find_nearby_projects(self.project_name, dist, print_data, include_retired, df)
         return ns
     
 
-    def find_nearby_similar_projects(self, dist:int=10, print_data:bool=True, include_retired:bool=False, df:DataFrame=None) -> DataFrame:
+    def find_nearby_similar_projects(self, dist:int=10, print_data:bool=True, include_retired:bool=False, df:pd.DataFrame=pd.DataFrame()) -> pd.DataFrame:
         """Creates a list of Projects within a certain distance of the reference
         Project that share similar racking properties. 
 
         * Similar Racking Criteria:
             * Same racking OEM
             * Fixed tilt:
                 * Same module tilt
@@ -879,21 +1004,21 @@
             include_retired (bool): See [find_nearby_projects()][ccrenew.dashboard.project.Project.find_nearby_projects]
             df (Dataframe): See [find_nearby_projects()][ccrenew.dashboard.project.Project.find_nearby_projects]
 
         Returns:
             Information about all Project within a certain distance
                 of the reference Project that share similar racking properties.
         """
-        nss = neighbs.find_nearby_similar_projects(self.project_name, dist, print_data, include_retired, df=None)
+        nss = neighbs.find_nearby_similar_projects(self.project_name, dist, print_data, include_retired, df=df)
         return nss
 
 
-    def run_bluesky(self, start: DateLike=None, end: DateLike=None, tran_ghi: str='add',
+    def run_bluesky(self, start: DateLike|None=None, end: DateLike|None=None, tran_ghi: str='add',
                 convert: bool=False, resample: bool=True, ghi_index: int=0, axis_tilt: int=0,
-                albedo: int=1, plot: bool=True, pool_size: int=6) -> pd.DataFrame:
+                surface_albedo: float=0.2, plot: bool=True, pool_size: int=6) -> None:
         """
         Pulls irradiance & weather data from Solcast for the Project & date range.
 
         Args:
             start (str or datetime): The start date for Solcast data. Default
                 will set it to the first day of the current month.
             end (str or datetime): The end date for Solcast data. Default will
@@ -904,24 +1029,26 @@
                     * `add` to add it to the df_cats dataframe.
                     * `only` to pull just the transposed GHI & not df_cats.
                     * `none` to pull just df_cats.
 
             plot (bool): Option to draw plots of the data from solcast.
 
         Returns:
-            df_solcast (pd.DataFrame): The Solcast irradiance & weather data.
+            df_bluesky (pd.DataFrame): The Solcast irradiance & weather data.
         """
         func_args = locals().copy()
         func_args.pop('self')
-        df_cats = utils.run_bluesky(self.project_name, **func_args)
+        # if self.df_bluesky.empty:
+        #     self.df_bluesky = blu.get_weather_data()
+        # df_cats = utils.run_bluesky(self.project_name, **func_args)
+        print("`Project.run_bluesky()` not currently implemented. Please use `Project.pvmodel.run_bluesky()`")
+        # return df_cats
 
-        return df_cats
 
-
-    def generate_power_from_invoice(self, start:Union[str, datetime], stop:Union[str, datetime], total_energy:Number, clipping_limit:Number=None) -> DataFrame:
+    def generate_power_from_invoice(self, start:str|datetime, stop:str|datetime, total_energy:Numeric, clipping_limit:Numeric|None=None) -> pd.DataFrame:
         """Generates power based upon [P_exp][ccrenew.dashboard.project.Project.P_exp].
         User needs to ensure that all weather and irradiance data are filled in before running this script.
 
         Args:
             start (str or datetime): Start date for calculations.
             stop (str or datetime): End date for calculations.
             total_energy (Number): Total energy (per meter) from the invoice to fill in over the date range.
@@ -934,22 +1061,22 @@
             clipping_limit = self.clipping_KW
         #use expected power (or POA though expected power is probs better)
         # QUESTION: DO WE WANT TO USE POWER OR POA HERE?
         #power_proportions will have a sum of 1, it represents what portion of power is contained in that hour
         power_proportions=self.df['P_exp'][start:stop]/(self.df['P_exp'][start:stop].sum())
         # power_proportions=project.df['POA_avg'][start:stop]/(project.df['POA_avg'][start:stop].sum())
 
-
         #get difference between curated power and actual invoiced to aim for 0
         remainder=total_energy
         #initiate a power_iterative term, its really the power when you remove points over clipping
         power_i= power_proportions*0
         
         #iteratively spread production over the month based on expected until remainder is near 0
         i = 0
+        power_data = pd.DataFrame()
         while remainder >(total_energy/(10*10**8)): #while loop instead of for because i am seeking a goal, not an amount of iterations
             power_data=(power_proportions*remainder)+power_i
             power_i=power_data.clip(upper=clipping_limit) #gets rid of points over clipping
             remainder=(power_data-power_i).sum()
             i+=1
             if i > 10000:
                 break
@@ -958,156 +1085,173 @@
         print('Power data successfully generated for {}'.format(self.project_name))
         print('\n')
         return power_data
 
 
     def plot_meters(self):
         """Plots all meters for the Project"""
-        if not self.plotter:
-            self.plotter = Plotter(self)
-        self.plotter.draw_dashboard_plots(plot_order='meters', close_plots=False)
+        # We'll check if the project is processed & process it if not.
+        # We won't flip the processed flag because we don't have neighbor data from a session
+        if not self.processed:
+            self._load_bool_file()
+            self.load_production_data()
+            self._process_data(neighbor_sensor_data={}, datasub=False, use_bluesky=False)
+            self.last_update_powertrack = datetime.fromtimestamp(0)
+        self.plotter.draw_plots(plot_order='meters', close_plots=False)
 
 
     def plot_snow(self):
         """Plots snow data for the Project"""
-        if not self.plotter:
-            self.plotter = Plotter(self)
-        self.plotter.draw_dashboard_plots(plot_order='snow', close_plots=False)
+        # We'll check if the project is processed & process it if not.
+        # We won't flip the processed flag because we don't have neighbor data from a session
+        if not self.processed:
+            self._load_bool_file()
+            self.load_production_data()
+            self._process_data(neighbor_sensor_data={}, datasub=False, use_bluesky=False)
+            self.last_update_powertrack = datetime.fromtimestamp(0)
+        self.plotter.draw_plots(plot_order='snow', close_plots=False)
 
 
     def save_pickle(self, store_plots=False):
         """Saves the Project object to a pickle in the
         [project_directory][ccrenew.dashboard.project.Project.project_directory].
         """
         if not store_plots and self.plotter:
-            self.plotter = None
+            self.plotter.plot_list = {}
         year = self.year
         pickle_name = utils.picklefy_project_name(self.project_name)
         pickle_file = str(year) + "_" + pickle_name + ".pickle"
-        pickle_path = os.path.join(self.pickle_jar, pickle_file)
+        pickle_path_sharepoint = Path(self.data_platform_dirs.sharepoint) / self.project_directory / self.project_name / 'Pickle_Jar' / pickle_file
+        pickle_path_s3 = Path(self.data_platform_dirs.s3) / self.project_directory / self.project_name / 'Pickle_Jar' / pickle_file
+        pickle_path_s3 = pickle_path_s3.as_posix().replace('s3:/', 's3://')
         
-        with open(pickle_path, 'wb') as f:
+        with open(pickle_path_sharepoint, 'wb') as f:
             pickle.dump(self, f)
         
+        fs = s3fs.S3FileSystem()
+        with fs.open(pickle_path_s3, 'wb') as f:
+            pickle.dump(self, f)
+
 
-    def get_tracker_ava(self) -> DataFrame:
+    def get_tracker_ava(self) -> pd.DataFrame:
         """Calculates tracker ava for the Project.
 
         Returns:
             Tracker ava.
         """
-        year = int(self.df.index[0].year)
         # create an empty df to avoid issues with sites w/o data
-        start = '1/1/'+str(year)
-        end = '12/31/'+str(year)
+        start = '1/1/'+str(self.year)
+        end = '12/31/'+str(self.year)
         index = pd.date_range(start, end)
         columns = [u'Ava', u'Ava NaN', u'Ava No Interp', u'Ava Variance', u'Date', u'Site', u'Type']
         df_hist = pd.DataFrame(index=index, columns=columns)
 
         # get sites that actually have data
         tracker_prefix = 'Tracker_data_pf/Ava_History/'
         bucket = 'perfdatadev.ccrenew.com'
         key = tracker_prefix+self.project_name+'.csv'
         df_hist2 = utils.retrieve_s3_df(bucket, key)
         if len(df_hist2) > 0:
-            df_hist2.index = pd.to_datetime(df_hist2['Date'])
-            df_hist2 = df_hist2[df_hist2.index.year == year]
+            df_hist2 = df_hist2.set_index(pd.to_datetime(df_hist2['Date']))
+            df_hist2 = df_hist2[df_hist2.index.year == self.year] # type: ignore
             # combine together and resample
             df_hist = df_hist.combine_first(df_hist2)
 
             df_hist = df_hist.resample('M').mean()
         else:
             df_hist = df_hist.resample('M').asfreq()
 
         df_hist = df_hist[['Ava', 'Ava NaN', 'Ava No Interp', 'Ava Variance']]
         df_hist.columns = ['tracker_ava', 'tracker_ava_nan', 'tracker_ava_interpremoved', 'tracker_variance_ava']
         df_hist.loc[df_hist.index < '7/1/2020'] = np.nan
         return df_hist
 
     
-    def export(self, server: str='dev', save_pickle: bool=True, dest: Union[str, list]='all') -> None:
+    def export(self, server: str, dest: Union[str, list], save_pickle: bool, report_type:str, **kwargs) -> None:
         """
         Export project to desired location(s).
 
         Args:
-            save_pickle (bool): Option to save pickle after exporting.
             server (str): SQL table to export to. Options are `prod` or `dev`.
-            dest (str or list): Option to export only certain parts of the project. `all` will export to all of the below destinations.
+            dest (str or list): Option to export only certain parts of the project.
+                `all` will export to all of the below destinations **except bool**.
+            save_pickle (bool): Option to save pickle after exporting.
 
         `dest` Options
 
         | dest      | Description                                                              |
         |-----------|--------------------------------------------------------------------------|
         |  `excel`  | Export dataframes to Excel dashboard template.                          |
         |   `df`    | Export dataframe to the `Dataframes` folder of the project's [project_directory][ccrenew.dashboard.project.Project.project_directory], S3, and Bartertown PostgreSQL database. |
         | `summary` | Export monthly summary data to S3 and Bartertown PostgreSQL database.   |
         |  `snow`   | Export [snow_data][ccrenew.dashboard.project.Project.snow_data] and [snow_coverage][ccrenew.dashboard.project.Project.snow_coverage] dataframes to S3. |
         |  `bool`   | Export bool file to the `Plant_Config_File` directory of the project's [project_directory][ccrenew.dashboard.project.Project.project_directory]. |
         """
-        def call_func(func, server):
-            func(server)
+        # Add positionals to kwargs
+        kwargs['server'] = server
+        kwargs['dest'] = dest
+        kwargs['save_pickle'] = save_pickle
+        kwargs['report_type'] = report_type
+
+        def call_func(func, **kwargs):
+            func(**kwargs)
 
         export_dict = {
-            'excel': self.export_excel,
-            'df': self.export_df,
-            'summary': self.export_summary,
-            'snow': self.export_snow,
-            'bool': self.export_bool
+            'excel': self._export_excel,
+            'df': self._export_df,
+            'summary': self._export_summary,
+            'snow': self._export_snow,
+            'weekly': self._export_weekly,
+            'bool': self._export_bool
         }
-        if dest == 'all':
+        if server.lower() == 'datasub':
+            dest = 'summary'
+        
+        if report_type.lower() == 'weekly':
+            dest = ['summary', 'weekly']
+        else:
+            export_dict.pop('weekly')
+
+        if isinstance(dest, str) and dest.lower() == 'all':
+            export_dict.pop('bool')
             for func in export_dict.values():
-                call_func(func, server)
+                call_func(func, **kwargs)
         else:
             if isinstance(dest, str):
                 func = export_dict[dest]
-                call_func(func, server)
+                call_func(func, **kwargs)
             elif isinstance(dest, Iterable):
                 for d in dest:
                     func = export_dict[d]
-                    call_func(func, server)
+                    call_func(func, **kwargs)
             else:
                 raise TypeError("`dest` must be a string or list. Please update input and resubmit.")
         
+        if dest == 'bool':
+            save_pickle = False
+
         if save_pickle:
             self.save_pickle()
 
 
-    def export_bool(self, server: str='dev') -> None:
-        """
-        Export the bool file for the project.
-
-        Args:
-            server (str): `prod` will update the BOOL file in the `Plant_Config_File` directory of the project's
-                [project_directory][ccrenew.dashboard.project.Project.project_directory].
-                `dev` will create a temporary file to test the export functionality then delete it.
-        """
-        # Update bool file
-        self._update_bool()
-
-        if server == 'dev':
-            filepath = Path(self.bool_filepath)
-            dev_filepath = filepath.parent / f"{filepath.stem}_dev{filepath.suffix}"
-            self.df_bool.to_csv(dev_filepath)
-            os.remove(dev_filepath)
-        else:
-            self.df_bool.to_csv(self.bool_filepath)
-
-
-    def export_excel(self, server:str='dev'):
+    def _export_excel(self, **kwargs) -> None:
         """
         Exports Dataframes to Excel dashboard template in the project's [project_directory][ccrenew.dashboard.project.Project.project_directory].
 
         Args:
             server (str): Option to insert data to prod or dev environments.
                 <ul>
                     <li><code>dev</code> will export the data to Excel to test if any errors then delete the file.</li>
                     <li><code>test</code> will export the Excel sheet to the project's <code>project_directory</code></li>
                 </ul>
 
         """
+        server = kwargs.get('server')
+        report_type = kwargs.get('report_type')
+
         template_filename = 'Dashboard_v07.xlsx'
         self.metadata = pd.DataFrame([], index=[1])
         self.metadata['date'] = str(datetime.now())
         self.metadata['username'] = os.getenv('username')
         self.metadata['version'] = sys.version
         try:
             self.metadata['filename'] = __file__
@@ -1139,127 +1283,152 @@
         #                    'Table_rev', 'data_day', 'Guarantee', 'Metadata']
 
         # Build filename for Excel output
         if self.project_name == 'Old Pageland Monroe Road Solar Farm':
             project_name = 'Old Pageland'
         else:
             project_name = self.project_name
+
         ts = datetime.now().strftime("%Y-%m-%d-T%H%M%m")
-        output_filename = project_name + '_' + ts +'.xlsx'
+        s3_filename = project_name + '_' + ts +'.xlsx'
+        sharepoint_filename = project_name + '.xlsx'
 
-        #  Create a copy of template and rename it in project folder to save analysis
-        template_filepath = os.path.join(self.dashboard_dir, 'Python_Functions', 'Dashboard_Template', template_filename)
-        output_dir = os.path.join(self.dashboard_dir, self.project_directory, self.project_name)
-        shutil.copy(template_filepath, output_dir)
-        output_template = os.path.join(output_dir, template_filename)
-        output_filepath = os.path.join(output_dir, output_filename)
-        os.rename(output_template, output_filepath)
+        if report_type.lower() == 'ul':
+            s3_filename = s3_filename.replace('.xlsx', '_UL.xlsx')
+            sharepoint_filename = sharepoint_filename.replace('.xlsx', '_UL.xlsx')
+
+        if server.lower() != 'prod':
+            s3_filename = s3_filename.replace('.xlsx', '_COPY.xlsx')
+            sharepoint_filename = sharepoint_filename.replace('.xlsx', '_COPY.xlsx')
+
+        # Create a copy of template in sharepoint
+        dashboard_root_dir = Path(self.data_platform_dirs.sharepoint)
+        template_filepath = dashboard_root_dir / 'Python_Functions' / 'Dashboard_Template' / template_filename
+        output_dir = dashboard_root_dir / self.project_directory / self.project_name
+        output_template = shutil.copy(template_filepath, output_dir)
+        output_filepath = output_dir / sharepoint_filename
+        try:
+            os.rename(output_template, output_filepath)
+        except FileExistsError:
+            os.remove(output_filepath)
+            os.rename(output_template, output_filepath)
 
+        # Write data to file on sharepoint
         df_tools.dfs_to_excel(output_filepath, df_dict)
-        if server == 'dev':
+
+        # Store copy on S3 with export timestamp
+        s3_filepath = Path(self.data_platform_dirs.s3) / self.project_directory / self.project_name / s3_filename
+        s3_filepath = make_s3_filepath(s3_filepath, obj_type='file')
+        bucket = s3_filepath.bucket
+        key = s3_filepath.key
+        s3_client.upload_file(output_filepath, Bucket=bucket, Key=key)
+
+        if server != 'prod':
             os.remove(output_filepath)
-    
+            s3_client.delete_object(Bucket=bucket, Key=key)
 
-    def export_df(self, server='dev'):
+    def _export_df(self, **kwargs) -> None:
         """
         Export dataframe to the `Dataframes` folder of the project's [project_directory][ccrenew.dashboard.project.Project.project_directory], S3, and Bartertown PostgreSQL database.
 
         Args:
             server (str): Option to insert data to prod or dev environments.
                 <ul>
-                    <li><code>dev</code> corresponds to <code>dev_analytic.am_processed_data</code> and <code>cypress-perfeng-datalake-dev-us-west-2</code>.</li>
-                    <li><code>test</code> corresponds to <code>dev_analytic.am_processed_data_dev</code> and <code>cypress-perfeng-datalake-onprem-us-west-2</code>.</li>
+                    <li><code>dev</code> corresponds to <code>dev_analytic.am_processed_data_dev</code> and <code>cypress-perfeng-datalake-onprem-us-west-2</code>.</li>
+                    <li><code>prod</code> corresponds to <code>dev_analytic.am_processed_data</code> and <code>cypress-perfeng-datalake-dev-us-west-2</code>.</li>
                 </ul>
         """
+        server = kwargs.get('server')
+        report_type = kwargs.get('report_type')
 
         # PostgreSQL initialization
         engine = ccr.get_sql_engine()
         metadata = MetaData()
 
-        #  Save to Dataframes
-        #add in method to save all historical CSVS
-        dst_df_file = self.data_source + self.project_name + '.csv'
-        dst_df_path = os.path.join(self.dashboard_dir, self.project_directory, self.project_name, 'Dataframes')
-        dst_df = os.path.join(dst_df_path, dst_df_file)
-        
-        try: 
-            os.makedirs(dst_df_path)
-        except OSError:
-            pass
-        
-        self.df[[x for x in self.df.columns if 'ERROR' not in x]].to_csv(dst_df)
-        if server == 'dev':
-            os.remove(dst_df)
-        
-        #send data to SQL
-        def restructure(df):
-            cols = df.columns.tolist()
-            df['timestamp'] = pd.to_datetime(df.index)
-            df2 = pd.melt(df, id_vars = ['timestamp'], value_vars = cols)
-            return df2
-        
-        #only use relevant cols
-        cols=['Inv_losses','Grid_losses','Snow_losses','Meter_Corrected_2']
-        
-        #STONE
-        #turn off losses on single inverter sites if meter_Corrected_2 > 0
-        if len(self.pos_Inv) == 1:
-            self.losses.loc[(self.losses['Meter_Corrected_2'] > 0), 'Inv_losses'] = 0
-        
-        
-        df_SQLhourly = restructure(self.losses[cols])
-        df_SQLhourly['site_name'] = self.project_name
-        #drop non float/int rows in value
-        df_SQLhourly_2 = df_SQLhourly.loc[df_SQLhourly['value'].apply(lambda x: type(x) in [float, int]), :]
-        
-        # Specify which table to use in Bartertown
-        if server.lower() == 'prod':
-            table_name = 'am_processed_data'
-        else:
-            table_name = 'am_processed_data_dev'
-
-        # Hacky way of upserting - we'll remove existing rows here
-        table = Table(table_name, metadata, autoload=True, autoload_with=engine, schema='dev_analytic')
-        stmt = delete(table).where(table.c.site_name == self.project_name).where(extract('year', table.c.timestamp) == self.year)
-        engine.execute(stmt)
+        #  Save to Dataframes folder on S3
+        df_filename = self.data_source + self.project_name + '.csv'
+        df_filepath = Path(self.data_platform_dirs.s3) / self.project_directory / self.project_name / 'Dataframes' / df_filename
+        df_filepath = df_filepath.as_posix().replace('s3:/', 's3://')
+        
+        if report_type.lower() == 'ul':
+            df_filepath = df_filepath.replace('.csv', '_UL_.csv')
+
+        if server != 'prod':
+            df_filepath = df_filepath.replace('.csv', '_COPY.csv')
+            self.df[[x for x in self.df.columns if 'ERROR' not in x]].to_csv(df_filepath)
+            s3_filepath = make_s3_filepath(df_filepath, obj_type='file')
+            s3_client.delete_object(Bucket=s3_filepath.bucket, Key=s3_filepath.key)
+        else:
+            self.df[[x for x in self.df.columns if 'ERROR' not in x]].to_csv(df_filepath)
+        
+        if report_type.lower() == 'monthly':
+            #send data to SQL
+            def restructure(df):
+                cols = df.columns.tolist()
+                df['timestamp'] = pd.to_datetime(df.index)
+                df2 = pd.melt(df, id_vars = ['timestamp'], value_vars = cols)
+                return df2
+            
+            #only use relevant cols
+            cols=['Inv_losses','Grid_losses','Snow_losses','Meter_Corrected_2']
+            
+            #STONE
+            #turn off losses on single inverter sites if meter_Corrected_2 > 0
+            if len(self.pos_Inv) == 1:
+                self.losses.loc[(self.losses['Meter_Corrected_2'] > 0), 'Inv_losses'] = 0
+            
+            
+            df_SQLhourly = restructure(self.losses[cols])
+            df_SQLhourly['site_name'] = self.project_name
+            #drop non float/int rows in value
+            df_SQLhourly_2 = df_SQLhourly.loc[df_SQLhourly['value'].apply(lambda x: type(x) in [float, int]), :]
+            
+            # Specify which table to use in Bartertown
+            if server.lower() == 'prod':
+                table_name = 'am_processed_data'
+            else:
+                table_name = 'am_processed_data_dev'
 
-        # Then insert rows here
-        df_SQLhourly_2.to_sql(name=table_name, 
-                              con=engine, 
-                              schema='dev_analytic',
-                              if_exists='append',
-                              index=False,
-                              chunksize=None,
-                              dtype=None
-        )
-        
-        # Export data to S3
-        upload_df=self.losses[cols]
-        upload_df['site_name']=self.project_name
-        upload_df['datetime']=upload_df.index       
-        upload_df=upload_df[['datetime']+cols+['site_name']]
-        if server.lower() == 'prod':
-            folder = f's3://cypress-perfeng-datalake-dev-us-west-2/Curated/HourlyLosses/year={self.year}'
-        else: 
-            folder = f's3://cypress-perfeng-datalake-onprem-us-west-2/Curated/HourlyLosses/year={self.year}'
-        filename = f'{self.year}_data_{self.project_name}_am_processed_data_sql.csv'
-        df_tools.write_to_s3(upload_df, folder, filename)
+            # Hacky way of upserting - we'll remove existing rows here
+            table = Table(table_name, metadata, autoload=True, autoload_with=engine, schema='dev_analytic')
+            stmt = delete(table).where(table.c.site_name == self.project_name).where(extract('year', table.c.timestamp) == self.year)
+            engine.execute(stmt)
+
+            # Then insert rows here
+            df_SQLhourly_2.to_sql(name=table_name, con=engine, schema='dev_analytic',
+                                if_exists='append', index=False, chunksize=None, dtype=None)
+            
+            # Export data to S3
+            upload_df=self.losses[cols]
+            upload_df['site_name']=self.project_name
+            upload_df['datetime']=upload_df.index       
+            upload_df=upload_df[['datetime']+cols+['site_name']]
+            if server.lower() == 'prod':
+                folder = f's3://cypress-perfeng-datalake-dev-us-west-2/Curated/HourlyLosses/year={self.year}'
+            else: 
+                folder = f's3://cypress-perfeng-datalake-onprem-us-west-2/Curated/HourlyLosses/year={self.year}'
+            filename = f'{self.year}_data_{self.project_name}_am_processed_data_sql.csv'
+            df_tools.write_to_s3(upload_df, folder, filename)
 
     
-    def export_summary(self, server='dev'):
+    def _export_summary(self, **kwargs) -> None:
         """Exports monthly summary data to S3 and Bartertown PostgreSQL database.
 
         Args:
             server (str): Option to insert data to prod or dev table.
                 <ul>
-                    <li><code>dev</code> corresponds to <code>dev_analytic.am_summary_data</code> and <code>cypress-perfeng-datalake-dev-us-west-2</code>.</li>
-                    <li><code>test</code> corresponds to <code>dev_analytic.am_summary_data_dev</code> and <code>cypress-perfeng-datalake-onprem-us-west-2</code>.</li>
+                    <li><code>dev</code> corresponds to <code>dev_analytic.am_summary_data_dev</code> and <code>cypress-perfeng-datalake-onprem-us-west-2</code>.</li>
+                    <li><code>prod</code> corresponds to <code>dev_analytic.am_summary_data</code> and <code>cypress-perfeng-datalake-dev-us-west-2</code>.</li>
+                    <li><code>datasub</code> corresponds to <code>dev_analytic.am_summary_data_datasub</code> and <code>cypress-perfeng-datalake-onprem-us-west-2</code>.</li>
                 <ul>
         """
-        # PostgreSQL initialization
+        server = kwargs.get('server')
+        report_type = kwargs.get('report_type')
+
+        # PostgreSQL initializatioo
         engine = ccr.get_sql_engine()
         metadata = MetaData()
 
         df_tracker_ava = self.get_tracker_ava()
         df_toSQL = pd.concat(
             [self.df_Pvsyst_2_month[[u'KWh_adj_by_days', 'NREL_Weather_Adj_%']],
                 self.df_month_2[['Plant_Perf_%', 'Snow_Adj_%', 'Grid_Ava_%', 'Inv_Ava_%', 'Meter_Corrected_2', 'PR_Plant']],
@@ -1285,15 +1454,15 @@
 
         # filter by months with no data, then filter for FC
         df_toSQL.loc[df_toSQL[u'KWh_adj_by_days'] == 0, :] = 0
         df_toSQL_FC = df_toSQL.copy()
         df_toSQL_FC.loc[self.df_Pvsyst_2_month['Post SC Date'] == 0, :] = 0
 
         # correct index
-        df_toSQL.index = df_toSQL.index.strftime('%b')
+        df_toSQL.index = df_toSQL.index.strftime('%b') #type: ignore
         df_toSQL_FC.index = df_toSQL.index
 
         # create Total row. Combination of sums and sumproducts
         df_toSQL_total = pd.DataFrame([], columns=df_toSQL.columns.tolist(), index=['Total'])
         df_toSQL_total_FC = df_toSQL_total.copy()
 
         sum_var = [
@@ -1371,20 +1540,26 @@
                     'POI Output (kWh)': 'om_unadjusted_p50_kwh',
                     'WAP_5': 'WAP_5'}
 
         df_toSQL['ccr_id'] = self.df_proj_keys['CCR_ID']
         df_toSQL['WAP_5'] = df_toSQL['Project_IPR_%'] / df_toSQL['NREL_Weather_Adj_%'].replace(0, np.nan) / df_toSQL['Snow_Adj_%'].replace(0, np.nan)
         df_toSQL = df_toSQL.rename(columns=column_map)
         df_toSQL = df_toSQL.rename(columns=lambda s: s.lower())
+        df_toSQL['row_created_date']=str(datetime.now())
 
         # Specify which table to use in Bartertown
         if server.lower() == 'prod':
             table_name = 'am_summary_data'
+        elif server.lower() == 'datasub':
+            table_name = 'am_summary_data_datasub'
         else:
             table_name = 'am_summary_data_dev'
+        
+        if report_type.lower() in ['ul', 'weekly']:
+            table_name = 'am_summary_data_UL'
 
         # Hacky way of upserting - we'll remove existing rows here
         table = Table(table_name, metadata, autoload=True, autoload_with=engine, schema='dev_analytic')
         stmt = delete(table).where(table.c.site_name == self.project_name).where(table.c.year == self.year)
         engine.execute(stmt)
 
         # Then insert rows here
@@ -1397,57 +1572,224 @@
                         dtype=None
         )
         
         # Export data to S3
         df_toSQL.index.rename('month', inplace=True)
         df_toSQL.drop(columns='year', inplace=True)
         df_toSQL = df_toSQL.replace([np.inf, -np.inf], 999999999)
-        df_toSQL['row_created_date']=str(datetime.now())
 
-        if server.lower() == 'prod':
-            folder = f's3://cypress-perfeng-datalake-dev-us-west-2/Curated/MonthlyLosses/year={self.year}'
+        if report_type.lower() == 'monthly':
+            if server.lower() == 'prod':
+                folder = f's3://cypress-perfeng-datalake-dev-us-west-2/Curated/MonthlyLosses/year={self.year}'
+            else:
+                folder = f's3://cypress-perfeng-datalake-onprem-us-west-2/Curated/MonthlyLosses/year={self.year}'
+            filename = f'{self.year}_data_{self.project_name}_sql_summary.csv'
+            df_tools.write_to_s3(df_toSQL, folder, filename)
+
+
+    def _export_weekly(self, **kwargs) -> None:
+        server = kwargs.get('server')
+
+        #todo: weekly reporting
+        df_Pvsyst_m = self.df_Pvsyst_2_month[['DC_corrected_PVsyst_WA', 'POI Output (kWh)']]
+        df_Pvsyst_m.index = df_Pvsyst_m.index.month
+        df_Pvsyst_m['days'] = self.df_Pvsyst_2.groupby('month')['POA (W/m2)'].count() / 24
+        df_Pvsyst_daily = df_Pvsyst_m[['DC_corrected_PVsyst_WA', 'POI Output (kWh)']].divide( df_Pvsyst_m['days'], axis=0)
+        
+        
+        df_daily = self.df.resample('d').sum()
+        for x in df_Pvsyst_daily.columns:
+            df_daily[x] = df_daily.index.to_series().dt.month.map(df_Pvsyst_daily[x])
+        
+        df_daily = df_daily.loc[df_daily.index > '2020-01-01'] #leap year causes this to get messed up, 366 days / 7 doesn't play nicely
+        #df_weekly = df_daily.resample('7D').sum()
+        df_weekly = df_daily.resample('W-SAT').sum() 
+        
+        df_weekly['NREL_Weather_Adj_%'] = df_weekly['DC_corrected_WA'] / df_weekly['DC_corrected_PVsyst_WA']
+        df_weekly['Weather_KWh'] = df_weekly['POI Output (kWh)'].multiply(df_weekly['NREL_Weather_Adj_%'])
+        
+        #  Calculate Percentages for Dashboard
+        df_weekly['Inv_Ava_%'] = df_weekly['Meter_Corrected_2'].div(df_weekly['Meter_&_ava']).fillna(1)
+        df_weekly['Grid_Ava_%'] = df_weekly['Meter_&_ava'].div(df_weekly['Meter_&_ava_&_grid']).fillna(1)
+        df_weekly['Snow_Adj_%'] = df_weekly['Meter_&_ava_&_grid'].div(df_weekly['Meter_losses&snow']).fillna(1)
+        df_weekly['Plant_Perf_%'] = df_weekly['Meter_losses&snow'].div(df_weekly['Weather_KWh']).fillna(0).replace(np.inf, 1).replace(-np.inf, 1)
+
+        # Select appropriate columns
+        df_weekly = df_weekly[['POI Output (kWh)','Meter_Corrected_2','Meter_&_ava',
+                               'Meter_&_ava_&_grid', 'Meter_losses&snow', 'Weather_KWh',
+                               'NREL_Weather_Adj_%', 'Inv_Ava_%', 'Grid_Ava_%', 'Snow_Adj_%', 'Plant_Perf_%']]
+
+        # Build filepath
+        week_folder = os.path.join(self.dashboard_dir, 'Python_Functions', 'Other Scripts', 'Weekly reporting', 'results', self.project_name)
+        weekly_filepath = os.path.join(week_folder, self.data_source + '.csv')
+
+        if self.data_platform == 's3':
+            weekly_filepath = Path(weekly_filepath).as_posix().replace('s3:/', 's3://')
+        
+        if server != 'prod':
+            weekly_filepath = weekly_filepath.replace('.csv', '_COPY.csv')
+            df_weekly.to_csv(weekly_filepath)
+            s3_filepath = make_s3_filepath(weekly_filepath, obj_type='file')
+            s3_client.delete_object(Bucket=s3_filepath.bucket, Key=s3_filepath.key)
         else:
-            folder = f's3://cypress-perfeng-datalake-onprem-us-west-2/Curated/MonthlyLosses/year={self.year}'
-        filename = f'{self.year}_data_{self.project_name}_sql_summary.csv'
-        df_tools.write_to_s3(df_toSQL, folder, filename)
-
+            df_weekly.to_csv(weekly_filepath)
+   
     
-    def export_snow(self, server:str='dev'):
+    def _export_snow(self, **kwargs) -> None:
         """
         Exports [snow_data][ccrenew.dashboard.project.Project.snow_data] and
         [snow_coverage][ccrenew.dashboard.project.Project.snow_coverage] dataframes to S3.
         
         Args:
             server (str): Snow data will only be exported if `server` == `prod`.
         """
+        server = kwargs.get('server')
+
         # Only export when running in prod
         if server == 'prod':
             folder = f's3://perfdatadev.ccrenew.com/snow_projects/{self.project_name}'
             snow_data_filename = f'{self.data_source}snow_data_project.csv'
             snow_coverage_filename = f'{self.data_source}snow_coverage_project.csv'
             df_tools.write_to_s3(self.snow_data, folder, snow_data_filename, index=True)
             df_tools.write_to_s3(self.snow_coverage, folder, snow_coverage_filename, index=True, header=False)
 
+    
+    def _export_bool(self, **kwargs) -> None:
+        """
+        Export the bool file for the project.
 
-    def _process_data(self, neighbor_sensors: dict, get_solcast: bool):
+        Args:
+            server (str): `prod` will update the BOOL file in the `Plant_Config_File` directory of the project's
+                [project_directory][ccrenew.dashboard.project.Project.project_directory].
+                `dev` will create a temporary file to test the export functionality then delete it.
+        """
+        server = kwargs.get('server')
+
+        # Update bool file
+        self._update_bool()
+
+        if server != 'prod':
+            if self.data_platform == 's3':
+                filepath = self.bool_filepath.replace('.csv', '_COPY.csv')
+                s3_filepath = make_s3_filepath(filepath, obj_type='file')
+                self.df_bool.to_csv(filepath)
+                s3_client.delete_object(Bucket=s3_filepath.bucket, Key=s3_filepath.key)
+            else:
+                dev_filepath = self.bool_filepath.replace('.csv', '_COPY.csv')
+                self.df_bool.to_csv(dev_filepath)
+                os.remove(dev_filepath)
+        else:
+            self.df_bool.to_csv(self.bool_filepath)
+
+
+    def _update_bool(self) -> None:
+        """
+        Generate bool data if bool file is not available.
+        """
+        # Load new production data if available & export to `powertrack_csv`
+        self.load_production_data()
+        self.__config_column_fix()
+
+        # Load df_bluesky if needed
+        if self.df_bluesky.empty:
+            self._fetch_bluesky_data()
+
+        # Set reference to sensor columns
+        temp_cols = self.col_ref['Temp_cols']
+        wind_cols = self.col_ref['Wind_cols']
+        weather_cols = self.col_ref['Weather_cols']
+        poa_cols = self.col_ref['POA_cols']
+        sensor_cols = self.col_ref['Sensor_cols']
+
+        # Subset sensor data to everything after the publish date
+        df_sensors = self.df.query("index.dt.date > @self.publish_date").reindex(columns=sensor_cols).copy()
+
+        # Store sensor data in the project object for the whole history
+        self.df_sensors = self.df.reindex(columns=sensor_cols)
+        if df_sensors.empty:
+            return
+
+        # Assign certain columns to appropriate dfs
+        df_weather = df_sensors[weather_cols]
+        df_poa = df_sensors[poa_cols]
+        df_poa_w_bs = df_poa.join(self.df_bluesky[['sat_ghi', 'sat_poa', 'proj_ghi', 'proj_ghi_poa']])
+        df_poa_w_bs = df_poa_w_bs.rename(columns={'sat_ghi': 'Satellite GHI',
+                                                  'sat_poa': 'Satellite POA',
+                                                  'proj_ghi': 'Project GHI',
+                                                  'proj_ghi_poa': 'Trans POA'})
+
+        # Apply data determination steps
+        # Find all values reporting NaN
+        comms = det.comms(df_sensors)
+
+        # Find all values reporting outside the supplied band
+        band_pass = det.band_pass(df_sensors, [(temp_cols, (-30, 120)),
+                                              (wind_cols, (0, 67)),
+                                              (poa_cols, (0, 1800))]
+                                            )
+        # Find all frozen values - separate POA from weather to ignore nighttime values for POA
+        frozen_window_size = 3
+        frozen_weather = det.frozen(df=df_weather, window=frozen_window_size)
+        frozen_poa = det.daylight_frozen(df=df_poa, pv_model=self.pv_model, window=frozen_window_size) # type: ignore
+
+        # Find all zeroes during daylight hours for POAs
+        zeroes_poa = det.daylight_zeroes(df=df_poa, pv_model=self.pv_model)
+        
+        # Find trackers that aren't tracking
+        if self.Tracker_site:
+            tracker_poa, datasub_stats = det.daylight_poa_mistracking(df=df_poa_w_bs, pv_model=self.pv_model, add_sparklines=False, degree=8) # type: ignore
+            poa = frozen_poa+zeroes_poa+tracker_poa
+        else:
+            poa = frozen_poa+zeroes_poa
+
+        # We'll come back to implement some more complex logic later
+        # spline_filter = det.spline_filter(df_sensors)
+
+        # Combine the comms & band pass dfs
+        df_bool = comms+band_pass
+
+        # Add frozen weather values
+        df_bool[weather_cols] = df_bool[weather_cols] + frozen_weather
+
+        # Add POA columns
+        poa = poa.reindex(index = df_bool.index, columns=df_bool[poa_cols].columns).fillna(False)
+        df_bool[poa_cols] = df_bool[poa_cols] + poa
+        
+        # Set `self.df_bool` equal to calculated bool if empty. Update if exists.
+        if self.df_bool.empty:
+            self.df_bool = ~df_bool
+        else:
+            # Update column order of self.df_bool to Tamb-Tmod-Wind-POA
+            # Add rows to self.df_bool if df_bool has more dates since df.update only works as a left join
+            self.df_bool = self.df_bool.reindex(columns = df_bool.columns, index=df_bool.index)
+            self.df_bool.update(~df_bool, overwrite=True)
+        
+        self.df_bool = self.df_bool.astype(bool)
+
+
+    def _process_data(self, neighbor_sensor_data:dict, datasub:bool, use_bluesky:bool):
         """Processes data for the project"""
         # TODO: update for reprocessing only to run the methods that update the required data
+        # Update object if datasub was used or not
+        self.datasub = datasub
 
         print('Processing data for {}'.format(self.project_name))
+        self._fetch_bluesky_data()
+
         # Update df_sensor_ON based on config file
         self._config_disable_sensors()
 
         # Configure PVSyst
         self.__pvsyst_adjustments()
 
         # Calculate monthly
         self.__calculate_monthly()
 
         # Fix columns before data gets used anywhere
-        self.__column_fix()
+        self.__config_column_fix()
 
         # Find sensor anomalies based on simple hard-coded rules
         self.__find_sensor_anomalies()
 
         self.df = self.df.fillna(0)
 
         # Correct POI data for battery sites
@@ -1460,16 +1802,16 @@
         # Calculate averages for the sensors on the site using `df_sensor_ON`
         self.__config_sensor_average_updates()
 
         # Calculate averages for the native sensors using bool file
         self._calculate_native_sensor_averages()
 
         # Perform data substitution based on bool file & available neighbor sensors
-        if self.year >= 2023:
-            self._calculate_data_sub_sensor_averages(neighbor_sensors, get_solcast=get_solcast)
+        if self.year >= 2023 and datasub:
+            self._calculate_datasub_sensor_averages(neighbor_sensor_data, use_bluesky=use_bluesky)
 
         # These next ones are pretty self explanatory
         self.__calculate_tcell()
         self.df = self.df.fillna(0)
         self.__calculate_availability()
         self.__calculate_snow_data()
         self.__calculate_PR()
@@ -1511,18 +1853,25 @@
             if str(row['#']).lower() == 'eval':
                 # This is where we do that silly hack listed above the for loop to turn off certain hours
                 filter = self.df_sensor_ON[self.df_sensor_ON.eval(row['description']) & (self.df_sensor_ON.index >= s) & (self.df_sensor_ON.index <= e)].index
             else:
                 filter = self.df_sensor_ON[(self.df_sensor_ON.index >= s) & (self.df_sensor_ON.index <= e)].index
         
             self.df_sensor_ON.loc[filter, sensor] = False
+
+            # Set any rows where a native sensor was turned off to 'Config'
             if sensor in self.col_ref['POA_cols']:
                 self.df.loc[filter, 'POA_source'] = 'Config'
 
-        # And now remove the 'Hour' column
+        # Next set any rows where a neighbor was turned on to 'Config'
+        neighbor_poa_cols = list(np.setdiff1d(self.pos_POA, self.col_ref['POA_cols']))
+        neighbor_poa_dates = (self.df_sensor_ON[neighbor_poa_cols] == True).any(axis=1)
+        self.df.loc[neighbor_poa_dates, 'POA_source'] = 'Config'
+
+        # Finally remove the 'Hour' column
         self.df_sensor_ON = self.df_sensor_ON.drop('Hour', axis=1)
 
 
     def __pvsyst_adjustments(self):
 
         # Add Tcell column. The function is in the weather adjusted function that are imported at the top of the script.
         self.df_Pvsyst['Tcell'] = weather.generate_Tcell(self.df_Pvsyst['POA (W/m2)'],
@@ -1539,15 +1888,16 @@
 
         # For PVsyst we need to shift the columns to adjust for DST.
         # It also deletes the last value. It is from the following year
         (self.df_Pvsyst_2, _,
         self.rates_year, self.normal_rate_flag) = rates.generate_Rate_column(self.project_name,
                                                                              self.config_filepath,
                                                                              shift_DST=None,
-                                                                             year=self.year)
+                                                                             year=self.year,
+                                                                             data_platform=self.data_platform)
         self.df_Pvsyst_2 = self.df_Pvsyst_2.iloc[:-1, :]
         self.rates_year = self.rates_year.iloc[:-1, :]
 
         # Also need to remove Feb 29, to match PVsyst file.
         self.df_Pvsyst_2 = self.df_Pvsyst_2[~((self.df_Pvsyst_2.index.month == 2) & (self.df_Pvsyst_2.index.day == 29))]
 
         # Adjust df_Pvsyst index to match the year that we're running
@@ -1627,27 +1977,22 @@
         self.df_Pvsyst_2_month['POA_weighted_Tcell'] /= self.df_Pvsyst_2_month['POA (W/m2)']
         self.df_Pvsyst_2_month['Blended_Rate'] = self.df_Pvsyst_2_month[['Revenue_IE_P50']].div(self.df_Pvsyst_2_month['Year 0 Actual Production (kWh)'].replace(0, np.nan), axis="index")
         self.df_Pvsyst_2_month['Blended_POI_rate'] = self.df_Pvsyst_2_month[['Revenue_IE_POI']].div(self.df_Pvsyst_2_month['Year 0 Actual Production (kWh)'].replace(0, np.nan), axis="index")
         self.df_Pvsyst_2_month['PR_IE_P50'] = self.df_Pvsyst_2_month[['Year 0 Actual Production (kWh)']].div(self.df_Pvsyst_2_month['DC_corrected_PVsyst'].replace(0, np.nan), axis="index")
         self.df_Pvsyst_2_month['PR_IE_P50_PR'] = self.df_Pvsyst_2_month[['Gen_NO_Clipping_PVsyst']].div(self.df_Pvsyst_2_month['DC_corrected_PVsyst_PR'].replace(0, np.nan), axis="index")
         
   
-    def __column_fix(self):
+    def __config_column_fix(self):
         '''
         this function, added 12/10/2020 (and some time after, sorry I'm slow),
         intends to provide an option to alter the AE file from the config file.
         Options here include allowing for setting 1 column equal to the sum of others,
         doing a dif on the cumulative meter or building a cumulative from a power column.
         To do "trip" this function put "column fix" in the Var_ID column on sensor offline page
         '''
-
-        # Initialize dates so we don't need to call Bluesky functions more than we need to
-        previous_start_date = 0
-        previous_end_date = 0
-
         # Loop through rows in the Sensor_Offline sheet of the config file
         for i, row in self.sensor_OFF.iterrows():
             option = row['Var_ID']
             end_date = row['end date']
             end_date = self.df.index[-1] if end_date == -1 else end_date
             if pd.to_datetime(end_date) > self.df.index[-1]:
                 end_date = str(self.df.index[-1])
@@ -1727,56 +2072,48 @@
                         df_temporary = self.df[fix_column].fillna(
                             0).loc[start_date] + self.df[func_outcome].loc[start_date:].fillna(0).cumsum()
 
                         self.df.loc[start_date:end_date, fix_column] = df_temporary.loc[start_date:end_date]
 
                 elif option.lower() == 'weather fix':
                     fix_type = func_choice.lower()
-                    if previous_start_date != start_date or previous_end_date != end_date:
-                        if fix_type == 'tran_ghi':
-                            df_weather = self.run_bluesky(start=start_date, end=end_date, tran_ghi='only', plot=False)
-                        else:
-                            df_weather = self.run_bluesky(start=start_date, end=end_date, tran_ghi='none', plot=False)
-                        previous_start_date = start_date
-                        previous_end_date = end_date
-
-                    if func_choice.lower()=='tran_ghi': 
+                    if fix_type == 'tran_ghi': 
                         print('Using Solcast GHI Transposed to POA')
                         try:
-                            self.df['POA_1'][(self.df.index >= start_date) & (self.df.index <= end_date)] = df_weather['sites_ghi_poa'][start_date:end_date]
+                            self.df['POA_1'][(self.df.index >= start_date) & (self.df.index <= end_date)] = self.df_bluesky['proj_ghi_poa'][start_date:end_date]
                         except KeyError:
                             raise Exception('Unable to transpose GHI for {}. Please review project or update config file and run again.'.format(self.project_name))
                         except ValueError as e:
                             raise Exception(f'Error pulling Solcast data for {self.project_name}: {e}')
                         
-                    elif func_choice.lower()=='sat_poa': 
+                    elif fix_type == 'sat_poa': 
                         print('Using Solcast POA')
                         try:
-                            self.df['POA_1'][(self.df.index >= start_date) & (self.df.index <= end_date)] = df_weather['poa'][start_date:end_date]
+                            self.df['POA_1'][(self.df.index >= start_date) & (self.df.index <= end_date)] = self.df_bluesky['sat_poa'][start_date:end_date]
                         except ValueError as e:
                             raise Exception(f'Error pulling Solcast data for {self.project_name}: {e}')
                         
-                    elif func_choice.lower()=='sat_tamb': 
+                    elif fix_type == 'sat_tamb': 
                         print('Using Solcast Ambient Temp')
                         try:
-                            self.df['Tamb_1'][(self.df.index >= start_date) & (self.df.index <= end_date)] = df_weather['Tamb'][start_date:end_date]
+                            self.df['Tamb_1'][(self.df.index >= start_date) & (self.df.index <= end_date)] = self.df_bluesky['Tamb_avg'][start_date:end_date]
                         except ValueError as e:
                             raise Exception(f'Error pulling Solcast data for {self.project_name}: {e}')
                         
-                    elif func_choice.lower()=='sat_tmod': 
+                    elif fix_type == 'sat_tmod': 
                         print('Using Solcast Ambient Temp and Wind to make Tmod')
                         try:
-                            self.df['Tmod_1'][(self.df.index >= start_date) & (self.df.index <= end_date)] = df_weather['Tmod'][start_date:end_date]
+                            self.df['Tmod_1'][(self.df.index >= start_date) & (self.df.index <= end_date)] = self.df_bluesky['Tmod_avg'][start_date:end_date]
                         except ValueError as e:
                             raise Exception(f'Error pulling Solcast data for {self.project_name}: {e}')
                         
-                    elif func_choice.lower()=='sat_wind': 
+                    elif fix_type == 'sat_wind': 
                         print('Using Solcast Wind Speed')
                         try:
-                            self.df['Wind_speed_1'][(self.df.index >= start_date) & (self.df.index <= end_date)] = df_weather['Wind_speed'][start_date:end_date]
+                            self.df['Wind_speed_1'][(self.df.index >= start_date) & (self.df.index <= end_date)] = self.df_bluesky['Wind_speed'][start_date:end_date]
                         except ValueError as e:
                             raise Exception(f'Error pulling Solcast data for {self.project_name}: {e}')
 
             else:
                 continue  # this continues if s and e both occur in a previous year
 
  
@@ -1937,115 +2274,35 @@
         self.df['Tmod_avg'] = aux.values
 
         # Average Tamb sensors
         aux = self.df[self.pos_Tamb][self.df_sensor_ON[self.pos_Tamb] == True].mean(axis=1)
         self.df['Tamb_avg'] = aux.values
 
 
-    def _update_bool(self):
-        """
-        Generate bool data if bool file is not available.
-        """
-        # Load new production data if available & export to `powertrack_csv`
-        self.load_production_data()
-        self.__column_fix()
-        self._fetch_solcast_data()
-
-        # Set reference to sensor columns
-        temp_cols = self.col_ref['Temp_cols']
-        wind_cols = self.col_ref['Wind_cols']
-        weather_cols = self.col_ref['Weather_cols']
-        poa_cols = self.col_ref['POA_cols']
-        sensor_cols = self.col_ref['Sensor_cols']
-
-        # Subset sensor data to everything after the publish date
-        if not self.publish_date:
-            self.publish_date = datetime(2023, 1, 1).date()
-        df_sensors = self.df.query("index.dt.date > @self.publish_date").reindex(columns=sensor_cols).copy()
-
-        # Store sensor data in the project object for the whole history
-        self.df_sensors = self.df.reindex(columns=sensor_cols)
-        if df_sensors.empty:
-            return
-
-        # Assign certain columns to appropriate dfs
-        df_weather = df_sensors[weather_cols]
-        df_poa = df_sensors[poa_cols]
-        df_poa_w_sol = df_poa.join(self.df_solcast[['POA_avg']].rename(columns={'POA_avg': 'Solcast'}))
-
-        # Apply data determination steps
-        # Find all values reporting NaN
-        comms = det.comms(df_sensors)
-
-        # Find all values reporting outside the supplied band
-        band_pass = det.band_pass(df_sensors, [(temp_cols, (-30, 120)),
-                                              (wind_cols, (0, 67)),
-                                              (poa_cols, (0, 1800))]
-                                            )
-        # Find all frozen values - separate POA from weather to ignore nighttime values for POA
-        frozen_window_size = 3
-        frozen_weather = det.frozen(df=df_weather, window=frozen_window_size)
-        frozen_poa = det.daylight_frozen(df=df_poa, project=self, window=frozen_window_size)
-
-        # Find all zeroes during daylight hours for POAs
-        zeroes_poa = det.daylight_zeroes(df=df_poa, project=self)
-        
-        # Find trackers that aren't tracking
-        if self.Tracker_site:
-            tracker_poa = det.daylight_poa_mistracking(df=df_poa_w_sol, project=self, degree=8)
-            poa = frozen_poa+zeroes_poa+tracker_poa
-        else:
-            poa = frozen_poa+zeroes_poa
-
-        # We'll come back to implement some more complex logic later
-        # spline_filter = det.spline_filter(df_sensors)
-
-        # Combine the comms & band pass dfs
-        df_bool = comms+band_pass
-
-        # Add frozen weather values
-        df_bool[weather_cols] = df_bool[weather_cols] + frozen_weather
-
-        # Add POA columns
-        poa = poa.reindex(index = df_bool.index).fillna(False)
-        df_bool[poa_cols] = df_bool[poa_cols] + poa
-        
-        # Set `self.df_bool` equal to calculated bool if empty. Update if exists.
-        if self.df_bool.empty:
-            self.df_bool = ~df_bool
-        else:
-            # Update column order of self.df_bool to Tamb-Tmod-Wind-POA
-            # Add rows to self.df_bool if df_bool has more dates since df.update only works as a left join
-            self.df_bool = self.df_bool.reindex(columns = df_bool.columns, index=df_bool.index)
-            self.df_bool.update(~df_bool, overwrite=True)
-        
-        self.df_bool = self.df_bool.astype(bool)
-
-
     def _calculate_native_sensor_averages(self):
         """
         Calculate average values for native sensors based on bool file.
         """
         native_col_groups = [zip(tup.col_list, itertools.repeat(tup.col_avg)) for tup in self.sensor_colmap]
-        native_col_dict = {(key if key else []): val for items in native_col_groups for key, val in items}
+        native_col_dict = {key: val for items in native_col_groups for key, val in items}
 
         df_bool_nan = self.df_bool.replace(False, np.nan)
         try:
             native_df = self.df[self.df_bool.columns]*df_bool_nan
         except KeyError:
             print(f"*** WARNING: {self.project_name} {str(sys.exc_info()[1]).replace(' not in index', '')} exists in BOOL file but not in Powertrack file. Please updated BOOL file to ensure consistent columns.")
             consistent_cols = self.df_bool.columns.intersection(self.df.columns)
             self.df_bool = self.df_bool.reindex(columns=consistent_cols)
             df_bool_nan = df_bool_nan.reindex(columns=consistent_cols)
             native_df = self.df[self.df_bool.columns]*df_bool_nan
 
         self.df_sensors_native_avg = native_df.groupby(native_col_dict, axis=1).mean()
 
 
-    def _calculate_data_sub_sensor_averages(self, neighbor_sensor_avgs: dict = {}, get_solcast=False):
+    def _calculate_datasub_sensor_averages(self, neighbor_sensor_avgs:dict = {}, use_bluesky:bool = False):
         """
         Calculate sensor averages based on bool file.
 
         Args:
             neighbor_sensor_avgs: Dict of neighbor name & sensor average df pairs.
             get_solcast: Option to query Athena for solcast data to use in data sub.
         """
@@ -2056,36 +2313,27 @@
         # Add any columns for sensors that are missing, i.e. if a project doesn't have a wind sensor
         # This will add a column of nans to be filled in with neighbor or solcast
         avg_cols = [col.col_avg for col in self.sensor_colmap]
         df_sensors_avg = df_sensors_avg.reindex(columns=avg_cols)
 
         # Exclude any rows that were changed in the config file
         try:
-            # First exclude any rows that where the native sensors were turned off
+            # First exclude any rows that were changed in the config file
            df_sensors_avg = df_sensors_avg[self.df['POA_source'] != 'Config']
         except KeyError:
             pass
-
-        # Next exclude any rows where a neighbor was turned on
-        neighbor_poa_cols = list(np.setdiff1d(self.pos_POA, self.col_ref['POA_cols']))
-        neighbor_poa_dates = (self.df_sensor_ON[neighbor_poa_cols] == True).any(axis=1)
-        df_sensors_avg = df_sensors_avg.loc[~neighbor_poa_dates]
-        self.df.loc[neighbor_poa_dates, 'POA_source'] = 'Config'
         
         # Check if `POA_source` column has assuming all Natives are good until changed
         # The rows where the config file didn't update would be NaN but now they're 0 due to the df.fillna(0) calls
         try:
             self.df['POA_source'] = self.df['POA_source'].replace([0, np.nan], 'Native')
         except KeyError:
             self.df['POA_source'] = 'Native'
         any_nulls = df_sensors_avg.isna().any().any()
 
-        # Query solcast data if self.df_solcast is empty
-        self._fetch_solcast_data()
-
         while any_nulls:
             for neighbor_name, df_neighbor_avg in neighbor_sensor_avgs.items():
                 # Check if the neighbor satisfies the conditions for using POA
                 if self.neighbor_list[neighbor_name]:
                     # Use POA data
                     neighbor_dates = df_sensors_avg[df_sensors_avg['POA_avg'].isnull()].index
                     self.df.loc[neighbor_dates, 'POA_source'] = neighbor_name
@@ -2098,30 +2346,46 @@
                     except:
                         non_poa = non_poa.fillna(df_neighbor_avg)
                     df_sensors_avg.update(non_poa)
 
                 any_nulls = df_sensors_avg[avg_cols].isna().any().any()
 
             # Pull solcast data if specified
-            if get_solcast:
-                # Update df_sensors_avg with solcast data
+            if use_bluesky:
+                # Fill in Temperature & wind data with solcast
+                df_sensors_avg = df_sensors_avg.fillna(self.df_bluesky)
+
+                # Update df_sensors_avg with bluesky data
+                # First substitute transposed GHI data
                 null_dates = df_sensors_avg[df_sensors_avg['POA_avg'].isnull()].index
-                solcast_dates = self.df_solcast.index.intersection(null_dates)
-                self.df.loc[solcast_dates, 'POA_source'] = 'Solcast'
-                df_sensors_avg = df_sensors_avg.fillna(self.df_solcast)
-            
+                df_sensors_avg['POA_avg'] = df_sensors_avg['POA_avg'].fillna(self.df_bluesky['proj_ghi_poa'])
+                proj_ghi_poa_dates = null_dates.difference(df_sensors_avg[df_sensors_avg['POA_avg'].isnull()].index)
+                self.df.loc[proj_ghi_poa_dates, 'POA_source'] = 'Trans GHI'
+
+                # Then substitute Solcast data
+                null_dates = df_sensors_avg[df_sensors_avg['POA_avg'].isnull()].index
+                df_sensors_avg['POA_avg'] = df_sensors_avg['POA_avg'].fillna(self.df_bluesky['sat_poa'])
+                sat_poa_dates = null_dates.difference(df_sensors_avg[df_sensors_avg['POA_avg'].isnull()].index)
+                self.df.loc[sat_poa_dates, 'POA_source'] = 'Satellite'
+
             any_nulls = False
 
         if self.Tracker_site:
             df_poa = self.df.loc[:, self.col_ref['POA_cols']]
-            df_poa_w_sol = df_poa.join(self.df_solcast[['POA_avg']].rename(columns={'POA_avg': 'Solcast'}))
-            tracker_poa = det.daylight_poa_mistracking(df=df_poa_w_sol, project=self, degree=8)
+            df_poa_w_bs = df_poa.join(self.df_bluesky[['sat_ghi', 'sat_poa', 'proj_ghi', 'proj_ghi_poa']])
+            df_poa_w_bs = df_poa_w_bs.rename(columns={'sat_ghi': 'Satellite GHI',
+                                                      'sat_poa': 'Satellite POA',
+                                                      'proj_ghi': 'Project GHI',
+                                                      'proj_ghi_poa': 'Trans POA'})
+
+            tracker_poa, datasub_stats = det.daylight_poa_mistracking(df=df_poa_w_bs, pv_model=self.pv_model, add_sparklines=False, degree=8) # type: ignore
             tracker_dates = tracker_poa[tracker_poa.all(axis=1)].index
             self.df.loc[tracker_dates, 'POA_source'] = self.df.loc[tracker_dates, 'POA_source'] + ' MT'
 
+        df_sensors_avg = df_sensors_avg.astype(float)
         self.df.update(df_sensors_avg)
 
     
     def __calculate_tcell(self):
         # Calculate Tcell from ambient temperature & Tcell from module temperature
         self.df['POA_avg'] = self.df['POA_avg'].fillna(0)
         self.df['Tcell_AMB'] = weather.generate_Tcell(self.df['POA_avg'],
@@ -2609,15 +2873,16 @@
                                                                        guarantee_input,
                                                                        self.df_perf)
             elif guarantee_id == 'SCEG':
                 self.df_perf, guarantee_result = perf.SCEG_performance_guarantee(self.project_name,
                                                                        self.df,
                                                                        self.df_Pvsyst,
                                                                        self.PIS_date,
-                                                                       self.df_perf)
+                                                                       self.df_perf,
+                                                                       data_platform=self.data_platform)
             elif guarantee_id == "Regions_OPR":
                 guarantee_input = pd.to_datetime(self.df_proj_keys['Guarantee_input'])
                 self.df_perf, guarantee_result = perf.Regions_performance_guarantee(self.df,
                                                                           self.df_month_2,
                                                                           self.df_Pvsyst,
                                                                           self.df_Pvsyst_2_month,
                                                                           guarantee_input,
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/session.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/session.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,71 @@
 # -*- coding: utf-8 -*-
+"""
+Module to coordinate processing of CCRenew Dashboard projects.
+"""
+from __future__ import annotations
 
-from socket import close
+import boto3
+import builtins
 from ccrenew.dashboard.utils.logging_conf import get_logging_config
-from collections.abc import Iterable
-from datetime import (
-    datetime,
-    timedelta)
+from datetime import datetime
 from dateutil import parser
-from dateutil.parser import ParserError
 import logging
 import logging.config
-from matplotlib import (
-    pyplot as plt,
-    rcParams)
 from matplotlib.pyplot import waitforbuttonpress
-from numbers import Number
-import numpy as np
 import os
 import pandas as pd
 from pandas.io.sql import SQLTable
+from pathlib import Path
 import pickle
+import s3fs
+import sys
 import time
 import traceback
-import types
+from typing import Iterable
 import warnings
 
-from ccrenew import __version__
-from ccrenew.dashboard import (
+from ccrenew import (
+    __version__,
     ccr,
     all_df_keys,
-    func_timer)
-from ccrenew.dashboard.plotting.plots import Plotter
+    ListLike
+)
+from ccrenew.dashboard import (
+    DataPlatformDirs,
+    func_timer,
+    get_modified_time,
+    make_s3_filepath
+)
+from ccrenew.dashboard import Plotter
 from ccrenew.dashboard.project import Project
 from ccrenew.dashboard.utils.df_tools import df_update_join
 import ccrenew.dashboard.utils.dashboard_utils as utils
 import ccrenew.dashboard.utils.project_neighbors as neighbs
 
 from ccrenew.dashboard.data_processing.batch_process import (
     export_pool,
     process_pool)
     
+
+# Create boto s3 client
+s3_client = boto3.client('s3')
+
 # suppress warnings about "A value is trying to be set on a copy of a slice from a DataFrame."
-pd.options.mode.chained_assignment = None
+pd.set_option('mode.chained_assignment', None)
 
 # Initialize logger
 # Get logging configuration from the logging.conf file in the same directory as this file
 username = os.getenv('username')
 dashboard_folder = ccr.file_project
-log_filename = '{}_dashboard-{}.log'.format(datetime.now().strftime('%Y-%m-%d_%H-%M-%S'), username)
-log_config = os.path.join(dashboard_folder, 'Python_Functions', 'logging.conf')
-log_file = os.path.join(dashboard_folder, 'Python_Functions', '_old', 'logs', log_filename)
-LOGGING_CONFIG = get_logging_config(log_file)
-logging.config.dictConfig(LOGGING_CONFIG)
+# log_filename = '{}_dashboard-{}.log'.format(datetime.now().strftime('%Y-%m-%d_%H-%M-%S'), username)
+# log_config = os.path.join(dashboard_folder, 'Python_Functions', 'logging.conf')
+# log_file = os.path.join(dashboard_folder, 'Python_Functions', '_old', 'logs', log_filename)
+# LOGGING_CONFIG = get_logging_config(log_file)
+# logging.config.dictConfig(LOGGING_CONFIG)
 
 # Create logger
 # logger = logging.getLogger(__name__)
 # logger.info('Beginning Dashboard Session')
 
 def _execute_insert(self, conn, keys, data_iter):
     #print "Using monkey-patched _execute_insert"
@@ -64,109 +74,132 @@
     # Python 2 compatibility:
     try:
         conn.execute(self.insert_statement().values(data))
     except AttributeError:
         conn.execute(self.table.insert().values(data))
     
 
-SQLTable._execute_insert = _execute_insert
+SQLTable._execute_insert = _execute_insert # type: ignore
 
     
-class DashboardSession(object):
+class DashboardSession:
     """Main orchestrator for processing, plotting, and exporting data for projects (i.e. sites).
 
     Args:
-        project_list (str or list, optional): List of [Projects][ccrenew.dashboard.project.Project] to initialize when initializing the session.
+        project_list (str or list): List of [Projects][ccrenew.dashboard.project.Project] to initialize when initializing the session.
         data_cutoff_date (str or datetime, optional): The last date you want to analyze. Defaults to the current date the dashboard is being run.
-        data_source (str, optional): The data source to run the dashboard on.
+        data_source (str, optional): The location where project data is stored.
+            Default is current year Sharepoint data. To pull S3 data add 's3' to the input. See below for examples.
+        
+    `data_source` examples:
+    
+    | data_source      | Explanation                  |
+    |------------------|------------------------------|
+    | `None`           | Current year Sharepoint data |
+    | `'s3'`           | Current year S3 data         |
+    | `'2022_data_'`   | 2022 Sharepoint data         |
+    | `'2022_data_s3'` | 2022 S3 data                 |
     """
 
     # Instantiate globals as class variables
-    dashboard_dir = ccr.file_project
-    df_keys = all_df_keys
+    df_keys = all_df_keys.copy()
     __version__ = __version__
 
     print('Pulling diagnostic comments from Smartsheets...')
     # Smartsheet comments from previous reporting months. I'm going to hardcode Jan 2021 as the earliest date (column index 69 - Nice) but we can change that easily
-    df_ss_comments: pd.DataFrame = ccr.get_ss_as_df('2819883898562436', drop_col_1=False, start_col=69, index_col='Project')
+    df_ss_comments = ccr.get_ss_as_df('2819883898562436', drop_col_1=False, start_col=69, index_col='Project')
 
     # Site lists
     tracker_sites = ['5840 Buffalo Road', 'Alexis', 'ATOOD II', 'Bar D', 'Barnhill Road Solar', 'Bay Branch',
                      'Bonanza', 'Bovine Solar', 'Bronson', 'Cascade', 'Chisum', 'Copperfield', 'Curie',
                      'Eddy II', 'Gaston II', 'Griffin', 'Grove Solar (NC)', 'Grove', 'Hardison Farm',
                      'Hopewell Friends', 'Hyline', 'IS - 46 Tracker', 'IS 67', 'Lampwick', 'Leggett Solar',
                      'Mars', 'Neff', 'Nimitz', 'Open Range', 'Palmetto Plains', 'Prince George 1',
                      'Prince George 2', 'Railroad', 'Shoe Creek', 'Siler', 'Simba', 'Springfield', 'Sterling',
                      'Thunderegg', 'Vale', 'Wagyu', 'Warren', 'Wendell', 'West Moore II', 'Yellow Jacket']
     battery_ac_funds = ['LGE']
-    battery_ac_sites = df_keys.query("Fund in @battery_ac_funds").index
+    battery_ac_sites = df_keys.query("Fund in @battery_ac_funds").index.tolist()
     battery_dc_sites = ['Salt Point', 'Dubois', 'Landau II', 'Clendenin A']
     
     # Type annotations & docstrings for documentation
-    df_keys: dict
+    df_keys: pd.DataFrame
     """Metadata for all projects."""
-    df_ss_comments: dict
+    df_ss_comments: pd.DataFrame
     """DataFrame with Smartsheet comments."""
     battery_ac_funds: list
     """Funds with projects with AC batteries."""
     battery_ac_sites: list
     """Projects with AC batteries."""
     battery_dc_sites: list
     """Projects with DC batteries."""
     tracker_sites: list
     """Projects with tracker-type racking."""
 
-    def __init__(self,
-                 project_list=None,
-                 data_cutoff_date=None,
-                 data_source=None,
-                 **kwargs):
+    def __init__(self, project_list:str|ListLike|None=None, data_cutoff_date:str|datetime|None=None,
+                 data_source:str|None=None, **kwargs):
 
         print('Initializing DashboardSession...')
         
         # Initialize a dict to store projects - key = project name; value = project object
         # utils.project_dict() overrides the __repr__ method of dict to pretty print the projects when you call it
         self.project_list = utils.project_dict()
 
         # Add projects to the session if provided
         if project_list:
-            if isinstance(project_list, (str, Iterable)):
+            if isinstance(project_list, (str, ListLike)):
                 self.add_projects(project_list)
             else:
                 print('`project_list` must be a string or list. The projects provided were not added to the DashboardSession. Please try again in the initialized DashboardSession.')
 
         # Parse & add data_cutoff_date if provided. Default to current date if not provided or error during parsing 
         if data_cutoff_date:
             try:
-                self.data_cutoff_date = parser.parse(data_cutoff_date)
+                self.data_cutoff_date = parser.parse(data_cutoff_date) # type: ignore
             except:
                 self.data_cutoff_date = datetime.today()
         else:
             self.data_cutoff_date = datetime.today()
 
-        # Set data source
-        if data_source:
-            self.data_source = data_source
+        def set_data_source(data_source:str|None) -> None:
+            if data_source:
+                self.data_source = data_source
+            else:
+                self.data_source = f"{datetime.now().year}_data_"
+
+        self.data_platform_dirs = DataPlatformDirs(ccr.file_project,
+                                                   's3://cypress-perfeng-datalake-dev-us-west-2/Raw/HourlyResolution/')
+
+        set_data_source(data_source)
+        if 's3' in self.data_source.lower():
+            data_source = self.data_source.replace(' ', '').replace('s3', '')
+            set_data_source(data_source)
+            self.dashboard_dir = self.data_platform_dirs.s3
+            self.data_platform = 's3'
         else:
-            self.data_source = f"{datetime.now().year}_data_"
-            
+            self.dashboard_dir = self.data_platform_dirs.sharepoint
+            self.data_platform = 'sharepoint'
+
         # Get snow dataframe
-        self.raw_snow_df, self.snow_file = utils.get_snow_df(dashboard_folder, self.data_source, file_format='csv')
+        self.raw_snow_df, self.snow_file = utils.get_snow_df(dashboard_folder, self.data_source, file_format='csv', data_platform=self.data_platform)
 
         # Create list for projects that have errored out
         self.errored_projects = {}
 
         # List of plotter objects for different projects
         self.plotters = {}
 
         # Type annotations & docstrings for documentation
-        self.project_list: list
+        self.project_list: dict
         """List of [Projects][ccrenew.dashboard.project.Project] that
         have been initialized & added to the
         [DashboardSession][ccrenew.dashboard.session.DashboardSession] instance."""
+        self.data_platform: str
+        """Backend architecture of the source data for a project. Either `s3` or `sharepoint`."""
+        self.data_source: str
+        """Location of the source data for projects based on production year."""
         self.raw_snow_df: pd.DataFrame
         """Snow data."""
         self.data_cutoff_date: datetime
         """Last day to process data."""
         self.errored_projects: dict
         """List of [Projects][ccrenew.dashboard.project.Project] that have encountered
         errors while processing & their error messages."""
@@ -177,119 +210,156 @@
         return 'DashboardSession object with {} projects'.format(len(self.project_list))
 
 
     def __str__(self):
         return 'DashboardSession object with {} projects'.format(len(self.project_list))
 
 
-    def add_project(self, project_name, get_neighbors=True):
+    def get_project(self, project_name:str|Project, add_neighbors:bool=True, report_type:str = 'monthly') -> Project:
+        """
+        Return a [Project][ccrenew.dashboard.project.Project] object given a project name.
+
+        Args:
+            project_name (str or Project): Name of a [Project][ccrenew.dashboard.project.Project] to return from the
+                [DashboardSession][ccrenew.dashboard.session.DashboardSession] instance.
+                If project does not yet exist in the session, it will be added then returned.
+            add_neighbors (bool, optional): Flag to add & initialize neighbor [Projects][ccrenew.dashboard.project.Project].
+            report_type (str): Method for processing the project. Options are `monthly`, `ul`, or `weekly`.
+
+        Returns:
+            Project object for the given the project name.
+                If the project does not exist in the session when the call is made, the project will be initialized & returned.
+        """
+        if isinstance(project_name, Project):
+            project = project_name
+        else:
+            try:
+                project = self.project_list[project_name]
+            except KeyError:
+                self.add_project(project_name, add_neighbors=add_neighbors, report_type=report_type)
+                project = self.project_list[project_name]
+ 
+        return project
+
+
+    def add_project(self, project_name:str|Project|ListLike, add_neighbors:bool = True, report_type:str = 'monthly') -> None:
         """Adds & initializes a [Project][ccrenew.dashboard.project.Project]
         to a [DashboardSession][ccrenew.dashboard.session.DashboardSession] instance.
 
         Args:
             project_name (str or Project): The name of the project to add to the [DashboardSession][ccrenew.dashboard.session.DashboardSession] instance.
-            get_neighbors (bool, optional): Flag to add & initialize neighbor [Projects][ccrenew.dashboard.project.Project].
+            add_neighbors (bool): Flag to add & initialize neighbor [Projects][ccrenew.dashboard.project.Project].
+            report_type (str): Method for processing the project. Options are `monthly`, `ul`, or `weekly`.
         """
         # Type validation
-        if not isinstance(project_name, (str, Iterable, Project)):
+        if not isinstance(project_name, (str, ListLike, Project)):
             raise TypeError("`project_name` must be a string, Project object, or Python list! Please reformat input and try again.")
 
         # Determine behavior based on what was passed to method
-        if isinstance(project_name, Iterable) and not isinstance(project_name, str):
-            self.add_projects(project_name)
+        if isinstance(project_name, ListLike):
+            project_list = list(project_name)
+            self.add_projects(project_list, add_neighbors=add_neighbors, report_type=report_type)
+
         elif project_name in self.project_list:
-            project = self.project_list[project_name]
+            return
+
         elif isinstance(project_name, Project):
             project = project_name
             self.project_list[project.project_name] = project
-        else:
-            project = self.__initialize_project(project_name, get_neighbors=get_neighbors)
-            self.project_list[project.project_name] = project
 
-        return project
+        else:
+            project = self.__initialize_project(project_name, add_neighbors=add_neighbors, report_type=report_type)
+            if not project.error_info:
+                self.project_list[project.project_name] = project
     
 
-    def add_projects(self, project_list, get_neighbors=True):
+    def add_projects(self, project_list:ListLike|str|Project, add_neighbors:bool = True, report_type:str = 'monthly') -> None:
         """Calls [add_project()][ccrenew.dashboard.session.DashboardSession.add_project] for each project in a list.
 
         Args:
             project_list (list, str): list of project names to add & initialize to the [DashboardSession][ccrenew.dashboard.session.DashboardSession] instance.
-            get_neighbors (bool, optional): See [add_project()][ccrenew.dashboard.session.DashboardSession.add_project].
+            add_neighbors (bool): See [add_project()][ccrenew.dashboard.session.DashboardSession.add_project].
+            report_type (str): See [add_project()][ccrenew.dashboard.session.DashboardSession.add_project].
         """
         if isinstance(project_list, (str, Project)):
-            self.add_project(project_list, get_neighbors=get_neighbors)
+            self.add_project(project_list, add_neighbors=add_neighbors, report_type=report_type)
 
-        elif isinstance(project_list, Iterable):
+        elif isinstance(project_list, ListLike):
             for project_name in project_list:
-                try:
-                    self.add_project(project_name, get_neighbors=get_neighbors)
-                except Exception as e:
-                    print(e)
+                project = self.get_project(project_name, add_neighbors=add_neighbors, report_type=report_type)
+                if project.error_info:
+                    print(f"Could not add {project_name} to the `DashboardSession` instance. See error below:")
+                    print(project.error_info)
                     continue
-        
+
         else:
             raise TypeError("`project_list` must be a string, Project object, or Python list! Please reformat input and try again.")
                 
 
-    def __initialize_project(self, project_name, get_neighbors=True):
+    def __initialize_project(self, project_name:str, add_neighbors:bool, report_type:str):
         """Initializes a project object with metadata
 
         Args:
             project_name (str): Name of a project to initialize.
-            get_neighbors (bool, optional): Flag to add & initialize neighbor projects. Defaults to True.
+            add_neighbors (bool): Flag to add & initialize neighbor projects.
+            report_type (str): Method for processing the project. Options are `monthly`, `ul`, or `weekly`.
 
         Returns:
             Project: An initialized Project object
         """
 
         try:
             df_proj_keys = self.df_keys.query("Project == @project_name").to_dict('records')[0]
             df_proj_ss_comments = self.df_ss_comments.query("index == @project_name").to_dict('records')[0]
         except IndexError:
             # Log that project was not found
             warn_msg = '"{}" not found in df keys. Please verify the project is present in df keys & the spelling is correct and try again'.format(project_name)
             print(warn_msg)
             # logger.warn(warn_msg)
-            # logger.warn(warn_msg)
-
-            # Remove project from project_list since we won't be able to initialize it
-            del self.project_list[project_name]
-            return
+            df_proj_keys = {'Racking': 'None'}
+            df_proj_ss_comments = {}
+            proj_init_dict = {'error_info': warn_msg}
 
         # Get neighbor projects
-        if get_neighbors:
-            neighbor_list = self.__get_neighbors(project_name)
-        else:
-            neighbor_list = {}
+        neighbor_list = self.__find_neighbors(project_name, add_neighbors=add_neighbors, report_type=report_type)
 
         # Set battery/tracker attributes
         Battery_AC_site = project_name in self.battery_ac_sites
         Battery_DC_site = project_name in self.battery_dc_sites
         Tracker_site = df_proj_keys['Racking'] == 'Tracker'
         
         proj_init_dict = {}
         proj_init_dict['project_name'] = project_name
         proj_init_dict['df_proj_keys'] = df_proj_keys
         proj_init_dict['df_proj_ss_comments'] = df_proj_ss_comments
         proj_init_dict['dashboard_dir'] = self.dashboard_dir
         proj_init_dict['data_cutoff_date'] = self.data_cutoff_date
+        proj_init_dict['data_platform'] = self.data_platform
+        proj_init_dict['data_platform_dirs'] = self.data_platform_dirs
         proj_init_dict['data_source'] = self.data_source
+        proj_init_dict['report_type'] = report_type
         proj_init_dict['Battery_AC_site'] = Battery_AC_site
         proj_init_dict['Battery_DC_site'] = Battery_DC_site
         proj_init_dict['Tracker_site'] = Tracker_site
         proj_init_dict['raw_snow_df'] = self.raw_snow_df
         proj_init_dict['snow_file'] = self.snow_file
         proj_init_dict['snow_file'] = self.snow_file
         proj_init_dict['neighbor_list'] = neighbor_list
 
-        project = Project(proj_init_dict)
+        try:
+            project = Project(proj_init_dict)
+        except:
+            print(f"**** {project_name} errored during initialization and will not be added to the DashboardSession.")
+            proj_init_dict['error_info'] = traceback.format_exc()
+            project = Project(proj_init_dict)
+
         return project
     
 
-    def __get_neighbors(self, project_name):
+    def __find_neighbors(self, project_name:str, add_neighbors:bool, report_type:str):
         # Find all neighbors that satisfy the distance and equipment requirements
         all_neighbors = neighbs.find_nearby_projects(project_name, print_data=False, include_retired=False).index.tolist()
         poa_neighbors = neighbs.find_nearby_similar_projects(project_name, print_data=False, include_retired=False).index.tolist()
         
         # Then remove the search project from the list
         # (Sometimes it will return an empty list if there is some data missing in `df_keys`) so we need to check if it returned a non-empty list first
         try:
@@ -303,445 +373,486 @@
 
         # We'll create a neighbor_list dictionary
         # Value=True: we can use it for POA data sub
         # Value=False: we can only use it for weather data sub
         neighbor_list = {project_name: True if project_name in poa_neighbors else False for project_name in all_neighbors}
 
         # If the project has neighbors, we'll add them to the DashboardSession instance
-        # Set get_neighbors to False so we don't get neighbors of neighbors of neighbors etc.
-        if neighbor_list:
-            self.add_projects(neighbor_list, get_neighbors=False)
+        # Set add_neighbors to False so we don't get neighbors of neighbors of neighbors etc.
+        if add_neighbors:
+            for neighbor in neighbor_list.copy():
+                try:
+                    self.add_project(neighbor, add_neighbors=False, report_type=report_type)
+                except:
+                    neighbor_list.pop(neighbor)
         
         return neighbor_list
 
 
-    def get_project(self, project_name: str, get_neighbors: bool=True) -> Project:
-        """
-        Return a [Project][ccrenew.dashboard.project.Project] object given a project name.
-
-        Args:
-            project_name (str or Project): Name of a [Project][ccrenew.dashboard.project.Project] to return from the
-                [DashboardSession][ccrenew.dashboard.session.DashboardSession] instance.
-                If project does not yet exist in the session, it will be added then returned.
-            get_neighbors (bool, optional): Flag to add & initialize neighbor [Projects][ccrenew.dashboard.project.Project].
-
-        Returns:
-            Project object for the given the project name.
-                If the project does not exist in the session when the call is made, the project will be initialized & returned.
-        """
-        if isinstance(project_name, Project):
-            return project_name
+    def _source_file_updates(self, project:Project, reprocess:bool) -> bool:
+        # Pull the last updated dates from the filesystem for the config, bool, & Powertrack files
         try:
-            project = self.project_list[project_name]
-        except KeyError:
-            self.add_project(project_name, get_neighbors=get_neighbors)
-            project = self.project_list[project_name]
- 
- 
-        return project
+            last_update_config_file = get_modified_time(project.config_filepath, self.data_platform, 'file')
+            last_update_bool_file = get_modified_time(project.bool_filepath, self.data_platform, 'file')
+            last_update_powertrack_file = get_modified_time(project.powertrack_filepath, self.data_platform, 'file')
+        except:
+            self.__update_project_filepaths(project)
+            last_update_config_file = get_modified_time(project.config_filepath, self.data_platform, 'file')
+            last_update_bool_file = get_modified_time(project.bool_filepath, self.data_platform, 'file')
+            last_update_powertrack_file = get_modified_time(project.powertrack_filepath, self.data_platform, 'file')
+
+        # Check if the config, bool, or Powertrack files have been updated.
+        # If not we don't need to process.
+        if reprocess:
+            project.last_update_config = datetime.fromtimestamp(0)
+            project.last_update_bool = datetime.fromtimestamp(0)
+            project.last_update_powertrack = datetime.fromtimestamp(0)
+
+        any_file_updates =  any([project.last_update_config != last_update_config_file,
+                                 project.last_update_bool != last_update_bool_file,
+                                 project.last_update_powertrack != last_update_powertrack_file])
+        
+        return any_file_updates
 
 
-    def process_project(self, project_name: str, reprocess: bool=False) -> Project:
+    def process_project(self, project_name:str|Project|ListLike, reprocess:bool = False, datasub:bool = False,
+                        use_solcast:bool = True, report_type:str = 'monthly', **kwargs) -> Project:
         """
         Process data for the given [Project][ccrenew.dashboard.project.Project].
 
         Args:
             project_name (str or Project): The name of the [Project][ccrenew.dashboard.project.Project] to process.
             reprocess (bool): Whether to reprocess the data. This option will likely
                 be uncommon as any changes to a [Project's][ccrenew.dashboard.project.Project] config file or powertrack file will
                 automatically reprocess that data. This could be used if any changes are made
                 outside of the config/powertrack file or a change is made to a neighbor.
+            datasub (bool): Option to use automatic data substitution algorithm.
+            use_solcast (bool): Option to use Solcast data in data sub process. `datasub`
+                must be set to `True` for this option to take effect.
+            report_type (str): Method for processing the project. Options are `monthly`, `ul`, or `weekly`.
         Returns:
             Processed Project object.
         """
-        if isinstance(project_name, Iterable) and not isinstance(project_name, str):
-            # If we call this method with a list we'll default to series processing
-            project_list = project_name
-            project = self.process_projects(project_list=project_list, method='series', reprocess=reprocess)
+        if isinstance(project_name, ListLike):
+            # If we call this method with a list we'll default to series processing & return the first project in the list
+            project_list = list(project_name)
+            self.process_projects(project_list=project_list, method='series', reprocess=reprocess,
+                                  datasub=datasub, use_solcast=use_solcast, report_type=report_type, **kwargs)
+
+            # BUGFIX: handle this when it doesn't return a valid project
+            project = self.project_list[project_list[0]]
             
             return project
 
         elif isinstance(project_name, (str, Project)):
             start = time.time()
+
             # Get project object
-            try:
-                project = self.get_project(project_name)
-            except Exception as e:
-                print(e)
-                # Create a blank object with project_name & error_info attributes for error handling
-                project = types.SimpleNamespace()
-                project.project_name = project_name
-                project.error_info = e
-                return project
+            project = self.get_project(project_name, report_type=report_type)
+            
+            # Add any neighbors that haven't been initialized yet
+            self.add_projects(project.neighbor_list, add_neighbors=False, report_type=report_type)
 
-            # Pull the last updated dates from the filesystem for the config, bool, & Powertrack files
-            try:
-                last_update_config_file = os.path.getmtime(project.config_filepath)
-                last_update_bool_file = os.path.getmtime(project.bool_filepath)
-                last_update_powertrack_file = os.path.getmtime(project.powertrack_filepath)
-            except:
-                self.__update_project_filepaths(project)
-                last_update_config_file = os.path.getmtime(project.config_filepath)
-                last_update_bool_file = os.path.getmtime(project.bool_filepath)
-                last_update_powertrack_file = os.path.getmtime(project.powertrack_filepath)
-
-            # Check if the config, bool, or Powertrack files have been updated.
-            # If not we don't need to process.
-            if any([project.last_update_config != last_update_config_file,
-                    project.last_update_bool != last_update_bool_file,
-                    project.last_update_powertrack != last_update_powertrack_file]):
+            if project.errored:
+                print(f"{project.project_name} errored. Error details:\n{project.error_info}")
+                return project
+            
+            # If the project has already been added to the session but we want to run it with a different process method
+            # We'll update the process method & force the config file to reload
+            if project.report_type != report_type:
+                project.report_type = report_type
+                project.last_update_config = datetime.fromtimestamp(0)
+
+            # Check if any source files (bool, config, powertrack) have been updated
+            if datasub != project.datasub:
+                reprocess = True
 
-                # Pull config and/or Powertrack data
+            if self._source_file_updates(project, reprocess):
+                # Pull updated source file data
                 self.__prepare_source_data(project)
             else:
-                if project.processed and not reprocess:
+                if project.processed:
                     print('{} already processed'.format(project.project_name))
 
                     return project
 
             # Process data - update neighbor sensors first then process the project
-            print(f'Processing {project_name}....')
-            project.neighbor_list = self.__get_neighbors(project_name)
-            self.__get_neighbor_sensor_data(project)
+            print(f'Fetching neighbor data for {project_name}....')
+
+            # Update neighbor data based on Get_Sensor in the config file
+            self.__get_config_neighbor_sensor_data(project)
             failed_neighbors = []
             for neighbor_name in project.neighbor_list:
                 try:
-                    neighbor = self.project_list[neighbor_name]
-                    if neighbor.df.empty:
-                        neighbor.load_production_data()
-                    if neighbor.df_sensors_native_avg.empty:
+                    neighbor = self.get_project(neighbor_name)
+                    if self._source_file_updates(neighbor, reprocess=False) or neighbor.df_sensors_native_avg.empty:
+                        self.__prepare_source_data(neighbor)
                         neighbor._calculate_native_sensor_averages()
-                except Exception as e:
-                    print(e)
+                except:
+                    print(f"Neighbor for {project.project_name} failed while processing")
+                    print(f"Neighbor name: {neighbor_name}")
+                    print(f"Error message: {traceback.format_exc()}")
                     failed_neighbors.append(neighbor_name)
+
                     continue
+
             for neighbor_name in failed_neighbors:
                 del project.neighbor_list[neighbor_name]
-            neighbor_sensors = {self.project_list[neighbor].project_name: self.project_list[neighbor].df_sensors_native_avg for neighbor in project.neighbor_list}
+
+            neighbor_sensor_data = {self.project_list[neighbor].project_name: self.project_list[neighbor].df_sensors_native_avg for neighbor in project.neighbor_list}
 
             try:
-                project._process_data(neighbor_sensors=neighbor_sensors, get_solcast=True)
+                project._process_data(neighbor_sensor_data=neighbor_sensor_data,
+                                      datasub=datasub, use_bluesky=use_solcast)
             except Exception:
                 print('\n')
                 print('###########################')
-                print(f'{project.project_name} not processed. See below for error information.')
+                print(f"{project.project_name} not processed. See below for error information. Error message can also be found in the Project's error_info attribute")
                 print(traceback.format_exc())
                 print('###########################')
 
-                project.last_update_powertrack = 0
+                project.last_update_powertrack = datetime.fromtimestamp(0)
                 project.errored = True
                 project.error_info = traceback.format_exc()
 
                 return project
             project.processed = True
             project.errored = False
+
             print('{} successfully processed. Processing time: {:.2f}s'.format(project.project_name, time.time()-start))
 
             return project
         else:
             raise TypeError("`project_name` must be a string or Project object! Please reformat input and try again.")
     
     
-    def process_projects(self, project_list, method='series', reprocess=False):
+    def process_projects(self, project_list:str|Project|list, method:str = 'series', reprocess:bool = False,
+                         datasub:bool = False, use_solcast:bool = True, report_type:str = 'monthly', **kwargs):
         """Calls [process_project()][ccrenew.dashboard.session.DashboardSession.process_project] for each
         [Project][ccrenew.dashboard.project.Project] in a list.
 
         Args:
             project_list (list): List of [Project][ccrenew.dashboard.project.Project] names process.
-            method (str): Option to perform processing operations in series or parallel.
-            reprocess (bool): See [process_project()][ccrenew.dashboard.session.DashboardSession.process_project].
-            method (str): Option to perform processing operations in series or parallel.
-            reprocess (bool): See [process_project()][ccrenew.dashboard.session.DashboardSession.process_project].
+            method (str): Option to perform processing operations in `series` or `parallel`.
+        
+        *See [process_project()][ccrenew.dashboard.session.DashboardSession.process_project] for information on other arguments.
         """
         if isinstance(project_list, (str, Project)):
             project_name = project_list
-            project = self.process_project(project_name, reprocess)
-
+            project = self.process_project(project_name, reprocess=reprocess, datasub=datasub,
+                                           use_solcast=use_solcast, report_type=report_type)
             return project
-        elif isinstance(project_list, Iterable):
+
+        elif isinstance(project_list, list):
             if len(project_list) == 1:
                 project_name = project_list[0]
-                project = self.process_project(project_name, reprocess)
-                project = self.process_project(project_name, reprocess)
-
+                project = self.process_project(project_name, reprocess=reprocess, datasub=datasub,
+                                               use_solcast=use_solcast, report_type=report_type)
                 return project
+            
             else:
-                if method == 'series':
-                    start = time.time()
-                    for i, project_name in enumerate(project_list):
-                        project = self.process_project(project_name, reprocess)
-                        if not project:
-                            continue
+                start = time.time()
+                successful_projects = []
+                errored_projects = []
 
-                        elapsed = time.time() - start
-                        print('*******************************************************')
-                        print(f'{project_name} complete. {i+1} of {len(project_list)} projects completed. Total elapsed time: {elapsed:2f}s')
-                        print('*******************************************************')
-
-                elif __name__ == 'ccrenew.dashboard.session':
-                    start = time.time()
-
-                    # We'll use half of the available processors for the machine to not completely bog it down.
-                    max_workers = int(os.cpu_count()/2)
-                    print(f"Processing {len(project_list)} projects with {min(max_workers, len(project_list))} workers.")
-                    print("Progress messages from workers will be suppressed in an interactive session.")
-                    print("Projects will report success upon completion and may not complete in the order in which they were submitted.")
-
-                    # Construct a dict of kwargs for each project to pass to `process_pool`
-                    kwargslist =  [{"project_name":project_name,
-                                    "session":DashboardSession,
-                                    "data_source": self.data_source,
-                                    "reprocess":reprocess,
-                                    "project_num":i+1,
-                                    "project_total":len(project_list),
-                                    "batch_start":start
-                                    } for i, project_name in enumerate(project_list)]
-
-                    # Results are a list of Future objects, where we can get the results of the function call from `.result()`
-                    results = process_pool(kwargslist)
-                    for result in results:
-                        processed_project_list = result.result()['project_list']
-                        for project_dict in processed_project_list:
-                            try:
-                                project_name, project = project_dict
-                                # If the project is already processed in the parent session we won't add it
-                                if project_name in self.project_list and self.project_list[project_name].processed:
-                                    pass
-                                else:
-                                    self.project_list[project_name] = project
-                            except:
-                                continue
-
-                elapsed = time.time() - start
-                print(f"\n{len(project_list)} projects processed. Elapsed time: {elapsed:.2f}s.\n")
                 if method == 'series':
-                    start = time.time()
                     for i, project_name in enumerate(project_list):
-                        project = self.process_project(project_name, reprocess)
-                        if not project:
+                        project = self.process_project(project_name, reprocess=reprocess, datasub=datasub, use_solcast=use_solcast)
+                        if not project or project.errored:
+                            print(f"{project_name} encountered an error while processing.")
+                            errored_projects.append(project_name)
+
                             continue
 
                         elapsed = time.time() - start
                         print('*******************************************************')
                         print(f'{project_name} complete. {i+1} of {len(project_list)} projects completed. Total elapsed time: {elapsed:2f}s')
                         print('*******************************************************')
+                        successful_projects.append(project.project_name)
 
                 elif __name__ == 'ccrenew.dashboard.session':
-                    start = time.time()
-
                     # We'll use half of the available processors for the machine to not completely bog it down.
-                    max_workers = int(os.cpu_count()/2)
+                    max_workers = int(os.cpu_count()/2) # type: ignore
                     print(f"Processing {len(project_list)} projects with {min(max_workers, len(project_list))} workers.")
                     print("Progress messages from workers will be suppressed in an interactive session.")
                     print("Projects will report success upon completion and may not complete in the order in which they were submitted.")
 
                     # Construct a dict of kwargs for each project to pass to `process_pool`
-                    kwargslist =  [{"project_name":project_name,
-                                    "session":DashboardSession,
-                                    "data_source": self.data_source,
-                                    "reprocess":reprocess,
-                                    "project_num":i+1,
-                                    "project_total":len(project_list),
-                                    "batch_start":start
+                    if self.data_platform == 's3':
+                        data_source = self.data_source + 's3'
+                    else:
+                        data_source = self.data_source
+
+                    kwargslist =  [{"project_name": project_name,
+                                    "session": DashboardSession,
+                                    "data_source": data_source,
+                                    "reprocess": reprocess,
+                                    "datasub": datasub,
+                                    "use_solcast": use_solcast,
+                                    "project_num": i+1,
+                                    "project_total": len(project_list),
+                                    "batch_start": start
                                     } for i, project_name in enumerate(project_list)]
 
                     # Results are a list of Future objects, where we can get the results of the function call from `.result()`
                     results = process_pool(kwargslist)
+
                     for result in results:
                         processed_project_list = result.result()['project_list']
                         for project_dict in processed_project_list:
                             try:
                                 project_name, project = project_dict
                                 # If the project is already processed in the parent session we won't add it
                                 if project_name in self.project_list and self.project_list[project_name].processed:
                                     pass
                                 else:
                                     self.project_list[project_name] = project
+                                
                             except:
                                 continue
 
+                        exported_project_name = result.result()['project_name']
+                        exported_project = self.project_list[exported_project_name]
+                        if exported_project.errored:
+                            errored_projects.append(exported_project_name)
+                        else:
+                            successful_projects.append(exported_project_name)
+
                 elapsed = time.time() - start
-                print(f"\n{len(project_list)} projects processed. Elapsed time: {elapsed:.2f}s.\n")
+                print(f"\n{len(successful_projects)} projects successfullly processed.\n{len(errored_projects)} errored. Elapsed time: {elapsed:.2f}s.\n")
+                print(f"Errored projects: {errored_projects}")
+       
         else:
             raise TypeError("`project_list` must be a string or Python list! Please reformat input and try again.")
 
 
-    def process_all_projects(self, method='parallel', reprocess=True):
+    def process_all_projects(self, method:str = 'parallel', reprocess:bool = True, datasub:bool = False,
+                             use_solcast:bool = True, report_type:str = 'monthly', **kwargs):
         """
         Processes all projects in the [project_list][ccrenew.dashboard.session.DashboardSession.project_list]
         for the [DashboardSession][ccrenew.dashboard.session.DashboardSession] instance.
 
-        Args:
-            method (str): Option to perform operations in series or parallel.
-            reprocess (bool): See [process_project()][ccrenew.dashboard.session.DashboardSession.process_project].
+        *See [process_project()][ccrenew.dashboard.session.DashboardSession.process_project] for information on function arguments.
         """
         project_list = list(self.project_list.keys())
-        self.process_projects(project_list, method=method, reprocess=reprocess)
+        self.process_projects(project_list, method=method, reprocess=reprocess,
+                              datasub=datasub, use_solcast=use_solcast, report_type=report_type)
     
 
-    def export_project(self, project_name: str, server: str='dev', save_pickle: bool=True, dest: str|list='all') -> None:
+    def export_project(self, project_name:str|ListLike, server:str = 'dev', dest:str|list = 'all',
+                       report_type:str = 'monthly', use_solcast:bool = True, save_pickle:bool = True, **kwargs) -> None:
         """
         Export project to desired location(s).
 
         Args:
             project_name (str or Project): Name of a project to export.
-            server (str): SQL table to export to. Options are `prod` or `dev`.
+            server (str): Environment . Options are `prod` or `dev`, or `datasub`.
+            dest (str or list): Option to export only certain parts of the project. `all` will export to all of the below destinations **except bool**.
+            report_type (str): Option to select which report type to run. Options are `monthly`, `ul`, and `weekly`.
             save_pickle (bool): Option to save pickle after exporting.
-            dest (str or list): Option to export only certain parts of the project. `all` will export to all of the below destinations.
+            **kwargs: Optional arguments passed to [process_project()][ccrenew.dashboard.session.DashboardSession.process_project].
 
         `dest` Options
 
         | dest      | Description                                                              |
         |-----------|--------------------------------------------------------------------------|
-        |  `excel`  | Export dataframes to Excel dashboard template.                          |
-        |   `df`    | Export dataframe to the `Dataframes` folder of the project's [project_directory][ccrenew.dashboard.project.Project.project_directory], S3, and Bartertown PostgreSQL database. |
-        | `summary` | Export monthly summary data to S3 and Bartertown PostgreSQL database.   |
+        |  `excel`  | Export dataframes to Excel dashboard template.                           |
+        |   `df`    | Export dataframe to the `Dataframes` folder of the project's [project_directory][ccrenew.dashboard.project.Project.project_directory], S3, and Bartertown PostgreSQL database. See below for export locations based on `server` selection. |
+        | `summary` | Export monthly summary data to S3 and Bartertown PostgreSQL database. See below for export locations based on `server` selection. |
         |  `snow`   | Export [snow_data][ccrenew.dashboard.project.Project.snow_data] and [snow_coverage][ccrenew.dashboard.project.Project.snow_coverage] dataframes to S3. |
         |  `bool`   | Export bool file to the `Plant_Config_File` directory of the project's [project_directory][ccrenew.dashboard.project.Project.project_directory]. |
+
+        `server` SQL Destinations
+
+        |   server   | `df`                  | `summary`               |
+        |------------|-----------------------|-------------------------|
+        |   `prod`   | am_processed_data     | am_summary_data         |
+        |   `dev`    | am_processed_data_dev | am_summary_data         |
+        | `datasub`  | am_processed_data_dev | am_summary_data_datasub |
+
+        `server` S3 Destinations
+
+        |   server   | bucket                                         | `df` prefix          | `summary` prefix      |
+        |------------|------------------------------------------------|----------------------|-----------------------|
+        |   `prod`   | s3://cypress-perfeng-datalake-dev-us-west-2    | Curated/HourlyLosses | Curated/MonthlyLosses |
+        |   `dev`    | s3://cypress-perfeng-datalake-onprem-us-west-2 | Curated/HourlyLosses | Curated/MonthlyLosses |
+        | `datasub`  | s3://cypress-perfeng-datalake-onprem-us-west-2 | Curated/HourlyLosses | Curated/MonthlyLosses |
         """
         # Pass function arguments to `export_projects()`.
         # Remove `self`, i.e. the DashboardSession instance
         func_args = locals().copy()
         func_args.pop('self')
 
-        if isinstance(project_name, Iterable) and not isinstance(project_name, str):
+        if isinstance(project_name, ListLike):
             # Rename project_name to project_list for `export_projects`
             func_args.pop('project_name')
-            func_args['project_list'] = project_name
+            func_args['project_list'] = list(project_name)
             self.export_projects(**func_args)
+
         elif isinstance(project_name, (str, Project)):
-            project = self.get_project(project_name)
+            project = self.get_project(project_name, report_type=report_type)
+            if project.errored:
+                raise Exception(f"{project.project_name} errored. Error details:\n{project.error_info}")
 
             # If we're only exporting the bool file then we don't need to process
             if dest != 'bool':
+                datasub = False
+                if server == 'datasub':
+                    datasub = True
+                self.process_project(project_name, datasub=datasub, use_solcast=use_solcast,
+                                     report_type=report_type, **kwargs)
+            else:
                 func_args['save_pickle'] = False
-                self.process_project(project_name)
 
             func_args.pop('project_name')
             project.export(**func_args)
             print(f"{project.project_name} successfully exported.")
         else:
             raise TypeError("`project_name` must be a string or Project object! Please reformat input and try again.")
 
-    
-    def export_projects(self, project_list: str, server: str='dev', save_pickle: bool=True, dest: str|list='all', method: str='series') -> None:
+  
+    def export_projects(self, project_list:ListLike|str, method:str = 'series', server:str = 'dev',
+                        dest:str|list = 'all', report_type:str = 'monthly', use_solcast:bool = True,
+                        save_pickle:bool = True, **kwargs) -> None:
         """Calls [export_project()][ccrenew.dashboard.session.DashboardSession.export_project] for each
         [Project][ccrenew.dashboard.project.Project] in a list.
 
         Args:
             project_list (list): List of [Project][ccrenew.dashboard.project.Project] names process.
-            server (str): See [export_project()][ccrenew.dashboard.session.DashboardSession.export_project].
-            save_pickle (bool): See [export_project()][ccrenew.dashboard.session.DashboardSession.export_project].
-            dest (str or list): See [export_project()][ccrenew.dashboard.session.DashboardSession.export_project].
-            method(str): Option to export in series or parallel.
+            method (str): Option to export in `series` or `parallel`.
+        
+        *See [export_project()][ccrenew.dashboard.session.DashboardSession.export_project] for information on other arguments.
         """
         # Store function arguments in case we need to pass them to `export_project()`.
         # Argument 0 is `self` so we'll pass arguments 1 and on
         func_args = locals().copy()
         func_args.pop('self')
         method = func_args.pop('method')
 
         if isinstance(project_list, (str, Project)):
             # Rename project_list to project_name for `export_project`
             func_args.pop('project_list')
             func_args['project_name'] = project_list
             self.export_project(**func_args)
-        elif isinstance(project_list, Iterable):
+
+        elif isinstance(project_list, ListLike):
             # If a list was passed, we'll pop the project list & use the remaining args
-            project_list = func_args.pop('project_list')
+            project_list = list(func_args.pop('project_list'))
 
             if len(project_list) == 1:
                 project_name = project_list[0]
                 self.export_project(project_name, **func_args)
+
             else:
+                start = time.time()
+                successful_projects = []
+                errored_projects = []
+
                 if method == 'series':
-                    start = time.time()
                     for i, project_name in enumerate(project_list):
-                        self.export_project(project_name, **func_args)
+                        try:
+                            self.export_project(project_name, **func_args)
+                        except:
+                            errored_projects.append(project_name)
+                            continue
                     
                         elapsed = time.time() - start
                         print('*******************************************************')
                         print(f'{project_name} complete. {i+1} of {len(project_list)} projects exported. Total elapsed time: {elapsed:2f}s')
                         print('*******************************************************')
+                        successful_projects.append(project_name)
                 
                 elif __name__ == 'ccrenew.dashboard.session':
-                    start = time.time()
 
                     # We'll use half of the available processors for the machine to not completely bog it down.
-                    max_workers = int(os.cpu_count()/2)
+                    max_workers = int(os.cpu_count()/2) # type: ignore
                     print(f"Exporting {len(project_list)} projects with {min(max_workers, len(project_list))} workers.")
                     print("Progress messages from workers will be suppressed in an interactive session.")
                     print("Projects will report success upon completion and may not complete in the order in which they were submitted.")
 
                     # Construct a dict of kwargs for each project to pass to `process_pool`
-                    kwargslist =  [{"project_name":project_name,
-                                    "session":DashboardSession,
-                                    "data_source": self.data_source,
-                                    "func_args":func_args,
-                                    "project_num":i+1,
-                                    "project_total":len(project_list),
-                                    "batch_start":start
+                    if self.data_platform == 's3':
+                        data_source = self.data_source + 's3'
+                    else:
+                        data_source = self.data_source
+
+                    kwargslist =  [{"project_name": project_name,
+                                    "session": DashboardSession,
+                                    "data_source": data_source,
+                                    "func_args": func_args,
+                                    "project_num": i+1,
+                                    "project_total": len(project_list),
+                                    "batch_start": start
                                     } for i, project_name in enumerate(project_list)]
 
                     # Results are a list of Future objects, where we can get the results of the function call from `.result()`
                     results = export_pool(kwargslist)
                     for result in results:
-                        exported_project_list = result.result()['project_list']
-                        for project_dict in exported_project_list:
+                        all_projects = result.result()['project_list']
+                        for project_dict in all_projects:
                             try:
                                 project_name, project = project_dict
                                 # If the project is already processed in the parent session we won't add it
                                 if project_name in self.project_list and self.project_list[project_name].processed:
                                     pass
                                 else:
                                     self.project_list[project_name] = project
+
                             except:
                                 continue
 
+                        exported_project_name = result.result()['project_name']
+                        exported_project = self.project_list[exported_project_name]
+                        if exported_project.errored:
+                            errored_projects.append(exported_project_name)
+                        else:
+                            successful_projects.append(exported_project_name)
+
                 elapsed = time.time() - start
-                print(f"\n{len(project_list)} projects exported. Elapsed time: {elapsed:.2f}s.\n")                        
+                print(f"\n{len(successful_projects)} projects successfullly exported.\n{len(errored_projects)} errored. Elapsed time: {elapsed:.2f}s.\n")
+                print(f"Errored projects: {errored_projects}")
 
         else:
             raise TypeError("`project_list` must be a string or Python list! Please reformat input and try again.")
 
 
     def remove_project(self, project_name:str) -> None:
         """Remove the selected project from the active session.
 
         Args:
             project_name (str): The name of the [Project][ccrenew.dashboard.project.Project]
                 to remove from the [DashboardSession][ccrenew.dashboard.session.DashboardSession] instance.
         """
         del self.project_list[project_name]
 
-    def get_ss_comments(self, project_name:str, num_comments: int=None) -> None:
+    def get_ss_comments(self, project_name:str, num_comments: int|None=None) -> None:
         """Prints Smartsheet comments for the [Project][ccrenew.dashboard.project.Project].
 
         Args:
             project_name (str): Name of the [Project][ccrenew.dashboard.project.Project] to pull comments for.
             num_comments (int, optional): Number of comments to show, starting from the
                 most recent. I.e. `5` will show the most recent 5 comments in the
                 Smartsheet. Defaults to None, which will show all comments starting in Jan 2021.
         """
-        project = self.get_project(project_name, get_neighbors=False)
+        project = self.get_project(project_name, add_neighbors=False)
         project.get_ss_comments(num_comments=num_comments)
 
 
     def save_pickle(self, project_name, store_plots=False):
         """Saves the [Project][ccrenew.dashboard.project.Project] to a serialized pickle in its
         [project_directory][ccrenew.dashboard.project.Project.project_directory].
 
         Args:
             project_name (str or Project): The name of the [Project][ccrenew.dashboard.project.Project] to pickle.
             store_plots (bool, optional): Option to store any plots that have been drawn with the project to the pickle.
 
         Raises:
             TypeError: if the wrong type is supplied to `project_name`.
         """
-        if isinstance(project_name, Iterable) and not isinstance(project_name, str):
+        if isinstance(project_name, list) and not isinstance(project_name, str):
             self.save_pickles(project_name, store_plots=store_plots)
         elif isinstance(project_name, (str, Project)):
             project = self.process_project(project_name)
             project.save_pickle(store_plots=store_plots)
         else:
             raise TypeError("`project_name` must be a string or Project object! Please reformat input and try again.")
 
@@ -753,15 +864,15 @@
         Args:
             project_list (list, str, or Project): List of [Project][ccrenew.dashboard.project.Project] names to pickle.
             store_plots (bool, optional): See [pickle_project()][ccrenew.dashboard.session.DashboardSession.pickle_project].
         """
         if isinstance(project_list, (str, Project)):
             project_name = project_list
             self.save_pickle(project_name, store_plots=store_plots)
-        elif isinstance(project_list, Iterable):
+        elif isinstance(project_list, list):
             for i, project_name in enumerate(project_list):
                 print('*******************************************************')
                 print(f'Pickling {project_name} - Project {i+1} of {len(project_list)}.')
                 print('*******************************************************')
                 self.save_pickle(project_name, store_plots=store_plots)
         else:
             raise TypeError("`project_list` must be a string or Python list! Please reformat input and try again.")
@@ -814,23 +925,30 @@
                                   project_name,
                                   'Pickle_Jar')
         
         pickle_name = utils.picklefy_project_name(project_name)
         pickle_file = year + "_" + pickle_name + ".pickle"
         pickle_path = os.path.join(pickle_jar, pickle_file)
         
+        if self.data_platform == 's3':
+            pickle_path = Path(pickle_path).as_posix().replace('s3:/', 's3://')
+            fs = s3fs.S3FileSystem()
+            open = fs.open
+        else:
+            open = builtins.open
+
         with open(pickle_path, 'rb') as f:
-            project = pickle.load(f)
+            project = pickle.load(f) # type: ignore
 
-        # Check if project version matches session version & re-process if not
+        # Check if project version matches session version & add the project fresh if not
         try:
             if project.__version__ != self.__version__:
-                project = self.process_project(project_name)
+                project = self.get_project(project_name, add_neighbors=False)
         except:
-            project = self.process_project(project_name)
+            project = self.get_project(project_name, add_neighbors=False)
 
         # Remove plotter object if show_plots=False
         if not show_plots and project.plotter:
             project.plotter.close_plots()
 
         # Update filepaths to work for any user
         project.dashboard_dir = self.dashboard_dir
@@ -844,14 +962,22 @@
                 self.data_cutoff_date = datetime.today()
         else:
             self.data_cutoff_date = datetime.today()
 
         # Add project to project_list
         self.project_list[project_name] = project
 
+        # Load neighbor pickles if possible
+        # `config_neighbor_sensors` is a set so we'll grab a copy of that & add in `neighbor_sensors`
+        all_neighbors = project.config_neighbor_sensors.copy()
+        all_neighbors.update(project.neighbor_list)
+        for neighbor in all_neighbors:
+            if neighbor not in self.project_list:
+                self.load_pickle(neighbor)
+
         return project
 
 
     def load_pickles(self, project_list, year=None, data_cutoff_date=None, show_plots=False):
         """Calls [load_pickle()][ccrenew.dashboard.session.DashboardSession.load_pickle]
         for each [Project][ccrenew.dashboard.project.Project] in a list.
 
@@ -861,36 +987,47 @@
             data_cutoff_date (str or datetime): See [load_pickle()][ccrenew.dashboard.session.DashboardSession.load_pickle]
             show_plots (bool): See [load_pickle()][ccrenew.dashboard.session.DashboardSession.load_pickle]
         """
         if isinstance(project_list, str):
             project_name = project_list
             self.load_pickle(project_name, year=year, data_cutoff_date=data_cutoff_date, show_plots=show_plots)
             return
-        elif isinstance(project_list, Iterable):
+        elif isinstance(project_list, list):
             for project_name in project_list:
                 try:
                     project = self.load_pickle(project_name, year=year, data_cutoff_date=data_cutoff_date, show_plots=show_plots)
-                    project.plotter = None
-                except Exception as e:
-                    print(e)
+                    if project:
+                        project.plotter.plot_list = {}
+                except:
+                    print(f"Error loading pickle for {project_name}")
+                    print(traceback.format_exc())
+
                     continue
         else:
             raise TypeError("`project_name` must be a string or Python list! Please reformat input and try again.")
 
 
-    def draw_plots(self, project_name, plot_order=None, *args, **kwargs):
+    def draw_plots(self, project_name:str|Project|ListLike, plot_order=[], reprocess:bool = False,
+                        datasub:bool = False, use_solcast:bool = True, *args, **kwargs):
         """Draws plots for the given project.
 
         Args:
             project_name (str, Project, or list): A project name or list of project names
                 to draw plots on for analysis. If a list is supplied it will plot
                 the projects one-by-one. The user must press a button in the final
                 plot of each project to move on to the next one.
             plot_order (list or str, optional): A list of plots to draw. This can
                 be any number of plots from one to all. Defaults to None, which will draw the below plots in the order listed.
+            reprocess (bool): Whether to reprocess the data. This option will likely
+                be uncommon as any changes to a [Project's][ccrenew.dashboard.project.Project] config file or powertrack file will
+                automatically reprocess that data. This could be used if any changes are made
+                outside of the config/powertrack file or a change is made to a neighbor.
+            datasub (bool): Option to use automatic data substitution algorithm.
+            use_solcast (bool): Option to use Solcast data in data sub process. `datasub`
+                must be set to `True` for this option to take effect.
 
         Default Plot Order
 
         | Plot Alias                | Plot Description                                          |
         |---------------------------|-----------------------------------------------------------|
         |    ``xplot_pwr_poa``      |    Crossplot of power meter & POA data                    |
         |    ``xplot_temp``         |    Crossplot of power meter & POA data, colored by Tamb   |
@@ -911,14 +1048,15 @@
 
         Other Optional Plots
 
         | Plot Alias                | Plot Description                                          |
         |---------------------------|-----------------------------------------------------------|
         |    ``meters``             |    Original & corrected power and cumulative meters       |
         |    ``native``             |    Native POA/GHI/Tamb/Tmod/Wind sensor subplots          |
+        |    ``inv_cum``            |    Inverter power & energy plots                          |
 
         Keyword Args:
             mth (int): The month to show on the Power vs POA crossplot. Defaults to current month.
             default_tool (str): The default tool for navigating around the plots. Options
                 are `zoom` and `pan`. Defaults to `zoom`.
             redraw (bool): Option to force the session to redraw the plots.
             open_folder (bool): Option to open the project's folder on the filesystem. Defaults to False.
@@ -933,167 +1071,53 @@
             screen (int): 1-based index of screen to draw plots on. I.e. a workstation
                 with 3 monitors would accept 1, 2, or 3 as an argument.
             poa_onboarding (bool): Plots POA correlation for all months instead of the
                 selected month. Defaults to False.
         """
         if isinstance(project_name, (str, Project)):
             redraw = kwargs.get('redraw', False)
-            project = self.process_project(project_name)
-            neighbor_sensors = {self.project_list[neighbor].project_name: self.project_list[neighbor].df_sensors_native_avg for neighbor in project.neighbor_list}
+            project = self.process_project(project_name, reprocess=reprocess, datasub=datasub, use_solcast=use_solcast)
+            neighbor_sensor_data = {self.project_list[neighbor].project_name: self.project_list[neighbor].df_sensors_native_avg for neighbor in project.neighbor_list}
             try:
                 if project.errored:
-                    raise Exception(f'{project.project_name} encountered an error while processing. Plots cannot be drawn at the moment. To investigate information on the error call `project.error_info`')
+                    raise Exception(f'{project.project_name} encountered an error while processing. Plots cannot be drawn at the moment. Error details:\n{project.error_info}')
             except AttributeError:
                 project.errored = False
 
-            try:
-                plotter = self.plotters[project_name]
-            except KeyError:
-                plotter = Plotter(project_name, neighbor_sensors)
-                self.plotters[project_name] = plotter
-
-            plotter._update_plotter_data(project, neighbor_sensors)
+            project.plotter._update_plotter_neighbors(neighbor_sensor_data)
 
             if not redraw:
                 # Check if the project has an active plotter object & if the plot order is the same
-                if plotter.plot_list == plot_order:
+                if project.plotter.plot_list == plot_order:
                     print('Plots already drawn. Add a new plot to the `plot_list` attribute or set `redraw` = True if you\'d like to redraw the current plots')
                 else:
-                    self.__draw_plots(plotter, plot_order=plot_order, *args, **kwargs)
+                    project.plotter.draw_plots(plot_order=plot_order, *args, **kwargs)
             else:
-                self.__draw_plots(plotter, plot_order=plot_order, *args, **kwargs)
+                project.plotter.draw_plots(plot_order=plot_order, *args, **kwargs)
+
+            # Update session.plotters dictionary
+            self.plotters[project_name] = project.plotter
 
-        elif isinstance(project_name, Iterable):
-            project_list = project_name
+        elif isinstance(project_name, ListLike):
+            project_list = list(project_name)
             project_count = len(project_list)
-            for i, project_name in enumerate(project_list):
-                project = self.get_project(project_name, get_neighbors=False)
+            for i, project_nm in enumerate(project_list):
+                project = self.get_project(project_nm, add_neighbors=False)
                 self.draw_plots(project.project_name, *args, **kwargs)
                 try:
                     print('Press any key in the last plot window to show plots for {}'.format(project_list[i+1]))
                 except IndexError:
                     print('Last plot in the list')
                 while True:
                     if i+1 == project_count:
                         break
                     if waitforbuttonpress():
                         break
 
 
-    def __draw_plots(self, plotter: Plotter, plot_order: list, *args, **kwargs):
-        """
-        Private method to orchestrate drawing of plots
-
-        Args:
-            plotter (Plotter): [Plotter][ccrenew.dashboard.plotting.plots.Plotter] to use to draw plots for analysis
-            plot_order (list): Order of plots to draw.
-        """
-        mth = kwargs.get('mth', None)
-        close_plots = kwargs.get('close_plots', True)
-        min_date = kwargs.get('min_date', None)
-        max_date = kwargs.get('max_date', None)
-        poa_onboarding = kwargs.get('poa_onboarding', False)
-        open_folder = kwargs.get('open_folder', False)
-        fullscreen = kwargs.get('fullscreen', True)
-        persist = kwargs.get('persist', False)
-            
-        # Close all existing plots if requested
-        if close_plots:
-            plotter.close_plots(close_plots)
-
-        # Default month to a month previous to today
-        if not mth:
-            mth = datetime.now().month - 1
-            
-        def parse_date(dt, direction, days=None):
-            if isinstance(dt, Number):
-                if direction == 'backward':
-                    dt = datetime.today() - timedelta(days=abs(dt))
-                else:
-                    dt = datetime.today() + timedelta(days=abs(dt))
-            else:
-                try:
-                    dt = parser.parse(dt)
-                except (ValueError, ParserError):
-                    if direction == 'backward':
-                        days = 45 if not days else days
-                        dt = datetime.today() - timedelta(days)
-                    else:
-                        days = 4 if not days else days
-                        dt = datetime.today() + timedelta(days)
-                except TypeError:
-                    pass
-
-            return dt
-
-        # Set min & max dates for plots
-        # If no min_date supplied we'll just leave it as None to show the whole plot
-        if min_date:
-            min_date = parse_date(min_date, 'backward')
-
-        # Default max_date to 4 days from today to give some padding to the right side of the plot
-        if max_date:
-            max_date = parse_date(max_date, 'forward', 0)
-        else:
-            max_date = parse_date(datetime.today(), 'forward')
-
-        # Set default date format parameters
-        rcParams["date.autoformatter.day"] = "%#m/%#d/%Y"
-        rcParams["date.autoformatter.hour"] = "%#m/%#d %H:%M"
-        rcParams['figure.titlesize'] = 'xx-large'
-        rcParams['figure.titleweight'] = 'bold'
-
-        plot_params = {'mth': mth,
-                       'min_date': min_date,
-                       'max_date': max_date,
-                       'poa_onboarding': poa_onboarding,
-                       'fullscreen': fullscreen}
-
-        # Display plots
-        if not plot_order:
-            plot_order = [
-                'xplot_pwr_poa',
-                'xplot_temp',
-                'temps',
-                'inv',
-                'pr',
-                '8760',
-                'weather',
-                'mtr_corrected',
-                'mtr_dif',
-                'poas',
-                'pwr_poa',
-                'ghi',
-                'irrad',
-                'tz',
-                'losses',
-                'poa_corr',
-            ]
-        
-            if plotter.project.Battery_AC_site:
-                plot_order.append('battery')
-            if plotter.project.Tracker_site:
-                plot_order.append('tracker')
-
-        if isinstance(plot_order, str):
-            plot_order = [plot_order]
-
-        for plot_name in plot_order:
-            plotter.plot_list[plot_name] = plotter._draw_plot(plot_name, plot_params, **kwargs)
-
-        if persist:
-            plt.show(block=True)
-        else:
-            plt.show()
-
-        if open_folder:
-            os.startfile(os.path.join(self.project.dashboard_dir,
-                                      self.project.project_directory,
-                                      self.project.project_name))
-
                 
     def __update_project_filepaths(self, project):
         """Sets filepaths for config file, Powertrack file, and Pickle Jar
 
         Args:
             project (Project): A `ccrenew.dashboard.project.Project`
 
@@ -1115,55 +1139,60 @@
         project.pickle_jar = project._find_pickle_jar() 
         
         return project
     
 
     def __prepare_source_data(self, project):
 
+        # Make sure filepath references are correct for config, bool, & Powertrack files + Pickle Jar
         self.__update_project_filepaths(project)
-        # Update config file
+
         # If the config file hasn't been updated it will use the data that's already been pulled
         # If the config file has been updated it will read the file & update the data
         self.__update_project_config(project)
 
-        # Load bool file
         # If the bool file hasn't been updated it will use the data that's already been pulled
         # If the bool file has been updated it will read the file & update the data
         project._load_bool_file()
 
-        # Load powertrack data
         # If the powertrack file hasn't been updated it will use the data that's already been pulled
         # If the powertrack file has been updated it will read the file & update the data
         project.load_production_data()
+
+        # fetch_solcast_data()
     
 
     def __update_project_config(self, project):
         
         # Store the list of sensors before pulling the config file
         sensors = project.Get_Sensor
         project._parse_config_file()
 
         # Check if new neighbor sensors have been added to the config & pull them if so
         if not sensors.equals(project.Get_Sensor):
             project._find_neighbor_sensors()
-            self.__get_neighbor_sensor_data(project)
+            self.__get_config_neighbor_sensor_data(project)
             
             
-    def __get_neighbor_sensor_data(self, project):
-        for neighbor_name in project.neighbor_sensors:
+    def __get_config_neighbor_sensor_data(self, project):
+        for neighbor_name in project.config_neighbor_sensors:
             # Update production data from neighbor
             try:
-                neighbor = self.get_project(neighbor_name, get_neighbors=False)
+                neighbor = self.get_project(neighbor_name, add_neighbors=False)
+                # Update session.plotters dictionary
             except KeyError:
                 print(f'Neighbor for {project.project_name} not found: {neighbor_name}. Sensor data for the neighbor will be blank. Check logs to determine why neighbor was not added to DashboardSession')
                 continue
             except Exception as e:
                 print(f'Neighbor for {project.project_name} errored: {neighbor_name}. Sensor data for the neighbor will be blank. Check logs to determine why neighbor was not added to DashboardSession.\nError details: {e}')
                 continue
             
+            if neighbor.errored:
+                continue
+
             # Reload neighbor's config or powertrack files if needed
             self.__prepare_source_data(neighbor)
 
             # Find the columns needed from the neighbor
             sensor_cols = project.Get_Sensor.loc[project.Get_Sensor['Source'] == neighbor_name, 'Value'].tolist()
 
             # Get the columns from the neighbor
@@ -1176,20 +1205,18 @@
             # If the neighbor errored out during initialization we'll just create a blank df for the neighbor
             except NameError:
                 neighbor_cols = [col + '_' + neighbor_name for col in sensor_cols]
                 project.df = project.df.reindex(columns = project.df.columns.tolist() + neighbor_cols)
                 project.df_sensor_ON = project.df_sensor_ON.reindex(columns = project.df_sensor_ON.columns.tolist() + neighbor_cols)
                 return
 
-            neighbor_df.rename(columns=lambda x: np.str(x) + '_' + neighbor_name, inplace=True)
+            neighbor_df.rename(columns=lambda x: str(x) + '_' + neighbor_name, inplace=True)
             neighbor_sensor_ON = neighbor.df_sensor_ON.reindex(index=project.df_sensor_ON.index, columns=sensor_cols)
             neighbor_sensor_ON.columns = neighbor_df.columns.tolist()
 
-            df_cols = project.df.columns.tolist()
+            # Add neighbor columns from config file
             project.df = df_update_join(project.df, neighbor_df)
-            # project.df = project.df[df_cols + neighbor_df.columns.tolist()]
+            project.df_sensor_ON = df_update_join(project.df_sensor_ON, neighbor_sensor_ON)
+            project.df_sensor_ON = project.df_sensor_ON.reindex(columns=project.df.columns.tolist())
 
             # Add the neighbor columns to the positional references
             project._locate_column_positions()
-
-            project.df_sensor_ON = df_update_join(project.df_sensor_ON, neighbor_sensor_ON)
-            project.df_sensor_ON = project.df_sensor_ON.reindex(columns=project.df.columns.tolist())
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/utils/df_tools.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/utils/df_tools.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/utils/logging_conf.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/utils/logging_conf.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.0rc0/src/ccrenew/dashboard/utils/project_neighbors.py` & `ccrenew-0.2.1/src/ccrenew/dashboard/utils/project_neighbors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Module to calculate distances between projects & acceptable neighbors to use
 for data substitution
 """
 
-
 import logging
-from numbers import Number
 import numpy as np
 from pandas import DataFrame, Series
 
-from ccrenew.dashboard import all_df_keys as df_keys
+from ccrenew import (
+    all_df_keys as df_keys,
+    Numeric,
+    SeriesLike)
 
-logger = logging.getLogger(__name__)
+# logger = logging.getLogger(__name__)
 
 
-def find_nearby_projects(project_name, dist=10, print_data=True, include_retired=False, df=None):
+def find_nearby_projects(project_name: str, dist:int = 10, print_data:bool = True,
+                         include_retired:bool = False, df:DataFrame = DataFrame()):
     """Creates a list of sites within a certain distance of the reference site.
 
     Args:
         project_name (str): Reference site.
         dist (int, optional): Number of miles to search around the reference site.
             Defaults to 10.
         include_retired (bool, optional): Whether to return sites that have been retired.
@@ -27,19 +29,19 @@
             Defaults to `df_keys` if no `df` supplied.
 
     Returns:
         nearby_sites (DataFrame): Contains information about all sites within the specified\
         distance from the reference site.
     """
     # Set `df` to `df_keys` if not supplied
-    if not isinstance(df, DataFrame):
+    if df.empty:
         df = df_keys
 
         # Exclude projects with ".1" in the CCR_ID
-        exclude_projects = df[['CCR_ID']].fillna('0').query("~CCR_ID.str.contains('\.1')")
+        exclude_projects = df[['CCR_ID']].fillna('0').query("~CCR_ID.str.contains('\\.1')")
         df = df.loc[exclude_projects.index]
 
         # Exclude retired projects if desired
         if not include_retired:
             df = df.query("Retired != True")
 
     # Rename 'Tilt/GCR' column to a valid python identifier
@@ -57,33 +59,33 @@
     if print_data:
         print('\n')
         print('Sites within {} miles of {}'.format(dist, project_name))
         print(nearby_sites)
         print('\n')
     return nearby_sites
 
-def find_similar_projects(project_name, include_retired=False, df=None):
+def find_similar_projects(project_name: str, include_retired:bool = False, df:DataFrame = DataFrame()):
     """Creates a list of sites that share similar racking properties to the reference project.
 
     Args:
         project_name (str): Reference project.
         include_retired (bool, optional): Whether to return sites that have been retired.
             Defaults to False, i.e. does not return retired sites.
         df (Dataframe, optional): Dataframe containing sitenames & lat/longs.
             Defaults to `df_keys` if no `df` supplied.
     Returns:
         DataFrame: Contains information about all sites with similar racking\
         properties to the reference site.
     """
     # Set `df` to `df_keys` if not supplied
-    if not isinstance(df, DataFrame):
+    if df.empty:
         df = df_keys
 
         # Exclude projects with ".1" in the CCR_ID
-        exclude_projects = df[['CCR_ID']].fillna('0').query("~CCR_ID.str.contains('\.1')")
+        exclude_projects = df[['CCR_ID']].fillna('0').query("~CCR_ID.str.contains('\\.1')")
         df = df.loc[exclude_projects.index]
 
         # Exclude retired projects if desired
         if not include_retired:
             df = df.query("Retired != True")
 
     # Rename 'Tilt/GCR' column to a valid python identifier
@@ -119,15 +121,15 @@
         query = "index == @project_name"
 
     # Get all sites that have matching info to the reference site
     similar_sites = df.query(query)
 
     return similar_sites
 
-def find_nearby_similar_projects(project_name, dist=10, print_data=True, include_retired=False, df=None):
+def find_nearby_similar_projects(project_name:str, dist:int = 10, print_data:bool = True, include_retired:bool = False, df:DataFrame = DataFrame()):
     """Creates a list of sites within a certain distance of the reference site
     that share similar racking properties. 
 
     Args:
         project_name (str): Reference site.
         dist (int, optional): Number of miles to search around the reference site.
             Defaults to 10.
@@ -145,15 +147,15 @@
     if print_data:
         print('\n')
         print('Similar sites within {} miles of {}'.format(dist, project_name))
         print(nearby_similar_sites)
         print('\n')
     return nearby_similar_sites
 
-def haversine(lon1, lat1, lon2, lat2):
+def haversine(lon1: Numeric|SeriesLike, lat1: Numeric|SeriesLike, lon2: Numeric|SeriesLike, lat2: Numeric|SeriesLike) -> Numeric|SeriesLike:
     """Calculate the great circle distance between two points
     on the earth (specified in decimal degrees).
 
     Args:
         lon1 (Number, np.ndarray, or Series): Longitude of point 1.
         lon1 (Number, np.ndarray, or Series): Latitude of point 1.
         lon1 (Number, np.ndarray, or Series): Longitude of point 2.
```

### Comparing `ccrenew-0.2.0rc0/src/ccrenew.egg-info/SOURCES.txt` & `ccrenew-0.2.1/src/ccrenew.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 LICENSE
 README.md
 setup.py
 src/ccrenew/__init__.py
+src/ccrenew/ccr.py
+src/ccrenew/cloud_data.py
+src/ccrenew/data_determination.py
 src/ccrenew.egg-info/PKG-INFO
 src/ccrenew.egg-info/SOURCES.txt
 src/ccrenew.egg-info/dependency_links.txt
 src/ccrenew.egg-info/top_level.txt
 src/ccrenew/dashboard/__init__.py
 src/ccrenew/dashboard/project.py
 src/ccrenew/dashboard/session.py
 src/ccrenew/dashboard/data_processing/BV_pp_deg.py
-src/ccrenew/dashboard/data_processing/Bluesky_weather_fucntions_v01.py
-src/ccrenew/dashboard/data_processing/CCR.py
 src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_IS6.py
 src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_smartercheck.py
 src/ccrenew/dashboard/data_processing/Correct_POI_data_v01.py
 src/ccrenew/dashboard/data_processing/Performance_Guarantees_v01.py
 src/ccrenew/dashboard/data_processing/Plant_Availability_v16_bbsc.py
 src/ccrenew/dashboard/data_processing/Rate_Structure_Python_with_DST_v07.py
 src/ccrenew/dashboard/data_processing/Table_by_Rate_Schedule_v01.py
 src/ccrenew/dashboard/data_processing/__init__.py
+src/ccrenew/dashboard/data_processing/_project_processing.py
 src/ccrenew/dashboard/data_processing/batch_process.py
 src/ccrenew/dashboard/data_processing/battery_deg.py
-src/ccrenew/dashboard/data_processing/data_determination.py
 src/ccrenew/dashboard/data_processing/snow_loss_functions_v3.py
 src/ccrenew/dashboard/data_processing/solcats_API.py
 src/ccrenew/dashboard/data_processing/weather_adjusted_functions_v03.py
 src/ccrenew/dashboard/plotting/__init__.py
 src/ccrenew/dashboard/plotting/plots.py
 src/ccrenew/dashboard/utils/__init__.py
 src/ccrenew/dashboard/utils/dashboard_utils.py
 src/ccrenew/dashboard/utils/df_tools.py
 src/ccrenew/dashboard/utils/logging_conf.py
-src/ccrenew/dashboard/utils/project_neighbors.py
+src/ccrenew/dashboard/utils/project_neighbors.py
+src/ccrenew/pvmodel/__init__.py
+src/ccrenew/pvmodel/project_model.py
```

