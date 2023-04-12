# Comparing `tmp/pavimentados-0.29.0.tar.gz` & `tmp/pavimentados-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pavimentados-0.29.0.tar", last modified: Wed Apr 12 21:31:00 2023, max compression
+gzip compressed data, was "dist\pavimentados-0.9.0.tar", last modified: Thu Feb  3 16:35:21 2022, max compression
```

## Comparing `pavimentados-0.29.0.tar` & `pavimentados-0.9.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-04-12 21:31:00.891499 pavimentados-0.29.0/
--rw-r--r--   0 vdurand  (644026607) 1010544492    11839 2023-03-28 19:27:29.000000 pavimentados-0.29.0/LICENSE.md
--rw-r--r--   0 vdurand  (644026607) 1010544492      292 2023-03-28 19:27:29.000000 pavimentados-0.29.0/MANIFEST.in
--rw-r--r--   0 vdurand  (644026607) 1010544492     6842 2023-04-12 21:31:00.891219 pavimentados-0.29.0/PKG-INFO
--rw-r--r--   0 vdurand  (644026607) 1010544492     6161 2023-03-28 19:27:29.000000 pavimentados-0.29.0/README.md
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-04-12 21:31:00.881348 pavimentados-0.29.0/pavimentados/
--rw-r--r--   0 vdurand  (644026607) 1010544492      243 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/__init__.py
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-04-12 21:31:00.884945 pavimentados-0.29.0/pavimentados/analyzers/
--rw-r--r--   0 vdurand  (644026607) 1010544492        0 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/analyzers/__init__.py
--rw-r--r--   0 vdurand  (644026607) 1010544492     8078 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/analyzers/calculators.py
--rw-r--r--   0 vdurand  (644026607) 1010544492     6792 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/analyzers/gps_sources.py
--rw-r--r--   0 vdurand  (644026607) 1010544492     2904 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/analyzers/utils.py
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-04-12 21:31:00.887925 pavimentados-0.29.0/pavimentados/configs/
--rw-r--r--   0 vdurand  (644026607) 1010544492        0 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/configs/__init__.py
--rw-r--r--   0 vdurand  (644026607) 1010544492       43 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/configs/images_processor.json
--rw-r--r--   0 vdurand  (644026607) 1010544492       38 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/configs/models_general.json
--rw-r--r--   0 vdurand  (644026607) 1010544492      406 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/configs/processor.json
--rw-r--r--   0 vdurand  (644026607) 1010544492      429 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/configs/siamese_config.json
--rw-r--r--   0 vdurand  (644026607) 1010544492       53 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/configs/state_signal_config.json
--rw-r--r--   0 vdurand  (644026607) 1010544492      176 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/configs/utils.py
--rw-r--r--   0 vdurand  (644026607) 1010544492      424 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/configs/yolo_config.json
--rw-r--r--   0 vdurand  (644026607) 1010544492     3259 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/downloader.py
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-04-12 21:31:00.888507 pavimentados-0.29.0/pavimentados/image/
--rw-r--r--   0 vdurand  (644026607) 1010544492        0 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/image/__init__.py
--rw-r--r--   0 vdurand  (644026607) 1010544492      236 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/image/utils.py
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-04-12 21:31:00.889367 pavimentados-0.29.0/pavimentados/models/
--rw-r--r--   0 vdurand  (644026607) 1010544492        0 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/models/__init__.py
--rw-r--r--   0 vdurand  (644026607) 1010544492    10758 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/models/structures.py
--rw-r--r--   0 vdurand  (644026607) 1010544492    16632 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/models/yolo.py
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-04-12 21:31:00.890822 pavimentados-0.29.0/pavimentados/processing/
--rw-r--r--   0 vdurand  (644026607) 1010544492        0 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/processing/__init__.py
--rw-r--r--   0 vdurand  (644026607) 1010544492     8706 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/processing/processors.py
--rw-r--r--   0 vdurand  (644026607) 1010544492     3448 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/processing/sources.py
--rw-r--r--   0 vdurand  (644026607) 1010544492     3106 2023-03-28 19:27:29.000000 pavimentados-0.29.0/pavimentados/processing/workflows.py
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-04-12 21:31:00.883441 pavimentados-0.29.0/pavimentados.egg-info/
--rw-r--r--   0 vdurand  (644026607) 1010544492     6842 2023-04-12 21:31:00.000000 pavimentados-0.29.0/pavimentados.egg-info/PKG-INFO
--rw-r--r--   0 vdurand  (644026607) 1010544492     1022 2023-04-12 21:31:00.000000 pavimentados-0.29.0/pavimentados.egg-info/SOURCES.txt
--rw-r--r--   0 vdurand  (644026607) 1010544492        1 2023-04-12 21:31:00.000000 pavimentados-0.29.0/pavimentados.egg-info/dependency_links.txt
--rw-r--r--   0 vdurand  (644026607) 1010544492      151 2023-04-12 21:31:00.000000 pavimentados-0.29.0/pavimentados.egg-info/requires.txt
--rw-r--r--   0 vdurand  (644026607) 1010544492       13 2023-04-12 21:31:00.000000 pavimentados-0.29.0/pavimentados.egg-info/top_level.txt
--rw-r--r--   0 vdurand  (644026607) 1010544492       38 2023-04-12 21:31:00.891565 pavimentados-0.29.0/setup.cfg
--rw-r--r--   0 vdurand  (644026607) 1010544492     1429 2023-04-12 21:29:39.000000 pavimentados-0.29.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/
+-rw-rw-rw-   0        0        0     1928 2022-01-12 04:50:35.000000 pavimentados-0.9.0/.gitignore
+-rw-rw-rw-   0        0        0     7169 2022-01-12 04:50:35.000000 pavimentados-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      297 2022-01-12 05:36:36.000000 pavimentados-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2264 2022-02-03 16:35:21.000000 pavimentados-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2022-02-03 15:40:33.000000 pavimentados-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados/
+-rw-rw-rw-   0        0        0      250 2022-01-12 06:27:39.000000 pavimentados-0.9.0/pavimentados/__init__.py
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados/analyzers/
+-rw-rw-rw-   0        0        0        0 2022-01-12 04:54:02.000000 pavimentados-0.9.0/pavimentados/analyzers/__init__.py
+-rw-rw-rw-   0        0        0     8242 2022-01-12 05:31:21.000000 pavimentados-0.9.0/pavimentados/analyzers/calculators.py
+-rw-rw-rw-   0        0        0     6785 2022-01-12 05:31:21.000000 pavimentados-0.9.0/pavimentados/analyzers/gps_sources.py
+-rw-rw-rw-   0        0        0     3011 2022-01-12 01:57:29.000000 pavimentados-0.9.0/pavimentados/analyzers/utils.py
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados/configs/
+-rw-rw-rw-   0        0        0        0 2022-01-12 04:53:49.000000 pavimentados-0.9.0/pavimentados/configs/__init__.py
+-rw-rw-rw-   0        0        0       45 2022-01-10 07:47:23.000000 pavimentados-0.9.0/pavimentados/configs/images_processor.json
+-rw-rw-rw-   0        0        0       40 2022-01-10 04:01:55.000000 pavimentados-0.9.0/pavimentados/configs/models_general.json
+-rw-rw-rw-   0        0        0      440 2022-01-10 04:58:59.000000 pavimentados-0.9.0/pavimentados/configs/processor.json
+-rw-rw-rw-   0        0        0      442 2022-01-10 03:40:03.000000 pavimentados-0.9.0/pavimentados/configs/siamese_config.json
+-rw-rw-rw-   0        0        0       56 2022-01-10 03:19:31.000000 pavimentados-0.9.0/pavimentados/configs/state_signal_config.json
+-rw-rw-rw-   0        0        0      186 2022-01-10 16:07:40.000000 pavimentados-0.9.0/pavimentados/configs/utils.py
+-rw-rw-rw-   0        0        0      439 2022-01-10 05:31:47.000000 pavimentados-0.9.0/pavimentados/configs/yolo_config.json
+-rw-rw-rw-   0        0        0     3358 2022-01-12 06:46:32.000000 pavimentados-0.9.0/pavimentados/downloader.py
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados/image/
+-rw-rw-rw-   0        0        0        0 2022-01-12 04:53:38.000000 pavimentados-0.9.0/pavimentados/image/__init__.py
+-rw-rw-rw-   0        0        0      245 2022-01-10 07:53:24.000000 pavimentados-0.9.0/pavimentados/image/utils.py
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados/models/
+-rw-rw-rw-   0        0        0        0 2022-01-12 04:53:27.000000 pavimentados-0.9.0/pavimentados/models/__init__.py
+-rw-rw-rw-   0        0        0    10292 2022-01-12 05:34:06.000000 pavimentados-0.9.0/pavimentados/models/structures.py
+-rw-rw-rw-   0        0        0    16632 2022-01-12 06:12:03.000000 pavimentados-0.9.0/pavimentados/models/yolo.py
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados/processing/
+-rw-rw-rw-   0        0        0        0 2022-01-12 04:53:16.000000 pavimentados-0.9.0/pavimentados/processing/__init__.py
+-rw-rw-rw-   0        0        0     7287 2022-01-12 05:31:22.000000 pavimentados-0.9.0/pavimentados/processing/processors.py
+-rw-rw-rw-   0        0        0     2714 2022-01-12 05:34:06.000000 pavimentados-0.9.0/pavimentados/processing/sources.py
+-rw-rw-rw-   0        0        0     2893 2022-01-12 05:31:22.000000 pavimentados-0.9.0/pavimentados/processing/workflows.py
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados.egg-info/
+-rw-rw-rw-   0        0        0     2264 2022-02-03 16:35:18.000000 pavimentados-0.9.0/pavimentados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1047 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-02-03 16:35:18.000000 pavimentados-0.9.0/pavimentados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2022-02-03 16:35:18.000000 pavimentados-0.9.0/pavimentados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2022-02-03 16:35:20.000000 pavimentados-0.9.0/pavimentados.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      182 2022-01-12 06:22:23.000000 pavimentados-0.9.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-02-03 16:35:21.000000 pavimentados-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1463 2022-01-12 06:46:36.000000 pavimentados-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pavimentados-0.29.0/pavimentados/analyzers/calculators.py` & `pavimentados-0.9.0/pavimentados/analyzers/calculators.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-from pavimentados.analyzers.utils import total_distance, area_calc, box_center, box_height, box_width, fail_id_generator, stack_columns_dataset, assign_group_calculations
-import numpy as np
-import pandas as pd
-
-first_aggregation_dict = {
-	'ind':'count',
-	'perc_area':'sum'
-}
-
-second_aggregation_dict = {
-	'distances':'sum',
-	'start_coordinate': 'first',
-	'start_latitude':'first',
-	'start_longitude':'first',
-	'end_coordenate': 'last',
-	'end_latitude':'last',
-	'end_longitude':'last',
-	'width':'mean',
-	'area':'sum',
-	'boxes':'sum'
-}
-
-third_aggregation_dict = {
-	'width':'sum',
-	'distances':np.mean,
-	'boxes':'count'
-}
-
-class Results_Calculator:
-
-	@staticmethod
-	def generate_paviment_results(results_obj, img_obj, gps_obj, min_fotogram_distance = 5, columns_to_have = ['Grieta Lineal Longitudinal','Intervalo Lineal Longitudinal','Grieta Lineal Transversal','Intervalo Lineal Transversal','Piel de Cocodrilo','Protuberancia, Bache','Otras fallas']):
-		"""
-		Genera la table final de resultados de pavimentos.
-		"""
-		# Genero el dataset.
-		data = gps_obj.gps_df.copy()
-		data['scores'] = results_obj['scores_pav']
-		data['boxes'] = results_obj['boxes_pav']
-		data['classes'] = results_obj['final_pav_clases']		
-		data['fotograma'] = data.index
-		altura, base = img_obj.get_altura_base()
-
-		# Calculamos la cantidad de detecciones por fotograma.
-		data['len'] = list(map(lambda x: len(x), data.scores.values))
-		data = data.loc[data.len>0].reset_index(drop=True)
-
-		# Como el dataframe tiene listas de detecciones por fotograma
-		# transformamos esas listas es varias lineas.
-		data_resulting = stack_columns_dataset(data, ['classes','scores','boxes'], [ 'latitude', 'longitude','distances','ind','fotograma','section'])
-		# Agregamos nuevas variables.
-		data_resulting['class_id'] = data_resulting.classes.values
-		data_resulting['area'] = list(map(lambda x: area_calc(x,altura, base), data_resulting.boxes.values))
-		data_resulting['center'] = list(map(lambda x: box_center(x, altura, base), data_resulting.boxes.values))
-		data_resulting['height'] = list(map(lambda x: box_height(x,altura), data_resulting.boxes.values))
-		data_resulting['width'] = list(map(lambda x: box_width(x,base), data_resulting.boxes.values))
-		data_resulting['total_area'] = base*altura
-		data_resulting['perc_area'] = data_resulting.area.values/data_resulting.total_area.values
-		
-		# Agrupamos data.
-		data_resulting_g = data_resulting.groupby(['latitude','longitude','fotograma','distances','classes','section']).aggregate(first_aggregation_dict).reset_index().rename({'ind':'cantidad'},axis=1).sort_values(['fotograma']).reset_index(drop=True)
-		data_resulting_g_total = data_resulting.groupby(['classes']).aggregate(first_aggregation_dict).reset_index().rename({'ind':'quantity'},axis=1).reset_index(drop=True)
-
-		# Generamos la ID de fail.
-		variables = list(data_resulting.classes.unique())
-		data_resulting = fail_id_generator(data_resulting, min_fotogram_distance)
-
-		# Agrupamos data por sections.
-		data_resulting_g_sections = data_resulting.groupby(['class_id','classes','fotograma','latitude','longitude','fail_id_section']).aggregate(third_aggregation_dict).reset_index().sort_values(['fotograma'])
-		data_resulting_g_sections2 = data_resulting.groupby(['class_id','classes','fotograma','latitude','longitude','section']).aggregate(third_aggregation_dict).reset_index().sort_values(['fotograma'])
-
-		# Agregamos nuevas variables.
-		data_resulting_g_sections = assign_group_calculations(data_resulting_g_sections)
-		data_resulting_g_sections2 = assign_group_calculations(data_resulting_g_sections2)
-		
-		# Generamos los datasets resulting.
-		data_resulting_fails = data_resulting_g_sections.groupby(['class_id','classes','fail_id_section']).aggregate(second_aggregation_dict).reset_index()
-		data_resulting_sections = data_resulting_g_sections2.groupby(['class_id','classes','section']).aggregate(second_aggregation_dict).reset_index()
-
-		table_summary_sections = data_resulting_sections.pivot_table(index=['section'], columns=['classes'], values=['distances']).fillna(0).astype('int')
-		table_summary_sections.columns = table_summary_sections.columns.droplevel(0)
-		index_sections_location = list(table_summary_sections.reset_index().section.values )
-		index_sections_location_end = list(np.array(index_sections_location)+1)
-		table_summary_sections['latitude'] = np.array(gps_obj.section_latitude)[index_sections_location]
-		table_summary_sections['longitude'] = np.array(gps_obj.section_longitude)[index_sections_location]
-		table_summary_sections['end_latitude'] = np.array(gps_obj.section_latitude)[index_sections_location_end]
-		table_summary_sections['end_longitude'] = np.array(gps_obj.section_longitude)[index_sections_location_end]
-		table_summary_sections['section_distance'] = np.array(gps_obj.section_distances)[index_sections_location]
-		for col in columns_to_have:
-			if col not in table_summary_sections.columns:
-				table_summary_sections[col]=0
-		table_summary_sections = table_summary_sections.reset_index()
-		table_summary_sections = pd.DataFrame(table_summary_sections.values, columns=list(table_summary_sections.columns))
-		table_summary_sections = table_summary_sections[['section',*columns_to_have, 'latitude','longitude','end_longitude',
-														 'end_latitude','section_distance']]
-		return table_summary_sections, data_resulting, data_resulting_fails
-
-	@staticmethod
-	def generate_final_results_signal(results_obj, gps_obj, classes_names_yolo_signal = ['ADTCIA','CIRCROJO','CRUZAMLLA','CUADBCO','CUADCAFE','CUADVERDE',
-																						 'CUADZUL','CUAMLLO','CURVA','INDAZUL','OBRA','OTRO','PROBROJO',
-																						 'ROMAMLLO','RUTA','SEMAFORO','STOP','TRIROJO']):
-		BOXES_SIGNAL = results_obj['boxes_signal']
-		CLASSES_SIGNAL = results_obj['classes_signal']
-		SIGNAL_CLASSES_siames = results_obj['final_signal_classes']
-		SIGNAL_CLASSES_BASE = results_obj['signal_base_predictions']
-		SIGNAL_STATE = results_obj['state_predictions']
-		SCORES_SIGNAL = results_obj['scores_signal']
-		final_latitude = gps_obj.gps_df.latitude.values
-		final_longitude = gps_obj.gps_df.longitude.values
-		fotograma = list(range(len(BOXES_SIGNAL)))
-
-		# Nos dice el cuadrante.
-		def position(center):
-			if center<0.33:
-				return 0
-			elif center<0.66:
-				return 1
-			else:
-				return 2
-
-		position_boxes = [[position((box[1]+box[3])/2) for box in BOXES_SIGNAL[f]] for f in range(len(BOXES_SIGNAL))]
-
-		rows = []
-		for f in fotograma:
-			for i in range(len(CLASSES_SIGNAL[f])):
-				r = [f, position_boxes[f][i], SCORES_SIGNAL[f][i], SIGNAL_STATE[f][i], SIGNAL_CLASSES_siames[f][i], SIGNAL_CLASSES_BASE[f][i], 
-				int(CLASSES_SIGNAL[f][i]), final_latitude[f], final_longitude[f]]
-				rows.append(r)
-
-
-		df = pd.DataFrame(rows, columns = ['fotogram', 'position_boxes', 'score', 'signal_state', 'signal_class_siames', 'signal_class_base', 
-			'signal_class', 'latitude', 'longitude'])
-
-		df['signal_class_siames_names'] = df['signal_class_siames'].values
-		df['signal_class_names'] = df['signal_class'].apply(lambda x: classes_names_yolo_signal[x])
-
-		yolo_classes_to_keep = []
-
-		x = tuple(zip(df['signal_class_siames_names'].values, df['signal_class_names'].values))
-
-		final_classes = []
-		for i in range(len(x)):
-			if x[i][1] in yolo_classes_to_keep:
-				final_classes.append(x[i][1])
-			else:
-				final_classes.append(x[i][0])
-
-		df['final_classes'] = final_classes
-		df['ID'] = range(len(df))
-
-		df = df.sort_values(['final_classes','position_boxes','fotogram']).reset_index(drop=True)
-
-		# cantidad de fotogramas a sacar repetidas.
-		N_fotogram = 5
-
-		for i in range(len(df)-1,0,-1):
-			if (df.loc[i-1, 'final_classes'] == df.loc[i, 'final_classes']) & \
-			(df.loc[i-1, 'position_boxes'] == df.loc[i, 'position_boxes']) & \
-			(np.abs(df.loc[i-1, 'fotogram']-df.loc[i, 'fotogram'])<=N_fotogram) & \
-			(df.loc[i, 'final_classes'] != 'OTRO'):
-				df.loc[i-1, 'ID'] = df.loc[i,'ID']
-
-		df = df.sort_values('fotogram', ascending=False).reset_index(drop=True).drop_duplicates(subset='ID')
-		df = df.sort_values('fotogram').reset_index(drop=True)
+from pavimentados.analyzers.utils import total_distance, area_calc, box_center, box_height, box_width, fail_id_generator, stack_columns_dataset, assign_group_calculations
+import numpy as np
+import pandas as pd
+
+first_aggregation_dict = {
+	'ind':'count',
+	'perc_area':'sum'
+}
+
+second_aggregation_dict = {
+	'distances':'sum',
+	'start_coordinate': 'first',
+	'start_latitude':'first',
+	'start_longitude':'first',
+	'end_coordenate': 'last',
+	'end_latitude':'last',
+	'end_longitude':'last',
+	'width':'mean',
+	'area':'sum',
+	'boxes':'sum'
+}
+
+third_aggregation_dict = {
+	'width':'sum',
+	'distances':np.mean,
+	'boxes':'count'
+}
+
+class Results_Calculator:
+
+	@staticmethod
+	def generate_paviment_results(results_obj, img_obj, gps_obj, min_fotogram_distance = 5, columns_to_have = ['Grieta Lineal Longitudinal','Intervalo Lineal Longitudinal','Grieta Lineal Transversal','Intervalo Lineal Transversal','Piel de Cocodrilo','Protuberancia, Bache','Otras fallas']):
+		"""
+		Genera la table final de resultados de pavimentos.
+		"""
+		# Genero el dataset.
+		data = gps_obj.gps_df.copy()
+		data['scores'] = results_obj['scores_pav']
+		data['boxes'] = results_obj['boxes_pav']
+		data['classes'] = results_obj['final_pav_clases']		
+		data['fotograma'] = data.index
+		altura, base = img_obj.get_altura_base()
+
+		# Calculamos la cantidad de detecciones por fotograma.
+		data['len'] = list(map(lambda x: len(x), data.scores.values))
+		data = data.loc[data.len>0].reset_index(drop=True)
+
+		# Como el dataframe tiene listas de detecciones por fotograma
+		# transformamos esas listas es varias lineas.
+		data_resulting = stack_columns_dataset(data, ['classes','scores','boxes'], [ 'latitude', 'longitude','distances','ind','fotograma','section'])
+		# Agregamos nuevas variables.
+		data_resulting['class_id'] = data_resulting.classes.values
+		data_resulting['area'] = list(map(lambda x: area_calc(x,altura, base), data_resulting.boxes.values))
+		data_resulting['center'] = list(map(lambda x: box_center(x, altura, base), data_resulting.boxes.values))
+		data_resulting['height'] = list(map(lambda x: box_height(x,altura), data_resulting.boxes.values))
+		data_resulting['width'] = list(map(lambda x: box_width(x,base), data_resulting.boxes.values))
+		data_resulting['total_area'] = base*altura
+		data_resulting['perc_area'] = data_resulting.area.values/data_resulting.total_area.values
+		
+		# Agrupamos data.
+		data_resulting_g = data_resulting.groupby(['latitude','longitude','fotograma','distances','classes','section']).aggregate(first_aggregation_dict).reset_index().rename({'ind':'cantidad'},axis=1).sort_values(['fotograma']).reset_index(drop=True)
+		data_resulting_g_total = data_resulting.groupby(['classes']).aggregate(first_aggregation_dict).reset_index().rename({'ind':'quantity'},axis=1).reset_index(drop=True)
+
+		# Generamos la ID de fail.
+		variables = list(data_resulting.classes.unique())
+		data_resulting = fail_id_generator(data_resulting, min_fotogram_distance)
+
+		# Agrupamos data por sections.
+		data_resulting_g_sections = data_resulting.groupby(['class_id','classes','fotograma','latitude','longitude','fail_id_section']).aggregate(third_aggregation_dict).reset_index().sort_values(['fotograma'])
+		data_resulting_g_sections2 = data_resulting.groupby(['class_id','classes','fotograma','latitude','longitude','section']).aggregate(third_aggregation_dict).reset_index().sort_values(['fotograma'])
+
+		# Agregamos nuevas variables.
+		data_resulting_g_sections = assign_group_calculations(data_resulting_g_sections)
+		data_resulting_g_sections2 = assign_group_calculations(data_resulting_g_sections2)
+		
+		# Generamos los datasets resulting.
+		data_resulting_fails = data_resulting_g_sections.groupby(['class_id','classes','fail_id_section']).aggregate(second_aggregation_dict).reset_index()
+		data_resulting_sections = data_resulting_g_sections2.groupby(['class_id','classes','section']).aggregate(second_aggregation_dict).reset_index()
+
+		table_summary_sections = data_resulting_sections.pivot_table(index=['section'], columns=['classes'], values=['distances']).fillna(0).astype('int')
+		table_summary_sections.columns = table_summary_sections.columns.droplevel(0)
+		index_sections_location = list(table_summary_sections.reset_index().section.values )
+		index_sections_location_end = list(np.array(index_sections_location)+1)
+		table_summary_sections['latitude'] = np.array(gps_obj.section_latitude)[index_sections_location]
+		table_summary_sections['longitude'] = np.array(gps_obj.section_longitude)[index_sections_location]
+		table_summary_sections['end_latitude'] = np.array(gps_obj.section_latitude)[index_sections_location_end]
+		table_summary_sections['end_longitude'] = np.array(gps_obj.section_longitude)[index_sections_location_end]
+		table_summary_sections['section_distance'] = np.array(gps_obj.section_distances)[index_sections_location]
+		for col in columns_to_have:
+			if col not in table_summary_sections.columns:
+				table_summary_sections[col]=0
+		table_summary_sections = table_summary_sections.reset_index()
+		table_summary_sections = pd.DataFrame(table_summary_sections.values, columns=list(table_summary_sections.columns))
+		table_summary_sections = table_summary_sections[['section',*columns_to_have, 'latitude','longitude','end_longitude',
+														 'end_latitude','section_distance']]
+		return table_summary_sections, data_resulting, data_resulting_fails
+
+	@staticmethod
+	def generate_final_results_signal(results_obj, gps_obj, classes_names_yolo_signal = ['ADTCIA','CIRCROJO','CRUZAMLLA','CUADBCO','CUADCAFE','CUADVERDE',
+																						 'CUADZUL','CUAMLLO','CURVA','INDAZUL','OBRA','OTRO','PROBROJO',
+																						 'ROMAMLLO','RUTA','SEMAFORO','STOP','TRIROJO']):
+		BOXES_SIGNAL = results_obj['boxes_signal']
+		CLASSES_SIGNAL = results_obj['classes_signal']
+		SIGNAL_CLASSES_siames = results_obj['final_signal_classes']
+		SIGNAL_CLASSES_BASE = results_obj['signal_base_predictions']
+		SIGNAL_STATE = results_obj['state_predictions']
+		SCORES_SIGNAL = results_obj['scores_signal']
+		final_latitude = gps_obj.gps_df.latitude.values
+		final_longitude = gps_obj.gps_df.longitude.values
+		fotograma = list(range(len(BOXES_SIGNAL)))
+
+		# Nos dice el cuadrante.
+		def position(center):
+			if center<0.33:
+				return 0
+			elif center<0.66:
+				return 1
+			else:
+				return 2
+
+		position_boxes = [[position((box[1]+box[3])/2) for box in BOXES_SIGNAL[f]] for f in range(len(BOXES_SIGNAL))]
+
+		rows = []
+		for f in fotograma:
+			for i in range(len(CLASSES_SIGNAL[f])):
+				r = [f, position_boxes[f][i], SCORES_SIGNAL[f][i], SIGNAL_STATE[f][i], SIGNAL_CLASSES_siames[f][i], SIGNAL_CLASSES_BASE[f][i], 
+				int(CLASSES_SIGNAL[f][i]), final_latitude[f], final_longitude[f]]
+				rows.append(r)
+
+
+		df = pd.DataFrame(rows, columns = ['fotogram', 'position_boxes', 'score', 'signal_state', 'signal_class_siames', 'signal_class_base', 
+			'signal_class', 'latitude', 'longitude'])
+
+		df['signal_class_siames_names'] = df['signal_class_siames'].values
+		df['signal_class_names'] = df['signal_class'].apply(lambda x: classes_names_yolo_signal[x])
+
+		yolo_classes_to_keep = []
+
+		x = tuple(zip(df['signal_class_siames_names'].values, df['signal_class_names'].values))
+
+		final_classes = []
+		for i in range(len(x)):
+			if x[i][1] in yolo_classes_to_keep:
+				final_classes.append(x[i][1])
+			else:
+				final_classes.append(x[i][0])
+
+		df['final_classes'] = final_classes
+		df['ID'] = range(len(df))
+
+		df = df.sort_values(['final_classes','position_boxes','fotogram']).reset_index(drop=True)
+
+		# cantidad de fotogramas a sacar repetidas.
+		N_fotogram = 5
+
+		for i in range(len(df)-1,0,-1):
+			if (df.loc[i-1, 'final_classes'] == df.loc[i, 'final_classes']) & \
+			(df.loc[i-1, 'position_boxes'] == df.loc[i, 'position_boxes']) & \
+			(np.abs(df.loc[i-1, 'fotogram']-df.loc[i, 'fotogram'])<=N_fotogram) & \
+			(df.loc[i, 'final_classes'] != 'OTRO'):
+				df.loc[i-1, 'ID'] = df.loc[i,'ID']
+
+		df = df.sort_values('fotogram', ascending=False).reset_index(drop=True).drop_duplicates(subset='ID')
+		df = df.sort_values('fotogram').reset_index(drop=True)
 		return df
