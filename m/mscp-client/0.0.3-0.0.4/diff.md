# Comparing `tmp/mscp_client-0.0.3.tar.gz` & `tmp/mscp_client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mscp_client-0.0.3.tar", last modified: Wed Apr  5 19:31:51 2023, max compression
+gzip compressed data, was "mscp_client-0.0.4.tar", last modified: Wed Apr 12 17:18:45 2023, max compression
```

## Comparing `mscp_client-0.0.3.tar` & `mscp_client-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 hbarrett  (1001) hbarrett  (1001)        0 2023-04-05 19:31:51.722541 mscp_client-0.0.3/
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)     1047 2023-03-22 20:21:54.000000 mscp_client-0.0.3/LICENSE
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)      327 2023-04-05 19:31:51.722541 mscp_client-0.0.3/PKG-INFO
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)       59 2023-03-22 20:20:59.000000 mscp_client-0.0.3/README.md
-drwxrwxr-x   0 hbarrett  (1001) hbarrett  (1001)        0 2023-04-05 19:31:51.718541 mscp_client-0.0.3/dist/
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)     3002 2023-03-22 20:26:53.000000 mscp_client-0.0.3/dist/mscp_client-0.0.1-py3-none-any.whl
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)     2783 2023-03-22 20:26:48.000000 mscp_client-0.0.3/dist/mscp_client-0.0.1.tar.gz
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)     6646 2023-04-05 15:39:39.000000 mscp_client-0.0.3/dist/mscp_client-0.0.2-py3-none-any.whl
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)    11963 2023-04-05 15:39:35.000000 mscp_client-0.0.3/dist/mscp_client-0.0.2.tar.gz
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)      442 2023-04-05 19:27:01.000000 mscp_client-0.0.3/pyproject.toml
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)       38 2023-04-05 19:31:51.722541 mscp_client-0.0.3/setup.cfg
-drwxrwxr-x   0 hbarrett  (1001) hbarrett  (1001)        0 2023-04-05 19:31:51.706541 mscp_client-0.0.3/src/
-drwxrwxr-x   0 hbarrett  (1001) hbarrett  (1001)        0 2023-04-05 19:31:51.718541 mscp_client-0.0.3/src/mscp_client/
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)     6891 2023-04-05 18:55:01.000000 mscp_client-0.0.3/src/mscp_client/__init__.py
-drwxrwxr-x   0 hbarrett  (1001) hbarrett  (1001)        0 2023-04-05 19:31:51.718541 mscp_client-0.0.3/src/mscp_client.egg-info/
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)      327 2023-04-05 19:31:51.000000 mscp_client-0.0.3/src/mscp_client.egg-info/PKG-INFO
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)      394 2023-04-05 19:31:51.000000 mscp_client-0.0.3/src/mscp_client.egg-info/SOURCES.txt
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)        1 2023-04-05 19:31:51.000000 mscp_client-0.0.3/src/mscp_client.egg-info/dependency_links.txt
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)       24 2023-04-05 19:31:51.000000 mscp_client-0.0.3/src/mscp_client.egg-info/requires.txt
--rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)       12 2023-04-05 19:31:51.000000 mscp_client-0.0.3/src/mscp_client.egg-info/top_level.txt
+drwxrwxr-x   0 hbarrett  (1001) hbarrett  (1001)        0 2023-04-12 17:18:45.109048 mscp_client-0.0.4/
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)     1047 2023-03-22 20:21:54.000000 mscp_client-0.0.4/LICENSE
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)      327 2023-04-12 17:18:45.109048 mscp_client-0.0.4/PKG-INFO
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)       59 2023-03-22 20:20:59.000000 mscp_client-0.0.4/README.md
+drwxrwxr-x   0 hbarrett  (1001) hbarrett  (1001)        0 2023-04-12 17:18:45.101048 mscp_client-0.0.4/dist/
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)     3002 2023-03-22 20:26:53.000000 mscp_client-0.0.4/dist/mscp_client-0.0.1-py3-none-any.whl
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)     2783 2023-03-22 20:26:48.000000 mscp_client-0.0.4/dist/mscp_client-0.0.1.tar.gz
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)     6646 2023-04-05 15:39:39.000000 mscp_client-0.0.4/dist/mscp_client-0.0.2-py3-none-any.whl
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)    11963 2023-04-05 15:39:35.000000 mscp_client-0.0.4/dist/mscp_client-0.0.2.tar.gz
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)      442 2023-04-12 17:18:35.000000 mscp_client-0.0.4/pyproject.toml
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)       38 2023-04-12 17:18:45.109048 mscp_client-0.0.4/setup.cfg
+drwxrwxr-x   0 hbarrett  (1001) hbarrett  (1001)        0 2023-04-12 17:18:45.097048 mscp_client-0.0.4/src/
+drwxrwxr-x   0 hbarrett  (1001) hbarrett  (1001)        0 2023-04-12 17:18:45.105048 mscp_client-0.0.4/src/mscp_client/
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)    10063 2023-04-12 14:25:52.000000 mscp_client-0.0.4/src/mscp_client/__init__.py
+drwxrwxr-x   0 hbarrett  (1001) hbarrett  (1001)        0 2023-04-12 17:18:45.109048 mscp_client-0.0.4/src/mscp_client/__pycache__/
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)     5778 2023-04-12 15:16:43.000000 mscp_client-0.0.4/src/mscp_client/__pycache__/__init__.cpython-310.pyc
+drwxrwxr-x   0 hbarrett  (1001) hbarrett  (1001)        0 2023-04-12 17:18:45.109048 mscp_client-0.0.4/src/mscp_client.egg-info/
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)      327 2023-04-12 17:18:45.000000 mscp_client-0.0.4/src/mscp_client.egg-info/PKG-INFO
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)      447 2023-04-12 17:18:45.000000 mscp_client-0.0.4/src/mscp_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)        1 2023-04-12 17:18:45.000000 mscp_client-0.0.4/src/mscp_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)       24 2023-04-12 17:18:45.000000 mscp_client-0.0.4/src/mscp_client.egg-info/requires.txt
+-rw-rw-r--   0 hbarrett  (1001) hbarrett  (1001)       12 2023-04-12 17:18:45.000000 mscp_client-0.0.4/src/mscp_client.egg-info/top_level.txt
```

### Comparing `mscp_client-0.0.3/LICENSE` & `mscp_client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mscp_client-0.0.3/dist/mscp_client-0.0.1-py3-none-any.whl` & `mscp_client-0.0.4/dist/mscp_client-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `mscp_client-0.0.3/dist/mscp_client-0.0.1.tar.gz` & `mscp_client-0.0.4/dist/mscp_client-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `mscp_client-0.0.3/dist/mscp_client-0.0.2-py3-none-any.whl` & `mscp_client-0.0.4/dist/mscp_client-0.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `mscp_client-0.0.3/dist/mscp_client-0.0.2.tar.gz` & `mscp_client-0.0.4/dist/mscp_client-0.0.2.tar.gz`

 * *Files identical despite different names*

