# Comparing `tmp/dreifus-0.0.4.tar.gz` & `tmp/dreifus-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/dreifus/dist/.tmp-qg5rbk2a/dreifus-0.0.4.tar", last modified: Wed Mar  8 19:13:06 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/dreifus/dist/.tmp-36f1wxmx/dreifus-0.0.5.tar", last modified: Tue Apr 11 22:04:55 2023, max compression
```

## Comparing `dreifus-0.0.4.tar` & `dreifus-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-03-08 19:13:06.164531 dreifus-0.0.4/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-03-08 19:13:06.158531 dreifus-0.0.4/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       10 2023-02-13 11:32:40.000000 dreifus-0.0.4/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1088 2023-03-08 19:11:41.000000 dreifus-0.0.4/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       38 2023-03-08 19:13:06.169041 dreifus-0.0.4/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      151 2023-02-13 09:12:52.000000 dreifus-0.0.4/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-03-08 19:13:03.101004 dreifus-0.0.4/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-03-08 19:13:04.117988 dreifus-0.0.4/src/dreifus/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 08:09:12.000000 dreifus-0.0.4/src/dreifus/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5229 2023-03-07 17:38:04.000000 dreifus-0.0.4/src/dreifus/camera.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4530 2023-02-24 12:54:22.000000 dreifus-0.0.4/src/dreifus/camera_bundle.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1483 2023-02-24 11:10:52.000000 dreifus-0.0.4/src/dreifus/graphics.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-03-08 19:13:05.090412 dreifus-0.0.4/src/dreifus/matrix/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      213 2023-03-08 15:24:40.000000 dreifus-0.0.4/src/dreifus/matrix/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5852 2023-02-23 11:03:29.000000 dreifus-0.0.4/src/dreifus/matrix/intrinsics_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3655 2023-02-13 10:22:40.000000 dreifus-0.0.4/src/dreifus/matrix/intrinsics_torch.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1315 2023-02-13 11:10:42.000000 dreifus-0.0.4/src/dreifus/matrix/pose_base.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    16268 2023-03-08 15:24:39.000000 dreifus-0.0.4/src/dreifus/matrix/pose_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13757 2023-02-13 11:30:59.000000 dreifus-0.0.4/src/dreifus/matrix/pose_torch.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1329 2023-03-08 15:24:39.000000 dreifus-0.0.4/src/dreifus/matrix/transform_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8999 2023-02-23 15:00:53.000000 dreifus-0.0.4/src/dreifus/pyvista.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3367 2023-02-24 12:49:30.000000 dreifus-0.0.4/src/dreifus/trajectory.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-03-08 19:13:05.315523 dreifus-0.0.4/src/dreifus/util/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 10:08:11.000000 dreifus-0.0.4/src/dreifus/util/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      274 2023-02-13 10:10:21.000000 dreifus-0.0.4/src/dreifus/util/typing.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-03-08 19:13:05.691098 dreifus-0.0.4/src/dreifus/vector/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      219 2023-02-13 13:27:37.000000 dreifus-0.0.4/src/dreifus/vector/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2078 2023-02-13 13:27:37.000000 dreifus-0.0.4/src/dreifus/vector/vector_base.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5215 2023-02-13 09:55:06.000000 dreifus-0.0.4/src/dreifus/vector/vector_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2340 2023-02-13 09:58:17.000000 dreifus-0.0.4/src/dreifus/vector/vector_torch.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-03-08 19:13:04.407439 dreifus-0.0.4/src/dreifus.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-03-08 19:13:01.000000 dreifus-0.0.4/src/dreifus.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      873 2023-03-08 19:13:03.000000 dreifus-0.0.4/src/dreifus.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-03-08 19:13:01.000000 dreifus-0.0.4/src/dreifus.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       64 2023-03-08 19:13:01.000000 dreifus-0.0.4/src/dreifus.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        8 2023-03-08 19:13:01.000000 dreifus-0.0.4/src/dreifus.egg-info/top_level.txt
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-03-08 19:13:06.102643 dreifus-0.0.4/test/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1165 2023-02-13 14:36:25.000000 dreifus-0.0.4/test/test_camera.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1439 2023-02-13 10:23:32.000000 dreifus-0.0.4/test/test_intrinsics.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3487 2023-02-13 15:28:18.000000 dreifus-0.0.4/test/test_pose.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3677 2023-02-13 11:26:58.000000 dreifus-0.0.4/test/test_vector.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:55.000000 dreifus-0.0.5/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-04-11 22:04:55.000000 dreifus-0.0.5/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       10 2023-02-13 11:32:40.000000 dreifus-0.0.5/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1087 2023-04-11 22:01:51.000000 dreifus-0.0.5/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       38 2023-04-11 22:04:55.000000 dreifus-0.0.5/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      151 2023-02-13 09:12:52.000000 dreifus-0.0.5/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:54.000000 dreifus-0.0.5/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:54.000000 dreifus-0.0.5/src/dreifus/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 08:09:12.000000 dreifus-0.0.5/src/dreifus/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5520 2023-04-11 17:10:32.000000 dreifus-0.0.5/src/dreifus/camera.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5078 2023-04-11 17:41:05.000000 dreifus-0.0.5/src/dreifus/camera_bundle.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1483 2023-02-24 11:10:52.000000 dreifus-0.0.5/src/dreifus/graphics.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:55.000000 dreifus-0.0.5/src/dreifus/matrix/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      251 2023-04-11 16:52:12.000000 dreifus-0.0.5/src/dreifus/matrix/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5852 2023-02-23 11:03:29.000000 dreifus-0.0.5/src/dreifus/matrix/intrinsics_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3655 2023-02-13 10:22:40.000000 dreifus-0.0.5/src/dreifus/matrix/intrinsics_torch.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1315 2023-02-13 11:10:42.000000 dreifus-0.0.5/src/dreifus/matrix/pose_base.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    17272 2023-04-11 17:19:43.000000 dreifus-0.0.5/src/dreifus/matrix/pose_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13757 2023-02-13 11:30:59.000000 dreifus-0.0.5/src/dreifus/matrix/pose_torch.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1329 2023-03-08 15:24:39.000000 dreifus-0.0.5/src/dreifus/matrix/transform_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     9337 2023-04-11 17:36:08.000000 dreifus-0.0.5/src/dreifus/pyvista.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3367 2023-02-24 12:49:30.000000 dreifus-0.0.5/src/dreifus/trajectory.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:55.000000 dreifus-0.0.5/src/dreifus/util/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 10:08:11.000000 dreifus-0.0.5/src/dreifus/util/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      274 2023-02-13 10:10:21.000000 dreifus-0.0.5/src/dreifus/util/typing.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:55.000000 dreifus-0.0.5/src/dreifus/vector/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      219 2023-02-13 13:27:37.000000 dreifus-0.0.5/src/dreifus/vector/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2078 2023-02-13 13:27:37.000000 dreifus-0.0.5/src/dreifus/vector/vector_base.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5371 2023-04-11 15:56:31.000000 dreifus-0.0.5/src/dreifus/vector/vector_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2340 2023-02-13 09:58:17.000000 dreifus-0.0.5/src/dreifus/vector/vector_torch.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:54.000000 dreifus-0.0.5/src/dreifus.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-04-11 22:04:53.000000 dreifus-0.0.5/src/dreifus.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      873 2023-04-11 22:04:54.000000 dreifus-0.0.5/src/dreifus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-04-11 22:04:53.000000 dreifus-0.0.5/src/dreifus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       63 2023-04-11 22:04:53.000000 dreifus-0.0.5/src/dreifus.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        8 2023-04-11 22:04:53.000000 dreifus-0.0.5/src/dreifus.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:55.000000 dreifus-0.0.5/test/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1165 2023-02-13 14:36:25.000000 dreifus-0.0.5/test/test_camera.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1439 2023-02-13 10:23:32.000000 dreifus-0.0.5/test/test_intrinsics.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3487 2023-02-13 15:28:18.000000 dreifus-0.0.5/test/test_pose.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3677 2023-02-13 11:26:58.000000 dreifus-0.0.5/test/test_vector.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dreifus-0.0.4/pyproject.toml` & `dreifus-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dreifus"
-version = "0.0.4"
+version = "0.0.5"
 description = "dreifus lifts your 3D camera experience and facilitates computer vision applications"
 authors = [
     { name = "Tobias Kirschstein", email = "tobias.kirschstein@gmail.com" },
 ]
 readme = "README.md"
 license = { text = "Apache 2.0" }
 requires-python = ">=3.8.0"