```

### Comparing `pavimentados-0.29.0/pavimentados/analyzers/gps_sources.py` & `pavimentados-0.9.0/pavimentados/analyzers/gps_sources.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,176 +1,172 @@
-from pathlib import Path
-import pynmea2
-import pandas as pd
-import os
-import datetime as dt
-from PIL import Image
-from PIL.ExifTags import TAGS
-import numpy as np
-from tqdm import tqdm
-from pavimentados.analyzers.utils import total_distance
-from scipy.interpolate import interp1d
-
-
-class GPS_Processer:
-	def __init__(self):
-		self._calculate_seconds_from_start()
-	
-	def _calculate_seconds_from_start(self):
-		self.gps_df['seconds_from_start'] = self.gps_df.seconds.values-self.gps_df.seconds.values[0]
-
-	def adjust_gps_data(self, number_images):
-		list_values = np.linspace(0,self.gps_df.seconds_from_start.max(), number_images).astype('float')
-		f2 = interp1d(self.gps_df['seconds_from_start'].values, self.gps_df['longitude'].values, kind='linear')
-		f3 = interp1d(self.gps_df['seconds_from_start'].values, self.gps_df['latitude'].values, kind='linear')
-		initial_latitud = self.gps_df.loc[0].latitude
-		initial_longitude = self.gps_df.loc[0].longitude
-		final_longitude = f2(list_values)
-		final_latitude= f3(list_values)
-		final_longitude[0] = initial_longitude
-		final_latitude[0] = initial_latitud
-		self.gps_df = pd.DataFrame({'latitude':final_latitude, 'longitude':final_longitude})
-
-	def generate_gps_metrics(self, min_distance_group):
-		latitudes = list(self.gps_df.latitude.values)
-		longitudes = list(self.gps_df.longitude.values)
-		distances = total_distance(latitudes[:-1], longitudes[:-1], latitudes[1:], longitudes[1:])
-		distances = np.append(distances, distances[-1])
-		id_distances = []
-		id_dist = 0
-		sum_dist = 0
-		self.section_latitude = [latitudes[0]]
-		self.section_longitude = [longitudes[0]]
-		self.section_distances = []
-		for i in range(len(distances)):
-			if sum_dist>min_distance_group:
-				id_dist+=1
-				self.section_distances.append(sum_dist)
-				sum_dist=0
-				self.section_latitude.append(latitudes[i])
-				self.section_longitude.append(longitudes[i])
-			sum_dist +=distances[i]
-			id_distances.append(id_dist)
-		self.section_distances.append(sum_dist)
-		self.section_latitude.append(latitudes[i])
-		self.section_longitude.append(longitudes[i])
-		self.gps_df['distances'] = distances
-		self.gps_df['section'] = id_distances
-
-class GPS_Standard_Loader(GPS_Processer):
-	def __init__(self, route, **kwargs):
-		self.route = Path(route)
-		self.gps_df = None
-		self.load_gps_data()
-		super().__init__()
-	
-	def load_gps_data(self):
-		data = []
-		with open(self.route) as file:
-			for line in file.readlines():
-				try:
-					data.append(pynmea2.parse(line))
-				except pynmea2.ParseError as e:
-					continue
-		gps = {}
-		for value in data:
-			salida = gps.get(value.sentence_type,None)
-			if salida ==None:
-				gps[value.sentence_type] = []
-			gps[value.sentence_type].append(value)
-		select = list(gps.keys())[0]
-		gps_list = gps[select]
-		self.gps_df = pd.DataFrame(list(map(lambda x:(x.timestamp,x.longitude,x.latitude),gps_list)), 
-			columns=['timestamp','longitude','latitude'])
-		self.gps_df = self.gps_df.drop_duplicates(subset=['longitude','latitude']).reset_index(drop=True)
-		if type(self.gps_df.loc[0].timestamp)==type('str'):
-			self.gps_df['seconds'] = list(map(lambda x: int(float(x))/1000, self.gps_df.timestamp.values))
-		else:
-			self.gps_df['seconds'] = list(map(lambda x: (x.hour*3600)+(x.minute*60)+(x.second), self.gps_df.timestamp.values))
-
-class GPS_CSV_Loader(GPS_Processer):
-	def __init__(self, route, **kwargs):
-		latitud_column = kwargs.get('latitud_column', None)
-		longitud_column = kwargs.get('longitud_column', None) 
-		time_column = kwargs.get('time_column', None)
-		date_column = kwargs.get('date_column', None) 
-		decimal_character = kwargs.get('decimal_character', ',')
-		
-		self.route = Path(route)
-		self.columns_names = []
-		if time_column!=None:
-			self.columns_names.append(time_column)
-		if date_column!=None:
-			self.columns_names.append(date_column)
-		if longitud_column!=None:
-			self.columns_names.append(longitud_column)
-		if latitud_column!=None:
-			self.columns_names.append(latitud_column)
-		self.decimal_character = decimal_character
-		self.load_gps_data()
-		super().__init__()
-	
-	def load_gps_data(self):
-		self.gps_df = pd.read_csv(self.route, sep=';', encoding='latin1', decimal=self.decimal_character)[self.columns_names]
-		if self.columns_names==3:
-			self.gps_df.columns = ['timestamp','longitude','latitude']
-			self.gps_df['timestamp'] = list(map(lambda x: dt.datetime.strptime(x, '%Y-%m-%d %H:%M:%S'), self.gps_df['timestamp']))
-		else:
-			self.gps_df.columns = ['time','date','longitude','latitude']
-			self.gps_df['timestamp'] = list(map(lambda x, y: dt.datetime.strptime(x+' '+y, '%Y-%m-%d %H:%M:%S'), self.gps_df['date'].values, self.gps_df['time'].values))
-			self.gps_df = self.gps_df[['timestamp','longitude','latitude']]
-		if type(self.gps_df.loc[0].timestamp)==type('str'):
-			self.gps_df['seconds'] = list(map(lambda x: int(float(x))/1000, self.gps_df.timestamp.values))
-		else:
-			self.gps_df['seconds'] = list(map(lambda x: (x.hour*3600)+(x.minute*60)+(x.second), self.gps_df.timestamp))
-
-class GPS_Image_Route_Loader(GPS_Processer):
-	def __init__(self, images_routes, **kwargs):
-		self.routes = images_routes
-		self.load_gps_data()
-		super().__init__()		
-	
-	def load_gps_data(self):
-		self.gps_df = pd.DataFrame(list(tqdm(map(lambda img_path: self.load_single_value(img_path), self.routes))))
-		self.gps_df['seconds'] = list(map(lambda x: (x.hour*3600)+(x.minute*60)+(x.second), self.gps_df.timestamp))		
-	
-	def load_single_value(self, img_path):
-		d = {}
-		image = Image.open(img_path)
-		exifdata = image.getexif()
-		for tag_id in exifdata:
-			tag = TAGS.get(tag_id, tag_id)
-			data = exifdata.get(tag_id)
-			try:
-				if isinstance(data, bytes):
-					data = data.decode()
-				d[tag] = data
-			except:
-				pass
-		lat = np.array(d['GPSInfo'][2])
-		lon = np.array(d['GPSInfo'][4])
-		lat = sum(np.array(lat[:,0]/lat[:,1]) * np.array([1.0,1.0/60.0,1.0/3600.0]))*(-1 if d['GPSInfo'][1]=='S' else 1)
-		lon = sum(np.array(lon[:,0]/lon[:,1]) * np.array([1.0,1.0/60.0,1.0/3600.0]))*(-1 if d['GPSInfo'][3]=='W' else 1)
-		time = dt.datetime.strptime(d['DateTimeOriginal'], '%Y:%m:%d %H:%M:%S')
-		return {'timestamp':time, 'longitude':lon, 'latitude':lat}
-
-
-class GPS_Image_Folder_Loader(GPS_Image_Route_Loader):
-	def __init__(self, route, **kwargs):
-		self.routes = [Path(route) / item for item in os.listdir(Path(route))]
-		self.load_gps_data()
-		super(GPS_Image_Route_Loader, self).__init__()	
-
-
-gps_source_options_dict = {
-	'image_routes' : GPS_Image_Route_Loader, 
-	'image_folder' : GPS_Image_Folder_Loader,
-	'csv' : GPS_CSV_Loader, 
-	'loc'  : GPS_Standard_Loader
-}
-
-def GPS_Data_Loader(source_type, gps_in, **kwargs):
-	if source_type not in gps_source_options_dict:
-		raise NameError(f'{source_type} not implemented on the method')
-	return gps_source_options_dict[source_type](gps_in,**kwargs)
-	
+from pathlib import Path
+import pynmea2
+import pandas as pd
+import os
+import datetime as dt
+from PIL import Image
+from PIL.ExifTags import TAGS
+import numpy as np
+from tqdm import tqdm
+from pavimentados.analyzers.utils import total_distance
+from scipy.interpolate import interp1d
+
+
+class GPS_Processer:
+	def __init__(self):
+		self._calculate_seconds_from_start()
+	
+	def _calculate_seconds_from_start(self):
+		self.gps_df['seconds_from_start'] = self.gps_df.seconds.values-self.gps_df.seconds.values[0]
+
+	def adjust_gps_data(self, number_images):
+		list_values = np.linspace(0,self.gps_df.seconds_from_start.max(), number_images).astype('float')
+		f2 = interp1d(self.gps_df['seconds_from_start'].values, self.gps_df['longitude'].values, kind='linear')
+		f3 = interp1d(self.gps_df['seconds_from_start'].values, self.gps_df['latitude'].values, kind='linear')
+		final_longitude = f2(list_values)
+		final_latitude= f3(list_values)
+		self.gps_df = pd.DataFrame({'latitude':final_latitude, 'longitude':final_longitude})
+
+	def generate_gps_metrics(self, min_distance_group):
+		latitudes = list(self.gps_df.latitude.values)
+		longitudes = list(self.gps_df.longitude.values)
+		distances = total_distance(latitudes[:-1], longitudes[:-1], latitudes[1:], longitudes[1:])
+		distances = np.append(distances, distances[-1])
+		id_distances = []
+		id_dist = 0
+		sum_dist = 0
+		self.section_latitude = [latitudes[0]]
+		self.section_longitude = [longitudes[0]]
+		self.section_distances = []
+		for i in range(len(distances)):
+			if sum_dist>min_distance_group:
+				id_dist+=1
+				self.section_distances.append(sum_dist)
+				sum_dist=0
+				self.section_latitude.append(latitudes[i])
+				self.section_longitude.append(longitudes[i])
+			sum_dist +=distances[i]
+			id_distances.append(id_dist)
+		self.section_distances.append(sum_dist)
+		self.section_latitude.append(latitudes[i])
+		self.section_longitude.append(longitudes[i])
+		self.gps_df['distances'] = distances
+		self.gps_df['section'] = id_distances
+
+class GPS_Standard_Loader(GPS_Processer):
+	def __init__(self, route, **kwargs):
+		self.route = Path(route)
+		self.gps_df = None
+		self.load_gps_data()
+		super().__init__()
+	
+	def load_gps_data(self):
+		data = []
+		with open(self.route) as file:
+			for line in file.readlines():
+				try:
+					data.append(pynmea2.parse(line))
+				except pynmea2.ParseError as e:
+					continue
+		gps = {}
+		for value in data:
+			salida = gps.get(value.sentence_type,None)
+			if salida ==None:
+				gps[value.sentence_type] = []
+			gps[value.sentence_type].append(value)
+		select = list(gps.keys())[0]
+		gps_list = gps[select]
+		self.gps_df = pd.DataFrame(list(map(lambda x:(x.timestamp,x.longitude,x.latitude),gps_list)), 
+			columns=['timestamp','longitude','latitude'])
+		self.gps_df = self.gps_df.drop_duplicates(subset=['longitude','latitude']).reset_index(drop=True)
+		if type(self.gps_df.loc[0].timestamp)==type('str'):
+			self.gps_df['seconds'] = list(map(lambda x: int(float(x))/1000, self.gps_df.timestamp.values))
+		else:
+			self.gps_df['seconds'] = list(map(lambda x: (x.hour*3600)+(x.minute*60)+(x.second), self.gps_df.timestamp.values))
+
+class GPS_CSV_Loader(GPS_Processer):
+	def __init__(self, route, **kwargs):
+		latitud_column = kwargs.get('latitud_column', None)
+		longitud_column = kwargs.get('longitud_column', None) 
+		time_column = kwargs.get('time_column', None)
+		date_column = kwargs.get('date_column', None) 
+		decimal_character = kwargs.get('decimal_character', ',')
+		
+		self.route = Path(route)
+		self.columns_names = []
+		if time_column!=None:
+			self.columns_names.append(time_column)
+		if date_column!=None:
+			self.columns_names.append(date_column)
+		if longitud_column!=None:
+			self.columns_names.append(longitud_column)
+		if latitud_column!=None:
+			self.columns_names.append(latitud_column)
+		self.decimal_character = decimal_character
+		self.load_gps_data()
+		super().__init__()
+	
+	def load_gps_data(self):
+		self.gps_df = pd.read_csv(self.route, sep=';', encoding='latin1', decimal=self.decimal_character)[self.columns_names]
+		if self.columns_names==3:
+			self.gps_df.columns = ['timestamp','longitude','latitude']
+			self.gps_df['timestamp'] = list(map(lambda x: dt.datetime.strptime(x, '%Y-%m-%d %H:%M:%S'), self.gps_df['timestamp']))
+		else:
+			self.gps_df.columns = ['time','date','longitude','latitude']
+			self.gps_df['timestamp'] = list(map(lambda x, y: dt.datetime.strptime(x+' '+y, '%Y-%m-%d %H:%M:%S'), self.gps_df['date'].values, self.gps_df['time'].values))
+			self.gps_df = self.gps_df[['timestamp','longitude','latitude']]
+		if type(self.gps_df.loc[0].timestamp)==type('str'):
+			self.gps_df['seconds'] = list(map(lambda x: int(float(x))/1000, self.gps_df.timestamp.values))
+		else:
+			self.gps_df['seconds'] = list(map(lambda x: (x.hour*3600)+(x.minute*60)+(x.second), self.gps_df.timestamp))
+
+class GPS_Image_Route_Loader(GPS_Processer):
+	def __init__(self, images_routes, **kwargs):
+		self.routes = images_routes
+		self.load_gps_data()
+		super().__init__()		
+	
+	def load_gps_data(self):
+		self.gps_df = pd.DataFrame(list(tqdm(map(lambda img_path: self.load_single_value(img_path), self.routes))))
+		self.gps_df['seconds'] = list(map(lambda x: (x.hour*3600)+(x.minute*60)+(x.second), self.gps_df.timestamp))		
+	
+	def load_single_value(self, img_path):
+		d = {}
+		image = Image.open(img_path)
+		exifdata = image.getexif()
+		for tag_id in exifdata:
+			tag = TAGS.get(tag_id, tag_id)
+			data = exifdata.get(tag_id)
+			try:
+				if isinstance(data, bytes):
+					data = data.decode()
+				d[tag] = data
+			except:
+				pass
+		lat = np.array(d['GPSInfo'][2])
+		lon = np.array(d['GPSInfo'][4])
+		lat = sum(np.array(lat[:,0]/lat[:,1]) * np.array([1.0,1.0/60.0,1.0/3600.0]))*(-1 if d['GPSInfo'][1]=='S' else 1)
+		lon = sum(np.array(lon[:,0]/lon[:,1]) * np.array([1.0,1.0/60.0,1.0/3600.0]))*(-1 if d['GPSInfo'][3]=='W' else 1)
+		time = dt.datetime.strptime(d['DateTimeOriginal'], '%Y:%m:%d %H:%M:%S')
+		return {'timestamp':time, 'longitude':lon, 'latitude':lat}
+
+
+class GPS_Image_Folder_Loader(GPS_Image_Route_Loader):
+	def __init__(self, route, **kwargs):
+		self.routes = [Path(route) / item for item in os.listdir(Path(route))]
+		self.load_gps_data()
+		super(GPS_Image_Route_Loader, self).__init__()	
+
+
+gps_source_options_dict = {
+	'image_routes' : GPS_Image_Route_Loader, 
+	'image_folder' : GPS_Image_Folder_Loader,
+	'csv' : GPS_CSV_Loader, 
+	'loc'  : GPS_Standard_Loader
+}
+
+def GPS_Data_Loader(source_type, gps_in, **kwargs):
+	if source_type not in gps_source_options_dict:
+		raise NameError(f'{source_type} not implemented on the method')
+	return gps_source_options_dict[source_type](gps_in,**kwargs)
+
```

### Comparing `pavimentados-0.29.0/pavimentados/analyzers/utils.py` & `pavimentados-0.9.0/pavimentados/analyzers/utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-import numpy as np
-import pandas as pd
-
-def total_distance(lat1,lon1,lat2,lon2):
-	"""
-	Calcula la distancia entre dos puntos (lat1, lon1) y (lat2, lon2).
-	"""
-
-	R = 6373.0 # approximate radius of earth in km.
-
-	lat1 = np.radians(lat1)
-	lon1 = np.radians(lon1)
-	lat2 = np.radians(lat2)
-	lon2 = np.radians(lon2)
-
-	dlon = lon2 - lon1
-	dlat = lat2 - lat1
-
-	a = np.sin(dlat / 2)**2 + np.cos(lat1) * np.cos(lat2) * np.sin(dlon / 2)**2
-	c = 2 * np.arctan2(np.sqrt(a), np.sqrt(1 - a))
-
-	distance = R * c*1000
-	return distance
-
-def area_calc(boxes,altura, base):
-	"""
-	Calcula el area de la caja.
-	"""
-	if len(boxes)>0:
-		return ((boxes[2]-boxes[0])*altura)*((boxes[3]-boxes[1])*base)
-	else:
-		return 0
-
-def box_center(boxes, altura, base):
-	"""
-	Calcula el centro de la caja.
-	"""
-	if len(boxes)>0:
-		return (((boxes[3]+boxes[1])/2)*base),(((boxes[2]+boxes[0])/2)*altura)
-	else:
-		return None,None
-
-def box_height(boxes,altura):
-	"""
-	Calcula la altura de la caja.
-	"""
-	if len(boxes)>0:
-		return ((boxes[2]-boxes[0])*altura)
-	else:
-		return None
-
-
-def box_width(boxes,base):
-	"""
-	Calcula la base de la caja.
-	"""
-	if len(boxes)>0:
-		return ((boxes[3]-boxes[1])*base)	
-	else:
-		return None
-
-
-def fail_id_generator(df, min_photogram_distance):
-	"""
-	Genera un ID de fail. Esto se realiza ya que cada fail es detectada en 
-	fotogramas simultaneos y es necesario identificarla como una misma fail.
-	"""
-
-	df_id_fails = []
-	id_fail = 0
-	for fail in list(df.classes.unique()):
-		df_fail = df.loc[df.classes==fail].copy().reset_index(drop=True)
-		fotogramas = df_fail.fotograma
-		id_section_fail = [id_fail]
-		for i in range(len(fotogramas)-1):
-			if (fotogramas[i+1]-fotogramas[i])>min_photogram_distance:
-				id_fail +=1
-			id_section_fail.append(id_fail)
-		id_section_fail = np.array(id_section_fail)
-		if len(id_section_fail)>0:
-			df_fail['fail_id_section'] = id_section_fail
-			df_id_fails.append(df_fail)
-	df = pd.concat(df_id_fails).sort_values(['fotograma','classes','fail_id_section']).reset_index(drop=True)
-	return df
-
-def stack_columns_dataset(df, variables, static_variables):
-	df['ind'] = df.index 
-	df_resulting = df[static_variables].copy()
-	c = 0
-	for v in variables:
-		d = pd.DataFrame([[i,t] for  i,T in df[['ind',v]].values for t in T], columns=['ind',v])
-		d['ind2'] = d.index
-		if c==0:
-			df_resulting = pd.merge(df_resulting,d, on='ind', how='left')
-			c+=1
-		else:
-			df_resulting = pd.merge(df_resulting,d, on=['ind','ind2'], how='left')
-	return df_resulting	
-
-def assign_group_calculations(df):
-	df['area'] = df.width.values*df.distances.values
-	df['start_coordinate'] = list(map(lambda x,y: (x,y), df.latitude.values, df.longitude.values))
-	df['end_coordenate'] = list(map(lambda x,y: (x,y), df.latitude.values, df.longitude.values))
-	df['start_latitude'] = df.latitude
-	df['end_latitude'] = df.latitude
-	df['start_longitude'] = df.longitude
-	df['end_longitude'] = df.longitude
+import numpy as np
+import pandas as pd
+
+def total_distance(lat1,lon1,lat2,lon2):
+	"""
+	Calcula la distancia entre dos puntos (lat1, lon1) y (lat2, lon2).
+	"""
+
+	R = 6373.0 # approximate radius of earth in km.
+
+	lat1 = np.radians(lat1)
+	lon1 = np.radians(lon1)
+	lat2 = np.radians(lat2)
+	lon2 = np.radians(lon2)
+
+	dlon = lon2 - lon1
+	dlat = lat2 - lat1
+
+	a = np.sin(dlat / 2)**2 + np.cos(lat1) * np.cos(lat2) * np.sin(dlon / 2)**2
+	c = 2 * np.arctan2(np.sqrt(a), np.sqrt(1 - a))
+
+	distance = R * c*1000
+	return distance
+
+def area_calc(boxes,altura, base):
+	"""
+	Calcula el area de la caja.
+	"""
+	if len(boxes)>0:
+		return ((boxes[2]-boxes[0])*altura)*((boxes[3]-boxes[1])*base)
+	else:
+		return 0
+
+def box_center(boxes, altura, base):
+	"""
+	Calcula el centro de la caja.
+	"""
+	if len(boxes)>0:
+		return (((boxes[3]+boxes[1])/2)*base),(((boxes[2]+boxes[0])/2)*altura)
+	else:
+		return None,None
+
+def box_height(boxes,altura):
+	"""
+	Calcula la altura de la caja.
+	"""
+	if len(boxes)>0:
+		return ((boxes[2]-boxes[0])*altura)
+	else:
+		return None
+
+
+def box_width(boxes,base):
+	"""
+	Calcula la base de la caja.
+	"""
+	if len(boxes)>0:
+		return ((boxes[3]-boxes[1])*base)	
+	else:
+		return None
+
+
+def fail_id_generator(df, min_photogram_distance):
+	"""
+	Genera un ID de fail. Esto se realiza ya que cada fail es detectada en 
+	fotogramas simultaneos y es necesario identificarla como una misma fail.
+	"""
+
+	df_id_fails = []
+	id_fail = 0
+	for fail in list(df.classes.unique()):
+		df_fail = df.loc[df.classes==fail].copy().reset_index(drop=True)
+		fotogramas = df_fail.fotograma
+		id_section_fail = [id_fail]
+		for i in range(len(fotogramas)-1):
+			if (fotogramas[i+1]-fotogramas[i])>min_photogram_distance:
+				id_fail +=1
+			id_section_fail.append(id_fail)
+		id_section_fail = np.array(id_section_fail)
+		if len(id_section_fail)>0:
+			df_fail['fail_id_section'] = id_section_fail
+			df_id_fails.append(df_fail)
+	df = pd.concat(df_id_fails).sort_values(['fotograma','classes','fail_id_section']).reset_index(drop=True)
+	return df
+
+def stack_columns_dataset(df, variables, static_variables):
+	df['ind'] = df.index 
+	df_resulting = df[static_variables].copy()
+	c = 0
+	for v in variables:
+		d = pd.DataFrame([[i,t] for  i,T in df[['ind',v]].values for t in T], columns=['ind',v])
+		d['ind2'] = d.index
+		if c==0:
+			df_resulting = pd.merge(df_resulting,d, on='ind', how='left')
+			c+=1
+		else:
+			df_resulting = pd.merge(df_resulting,d, on=['ind','ind2'], how='left')
+	return df_resulting	
+
+def assign_group_calculations(df):
+	df['area'] = df.width.values*df.distances.values
+	df['start_coordinate'] = list(map(lambda x,y: (x,y), df.latitude.values, df.longitude.values))
+	df['end_coordenate'] = list(map(lambda x,y: (x,y), df.latitude.values, df.longitude.values))
+	df['start_latitude'] = df.latitude
+	df['end_latitude'] = df.latitude
+	df['start_longitude'] = df.longitude
+	df['end_longitude'] = df.longitude
 	return df