### Comparing `mscp_client-0.0.3/src/mscp_client/__init__.py` & `mscp_client-0.0.4/src/mscp_client/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -51,57 +51,76 @@
                     result[entity_type] = {type: id_ for type, id_ in data} if 'type' in entity_type else {name: id_ for name, id_ in data}
                 else:
                     # If the entity_type contains 'type', use 'id' and 'type' as key-value pairs
                     # Otherwise, use 'id' and 'name' as key-value pairs
                     result[entity_type] = {id_: type for type, id_ in data} if 'type' in entity_type else {id_: name for name, id_ in data}
             # Return the result dictionary containing the mapping of ids to names/types (or reverse)
             return result
-
+        
+    # This function takes in an optional argument entity_types that defaults to None.
+    # It returns the result of get_name_ids() method invoked on self, with arguments entity_types and False.
     def get_id_names(self, entity_types=None):
         return self.get_name_ids(entity_types, False)
 
     def render_legacy_gws(self, df):
         """
         Transforms a data frame containing new data into a legacy frame format.
         Returns a new data frame with the transformed data.
         """
         #First we fetch the lelel calcs from the db and put them in a dataframe
         q = "SELECT * FROM gws_level_calc"
         calcs_df = pd.read_sql_query(sql=text(q), con=self.engine.connect())
 
-        #then we get a dict of ids to names and names to ids:
+        #We get a dict of ids to names and names to ids. These are used later on.
         id_to_names=self.get_id_names()
         names_to_ids=self.get_name_ids()
 
         # merge by station_id. This is nessicary to merge the start and end dates so we can compare dates later on.
         merged_data = pd.merge(df, calcs_df, on=['station_id'])
 
         # This is where we do date comparison to get the correct formula inputs.
         merged_data = merged_data[(merged_data['timestamp'] >= merged_data['start_date']) & (
             merged_data['timestamp'] <= merged_data['end_date'])]
         
+        #####Calculate the depth to water in feet#####
         # Divide the monument_height_in by 12 to convert the height from inches to feet.
         # Divide the value by 25.4 to convert it from millimeters to inches, and then divide the result by 12 to convert it to feet.
         # Subtract the values obtained in steps 1 and 2 from the hang_length_ft values.
         merged_data['port1_dtw_ft'] = merged_data['hang_length_ft'] - \
             (merged_data['monument_height_in']/12) - \
             ((merged_data['value']/25.4)/12)
-
+        
         # get the measurement_id for the 'Depth To Water In Feet' measurement
         dtw_id = names_to_ids["measurements"]['Depth To Water In Feet']