@@ -18,15 +18,15 @@
     "Operating System :: OS Independent"
 ]
 #urls = { Documentation = "<<<ENTER_LINK_TO_DOCUMENTATION>>>" }
 # Main dependencies
 dependencies = [
     "opencv-python>=4.6",
     "numpy",
-    "scipy>=1.10",
+    "scipy>=1.9",
     "torch",
     "pyvista>=0.38"
 ]
 
 [project.optional-dependencies]
 # Development packages, install via dreifus[dev]
 dev = [
```

### Comparing `dreifus-0.0.4/src/dreifus/camera.py` & `dreifus-0.0.5/src/dreifus/camera.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import math
 from enum import Enum, auto
 
+import numpy as np
+
 from dreifus.vector import Vec3
 
 
 class AxisDirection(Enum):
     X = (1, 0, 0)
     NEG_X = (-1, 0, 0)
 
     Y = (0, 1, 0)
     NEG_Y = (0, -1, 0)
 
     Z = (0, 0, 1)
     NEG_Z = (0, 0, -1)
 
     def __init__(self, x: int, y: int, z: int):
+        assert sum([x == 0, y == 0, z == 0]) == 2, "Exactly two coordinates have to be zero"
+        assert sum([abs(x) == 1, abs(y) == 1, abs(z) == 1]) == 1, "Exactly one coordinate has to be 1 or -1"
+
         self.axis = Vec3(x, y, z)
+        self.axis_id = np.abs(np.array([x, y, z])).argmax()
+
 
     def sign(self) -> int:
         return self.axis.sum()
 
     def axis_name(self) -> str:
         if '_' in self.name:
             axis_name = self.name.split('_')[1]
```

### Comparing `dreifus-0.0.4/src/dreifus/camera_bundle.py` & `dreifus-0.0.5/src/dreifus/camera_bundle.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,31 +4,44 @@
 from dreifus.camera import PoseType
 
 from dreifus.matrix import Pose
 from dreifus.vector import Vec3, rotation_matrix_between_vectors, offset_vector_between_line_and_point, \
     angle_between_vectors
 
 
-def calculate_look_center(cam_to_world_poses: List[Pose], distance_to_center: float) -> Vec3:
-    look_centers = []
-    for cam_to_world in cam_to_world_poses:
-        look_direction = -cam_to_world.get_look_direction()  # TODO: get_look_direction() is negated now, can we remove the minus?
-        position = cam_to_world.get_translation()
-        # TODO: This is not a very sophisticated approach
-        look_center = position + distance_to_center * look_direction
-        look_centers.append(look_center)
+def calculate_look_center(cam_to_world_poses: List[Pose]) -> Vec3:
+    a = []  # point on look-direction line (i.e., position of camera)
+    d = []  # look direction
 
-    return Vec3(np.mean(look_centers, axis=0))
+    for cam_to_world_pose in cam_to_world_poses:
+        position = cam_to_world_pose.get_translation()
+        look_direction = cam_to_world_pose.get_look_direction()
+
+        a.append(position)
+        d.append(look_direction)
+
+    # See https://stackoverflow.com/questions/48154210/3d-point-closest-to-multiple-lines-in-3d-space
+    M = np.zeros((3, 3))
+    for k in range(3):
+        ms = [d[i][k] * d[i] - (d[i].dot(d[i])) * Vec3.unit(k) for i in range(3)]
+        M[k] = sum(ms)
+
+    b = sum([d[i] * (a[i].dot(d[i])) - a[i] * (d[i].dot(d[i])) for i in range(3)])
+
+    look_center = np.linalg.solve(M, b)
+
+    return Vec3(look_center)
 
 
 def align_poses(world_to_cam_poses: List[Pose],
                 up: Optional[Vec3] = Vec3(0, 1, 0),
                 look: Optional[Vec3] = Vec3(0, 0, -1),
                 look_center: Optional[Vec3] = Vec3(0, 0, 0),
-                cam_to_world: bool = False) -> List[Pose]:
+                cam_to_world: bool = False,
+                inplace: bool = False) -> List[Pose]:
     """
     Calibration poses can be arbitrarily aligned. This method provides a utility to transform a set of camera poses
     such that their up/look directions and look center correspond to the specified values.
     calibration poses are expected in world_to_cam format and OpenCV coordinate convention
     (i.e., x -> right, y -> down, z -> forward).
     Per default, the set of camera poses will be transformed to look at the center in an OpenGL world
     (i.e., x -> right, y -> up, z -> backward).
@@ -42,14 +55,17 @@
         cam_to_world: whether the provided poses are already cam_to_world
 
     Returns
     -------
         the re-aligned camera poses
     """
 