```

### Comparing `pavimentados-0.29.0/pavimentados/downloader.py` & `pavimentados-0.9.0/pavimentados/downloader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-from pathlib import Path
-import boto3
-import os
-import sys
-import logging
-import tempfile
-from urllib import parse, request
-import tarfile
-
-logger = logging.getLogger()
-pavimentados_path = Path(__file__).parent
-models_url = 'https://pavimenta2-artifacts.s3.amazonaws.com/models.tar.gz'
-
-class Downloader:
-
-	def __init__(self, models_path = pavimentados_path / 'models' ):
-		"""
-		This class allows to download de models and other model data from the Inter-American Development Bank repositories
-		
-		Parameters
-		----------
-
-		models_path: str (default instalation path of package)
-			The route where is going to download and check the artifacts of the models
-		"""
-		self.models_path = models_path
-	
-	def check_artifacts(self):
-		"""
-		This function allows to check if the path for downloads exists
-		"""
-		if not Path(self.models_path / 'artifacts').is_dir():
-			raise ImportError('The route for the models is not present, it means that the models are not downloaded on this environment, use viasegura.download_models function to download them propertly')
-	
-	def check_files(self, filePath):
-
-		"""
-		This function allows to chec if an specific file exists
-
-		Parameters
-		----------
-
-		filePath: str
-			Route of the file to be checked
-
-		"""
-		if Path(filePath).is_file():
-			return True
-		else:
-			return False
-	
-	def download(self, url = None, aws_access_key=None, signature = None, expires = None):
-		"""
-		This function allows to dowload the corresponding packages using the route already on the created instance
-
-		Parameters
-		----------
-		
-		url: str
-			The signed url for downloading the models
-
-		aws_access_key: str
-			The aws access key id provided by the interamerican development bank to have access to the models
-
-		signature: str
-			The aws signature provided from IDB to download the models
-
-		expires: int
-			Time in seconds provided by the IDB in which the signature will expire
-
-		"""
-		if url:
-			self.models_path.mkdir(parents=True, exist_ok=True)
-			temp_file_path = tempfile.NamedTemporaryFile(suffix='.tar.gz').name
-			logger.info('Downloading models')
-			try:
-				request.urlretrieve(url, temp_file_path)
-			except:
-				raise Exception('Provided signature is invalid.')
-
-			logger.info('Uncompressing models')
-			with tarfile.open(temp_file_path, mode='r:gz') as tfile:
-				tfile.extractall(str(self.models_path))
-			logger.info('Models are available')
-			os.remove(temp_file_path)
-		elif aws_access_key:
-			self.models_path.mkdir(parents=True, exist_ok=True)
-			params = {
-				'AWSAccessKeyId': aws_access_key,
-				'Signature': signature,
-				'Expires': expires
-			}
-			composed_url = '{}?{}'.format(models_url, parse.urlencode(params))
-			temp_file_path = tempfile.NamedTemporaryFile(suffix='.tar.gz').name
-			logger.info('Downloading models')
-			try:
-				request.urlretrieve(composed_url, temp_file_path)
-			except:
-				raise Exception('Provided signature is invalid.')
-			logger.info('Uncompressing models')
-			with tarfile.open(temp_file_path, mode='r:gz') as tfile:
-				tfile.extractall(str(self.models_path))
-			logger.info('Models are available')
-			os.remove(temp_file_path)
-		else:
+from pathlib import Path
+import boto3
+import os
+import sys
+import logging
+import tempfile
+from urllib import parse, request
+import tarfile
+
+logger = logging.getLogger()
+viasegura_path = Path(__file__).parent
+models_url = 'https://pavimenta2-artifacts.s3.amazonaws.com/models.tar.gz'
+
+class Downloader:
+
+	def __init__(self, models_path = viasegura_path / 'models' ):
+		"""
+		This class allows to download de models and other model data from the Inter-American Development Bank repositories
+		
+		Parameters
+		----------
+
+		models_path: str (default instalation path of package)
+			The route where is going to download and check the artifacts of the models
+		"""
+		self.models_path = models_path
+	
+	def check_artifacts(self):
+		"""
+		This function allows to check if the path for downloads exists
+		"""
+		if not Path(self.models_path / 'artifacts').is_dir():
+			raise ImportError('The route for the models is not present, it means that the models are not downloaded on this environment, use viasegura.download_models function to download them propertly')
+	
+	def check_files(self, filePath):
+
+		"""
+		This function allows to chec if an specific file exists
+
+		Parameters
+		----------
+
+		filePath: str
+			Route of the file to be checked
+
+		"""
+		if Path(filePath).is_file():
+			return True
+		else:
+			return False
+	
+	def download(self, url = None, aws_access_key=None, signature = None, expires = None):
+		"""
+		This function allows to dowload the corresponding packages using the route already on the created instance
+
+		Parameters
+		----------
+		
+		url: str
+			The signed url for downloading the models
+
+		aws_access_key: str
+			The aws access key id provided by the interamerican development bank to have access to the models
+
+		signature: str
+			The aws signature provided from IDB to download the models
+
+		expires: int
+			Time in seconds provided by the IDB in which the signature will expire
+
+		"""
+		if url:
+			self.models_path.mkdir(parents=True, exist_ok=True)
+			temp_file_path = tempfile.NamedTemporaryFile(suffix='.tar.gz').name
+			logger.info('Downloading models')
+			try:
+				request.urlretrieve(url, temp_file_path)
+			except:
+				raise Exception('Provided signature is invalid.')
+
+			logger.info('Uncompressing models')
+			with tarfile.open(temp_file_path, mode='r:gz') as tfile:
+				tfile.extractall(str(self.models_path))
+			logger.info('Models are available')
+			os.remove(temp_file_path)
+		elif aws_access_key:
+			self.models_path.mkdir(parents=True, exist_ok=True)
+			params = {
+				'AWSAccessKeyId': aws_access_key,
+				'Signature': signature,
+				'Expires': expires
+			}
+			composed_url = '{}?{}'.format(models_url, parse.urlencode(params))
+			temp_file_path = tempfile.NamedTemporaryFile(suffix='.tar.gz').name
+			logger.info('Downloading models')
+			try:
+				request.urlretrieve(composed_url, temp_file_path)
+			except:
+				raise Exception('Provided signature is invalid.')
+			logger.info('Uncompressing models')
+			with tarfile.open(temp_file_path, mode='r:gz') as tfile:
+				tfile.extractall(str(self.models_path))
+			logger.info('Models are available')
+			os.remove(temp_file_path)
+		else:
 			raise NameError('Must provide any valid method of download either signature or valid url, please contact IDB to obtain the proper data')