+
         water_level_id = names_to_ids["measurements"]['Water Level']
-        # create a new DataFrame for the rows with measurement_id == 1.
-        subset_df = merged_data[merged_data['measurement_id'] == water_level_id].copy()
+        
+        # create a new DataFrame for the rows with measurement_id equal to the water level id.
+        dtw_subset_df = merged_data[merged_data['measurement_id'] == water_level_id].copy()
 
         # set the measurement_id and value columns for the new rows
-        subset_df.loc[:, 'measurement_id'] = dtw_id
-        subset_df.loc[:, 'value'] = subset_df['port1_dtw_ft']
+        dtw_subset_df.loc[:, 'measurement_id'] = dtw_id
+        dtw_subset_df.loc[:, 'value'] = dtw_subset_df['port1_dtw_ft']
+
+        ##########Calculate Ground Water Elevation in Feet##########
+
+        # Subtract the port1_dtw_ft values from the surface_elevation_ft values to get ground water elevation in feet.
+        merged_data['port1_gwelev_ft'] = merged_data['surface_elevation_ft']-merged_data['port1_dtw_ft']
+        
+        # get the measurement_id for the 'Ground Water Elevation In Feet' measurement
+        gwelev_id = names_to_ids["measurements"]['Water Elevation In Feet']
+        
+        gwelev_subset_df = merged_data[merged_data['measurement_id'] == water_level_id].copy()
+        
+        # set the measurement_id and value columns for the new rows
+        gwelev_subset_df.loc[:, 'measurement_id'] = gwelev_id
+        gwelev_subset_df.loc[:, 'value'] = gwelev_subset_df['port1_gwelev_ft']
 
         # add the new rows back to the merged dataframe
-        merged_df = pd.concat([merged_data, subset_df], ignore_index=True)
+        merged_df = pd.concat([merged_data, dtw_subset_df,gwelev_subset_df], ignore_index=True)
 
         # Map the ids to the names.
         merged_df["logger_id"] = merged_df["logger_id"].map(
             id_to_names["loggers"])
         merged_df["station_id"] = merged_df["station_id"].map(
             id_to_names["stations"])
         merged_df["measurement_id"] = merged_df["measurement_id"].map(
@@ -123,13 +142,56 @@
                             columns='measurement_port',
                             values='qa_codes_id',
                             aggfunc=lambda x: ' '.join(str(v) for v in x if v != -1))
 
         # Replace the placeholder values with null values after the pivot table is created
         qa_pivot = qa_pivot.replace(-1, np.nan)
 
-        #Rename the columns so we know wich cols are values and wich are QAQC codes.
+        #Rename the columns so we know which cols are values and which are QAQC codes.
         qa_pivot.columns = ['QAQC ' + col for col in qa_pivot.columns]
         #Concat the two dataframes together and reset the index.
         result = pd.concat([pivot, qa_pivot], axis=1).reset_index()
         #Return the result
         return result
+    
+    def render_legacy_sms(self, df):
+        """
+        Transforms a data frame containing new data into a legacy frame format.
+        Returns a new data frame with the transformed data.
+        """
+        #We get a dict of ids to names and names to ids. These are used later on.
+        id_to_names=self.get_id_names()
+        names_to_ids=self.get_name_ids()
+                # Map the ids to the names.
+        df["logger_id"] = df["logger_id"].map(
+            id_to_names["loggers"])
+        df["station_id"] = df["station_id"].map(
+            id_to_names["stations"])
+        df["measurement_id"] = df["measurement_id"].map(
+            id_to_names["measurements"])
+
+        # Create a new column that combines measurement_id and port_number
+        df['measurement_port'] = df['measurement_id'] + \
+            ' port ' + df['port_number'].astype(str)
+        
+        pivot = df.pivot_table(index=['logger_id', 'station_id', 'timestamp'],
+                                columns='measurement_port',
+                                values='value')
+        
+
+        # Fill null values in 'qa_codes_id' column with a placeholder value, e.g., -1
+        df['qa_codes_id'] = df['qa_codes_id'].fillna(-1)
+        #Pivot the data frame for QAQC codes so it is more like legacy data
+        qa_pivot = df.pivot_table(index=['logger_id', 'station_id', 'timestamp'],
+                            columns='measurement_port',
+                            values='qa_codes_id',
+                            aggfunc=lambda x: ' '.join(str(v) for v in x if v != -1))
+
+        # Replace the placeholder values with null values after the pivot table is created
+        qa_pivot = qa_pivot.replace(-1, np.nan)
+
+        #Rename the columns so we know wich cols are values and wich are QAQC codes.
+        qa_pivot.columns = ['QAQC ' + col for col in qa_pivot.columns]
+        #Concat the two dataframes together and reset the index.
+        result = pd.concat([pivot, qa_pivot], axis=1).reset_index()
+        
+        return result
```