+    if not inplace:
+        world_to_cam_poses = [pose.copy() for pose in world_to_cam_poses]
+
     if cam_to_world:
         cam_to_world_poses = world_to_cam_poses
     else:
         cam_to_world_poses = [cam_pose.invert() for cam_pose in world_to_cam_poses]
 
     # Align up direction
     if up is not None:
@@ -65,20 +81,23 @@
         average_look_direction = np.mean(look_directions, axis=0)
         align_look_rotation = rotation_matrix_between_vectors(average_look_direction, look)
         rotator_look = Pose(align_look_rotation, Vec3(), pose_type=PoseType.CAM_2_CAM)
         cam_to_world_poses = [rotator_look @ cam_pose for cam_pose in cam_to_world_poses]
 
     # Align the look center
     if look_center is not None:
-        look_directions = [cam_pose.get_look_direction() for cam_pose in cam_to_world_poses]
-        cameras_center = np.mean([cam_pose.get_translation() for cam_pose in cam_to_world_poses], axis=0)
-        average_look_direction = np.mean(look_directions, axis=0)
-        # TODO: This won't move cameras much if cameras_center is already at look_center
-        #   Would have to somehow find the point that is closest to all camera rays
-        offset_vector = offset_vector_between_line_and_point(cameras_center, average_look_direction, look_center)
+        original_look_center = calculate_look_center(cam_to_world_poses)
+        offset_vector = look_center - original_look_center
+
+        # look_directions = [cam_pose.get_look_direction() for cam_pose in cam_to_world_poses]
+        # cameras_center = np.mean([cam_pose.get_translation() for cam_pose in cam_to_world_poses], axis=0)
+        # average_look_direction = np.mean(look_directions, axis=0)
+        # # TODO: This won't move cameras much if cameras_center is already at look_center
+        # #   Would have to somehow find the point that is closest to all camera rays
+        # offset_vector = offset_vector_between_line_and_point(cameras_center, average_look_direction, look_center)
         for cam_pose in cam_to_world_poses:
             cam_pose.move(offset_vector)
 
     if up is not None:
         # Aligning the look direction might mess up the up direction again
         up_directions = [cam_pose.get_up_direction() for cam_pose in cam_to_world_poses]
         average_up_direction = np.mean(up_directions, axis=0)