```

### Comparing `pavimentados-0.29.0/pavimentados/models/structures.py` & `pavimentados-0.9.0/pavimentados/models/structures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,251 +1,239 @@
-from pavimentados.models.yolo import YoloV3
-from pavimentados.configs.utils import Config_Basic
-from pathlib import Path
-import tensorflow as tf
-import json
-import cv2
-from tqdm import tqdm
-import os
-import numpy as np
-import joblib
-
-pavimentados_path = Path(__file__).parent.parent
-
-def image_encoder(FILTERS, KERNEL, STRIDE, POOL, USE_BATCH_NORM, USE_DROPOUT, SIAMESE_IMAGE_SIZE):
-	inputs = tf.keras.layers.Input(SIAMESE_IMAGE_SIZE)
-
-	x = inputs
-	for i in range(len(FILTERS)):
-		x = tf.keras.layers.Conv2D(filters = FILTERS[i], 
-			kernel_size = KERNEL[i], strides = STRIDE[i], 
-			padding = 'same', 
-			name = 'encoder_conv_' + str(i))(x)
-
-		if USE_BATCH_NORM:
-			x = tf.keras.layers.BatchNormalization()(x)
-
-		x = tf.keras.layers.LeakyReLU()(x)
-
-		x = tf.keras.layers.MaxPooling2D(pool_size = POOL[i], padding='same')(x)
-
-		if USE_DROPOUT:
-			x = tf.keras.layers.Dropout(rate=0.25)(x)
-
-	x = tf.keras.layers.Flatten()(x)
-	output = x
-	return tf.keras.Model(inputs, output)
-
-class ComparationLayer(tf.keras.layers.Layer):
-	def __init__(self, comparison_matrix, layer_type,  **kwargs):
-		self.IM2_compress_list = comparison_matrix
-		self.layer_type = layer_type
-		super(ComparationLayer, self).__init__(**kwargs)
-
-	def build(self, input_shape):
-		self.built = True
-
-	def call(self, inputs):
-		x = inputs/tf.keras.backend.sqrt(tf.keras.layers.Dot(1)([inputs,inputs]))
-		x_l = []
-		for i in range(len(self.IM2_compress_list)):
-			x_l.append(tf.keras.backend.dot(x,tf.transpose(self.IM2_compress_list[i])))
-		if self.layer_type == 0:
-			x = tf.concat(x_l,axis=1)
-			x = tf.keras.backend.argmax(x,axis=1)
-			out = tf.math.floormod(x, 16)
-			return out
-		else:
-			out = tf.concat([tf.expand_dims(x_l[i],axis=1) for i in range(len(x_l))], axis=1)
-			return out
-	
-	def get_config(self):
-		return {'IM2_compress_c'+str(i+1): self.IM2_compress_list[i] for i in range(len(self.IM2_compress_list))}
-
-class Pav_Model(Config_Basic):
-	def __init__(self, device = '/device:CPU:0', config_file = pavimentados_path / 'configs'  / 'models_general.json'):
-		self.load_config(config_file)
-		self.general_path = pavimentados_path / Path(self.config['general_path'])
-		self.model = None
-		self.device = device
-		
-	def predict(self,data):
-		with tf.device(self.device):
-			return self.model.predict(data)
-		
-	def load_model(self):
-		pass
-
-class Yolo_Model(Pav_Model):
-	
-	def __init__(self,device = None, config_file = pavimentados_path / 'configs'  / 'yolo_config.json', general_config_file = pavimentados_path /'configs' / 'models_general.json', artifacts_path = None):
-		super().__init__(device, config_file = general_config_file)
-		self.general_config = self.config.copy()
-		self.load_config(config_file)
-		self.config['yolo_pav_dict_clases'] = {int(k):v for k,v in self.config['yolo_pav_dict_clases'].items()}
-		if artifacts_path:
-			self.yolo_paviment_path = Path(artifacts_path) / self.config['yolo_paviment_path']
-			self.yolo_signal_path = Path(artifacts_path) / self.config['yolo_signal_path']
-		else:
-			self.yolo_paviment_path = self.general_path / self.config['yolo_paviment_path']
-			self.yolo_signal_path = self.general_path / self.config['yolo_signal_path']
-		self.load_model()
-	
-	def load_model(self):
-		"""
-		Carga los modelos de YOLO.
-		""" 
-		with tf.device(self.device):
-
-			# Carga las clases de modelo de pavimentos.
-			classes_paviment = list({name: idx for idx, name in enumerate(open(self.yolo_paviment_path / 'classes'/'classes.names').read().splitlines())}.keys())
-			self.num_classes_paviment = len(classes_paviment)
-
-			# Carga las clases de modelo de señales,
-			classes_signal = list({name: idx for idx, name in enumerate(open(self.yolo_signal_path / 'classes'/'classes.names').read().splitlines())}.keys())
-			self.num_classes_signal = len(classes_signal)
-
-			# Une las clases de ambos modelos.
-			self.full_classes = [*classes_paviment, *classes_signal]
-
-			# Carga el path de los pesos de yolo de pavimentos y señales.
-			path_weights_paviment = self.yolo_paviment_path / 'checkpoints_model' / 'yolov3_train_8.tf'
-			path_weights_signal = self.yolo_signal_path / 'checkpoints_model' / 'yolov3_train_8.tf'
-
-			# Instancia los modelos.
-			yolo_paviment = YoloV3(classes=self.num_classes_paviment, model_name = 'yolov3_paviment')
-			yolo_signal = YoloV3(classes=self.num_classes_signal, model_name = 'yolov3_signal')
-
-			# Carga los pesos.
-			yolo_paviment.load_weights(path_weights_paviment).expect_partial()
-			yolo_signal.load_weights(path_weights_signal).expect_partial()
-
-			# Genera modelo final.
-			input_model = tf.keras.Input(shape=(416,416,3), name='image')
-			paviment_output = yolo_paviment(input_model)
-			signal_output = yolo_signal(input_model)
-			self.model = tf.keras.models.Model(input_model,[paviment_output,signal_output])
-
-class Siamese_Model(Pav_Model):
-	
-	def __init__(self,device = None, config_file = pavimentados_path / 'configs'  / 'siamese_config.json', general_config_file = pavimentados_path / 'configs'  / 'models_general.json', artifacts_path = None):
-		super().__init__(device, config_file = general_config_file)
-		self.general_config = self.config.copy()
-		self.load_config(config_file)
-		if artifacts_path:
-			self.siamese_path = Path(artifacts_path) / self.config['siamese_path']
-		else:
-			self.siamese_path = pavimentados_path / self.general_path / self.config['siamese_path']
-		self.load_model()
-	
-	def load_model(self):
-		"""
-		Carga los modelos de YOLO.
-		""" 
-		with tf.device(self.device):
-			FIRST_COMPARISON_EXAMPLES_NUMBER = self.config['FIRST_COMPARISON_EXAMPLES_NUMBER']
-			SECOND_COMPARISON_EXAMPLES_NUMBER = self.config['SECOND_COMPARISON_EXAMPLES_NUMBER']
-			FIRST_COMPARISON_FOLDER = self.config['FIRST_COMPARISON_FOLDER']
-			SECOND_COMPARISON_FOLDER = self.config['SECOND_COMPARISON_FOLDER']
-			
-			SIAMESE_IMAGE_SIZE = tuple(self.config['SIAMESE_IMAGE_SIZE'])
-			FILTERS = self.config['FILTERS']
-			KERNEL = self.config['KERNEL']
-			STRIDE = self.config['STRIDE']
-			POOL = self.config['POOL']
-			USE_BATCH_NORM = bool(self.config['USE_BATCH_NORM'])
-			USE_DROPOUT = bool(self.config['USE_DROPOUT'])
-			IM2_TOTAL_C = []
-			
-			for i in range(FIRST_COMPARISON_EXAMPLES_NUMBER):
-				IM2_TOTAL_C.append([])
-			
-			class_names_first = {}
-			self.class_names_last = {}
-			c = 0
-			search_path = self.siamese_path / FIRST_COMPARISON_FOLDER
-			for path in tqdm(os.listdir(search_path)):
-				class_names_first[path] = c
-				self.class_names_last[path] = []
-				c +=1
-				item_search_path = search_path / path
-				x = os.listdir(item_search_path)
-				images_files = [item_search_path / i for i in x]
-				if len(images_files)>=FIRST_COMPARISON_EXAMPLES_NUMBER:
-					for i in range(FIRST_COMPARISON_EXAMPLES_NUMBER):
-						IM2_TOTAL_C[i].append(cv2.resize(cv2.imread(str(images_files[i])), SIAMESE_IMAGE_SIZE[:2], interpolation = cv2.INTER_AREA).astype(float)/255)
-
-			for i in range(FIRST_COMPARISON_EXAMPLES_NUMBER):
-				IM2_TOTAL_C[i] = np.array(IM2_TOTAL_C[i])
-			self.inv_class_names_first = {v: k for k, v in class_names_first.items()}
-
-			dict_clases_sub = joblib.load(self.siamese_path / 'dict_senales_clases.pickle')
-			inv_dict_clases_sub = {item:k for k,v in dict_clases_sub.items() for item in v}
-			
-			IM2_LAST_C = []
-			for i in range(SECOND_COMPARISON_EXAMPLES_NUMBER):
-				IM2_LAST_C.append([])
-				
-			c = 0
-			self.class_names_last_complete = {}
-			search_path = self.siamese_path / SECOND_COMPARISON_FOLDER
-			for path in tqdm(os.listdir(search_path)):
-				if inv_dict_clases_sub.get(path, None):
-					self.class_names_last[inv_dict_clases_sub[path]].append(c)
-					self.class_names_last_complete[c] = path
-					c +=1
-					item_search_path = search_path / path
-					x = os.listdir(item_search_path)
-					images_files = [item_search_path / i for i in x]
-					if len(images_files)>=SECOND_COMPARISON_EXAMPLES_NUMBER:
-						for i in range(SECOND_COMPARISON_EXAMPLES_NUMBER):
-							IM2_LAST_C[i].append(cv2.resize(cv2.imread(str(images_files[i])), SIAMESE_IMAGE_SIZE[:2], interpolation = cv2.INTER_AREA).astype(float)/255)
-
-			for i in range(SECOND_COMPARISON_EXAMPLES_NUMBER):
-				IM2_LAST_C[i] = np.array(IM2_LAST_C[i])
-			
-			print('Createing siamese model')
-			image_conv_encoder = image_encoder(FILTERS,KERNEL,STRIDE,POOL,USE_BATCH_NORM,USE_DROPOUT, SIAMESE_IMAGE_SIZE)
-			image_conv_encoder_last = image_encoder(FILTERS,KERNEL,STRIDE,POOL,USE_BATCH_NORM,USE_DROPOUT, SIAMESE_IMAGE_SIZE)
-			print('Loading Weights siamese')
-			image_conv_encoder.load_weights(str(self.siamese_path / "image_encoder_weights_first")+'/')
-			image_conv_encoder_last.load_weights(str(self.siamese_path / "image_conv_encoder_weights")+'/')
-			print('Siamese model first loaded')
-			IM2_compress_c = []
-			for i in range(FIRST_COMPARISON_EXAMPLES_NUMBER):
-				IM2_compress = image_conv_encoder.predict(IM2_TOTAL_C[i])
-				IM2_compress_c.append(IM2_compress/tf.keras.backend.sqrt(tf.keras.layers.Dot(1)([IM2_compress,IM2_compress])))
-			IM2_compress_last_c = []
-			for i in range(SECOND_COMPARISON_EXAMPLES_NUMBER):
-				IM2_compress_last = image_conv_encoder.predict(IM2_LAST_C[i])
-				IM2_compress_last_c.append(IM2_compress_last/tf.keras.backend.sqrt(tf.keras.layers.Dot(1)([IM2_compress_last,IM2_compress_last])))
-
-			input_model = tf.keras.layers.Input(SIAMESE_IMAGE_SIZE)
-			x1 = image_conv_encoder(input_model)
-			x2 = image_conv_encoder_last(input_model)
-			out1 = ComparationLayer(IM2_compress_c, 0)(x1)
-			out2 = ComparationLayer(IM2_compress_last_c, 1)(x2)
-			self.model = tf.keras.Model(input_model, [out1,out2])
-
-	def predict(self, data):
-		with tf.device(self.device):
-			pred = self.model.predict(data)
-		prediction_first = list(map(self.inv_class_names_first.get, pred[0]))
-		prediction_last_comp_layer = list(map(self.class_names_last.get, prediction_first))
-		pred_class_last = list(map(lambda p_l_c_l, p: self.class_names_last_complete[p_l_c_l[np.argmax(p[:,p_l_c_l])%len(p_l_c_l)]], prediction_last_comp_layer, pred[1]))
-		return pred, prediction_first, pred_class_last
-
-class State_Signal_Model(Pav_Model):
-	
-	def __init__(self,device = None, config_file = pavimentados_path/ 'configs'  / 'state_signal_config.json', general_config_file = pavimentados_path / 'configs'	/ 'models_general.json', artifacts_path = None):
-		super().__init__(device, config_file = general_config_file)
-		self.general_config = self.config.copy()
-		self.load_config(config_file)
-		if artifacts_path:
-			self.state_signal_model_path = Path(artifacts_path) / self.config['state_signal_model_path']
-		else:
-			self.state_signal_model_path = pavimentados_path / self.general_path / self.config['state_signal_model_path']
-		self.load_model()
-	
-	def load_model(self):
-		with tf.device(self.device):
+from pavimentados.models.yolo import YoloV3
+from pavimentados.configs.utils import Config_Basic
+from pathlib import Path
+import tensorflow as tf
+import json
+import cv2
+from tqdm import tqdm
+import os
+import numpy as np
+import joblib
+
+def image_encoder(FILTERS, KERNEL, STRIDE, POOL, USE_BATCH_NORM, USE_DROPOUT, SIAMESE_IMAGE_SIZE):
+	inputs = tf.keras.layers.Input(SIAMESE_IMAGE_SIZE)
+
+	x = inputs
+	for i in range(len(FILTERS)):
+		x = tf.keras.layers.Conv2D(filters = FILTERS[i], 
+			kernel_size = KERNEL[i], strides = STRIDE[i], 
+			padding = 'same', 
+			name = 'encoder_conv_' + str(i))(x)
+
+		if USE_BATCH_NORM:
+			x = tf.keras.layers.BatchNormalization()(x)
+
+		x = tf.keras.layers.LeakyReLU()(x)
+
+		x = tf.keras.layers.MaxPooling2D(pool_size = POOL[i], padding='same')(x)
+
+		if USE_DROPOUT:
+			x = tf.keras.layers.Dropout(rate=0.25)(x)
+
+	x = tf.keras.layers.Flatten()(x)
+	output = x
+	return tf.keras.Model(inputs, output)
+
+class ComparationLayer(tf.keras.layers.Layer):
+	def __init__(self, comparison_matrix, layer_type,  **kwargs):
+		self.IM2_compress_list = comparison_matrix
+		self.layer_type = layer_type
+		super(ComparationLayer, self).__init__(**kwargs)
+
+	def build(self, input_shape):
+		self.built = True
+
+	def call(self, inputs):
+		x = inputs/tf.keras.backend.sqrt(tf.keras.layers.Dot(1)([inputs,inputs]))
+		x_l = []
+		for i in range(len(self.IM2_compress_list)):
+			x_l.append(tf.keras.backend.dot(x,tf.transpose(self.IM2_compress_list[i])))
+		if self.layer_type == 0:
+			x = tf.concat(x_l,axis=1)
+			x = tf.keras.backend.argmax(x,axis=1)
+			out = tf.math.floormod(x, 16)
+			return out
+		else:
+			out = tf.concat([tf.expand_dims(x_l[i],axis=1) for i in range(len(x_l))], axis=1)
+			return out
+	
+	def get_config(self):
+		return {'IM2_compress_c'+str(i+1): self.IM2_compress_list[i] for i in range(len(self.IM2_compress_list))}
+
+class Pav_Model(Config_Basic):
+	def __init__(self, device = '/device:CPU:0', config_file = Path('configs')  / 'models_general.json'):
+		self.load_config(config_file)
+		self.general_path = Path(self.config['general_path'])
+		self.model = None
+		self.device = device
+		
+	def predict(self,data):
+		with tf.device(self.device):
+			return self.model.predict(data)
+		
+	def load_model(self):
+		pass
+
+class Yolo_Model(Pav_Model):
+	
+	def __init__(self,device = None, config_file = Path('configs')  / 'yolo_config.json', general_config_file = Path('configs') / 'models_general.json'):
+		super().__init__(device, config_file = general_config_file)
+		self.general_config = self.config.copy()
+		self.load_config(config_file)
+		self.config['yolo_pav_dict_clases'] = {int(k):v for k,v in self.config['yolo_pav_dict_clases'].items()}
+		self.yolo_paviment_path = self.general_path / self.config['yolo_paviment_path']
+		self.yolo_signal_path = self.general_path / self.config['yolo_signal_path']
+		self.load_model()
+	
+	def load_model(self):
+		"""
+		Carga los modelos de YOLO.
+		""" 
+		with tf.device(self.device):
+
+			# Carga las clases de modelo de pavimentos.
+			classes_paviment = list({name: idx for idx, name in enumerate(open(self.yolo_paviment_path / 'classes'/'classes.names').read().splitlines())}.keys())
+			self.num_classes_paviment = len(classes_paviment)
+
+			# Carga las clases de modelo de señales,
+			classes_signal = list({name: idx for idx, name in enumerate(open(self.yolo_signal_path / 'classes'/'classes.names').read().splitlines())}.keys())
+			self.num_classes_signal = len(classes_signal)
+
+			# Une las clases de ambos modelos.
+			self.full_classes = [*classes_paviment, *classes_signal]
+
+			# Carga el path de los pesos de yolo de pavimentos y señales.
+			path_weights_paviment = self.yolo_paviment_path / 'checkpoints_model' / 'yolov3_train_8.tf'
+			path_weights_signal = self.yolo_signal_path / 'checkpoints_model' / 'yolov3_train_8.tf'
+
+			# Instancia los modelos.
+			yolo_paviment = YoloV3(classes=self.num_classes_paviment, model_name = 'yolov3_paviment')
+			yolo_signal = YoloV3(classes=self.num_classes_signal, model_name = 'yolov3_signal')
+
+			# Carga los pesos.
+			yolo_paviment.load_weights(path_weights_paviment).expect_partial()
+			yolo_signal.load_weights(path_weights_signal).expect_partial()
+
+			# Genera modelo final.
+			input_model = tf.keras.Input(shape=(416,416,3), name='image')
+			paviment_output = yolo_paviment(input_model)
+			signal_output = yolo_signal(input_model)
+			self.model = tf.keras.models.Model(input_model,[paviment_output,signal_output])
+
+class Siamese_Model(Pav_Model):
+	
+	def __init__(self,device = None, config_file = Path('configs')  / 'siamese_config.json', general_config_file = Path('configs')  / 'models_general.json'):
+		super().__init__(device, config_file = general_config_file)
+		self.general_config = self.config.copy()
+		self.load_config(config_file)
+		self.siamese_path = self.general_path / self.config['siamese_path']
+		self.load_model()
+	
+	def load_model(self):
+		"""
+		Carga los modelos de YOLO.
+		""" 
+		with tf.device(self.device):
+			FIRST_COMPARISON_EXAMPLES_NUMBER = self.config['FIRST_COMPARISON_EXAMPLES_NUMBER']
+			SECOND_COMPARISON_EXAMPLES_NUMBER = self.config['SECOND_COMPARISON_EXAMPLES_NUMBER']
+			FIRST_COMPARISON_FOLDER = self.config['FIRST_COMPARISON_FOLDER']
+			SECOND_COMPARISON_FOLDER = self.config['SECOND_COMPARISON_FOLDER']
+			
+			SIAMESE_IMAGE_SIZE = tuple(self.config['SIAMESE_IMAGE_SIZE'])
+			FILTERS = self.config['FILTERS']
+			KERNEL = self.config['KERNEL']
+			STRIDE = self.config['STRIDE']
+			POOL = self.config['POOL']
+			USE_BATCH_NORM = bool(self.config['USE_BATCH_NORM'])
+			USE_DROPOUT = bool(self.config['USE_DROPOUT'])
+			IM2_TOTAL_C = []
+			
+			for i in range(FIRST_COMPARISON_EXAMPLES_NUMBER):
+				IM2_TOTAL_C.append([])
+			
+			class_names_first = {}
+			self.class_names_last = {}
+			c = 0
+			search_path = self.siamese_path / FIRST_COMPARISON_FOLDER
+			for path in tqdm(os.listdir(search_path)):
+				class_names_first[path] = c
+				self.class_names_last[path] = []
+				c +=1
+				item_search_path = search_path / path
+				x = os.listdir(item_search_path)
+				images_files = [item_search_path / i for i in x]
+				if len(images_files)>=FIRST_COMPARISON_EXAMPLES_NUMBER:
+					for i in range(FIRST_COMPARISON_EXAMPLES_NUMBER):
+						IM2_TOTAL_C[i].append(cv2.resize(cv2.imread(str(images_files[i])), SIAMESE_IMAGE_SIZE[:2], interpolation = cv2.INTER_AREA).astype(float)/255)
+
+			for i in range(FIRST_COMPARISON_EXAMPLES_NUMBER):
+				IM2_TOTAL_C[i] = np.array(IM2_TOTAL_C[i])
+			self.inv_class_names_first = {v: k for k, v in class_names_first.items()}
+
+			dict_clases_sub = joblib.load(self.siamese_path / 'dict_senales_clases.pickle')
+			inv_dict_clases_sub = {item:k for k,v in dict_clases_sub.items() for item in v}
+			
+			IM2_LAST_C = []
+			for i in range(SECOND_COMPARISON_EXAMPLES_NUMBER):
+				IM2_LAST_C.append([])
+				
+			c = 0
+			self.class_names_last_complete = {}
+			search_path = self.siamese_path / SECOND_COMPARISON_FOLDER
+			for path in tqdm(os.listdir(search_path)):
+				if inv_dict_clases_sub.get(path, None):
+					self.class_names_last[inv_dict_clases_sub[path]].append(c)
+					self.class_names_last_complete[c] = path
+					c +=1
+					item_search_path = search_path / path
+					x = os.listdir(item_search_path)
+					images_files = [item_search_path / i for i in x]
+					if len(images_files)>=SECOND_COMPARISON_EXAMPLES_NUMBER:
+						for i in range(SECOND_COMPARISON_EXAMPLES_NUMBER):
+							IM2_LAST_C[i].append(cv2.resize(cv2.imread(str(images_files[i])), SIAMESE_IMAGE_SIZE[:2], interpolation = cv2.INTER_AREA).astype(float)/255)
+
+			for i in range(SECOND_COMPARISON_EXAMPLES_NUMBER):
+				IM2_LAST_C[i] = np.array(IM2_LAST_C[i])
+			
+			print('Createing siamese model')
+			image_conv_encoder = image_encoder(FILTERS,KERNEL,STRIDE,POOL,USE_BATCH_NORM,USE_DROPOUT, SIAMESE_IMAGE_SIZE)
+			image_conv_encoder_last = image_encoder(FILTERS,KERNEL,STRIDE,POOL,USE_BATCH_NORM,USE_DROPOUT, SIAMESE_IMAGE_SIZE)
+			print('Loading Weights siamese')
+			image_conv_encoder.load_weights(str(self.siamese_path / "image_encoder_weights_first")+'/')
+			image_conv_encoder_last.load_weights(str(self.siamese_path / "image_conv_encoder_weights")+'/')
+			print('Siamese model first loaded')
+			IM2_compress_c = []
+			for i in range(FIRST_COMPARISON_EXAMPLES_NUMBER):
+				IM2_compress = image_conv_encoder.predict(IM2_TOTAL_C[i])
+				IM2_compress_c.append(IM2_compress/tf.keras.backend.sqrt(tf.keras.layers.Dot(1)([IM2_compress,IM2_compress])))
+			IM2_compress_last_c = []
+			for i in range(SECOND_COMPARISON_EXAMPLES_NUMBER):
+				IM2_compress_last = image_conv_encoder.predict(IM2_LAST_C[i])
+				IM2_compress_last_c.append(IM2_compress_last/tf.keras.backend.sqrt(tf.keras.layers.Dot(1)([IM2_compress_last,IM2_compress_last])))
+
+			input_model = tf.keras.layers.Input(SIAMESE_IMAGE_SIZE)
+			x1 = image_conv_encoder(input_model)
+			x2 = image_conv_encoder_last(input_model)
+			out1 = ComparationLayer(IM2_compress_c, 0)(x1)
+			out2 = ComparationLayer(IM2_compress_last_c, 1)(x2)
+			self.model = tf.keras.Model(input_model, [out1,out2])
+
+	def predict(self, data):
+		with tf.device(self.device):
+			pred = self.model.predict(data)
+		prediction_first = list(map(self.inv_class_names_first.get, pred[0]))
+		prediction_last_comp_layer = list(map(self.class_names_last.get, prediction_first))
+		pred_class_last = list(map(lambda p_l_c_l, p: self.class_names_last_complete[p_l_c_l[np.argmax(p[:,p_l_c_l])%len(p_l_c_l)]], prediction_last_comp_layer, pred[1]))
+		return pred, prediction_first, pred_class_last
+
+class State_Signal_Model(Pav_Model):
+	
+	def __init__(self,device = None, config_file = Path('configs')  / 'state_signal_config.json', general_config_file = Path('configs')	/ 'models_general.json'):
+		super().__init__(device, config_file = general_config_file)
+		self.general_config = self.config.copy()
+		self.load_config(config_file)
+		self.state_signal_model_path = self.general_path / self.config['state_signal_model_path']
+		self.load_model()
+	
+	def load_model(self):
+		with tf.device(self.device):
 			self.model = tf.keras.models.load_model(self.state_signal_model_path / os.listdir(self.state_signal_model_path)[0])
