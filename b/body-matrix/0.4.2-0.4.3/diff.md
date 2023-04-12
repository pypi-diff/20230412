# Comparing `tmp/body_matrix-0.4.2.tar.gz` & `tmp/body_matrix-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/troydo42/Desktop/Body_Matrix/dist/.tmp-664coy90/body_matrix-0.4.2.tar", last modified: Thu Mar 30 10:53:43 2023, max compression
+gzip compressed data, was "/Users/troydo42/Desktop/Body_Matrix/dist/.tmp-3dazmxqk/body_matrix-0.4.3.tar", last modified: Wed Apr 12 04:06:52 2023, max compression
```

## Comparing `body_matrix-0.4.2.tar` & `body_matrix-0.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-03-30 10:53:43.000000 body_matrix-0.4.2/
--rw-r--r--   0 troydo42   (501) staff       (20)     1069 2023-01-16 08:57:57.000000 body_matrix-0.4.2/LICENSE
--rw-r--r--   0 troydo42   (501) staff       (20)     2696 2023-03-30 10:53:43.000000 body_matrix-0.4.2/PKG-INFO
--rw-r--r--   0 troydo42   (501) staff       (20)     2170 2023-03-30 07:26:33.000000 body_matrix-0.4.2/README.md
--rw-r--r--   0 troydo42   (501) staff       (20)      631 2023-03-30 10:52:55.000000 body_matrix-0.4.2/pyproject.toml
--rw-r--r--   0 troydo42   (501) staff       (20)       38 2023-03-30 10:53:43.000000 body_matrix-0.4.2/setup.cfg
-drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-03-30 10:53:43.000000 body_matrix-0.4.2/src/
-drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-03-30 10:53:43.000000 body_matrix-0.4.2/src/body_matrix/
--rw-r--r--   0 troydo42   (501) staff       (20)        0 2023-01-16 08:47:57.000000 body_matrix-0.4.2/src/body_matrix/__init__.py
--rw-r--r--   0 troydo42   (501) staff       (20)     7889 2023-03-30 08:20:13.000000 body_matrix-0.4.2/src/body_matrix/draw.py
--rw-r--r--   0 troydo42   (501) staff       (20)     5109 2023-03-30 10:50:19.000000 body_matrix-0.4.2/src/body_matrix/export.py
--rw-r--r--   0 troydo42   (501) staff       (20)     4474 2023-02-13 04:33:58.000000 body_matrix-0.4.2/src/body_matrix/infer.py
--rw-r--r--   0 troydo42   (501) staff       (20)     1753 2023-02-24 03:48:47.000000 body_matrix-0.4.2/src/body_matrix/load.py
--rw-r--r--   0 troydo42   (501) staff       (20)     6395 2023-03-30 07:40:07.000000 body_matrix-0.4.2/src/body_matrix/measure.py
--rw-r--r--   0 troydo42   (501) staff       (20)     8415 2023-03-30 10:51:29.000000 body_matrix-0.4.2/src/body_matrix/process.py
--rw-r--r--   0 troydo42   (501) staff       (20)     6744 2023-02-22 04:35:41.000000 body_matrix-0.4.2/src/body_matrix/score.py
-drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-03-30 10:53:43.000000 body_matrix-0.4.2/src/body_matrix.egg-info/
--rw-r--r--   0 troydo42   (501) staff       (20)     2696 2023-03-30 10:53:43.000000 body_matrix-0.4.2/src/body_matrix.egg-info/PKG-INFO
--rw-r--r--   0 troydo42   (501) staff       (20)      394 2023-03-30 10:53:43.000000 body_matrix-0.4.2/src/body_matrix.egg-info/SOURCES.txt
--rw-r--r--   0 troydo42   (501) staff       (20)        1 2023-03-30 10:53:43.000000 body_matrix-0.4.2/src/body_matrix.egg-info/dependency_links.txt
--rw-r--r--   0 troydo42   (501) staff       (20)       19 2023-03-30 10:53:43.000000 body_matrix-0.4.2/src/body_matrix.egg-info/top_level.txt
+drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-04-12 04:06:52.000000 body_matrix-0.4.3/
+-rw-r--r--   0 troydo42   (501) staff       (20)     1069 2023-01-16 08:57:57.000000 body_matrix-0.4.3/LICENSE
+-rw-r--r--   0 troydo42   (501) staff       (20)     2696 2023-04-12 04:06:52.000000 body_matrix-0.4.3/PKG-INFO
+-rw-r--r--   0 troydo42   (501) staff       (20)     2170 2023-03-30 07:26:33.000000 body_matrix-0.4.3/README.md
+-rw-r--r--   0 troydo42   (501) staff       (20)      631 2023-04-12 04:05:52.000000 body_matrix-0.4.3/pyproject.toml
+-rw-r--r--   0 troydo42   (501) staff       (20)       38 2023-04-12 04:06:52.000000 body_matrix-0.4.3/setup.cfg
+drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-04-12 04:06:52.000000 body_matrix-0.4.3/src/
+drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-04-12 04:06:52.000000 body_matrix-0.4.3/src/body_matrix/
+-rw-r--r--   0 troydo42   (501) staff       (20)        0 2023-01-16 08:47:57.000000 body_matrix-0.4.3/src/body_matrix/__init__.py
+-rw-r--r--   0 troydo42   (501) staff       (20)     7892 2023-04-12 03:59:49.000000 body_matrix-0.4.3/src/body_matrix/draw.py
+-rw-r--r--   0 troydo42   (501) staff       (20)     5111 2023-04-12 03:58:06.000000 body_matrix-0.4.3/src/body_matrix/export.py
+-rw-r--r--   0 troydo42   (501) staff       (20)     4488 2023-04-12 03:59:25.000000 body_matrix-0.4.3/src/body_matrix/infer.py
+-rw-r--r--   0 troydo42   (501) staff       (20)     1753 2023-02-24 03:48:47.000000 body_matrix-0.4.3/src/body_matrix/load.py
+-rw-r--r--   0 troydo42   (501) staff       (20)     6397 2023-04-12 04:00:23.000000 body_matrix-0.4.3/src/body_matrix/measure.py
+-rw-r--r--   0 troydo42   (501) staff       (20)     8453 2023-04-12 04:01:05.000000 body_matrix-0.4.3/src/body_matrix/process.py
+-rw-r--r--   0 troydo42   (501) staff       (20)     6748 2023-04-12 04:02:27.000000 body_matrix-0.4.3/src/body_matrix/score.py
+drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-04-12 04:06:52.000000 body_matrix-0.4.3/src/body_matrix.egg-info/
+-rw-r--r--   0 troydo42   (501) staff       (20)     2696 2023-04-12 04:06:51.000000 body_matrix-0.4.3/src/body_matrix.egg-info/PKG-INFO
+-rw-r--r--   0 troydo42   (501) staff       (20)      394 2023-04-12 04:06:52.000000 body_matrix-0.4.3/src/body_matrix.egg-info/SOURCES.txt
+-rw-r--r--   0 troydo42   (501) staff       (20)        1 2023-04-12 04:06:51.000000 body_matrix-0.4.3/src/body_matrix.egg-info/dependency_links.txt
+-rw-r--r--   0 troydo42   (501) staff       (20)       19 2023-04-12 04:06:51.000000 body_matrix-0.4.3/src/body_matrix.egg-info/top_level.txt
```

### Comparing `body_matrix-0.4.2/LICENSE` & `body_matrix-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `body_matrix-0.4.2/PKG-INFO` & `body_matrix-0.4.3/src/body_matrix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: body_matrix
-Version: 0.4.2
+Name: body-matrix
+Version: 0.4.3
 Summary: Package to Calculate Human Body Measurements
 Author-email: Hoang Do <hoang.do.2102@gmail.com>
 Project-URL: Homepage, https://github.com/akando42/body_matrix
 Project-URL: Bug Tracker, https://github.com/akando42/body_matrix/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `body_matrix-0.4.2/README.md` & `body_matrix-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `body_matrix-0.4.2/pyproject.toml` & `body_matrix-0.4.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "av>=8.0", "torchvision>=0.13"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "body_matrix"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="Hoang Do", email="hoang.do.2102@gmail.com" },
 ]
 description = "Package to Calculate Human Body Measurements"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `body_matrix-0.4.2/src/body_matrix/draw.py` & `body_matrix-0.4.3/src/body_matrix/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 	sample = image.copy()
 	draw = ImageDraw.Draw(sample) 
 			
 	for index, point in enumerate(coordinates.values()):
 		label = str(index) 
 		radius = 6
 