```

### Comparing `dreifus-0.0.4/src/dreifus/graphics.py` & `dreifus-0.0.5/src/dreifus/graphics.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.4/src/dreifus/matrix/intrinsics_numpy.py` & `dreifus-0.0.5/src/dreifus/matrix/intrinsics_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.4/src/dreifus/matrix/intrinsics_torch.py` & `dreifus-0.0.5/src/dreifus/matrix/intrinsics_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.4/src/dreifus/matrix/pose_base.py` & `dreifus-0.0.5/src/dreifus/matrix/pose_base.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.4/src/dreifus/matrix/pose_numpy.py` & `dreifus-0.0.5/src/dreifus/matrix/pose_numpy.py`

 * *Files 7% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     def get_rodriguez_vector(self) -> Vec3:
         return Vec3(cv2.Rodrigues(self.get_rotation_matrix())[0].squeeze())
 
     def get_quaternion(self) -> Vec4:
         return Vec4(R.from_matrix(self.get_rotation_matrix()).as_quat())
 
     def get_translation(self) -> Vec3:
+        assert self.pose_type == PoseType.CAM_2_WORLD, "camera position only makes sense for CAM_2_WORLD poses"
         return Vec3(self[:3, 3])
 
     def set_translation(self, x: Vec3TypeX, y: Optional[FloatType] = None, z: Optional[FloatType] = None):
         x, y, z = unpack_3d_params(x, y, z)
         if x is not None:
             self[0, 3] = x
         if y is not None:
@@ -142,19 +143,27 @@
         euler_x, euler_y, euler_z = unpack_3d_params(euler_x, euler_y, euler_z, default=0)
         self[:3, :3] = R.from_euler(order, [euler_x, euler_y, euler_z]).as_matrix()
 
     def rotate_euler(self,
                      order: str,
                      euler_x: Vec3TypeX = 0,
                      euler_y: Optional[float] = None,
-                     euler_z: Optional[float] = None):
+                     euler_z: Optional[float] = None,
+                     inplace: bool = True) -> 'Pose':
+        if inplace:
+            pose = self
+        else:
+            pose = self.copy()
+
         euler_x, euler_y, euler_z = unpack_3d_params(euler_x, euler_y, euler_z, default=0)
         euler_rotation = Vec3(euler_x, euler_y, euler_z)
-        current_euler_angles = self.get_euler_angles(order)
-        self.set_rotation_euler(order, current_euler_angles + euler_rotation)
+        current_euler_angles = pose.get_euler_angles(order)
+        pose.set_rotation_euler(order, current_euler_angles + euler_rotation)
+
+        return pose
 
     def invert(self) -> 'Pose':
         inverted_rotation = self.get_rotation_matrix().T
         inverted_translation = -inverted_rotation @ self.get_translation()
         inverted_pose = Pose(inverted_rotation,
                              inverted_translation,
                              camera_coordinate_convention=self.camera_coordinate_convention,
@@ -175,15 +184,15 @@
         ----------
             axis: which axis to negate.
         """
 
         # negates the column of the rotation matrix
         self[:3, axis] *= -1
 
-    def swap_axes(self, permutation: List[Union[int, str]]):
+    def swap_axes(self, permutation: List[Union[int, str]], inplace: bool = True) -> 'Pose':
         """
         Negates/swaps entire rows of the pose matrix.
         Essentially, applies a rotation / flip operation around the world origin to the camera object.
         E.g., swap_axes(['-x', 'y', 'z']) will move an origin-facing camera that was at (3, 1, 1) to (-3, 1, 1).
         The moved camera will still face the origin afterwards (i.e., the camera is not just moved but also rotated).
         Alternatively, instead of flipping the camera along axis-aligned planes, swap_axes() can be interpreted as
         flipping the actual scene in world space while keeping the camera where it was.
@@ -191,14 +200,19 @@
         Assumes the current pose is cam2world
 
         Parameters
         ----------
             permutation: 3-tuple of axis indicators (either 0, 1, 2 or x, y, z with optional '-' signs)
         """
 
+        if inplace:
+            pose = self
+        else:
+            pose = self.copy()
+
         axis_switcher = np.zeros((4, 4))
         axis_order = ['x', 'y', 'z']
         for idx, a in enumerate(permutation):
             v = 1
             if isinstance(a, int):
                 ax = a
             else:
@@ -208,23 +222,29 @@
                     # Axis shall be flipped
                     v = -1
 
             axis_switcher[idx, ax] = v
         axis_switcher[3, 3] = 1
 
         # Negates / Flips rows
-        self[:, :] = axis_switcher @ self
+        pose[:, :] = axis_switcher @ pose
+
+        return pose
 
     def change_camera_coordinate_convention(self,
-                                            new_camera_coordinate_convention: CameraCoordinateConvention) -> 'Pose':
+                                            new_camera_coordinate_convention: CameraCoordinateConvention,
+                                            inplace: bool = True) -> 'Pose':
         assert self.pose_type == PoseType.CAM_2_WORLD, "Camera coordinate conventions can only be changed on CAM_2_WORLD matrices"
 
         current_ccc = self.camera_coordinate_convention
 
-        pose = self.copy()
+        if inplace:
+            pose = self
+        else:
+            pose = self.copy()
 
         if current_ccc.x_direction != new_camera_coordinate_convention.x_direction:
             pose.negate_orientation_axis(0)
 
         if current_ccc.y_direction != new_camera_coordinate_convention.y_direction:
             pose.negate_orientation_axis(1)
 
@@ -250,36 +270,44 @@
 
     def get_look_direction(self) -> 'Vec3':
         # Assumes the current pose is cam2world
         # Assigns meaning to the coordinate axes. Hence, the coordinate system convention is important
         # Assumes an OpenCV camera coordinate system convention (x -> right, y -> down, z -> forward/look)
 
         assert self.pose_type == PoseType.CAM_2_WORLD
-        look_direction = self[:3, 2]
+        forward_direction = self.camera_coordinate_convention.forward_direction
+        axis = forward_direction.axis_id
+        sign = forward_direction.sign()
+        look_direction = sign * Vec3(self[:3, axis])
 
         return look_direction
 
     def get_up_direction(self) -> 'Vec3':
         # Assumes the current pose is cam2world
         # Assigns meaning to the coordinate axes. Hence, the coordinate system convention is important
         # Assumes an OpenCV camera coordinate system convention (x -> right, y -> down, z -> forward)
 
         assert self.pose_type == PoseType.CAM_2_WORLD
-        up_direction = -self[:3, 1]
+        up_direction = self.camera_coordinate_convention.up_direction
+        axis = up_direction.axis_id
+        sign = up_direction.sign()
+
+        up_direction = sign * Vec3(self[:3, up_direction])
 
         return up_direction
 
     def look_at(self, at: Vec3, up: Vec3 = Vec3(0, 0, 1)):
         # This method assigns meaning to the coordinate axes. Hence, the coordinate system convention is important
         # We use the OpenCV camera coordinate system convention
 
         # Poses are always assumed to be cam2world
         # That way the translation part of the pose matrix is the location of the object in world space
 
         assert self.pose_type == PoseType.CAM_2_WORLD
+        assert self.camera_coordinate_convention == CameraCoordinateConvention.OPEN_CV
 
         eye = self.get_translation()
         z_axis = (at - eye).normalize()  # Assumes z-axis is forward
         x_axis = z_axis.cross(up).normalize()  # Assumes y-axis is up
         y_axis = x_axis.cross(z_axis).normalize()
 
         # Important as otherwise rotation matrix has negative determinant (would be left-handed).
```