```

### Comparing `pavimentados-0.29.0/pavimentados/models/yolo.py` & `pavimentados-0.9.0/pavimentados/models/yolo.py`

 * *Files identical despite different names*

### Comparing `pavimentados-0.29.0/pavimentados/processing/workflows.py` & `pavimentados-0.9.0/pavimentados/processing/workflows.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from pavimentados.analyzers.gps_sources import GPS_Data_Loader
-from pavimentados.analyzers.calculators import Results_Calculator as calculator
-from pavimentados.processing.sources import Image_Source_Loader
-
-class Workflow_Processor:
-	def __init__(self, images_input, **kwargs):
-		image_source_type = kwargs.get('image_source_type', 'image_folder')
-		gps_source_type = kwargs.get('gps_source_type', 'image_folder')
-		gps_in = kwargs.get('gps_input', images_input if gps_source_type == image_source_type else None)
-		adjust_gps = kwargs.get('adjust_gps', False)
-		gps_sections_distance = kwargs.get('gps_sections_distance', 100)
-		
-		self.img_obj = Image_Source_Loader(image_source_type, images_input)
-		self.gps_data = GPS_Data_Loader(gps_source_type, gps_in, **kwargs)
-		if adjust_gps:
-			self.gps_data.adjust_gps_data(self.img_obj.get_len())
-		self.gps_data.generate_gps_metrics(gps_sections_distance)
-		self.executed = False
-	
-	def execute_model(self, processor, batch_size = 8, video_output_file=None, image_folder_output = None):
-		self.results = processor.process_images_group(self.img_obj, batch_size = batch_size, video_output_file=video_output_file, image_folder_output = image_folder_output)
-		self.executed = True
-		
-	def process_result(self, processor, min_fotogram_distance = 5):
-		self.table_summary_sections, self.data_resulting, self.data_resulting_fails = calculator.generate_paviment_results(self.results, self.img_obj, self.gps_data, columns_to_have = self.paviment_classes_names, min_fotogram_distance = min_fotogram_distance)
-		self.signals_summary = calculator.generate_final_results_signal(self.results, self.gps_data, classes_names_yolo_signal = self.classes_names_yolo_signal)
-	
-	def get_results(self):
-		if not self.executed:
-			raise ValueError(f'Workflow not yet executed, use execute method to store the results after executing models')
-		return {
-			'table_summary_sections': self.table_summary_sections,
-			'data_resulting':self.data_resulting,
-			'data_resulting_fails':self.data_resulting_fails,
-			'signals_summary':self.signals_summary,
-			'raw_results':self.results
-		}
-	
-	def execute(self, processor, min_fotogram_distance = 5, batch_size = 8, return_results = True, video_output_file=None, image_folder_output = None):
-		self.paviment_classes_names = list(processor.processor.yolo_model.config['yolo_pav_dict_clases'].values())
-		self.execute_model(processor, batch_size = batch_size, video_output_file=video_output_file, image_folder_output = image_folder_output)
-		self.classes_names_yolo_signal = processor.processor.yolo_model.full_classes[processor.processor.yolo_model.num_classes_paviment:]
-		self.process_result(self, min_fotogram_distance = min_fotogram_distance)
-		if return_results:
-			return self.get_results()
-		
-	def adjust_results(self, min_fotogram_distance = 5, return_results = True):
-		if not self.executed:
-			raise ValueError(f'Workflow not yet executed, use execute method to store the results after executing models')
-		self.process_result(self, min_fotogram_distance = min_fotogram_distance)
-		if return_results:
+from pavimentados.analyzers.gps_sources import GPS_Data_Loader
+from pavimentados.analyzers.calculators import Results_Calculator as calculator
+from pavimentados.processing.sources import Image_Source_Loader
+
+class Workflow_Processor:
+	def __init__(self, images_input, **kwargs):
+		image_source_type = kwargs.get('image_source_type', 'image_folder')
+		gps_source_type = kwargs.get('gps_source_type', 'image_folder')
+		gps_in = kwargs.get('gps_input', images_input if gps_source_type == image_source_type else None)
+		adjust_gps = kwargs.get('adjust_gps', False)
+		gps_sections_distance = kwargs.get('gps_sections_distance', 100)
+		
+		self.img_obj = Image_Source_Loader(image_source_type, images_input)
+		self.gps_data = GPS_Data_Loader(gps_source_type, gps_in, **kwargs)
+		if adjust_gps:
+			self.gps_data.adjust_gps_data(self.img_obj.get_len())
+		self.gps_data.generate_gps_metrics(gps_sections_distance)
+		self.executed = False
+	
+	def execute_model(self, processor, batch_size = 8):
+		self.results = processor.process_images_group(self.img_obj, batch_size = batch_size)
+		self.executed = True
+		
+	def process_result(self, processor, min_fotogram_distance = 5):
+		self.table_summary_sections, self.data_resulting, self.data_resulting_fails = calculator.generate_paviment_results(self.results, self.img_obj, self.gps_data, columns_to_have = self.paviment_classes_names, min_fotogram_distance = min_fotogram_distance)
+		self.signals_summary = calculator.generate_final_results_signal(self.results, self.gps_data, classes_names_yolo_signal = self.classes_names_yolo_signal)
+	
+	def get_results(self):
+		if not self.executed:
+			raise ValueError(f'Workflow not yet executed, use execute method to store the results after executing models')
+		return {
+			'table_summary_sections': self.table_summary_sections,
+			'data_resulting':self.data_resulting,
+			'data_resulting_fails':self.data_resulting_fails,
+			'signals_summary':self.signals_summary,
+			'raw_results':self.results
+		}
+	
+	def execute(self, processor, min_fotogram_distance = 5, batch_size = 8, return_results = True):
+		self.paviment_classes_names = list(processor.processor.yolo_model.config['yolo_pav_dict_clases'].values())
+		self.execute_model(processor, batch_size = batch_size)
+		self.classes_names_yolo_signal = processor.processor.yolo_model.full_classes[processor.processor.yolo_model.num_classes_paviment:]
+		self.process_result(self, min_fotogram_distance = min_fotogram_distance)
+		if return_results:
+			return self.get_results()
+		
+	def adjust_results(self, min_fotogram_distance = 5, return_results = True):
+		if not self.executed:
+			raise ValueError(f'Workflow not yet executed, use execute method to store the results after executing models')
+		self.process_result(self, min_fotogram_distance = min_fotogram_distance)
+		if return_results:
 			return self.get_results()