-		print(point)
+		#print(point)
 
 		draw.ellipse(
 			[(point[0]-radius, point[1]-radius), (point[0]+radius, point[1]+radius)],
 			fill="#40389F",
 			outline="#ffffff",
 			width=1
 		)
@@ -268,15 +268,15 @@
 		fill="#FFFFFF",
 	)
 	text_anchor = (
 		lh[0] + int(hip_width/3),
 		middle_hip[1] + int(hip_width/30)
 	)
 
-	print(int(hip_width/20))
+	# print(int(hip_width/20))
 
 	draw.text(
 		text_anchor,
 		str(score), 
 		fill="#1C3D90",
 	    font=font,
 	    align="center"
```

### Comparing `body_matrix-0.4.2/src/body_matrix/export.py` & `body_matrix-0.4.3/src/body_matrix/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 		frame = av.VideoFrame.from_image(image)
 		for packet in stream.encode(frame):
 			container.mux(packet)
 			
 	def slow_motion_reverse(pil_images):
 		frames_count = len(pil_images)
 		total_frames = frames_count * 2 * repeat_rate
-		print("Total Frames is ", total_frames)
+		# print("Total Frames is ", total_frames)
 		
 		for idx in range(total_frames):
 			local_index = idx%len(pil_images)
 			play_times = int(idx/len(pil_images))
 		
 			if play_times % 2 == 0 and play_times < (repeat_rate * 2 - 1):
 				frame_index = local_index
```

### Comparing `body_matrix-0.4.2/src/body_matrix/infer.py` & `body_matrix-0.4.3/src/body_matrix/infer.py`

 * *Files 23% similar despite different names*

```diff
@@ -64,22 +64,22 @@
         distance, area = measure.distance_from_vertical_line(frame, bbox) 
         
         focuses.append(area/distance)
         distances.append(distance)
         areas.append(area)
         bboxes.append(bbox)
 
-    print("Distances: ",distances)
-    print("Areas: ", areas)
-    print("FOCUSES: ", focuses)
+    # print("Distances: ",distances)
+    # print("Areas: ", areas)
+    # print("FOCUSES: ", focuses)
 
     distance_score, distance_index = score.find_nearest(distances, 0)
     focus_score, focus_index = score.find_largest(focuses, 0)
     
-    print("Select keypoint index", focus_index)
+    # print("Select keypoint index", focus_index)
     selected_bbox = bboxes[focus_index] 
     selected_keypoints = torch.squeeze(keypoints[idx][focus_index], dim=0)
     # SHApoints = getSHAPositions(kp)
     # labels = ["ls","rs","lw", "rw", "lh","rh","la","ra"]
     # points_image = drawMarkers(labels, SHApoints, frame)
     return selected_bbox, selected_keypoints
 
@@ -92,32 +92,32 @@
     predictions = segment_model([input_image.to(device)])
     masks = predictions[0]['masks']
     scores = predictions[0]['scores']
     boxes = predictions[0]['boxes']
     idx = torch.where(scores > segment_min_accuracy)
     main_boxes = torch.unsqueeze(boxes[idx], dim=1)
 
-    print("Found ", len(main_boxes), " person in the frame")
+    # print("Found ", len(main_boxes), " person in the frame")
     # index = len(main_boxes) - 1
     
     distances = []
     for selector, box in enumerate(main_boxes):
         bbox = [
             box[0][0].item(), 
             box[0][1].item(),
             box[0][2].item(),
             box[0][3].item()
         ]
         
         distance_from_selected = measure.two_boxes_distance(bbox, selected_bbox)
         distances.append(distance_from_selected)
             
-    print(distances)
+    # print(distances)
     distance, index = score.find_nearest(distances, 0)
-    print(distance, index)
+    # print(distance, index)
     
     mask = torch.squeeze(masks[index][0], dim=1)
     mask_image = to_pil_image(mask)
     
     ### Find the Minimum Pixel Threshold for Mask
     numpy_mask = mask.detach().cpu().numpy()
     counts, values = np.histogram(numpy_mask, bins=10)
```

### Comparing `body_matrix-0.4.2/src/body_matrix/load.py` & `body_matrix-0.4.3/src/body_matrix/load.py`

 * *Files identical despite different names*

### Comparing `body_matrix-0.4.2/src/body_matrix/measure.py` & `body_matrix-0.4.3/src/body_matrix/measure.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     center_y = (bbox[3] + bbox[1])/2
     center = [center_x, center_y]
     return center
 
 
 ### Two_Boxes_Distance
 def two_boxes_distance(bbox1, bbox2):
-    print(bbox1)
-    print(bbox2)
+    #print(bbox1)
+    #print(bbox2)
     bbox1_center = box_center_coordinate(bbox1)
     bbox2_center = box_center_coordinate(bbox2)
     x_dif = bbox1_center[0] - bbox2_center[0]
     y_dif = bbox1_center[1] - bbox2_center[1]
     
     distance = math.sqrt(x_dif * x_dif + y_dif * y_dif)
     return distance
```

### Comparing `body_matrix-0.4.2/src/body_matrix/process.py` & `body_matrix-0.4.3/src/body_matrix/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,60 +160,60 @@
 
 	if rw[1] < rh[1] and lw[1] < lh[1]:
 		hip_kps = {
 			'left_hip': hip_line_coordinates[0],
 			'right_hip': hip_line_coordinates[-1]
 		}
 
-		print(
-			"both hand high", hip_kps,
-			"\nLeft: ", lw, lh, 
-			"\nRight: ", rw, rh
-		)
+		# print(
+		# 	"both hand high", hip_kps,
+		# 	"\nLeft: ", lw, lh, 
+		# 	"\nRight: ", rw, rh
+		# )
 		return hip_kps
 
 	elif rw[1] > rh[1] and lw[1] > lh[1]:
 		hip_kps = {}
-		print(
-			"both hand low", hip_kps,
-			"\nLeft hand: ", lw[1], lh[1], 
-			"\nRight: ", rw[1], rh[1]
-		)
+		# print(
+		# 	"both hand low", hip_kps,
+		# 	"\nLeft hand: ", lw[1], lh[1], 
+		# 	"\nRight: ", rw[1], rh[1]
+		# )
 
 	elif int(lw[1]) >= int(lw[0] * hip_alpha + hip_beta)*0.9:
 		precise_rh = hip_line_coordinates[-1]
 		precise_lhX = 2 * middle_hip[0] - rh[0]
 		precise_lhY = hip_alpha * precise_lhX + hip_beta
 		precise_lh = [int(precise_lhX), int(precise_lhY)]
 		hip_kps = {
 			'left_hip': precise_lh,
 			'right_hip': precise_rh
 		}
-		print(
-			"low left hand", hip_kps, 
-			"\n Left Wrist", lw,
-			"\n Left Hip: ", lh)
+		# print(
+		# 	"low left hand", hip_kps, 
+		# 	"\n Left Wrist", lw,
+		# 	"\n Left Hip: ", lh)
 		return hip_kps
 		
 		
 	elif int(rw[1]) >= int(rw[0] * hip_alpha + hip_beta)*0.9:
 		precise_lh = hip_line_coordinates[0]
 		precise_rhX = 2 * middle_hip[0] - precise_lh[0]
 		precise_rhY = hip_alpha * precise_rhX + hip_beta
 		precise_rh = [int(precise_rhX), int(precise_rhY)] 
 		
 		hip_kps = {
 			'left_hip': precise_lh,
 			'right_hip': precise_rh
 		}
-		print(
-			"low right hand", hip_kps,
-			"\n Right Wrist: ", rw,
-			"\n Right Hip: ", rh
-		)
+		# print(
+		# 	"low right hand", hip_kps,
+		# 	"\n Right Wrist: ", rw,
+		# 	"\n Right Hip: ", rh
+		# )
 		return hip_kps
 
 
 # Find Hip Points with Segmentation Area
 def find_hip_points(lh, rh, lw, rw, segment_area):
 	lhX = lh[0]
 	lhY = lh[1]
```

### Comparing `body_matrix-0.4.2/src/body_matrix/score.py` & `body_matrix-0.4.3/src/body_matrix/score.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             
     np_scores = np.array(scores)
     mean = np.mean(np_scores)
     median = np.median(np_scores)
     minim = np.min(np_scores)
     maxim = np.max(np_scores)
     histogram_scores = np.histogram(np_scores)
-    print(mean, median)
+    #print(mean, median)
     sns.distplot(np_scores, hist=True)
     
     return mean, median, minim, maxim
 
 
 def SHA_score(ls, rs, lh, rh, la, ra):
     sL = measure.two_points_distance(ls, rs)
@@ -100,15 +100,15 @@
     shoulder_kps = process.find_shoulder_points(
         selected_kps['left_shoulder'], 
         selected_kps['right_shoulder'],
         segment_area
     )
 
     if hip_kps == None or shoulder_kps == None:
-        print("KEYPOINT ERRORS")
+        #print("KEYPOINT ERRORS")
         return None
     
     main_points = {}
     main_points.update(hip_kps)
     main_points.update(shoulder_kps)
     main_points.update(
         {
@@ -177,15 +177,15 @@
         shoulder_kps = process.find_shoulder_points(
             selected_kps['left_shoulder'], 
             selected_kps['right_shoulder'],
             segment_area
         )
 
         if hip_kps == None or shoulder_kps == None:
-            print("KEYPOINT ERRORS")
+            #print("KEYPOINT ERRORS")
             continue
         
         main_points = {}
         main_points.update(hip_kps)
         main_points.update(shoulder_kps)
         main_points.update(
             {
@@ -197,15 +197,15 @@
         middle_hip = measure.find_middle_point(
             main_points['left_hip'],
             main_points['right_hip']
         )
 
         float_labeled_frame = image
         for key, value in main_points.items():
-            print(key, value)
+            #print(key, value)
             float_labeled_frame = draw.floating_rectangle_label(
                 image = float_labeled_frame, 
                 longitude_coordinate = middle_hip[0], 
                 point=value, 
                 label_text=key, 
                 label_size=16, 
                 label_color="#ffffff",
```

### Comparing `body_matrix-0.4.2/src/body_matrix.egg-info/PKG-INFO` & `body_matrix-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: body-matrix
-Version: 0.4.2
+Name: body_matrix
+Version: 0.4.3
 Summary: Package to Calculate Human Body Measurements
 Author-email: Hoang Do <hoang.do.2102@gmail.com>
 Project-URL: Homepage, https://github.com/akando42/body_matrix
 Project-URL: Bug Tracker, https://github.com/akando42/body_matrix/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