### Comparing `dreifus-0.0.4/src/dreifus/matrix/pose_torch.py` & `dreifus-0.0.5/src/dreifus/matrix/pose_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.4/src/dreifus/matrix/transform_numpy.py` & `dreifus-0.0.5/src/dreifus/matrix/transform_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.4/src/dreifus/pyvista.py` & `dreifus-0.0.5/src/dreifus/pyvista.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,16 @@
                        intrinsics: Intrinsics,
                        img_w: Optional[float] = None,
                        img_h: Optional[float] = None,
                        image: Optional[np.ndarray] = None,
                        color='lightgray',
                        size: float = 0.3,
                        label: Optional[Union[str, int]] = None,
-                       line_width: float = 1):
+                       line_width: float = 1,
+                       look_vector_length: float = 0):
 
     if pose.pose_type == PoseType.WORLD_2_CAM:
         pose = pose.invert()
 
     pose = pose.change_camera_coordinate_convention(CameraCoordinateConvention.OPEN_CV)
 
     assert pose.pose_type == PoseType.CAM_2_WORLD
@@ -196,14 +197,20 @@
          points_world_up_triangle[[1], :3],
          points_world_up_triangle[[2], :3],
          points_world_up_triangle[[2], :3],
          points_world_up_triangle[[0], :3]], axis=0),
         width=line_width,
         color=color)
 