```

### Comparing `pavimentados-0.29.0/pavimentados.egg-info/SOURCES.txt` & `pavimentados-0.9.0/pavimentados.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-LICENSE.md
+.gitignore
+LICENSE
 MANIFEST.in
 README.md
+requirements.txt
 setup.py
 pavimentados/__init__.py
 pavimentados/downloader.py
 pavimentados.egg-info/PKG-INFO
 pavimentados.egg-info/SOURCES.txt
 pavimentados.egg-info/dependency_links.txt
 pavimentados.egg-info/requires.txt
```

### Comparing `pavimentados-0.29.0/setup.py` & `pavimentados-0.9.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from setuptools import setup, find_packages
-import pkg_resources
-from pathlib import Path
-
-this_directory = Path(__file__).parent
-VERSION = '0.29.0'
-DESCRIPTION = 'A python package Library which implement IA algorithims to detect cracks and failures on roads. The package is wrapper around all the models and provides an interfaces to use them properly'
-
-LONG_DESCRIPTION = (this_directory / "README.md").read_text()
-
-
-with Path('requirements.txt').open() as requirements_txt:
-    install_requires = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
-
-setup(
-       # the name must match the folder name 'verysimplemodule'
-        name="pavimentados", 
-        version=VERSION,
-        author="Jose Maria Marquez Blanco",
-        author_email="jose.marquez.blanco@gmail.com",
-        description=DESCRIPTION,
-        long_description=LONG_DESCRIPTION,
-        long_description_content_type='text/markdown',
-        packages=find_packages(),
-        install_requires=install_requires,        
-        keywords=['Machine Learning', 'crack detections', 'computer vision', 'safe road'],
-        classifiers= [
-            "Development Status :: 3 - Alpha",
-            "Programming Language :: Python :: 3",
-            "Operating System :: OS Independent",
-            "Programming Language :: Python :: 3.7",    
-        ],
-        python_requires=">=3.7", 
-        include_package_data=True
+from setuptools import setup, find_packages
+import pkg_resources
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+VERSION = '0.9.0' 
+DESCRIPTION = 'A python package Library which implement IA algorithims to detect cracks and failures on roads. The package is wrapper around all the models and provides an interfaces to use them properly'
+
+LONG_DESCRIPTION = (this_directory / "README.md").read_text()
+
+
+with Path('requirements.txt').open() as requirements_txt:
+    install_requires = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
+
+setup(
+       # the name must match the folder name 'verysimplemodule'
+        name="pavimentados", 
+        version=VERSION,
+        author="Jose Maria Marquez Blanco",
+        author_email="jose.marquez.blanco@gmail.com",
+        description=DESCRIPTION,
+        long_description=LONG_DESCRIPTION,
+        long_description_content_type='text/markdown',
+        packages=find_packages(),
+        install_requires=install_requires,        
+        keywords=['Machine Learning', 'crack detections', 'computer vision', 'safe road'],
+        classifiers= [
+            "Development Status :: 3 - Alpha",
+            "Programming Language :: Python :: 3",
+            "Operating System :: OS Independent",
+            "Programming Language :: Python :: 3.7",    
+        ],
+        python_requires=">=3.7", 
+        include_package_data=True
 )
```