+    # Draw look direction line
+    if look_vector_length > 0:
+        position = pose.get_translation()
+        look_direction = pose.get_look_direction()
+        p.add_lines(np.stack([position, position + look_vector_length * look_direction]), width=line_width, color=color)
+
     if label is not None:
         p_center = center
         # (p_top_left + 0.5 * (p_bottom_right - p_top_left))[:3]
         p.add_point_labels([p_center], [label],
                            fill_shape=False, shape=None, show_points=False, text_color=color)
```

### Comparing `dreifus-0.0.4/src/dreifus/trajectory.py` & `dreifus-0.0.5/src/dreifus/trajectory.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.4/src/dreifus/vector/vector_base.py` & `dreifus-0.0.5/src/dreifus/vector/vector_base.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.4/src/dreifus/vector/vector_numpy.py` & `dreifus-0.0.5/src/dreifus/vector/vector_numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,20 @@
                 z: Optional[float] = None) -> 'Vec3':
         # TODO: Allow no arguments -> 0 vector
         vec3 = super().__new__(cls, (3,), dtype=np.float32)
         x, y, z = unpack_3d_params(x, y, z, default=0)
         vec3[:] = [x, y, z]
         return vec3
 
+    @staticmethod
+    def unit(dimension: int) -> 'Vec3':
+        unit_vector = Vec3()
+        unit_vector[dimension] = 1
+        return unit_vector
+
     @property
     def x(self) -> float:
         return self[0]
 
     @property
     def y(self) -> float:
         return self[1]
```

### Comparing `dreifus-0.0.4/src/dreifus/vector/vector_torch.py` & `dreifus-0.0.5/src/dreifus/vector/vector_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.4/src/dreifus.egg-info/SOURCES.txt` & `dreifus-0.0.5/src/dreifus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.4/test/test_camera.py` & `dreifus-0.0.5/test/test_camera.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.4/test/test_intrinsics.py` & `dreifus-0.0.5/test/test_intrinsics.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.4/test/test_pose.py` & `dreifus-0.0.5/test/test_pose.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.4/test/test_vector.py` & `dreifus-0.0.5/test/test_vector.py`

 * *Files identical despite different names*

