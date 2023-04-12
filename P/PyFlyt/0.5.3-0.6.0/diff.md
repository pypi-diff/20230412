# Comparing `tmp/PyFlyt-0.5.3.tar.gz` & `tmp/PyFlyt-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.5.3.tar", last modified: Sun Apr  2 17:07:15 2023, max compression
+gzip compressed data, was "PyFlyt-0.6.0.tar", last modified: Wed Apr 12 14:05:24 2023, max compression
```

## Comparing `PyFlyt-0.5.3.tar` & `PyFlyt-0.6.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.5.3/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     8840 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/PKG-INFO
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.927697 PyFlyt-0.5.3/PyFlyt/
--rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.5.3/PyFlyt/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.927697 PyFlyt-0.5.3/PyFlyt/core/
--rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.5.3/PyFlyt/core/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/PyFlyt/core/abstractions/
--rw-rw-r--   0 jet       (1000) jet       (1000)      312 2023-03-08 14:09:51.000000 PyFlyt-0.5.3/PyFlyt/core/abstractions/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      587 2023-03-08 14:09:51.000000 PyFlyt-0.5.3/PyFlyt/core/abstractions/base_controller.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5063 2023-03-10 16:25:31.000000 PyFlyt-0.5.3/PyFlyt/core/abstractions/base_drone.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     8371 2023-03-24 01:31:39.000000 PyFlyt-0.5.3/PyFlyt/core/abstractions/boosters.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     3095 2023-04-01 23:29:12.000000 PyFlyt-0.5.3/PyFlyt/core/abstractions/boring_bodies.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4909 2023-03-08 21:51:29.000000 PyFlyt-0.5.3/PyFlyt/core/abstractions/camera.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5937 2023-03-08 17:00:02.000000 PyFlyt-0.5.3/PyFlyt/core/abstractions/gimbals.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12966 2023-03-25 23:40:03.000000 PyFlyt-0.5.3/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4464 2023-03-06 21:49:03.000000 PyFlyt-0.5.3/PyFlyt/core/abstractions/motors.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.5.3/PyFlyt/core/abstractions/pid.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12589 2023-04-02 16:44:52.000000 PyFlyt-0.5.3/PyFlyt/core/aviary.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/PyFlyt/core/drones/
--rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-03-06 21:31:59.000000 PyFlyt-0.5.3/PyFlyt/core/drones/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9722 2023-03-10 16:25:31.000000 PyFlyt-0.5.3/PyFlyt/core/drones/fixedwing.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    18152 2023-03-10 23:03:47.000000 PyFlyt-0.5.3/PyFlyt/core/drones/quadx.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11760 2023-04-01 22:36:15.000000 PyFlyt-0.5.3/PyFlyt/core/drones/rocket.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-01 18:23:35.000000 PyFlyt-0.5.3/PyFlyt/core/load_objs.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/PyFlyt/gym_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.5.3/PyFlyt/gym_envs/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/PyFlyt/gym_envs/fixedwing_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9213 2023-04-01 11:12:42.000000 PyFlyt-0.5.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5510 2023-03-14 20:29:10.000000 PyFlyt-0.5.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/PyFlyt/gym_envs/quadx_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8947 2023-04-01 11:10:58.000000 PyFlyt-0.5.3/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.5.3/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     3531 2023-03-13 17:50:16.000000 PyFlyt-0.5.3/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5733 2023-03-15 21:27:33.000000 PyFlyt-0.5.3/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/PyFlyt/gym_envs/rocket_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)    11588 2023-04-01 23:23:38.000000 PyFlyt-0.5.3/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7959 2023-04-02 00:34:42.000000 PyFlyt-0.5.3/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6312 2023-03-01 18:18:28.000000 PyFlyt-0.5.3/PyFlyt/gym_envs/waypoint_handler.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/PyFlyt/models/
--rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.5.3/PyFlyt/models/landing_pad.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.5.3/PyFlyt/models/race_gate.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.5.3/PyFlyt/models/target.urdf
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.927697 PyFlyt-0.5.3/PyFlyt/models/vehicles/
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/PyFlyt/models/vehicles/cf2x/
--rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.5.3/PyFlyt/models/vehicles/cf2x/cf2.dae
--rw-rw-r--   0 jet       (1000) jet       (1000)     2580 2023-03-10 23:54:13.000000 PyFlyt-0.5.3/PyFlyt/models/vehicles/cf2x/cf2x.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1241 2023-03-10 22:05:19.000000 PyFlyt-0.5.3/PyFlyt/models/vehicles/cf2x/cf2x.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/PyFlyt/models/vehicles/fixedwing/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.5.3/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.5.3/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/PyFlyt/models/vehicles/primitive_drone/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3501 2023-03-10 23:52:15.000000 PyFlyt-0.5.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1238 2023-03-10 23:21:42.000000 PyFlyt-0.5.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/PyFlyt/models/vehicles/quadplane/
--rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.5.3/PyFlyt/models/vehicles/quadplane/quadplane.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.5.3/PyFlyt/models/vehicles/quadplane/quadplane.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/PyFlyt/models/vehicles/rocket/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 00:35:05.000000 PyFlyt-0.5.3/PyFlyt/models/vehicles/rocket/rocket.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-01 23:53:56.000000 PyFlyt-0.5.3/PyFlyt/models/vehicles/rocket/rocket.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.927697 PyFlyt-0.5.3/PyFlyt.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8840 2023-04-02 17:07:15.000000 PyFlyt-0.5.3/PyFlyt.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)     1895 2023-04-02 17:07:15.000000 PyFlyt-0.5.3/PyFlyt.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-04-02 17:07:15.000000 PyFlyt-0.5.3/PyFlyt.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       57 2023-04-02 17:07:15.000000 PyFlyt-0.5.3/PyFlyt.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-04-02 17:07:15.000000 PyFlyt-0.5.3/PyFlyt.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     1184 2023-04-02 16:50:59.000000 PyFlyt-0.5.3/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)     7023 2023-03-27 13:11:45.000000 PyFlyt-0.5.3/readme.md
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.5.3/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-02 17:07:15.931697 PyFlyt-0.5.3/tests/
--rw-rw-r--   0 jet       (1000) jet       (1000)     6511 2023-04-01 11:12:22.000000 PyFlyt-0.5.3/tests/test_core.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-03-15 18:01:34.000000 PyFlyt-0.5.3/tests/test_gym_envs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.6.0/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8851 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PKG-INFO
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.218394 PyFlyt-0.6.0/PyFlyt/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.6.0/PyFlyt/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.218394 PyFlyt-0.6.0/PyFlyt/core/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.6.0/PyFlyt/core/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/core/abstractions/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      352 2023-04-07 22:21:54.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-04-11 22:38:25.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/base_controller.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7626 2023-04-12 13:36:46.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/base_drone.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11784 2023-04-12 01:16:04.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/boosters.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4211 2023-04-12 01:15:08.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/boring_bodies.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7686 2023-04-12 01:27:48.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/camera.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6365 2023-04-11 23:16:18.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/gimbals.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12428 2023-04-12 01:36:15.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4651 2023-04-11 23:13:32.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/motors.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.6.0/PyFlyt/core/abstractions/pid.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15163 2023-04-12 14:05:07.000000 PyFlyt-0.6.0/PyFlyt/core/aviary.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/core/drones/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.6.0/PyFlyt/core/drones/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9602 2023-04-12 13:37:24.000000 PyFlyt-0.6.0/PyFlyt/core/drones/fixedwing.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    18116 2023-04-12 13:37:02.000000 PyFlyt-0.6.0/PyFlyt/core/drones/quadx.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11668 2023-04-12 13:37:20.000000 PyFlyt-0.6.0/PyFlyt/core/drones/rocket.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-01 18:23:35.000000 PyFlyt-0.6.0/PyFlyt/core/load_objs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/gym_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/gym_envs/fixedwing_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5510 2023-04-07 22:18:42.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3531 2023-03-13 17:50:16.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5733 2023-04-07 22:18:54.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/gym_envs/rocket_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8772 2023-04-12 13:57:31.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.6.0/PyFlyt/gym_envs/waypoint_handler.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/models/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.6.0/PyFlyt/models/landing_pad.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.6.0/PyFlyt/models/race_gate.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.6.0/PyFlyt/models/target.urdf
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.218394 PyFlyt-0.6.0/PyFlyt/models/vehicles/
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/models/vehicles/cf2x/
+-rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/cf2x/cf2.dae
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2580 2023-03-10 23:54:13.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/cf2x/cf2x.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1241 2023-03-10 22:05:19.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/cf2x/cf2x.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/models/vehicles/fixedwing/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/models/vehicles/primitive_drone/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3501 2023-03-10 23:52:15.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1238 2023-03-10 23:21:42.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/models/vehicles/quadplane/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/quadplane/quadplane.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/quadplane/quadplane.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/PyFlyt/models/vehicles/rocket/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/rocket/rocket.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-02 23:08:08.000000 PyFlyt-0.6.0/PyFlyt/models/vehicles/rocket/rocket.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.218394 PyFlyt-0.6.0/PyFlyt.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8851 2023-04-12 14:05:24.000000 PyFlyt-0.6.0/PyFlyt.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1895 2023-04-12 14:05:24.000000 PyFlyt-0.6.0/PyFlyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-04-12 14:05:24.000000 PyFlyt-0.6.0/PyFlyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       57 2023-04-12 14:05:24.000000 PyFlyt-0.6.0/PyFlyt.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-04-12 14:05:24.000000 PyFlyt-0.6.0/PyFlyt.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1184 2023-04-12 14:05:16.000000 PyFlyt-0.6.0/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7034 2023-04-08 01:06:54.000000 PyFlyt-0.6.0/readme.md
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.6.0/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-12 14:05:24.222394 PyFlyt-0.6.0/tests/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6511 2023-04-01 11:12:22.000000 PyFlyt-0.6.0/tests/test_core.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-04-12 01:51:05.000000 PyFlyt-0.6.0/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.5.3/LICENSE.txt` & `PyFlyt-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PKG-INFO` & `PyFlyt-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.5.3
+Version: 0.6.0
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -37,16 +37,18 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![hits](https://hits.dwyl.com/jjshoots/PyFlyt.svg)](https://hits.dwyl.com/jjshoots/PyFlyt)
 [![total downloads](https://static.pepy.tech/personalized-badge/pyflyt?period=total&units=international_system&left_color=grey&right_color=green&left_text=total%20downloads)](https://pepy.tech/project/pyflyt)
 [![weekly downloads](https://static.pepy.tech/personalized-badge/pyflyt?period=week&units=international_system&left_color=grey&right_color=green&left_text=weekly%20downloads)](https://pepy.tech/project/pyflyt)
 
 # PyFlyt - UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research
 
+## [View the documentation here!](https://jjshoots.github.io/PyFlyt/documentation.html)
+
 <p align="center">
-    <img src="https://github.com/jjshoots/PyFlyt/blob/master/readme_assets/pyflyt_cover_photo.png?raw=true" width="800px"/>
+    <img src="https://github.com/jjshoots/PyFlyt/blob/master/readme_assets/pyflyt_cover_photo.png?raw=true" width="650px"/>
 </p>
 
 This is a library for testing reinforcement learning algorithms on UAVs.
 This repo is still under development.
 We are also actively looking for users and developers, if this sounds like you, don't hesitate to get in touch!
 
 PyFlyt currently supports two separate UAV platforms:
@@ -84,25 +86,23 @@
 
 ## Usage
 
 Usage is similar to any other Gymnasium and (soon) PettingZoo environment:
 
 ```py
 import gymnasium
-import PyFlyt.gym_envs
-
-env = gymnasium.make("PyFlyt/QuadX-Hover-v0")
+import PyFlyt.gym_envs # noqa
 
-# omit the below line to remove rendering and let the simulation go as fast as possible
-env.render()
+env = gymnasium.make("PyFlyt/QuadX-Hover-v0", render_mode="human")
 obs = env.reset()
 
 termination = False
 truncation = False
-while not termination and not truncation:
+
+while not termination or truncation:
     observation, reward, termination, truncation, info = env.step(env.action_space.sample())
 ```
 
 ## Environments
 
 ### `PyFlyt/QuadX-Hover-v0`
```

### Comparing `PyFlyt-0.5.3/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.6.0/PyFlyt/core/abstractions/base_controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     @abstractmethod
     def reset(self):
         """Reset the internal state of the controller."""
         pass
 
     @abstractmethod
-    def step(self, state: np.ndarray, setpoint: np.ndarray):
+    def step(self, state: np.ndarray, setpoint: np.ndarray) -> np.ndarray:
         """Step the controller.
 
         Args:
             state (np.ndarray): state
             setpoint (np.ndarray): setpoint
         """
         pass
```

### Comparing `PyFlyt-0.5.3/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.6.0/PyFlyt/core/abstractions/boosters.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,38 @@
 import warnings
 
 import numpy as np
 from pybullet_utils import bullet_client
 
 
 class Boosters:
-    """Boosters."""
+    """Vectorized implementation of a series of fueled boosters.
+
+    The `Boosters` component is used to represent an array of fueled boosters, each at arbitrary locations with different parameters.
+    Fueled boosters are propulsion units that produce no meaningful torque around their thrust axis and have limited throttleability.
+    More crucially, they depend on a fuel source that depletes with usage, changing the mass and inertia properties of the drone.
+    Additionally, some boosters, typically of the solid fuel variety, cannot be extinguished and reignited, a property we call reignitability.
+
+    Args:
+        p (bullet_client.BulletClient): PyBullet physics client ID.
+        physics_period (float): physics period of the simulation.
+        np_random (np.random.RandomState): random number generator of the simulation.
+        uav_id (int): ID of the drone.
+        booster_ids (np.ndarray | list[int]): list of integers representing the link index that each booster should be attached to.
+        fueltank_ids (np.ndarray | list[None | int]): list of integers representing the link index for the fuel tank that each booster is attached to.
+        tau (np.ndarray): list of floats representing the ramp up time constant of each booster.
+        total_fuel_mass (np.ndarray): list of floats representing the fuel mass of each fuel tank at maximum fuel.
+        max_fuel_rate (np.ndarray): list of floats representing the maximum fuel burn rate for each booster.
+        max_inertia (np.ndarray): an `(n, 3)` array representing the diagonal elements of the moment of inertia matrix for each fuel tank at full fuel load.
+        min_thrust (np.ndarray): list of floats representing the thrust output for each booster at a minimum duty cycle that is NOT OFF.
+        max_thrust (np.ndarray): list of floats representing the maximum thrust output for each booster.
+        thrust_unit (np.ndarray): an `(n, 3)` array representing the unit vector pointing in the direction of force for each booster, relative to the booster link's body frame.
+        reignitable (np.ndarray | list[bool]): a list of booleans representing whether the booster can be extinguished and then reignited.
+        noise_ratio (np.ndarray): a list of floats representing the percent amount of fluctuation present in each booster.
+    """
 
     def __init__(
         self,
         p: bullet_client.BulletClient,
         physics_period: float,
         np_random: np.random.RandomState,
         uav_id: int,
@@ -27,29 +50,29 @@
         thrust_unit: np.ndarray,
         reignitable: np.ndarray | list[bool],
         noise_ratio: np.ndarray,
     ):
         """Used for simulating an array of boosters.
 
         Args:
-            p (bullet_client.BulletClient): p
-            physics_period (float): physics_period
-            np_random (np.random.RandomState): np_random
-            uav_id (int): uav_id
-            booster_ids (list[int]): booster_ids
-            fueltank_ids (list[None | int]): fueltank_ids
-            tau (np.ndarray): booster ramp time constant
-            total_fuel_mass (np.ndarray): total_fuel_mass
-            max_fuel_rate (np.ndarray): max_fuel_rate
-            max_inertia (np.ndarray): diagonal elements of the inertia tensor
-            min_thrust (np.ndarray): min_thrust
-            max_thrust (np.ndarray): max_thrust
-            thrust_unit (np.ndarray): unit vector of the direction thrust is pointing
-            reignitable (list[bool]): whether we can turn off and on the booster
-            noise_ratio (np.ndarray): noise_ratio
+            p (bullet_client.BulletClient): PyBullet physics client ID.
+            physics_period (float): physics period of the simulation.
+            np_random (np.random.RandomState): random number generator of the simulation.
+            uav_id (int): ID of the drone.
+            booster_ids (np.ndarray | list[int]): list of integers representing the link index that each booster should be attached to.
+            fueltank_ids (np.ndarray | list[None | int]): list of integers representing the link index for the fuel tank that each booster is attached to.
+            tau (np.ndarray): list of floats representing the ramp up time constant of each booster.
+            total_fuel_mass (np.ndarray): list of floats representing the fuel mass of each fuel tank at maximum fuel.
+            max_fuel_rate (np.ndarray): list of floats representing the maximum fuel burn rate for each booster.
+            max_inertia (np.ndarray): an `(n, 3)` array representing the diagonal elements of the moment of inertia matrix for each fuel tank at full fuel load.
+            min_thrust (np.ndarray): list of floats representing the thrust output for each booster at a minimum duty cycle that is NOT OFF.
+            max_thrust (np.ndarray): list of floats representing the maximum thrust output for each booster.
+            thrust_unit (np.ndarray): an `(n, 3)` array representing the unit vector pointing in the direction of force for each booster, relative to the booster link's body frame.
+            reignitable (np.ndarray | list[bool]): a list of booleans representing whether the booster can be extinguished and then reignited.
+            noise_ratio (np.ndarray): a list of floats representing the percent amount of fluctuation present in each booster.
         """
         self.p = p
         self.physics_period = physics_period
         self.np_random = np_random
 
         # store IDs
         self.uav_id = uav_id
@@ -91,15 +114,15 @@
         self.ratio_fuel_rate = self.max_fuel_rate / self.total_fuel_mass
         self.noise_ratio = noise_ratio
 
     def reset(self, starting_fuel_ratio: float | np.ndarray = 1.0):
         """Reset the boosters.
 
         Args:
-            starting_fuel_ratio (float | np.ndarray): starting_fuel_ratio
+            starting_fuel_ratio (float | np.ndarray): ratio amount of fuel that the booster is reset to
         """
         # deal with everything in percents
         self.ratio_fuel_remaining = (
             np.ones((self.num_boosters,), dtype=np.float64) * starting_fuel_ratio
         )
         self.throttle = np.zeros((self.num_boosters,), dtype=np.float64)
         self.ignition_state = np.zeros((self.num_boosters,), dtype=bool)
@@ -114,15 +137,19 @@
             [
                 self.ignition_state.flatten(),  # [n]
                 self.ratio_fuel_remaining.flatten(),  # [n]
                 self.throttle.flatten(),  # [n]
             ]
         )
 
-    def settings2forces(
+    def state_update(self):
+        """This does not need to be called for boosters."""
+        warnings.warn("`state_update` does not need to be called for boosters.")
+
+    def physics_update(
         self, ignition: np.ndarray, pwm: np.ndarray, rotation: None | np.ndarray = None
     ):
         """Converts booster settings into forces on the booster and inertia change on fuel tank.
 
         Args:
             ignition (np.ndarray): (num_boosters,) array of booleans for engine on or off
             pwm (np.ndarray): (num_boosters,) array of floats between [0, 1] for min or max thrust
```

### Comparing `PyFlyt-0.5.3/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.6.0/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,36 +4,48 @@
 import warnings
 
 import numpy as np
 from pybullet_utils import bullet_client
 
 
 class BoringBodies:
-    """BoringBodies."""
+    """Vectorized implementation of a series of plain bodies affected by aerodynamics.
+
+    The `BoringBodies` component is used to represent a normal body moving through the air.
+
+    Args:
+        p (bullet_client.BulletClient): PyBullet physics client ID.
+        physics_period (float): physics period of the simulation.
+        np_random (np.random.RandomState): random number generator of the simulation.
+        uav_id (int): ID of the drone.
+        body_ids (np.ndarray): (n,) array of IDs for the links representing the bodies
+        drag_coefs (np.ndarray): (n, 3) array of drag coefficients for each body in the link-referenced XYZ directions
+        normal_areas (np.ndarray): (n, 3) array of frontal areas in the link-referenced XYZ directions
+    """
 
     def __init__(
         self,
         p: bullet_client.BulletClient,
         physics_period: float,
         np_random: np.random.RandomState,
         uav_id: int,
         body_ids: np.ndarray,
         drag_coefs: np.ndarray,
         normal_areas: np.ndarray,
     ):
         """Used for simulating a body moving through the air.
 
         Args:
-            p (bullet_client.BulletClient): p
-            physics_period (float): physics_period
-            np_random (np.random.RandomState): np_random
-            uav_id (int): uav_id
-            body_ids (np.ndarray): (n,) array of ids for the links representing the bodies
-            drag_coefs (np.ndarray): (n, 3) array of drag coefs in the x, y, z
-            normal_areas (np.ndarray): (n, 3) array of frontal areas in the x, y, z
+            p (bullet_client.BulletClient): PyBullet physics client ID.
+            physics_period (float): physics period of the simulation.
+            np_random (np.random.RandomState): random number generator of the simulation.
+            uav_id (int): ID of the drone.
+            body_ids (np.ndarray): (n,) array of IDs for the links representing the bodies
+            drag_coefs (np.ndarray): (n, 3) array of drag coefficients for each body in the link-referenced XYZ directions
+            normal_areas (np.ndarray): (n, 3) array of frontal areas in the link-referenced XYZ directions
         """
         self.p = p
         self.physics_period = physics_period
         self.np_random = np_random
 
         # store IDs
         self.uav_id = uav_id
@@ -50,15 +62,21 @@
         # runtime parameters
         self.local_body_velocities = np.zeros((len(self.body_ids), 3))
 
     def reset(self):
         """Reset the boring bodies."""
         self.local_body_velocities = np.zeros((len(self.body_ids), 3))
 
-    def update_local_velocity(self, rotation_matrices: np.ndarray):
+    def get_states(self):
+        """`get_states` does not exist for boring bodies, they're boring."""
+        raise NotImplementedError(
+            "`get_states` does not exist for boring bodies, they're boring."
+        )
+
+    def state_update(self, rotation_matrices: np.ndarray):
         """Updates the local surface velocity of the boring body.
 
         Args:
             rotation_matrices (np.ndarray): (n, 3, 3) array of rotation matrices of the bodies
         """
         # get all the states for all the bodies
         body_velocities = self.p.getLinkStates(
@@ -72,15 +90,15 @@
         # rotate all velocities to be in local frame
         body_velocities = np.matmul(rotation_matrices, body_velocities)
         body_velocities = np.squeeze(body_velocities, axis=-1)
 
         # update the variable
         self.local_body_velocities = body_velocities
 
-    def update_forces(self):
+    def physics_update(self):
         """Applies a force to the boring bodies depending on their local surface velocities."""
         forces = (
             -np.sign(self.local_body_velocities)
             * self.drag_consts
             * self.local_body_velocities**2
         )
         for i, force in enumerate(forces):
```

### Comparing `PyFlyt-0.5.3/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.6.0/PyFlyt/core/abstractions/gimbals.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,14 +109,24 @@
         """
         return np.concatenate(
             [
                 self.gimbal_state.flatten(),  # [n, 2]
             ]
         )
 
+    def state_update(self):
+        """This does not need to be called for gimbals."""
+        warnings.warn("`state_update` does not need to be called for gimbals.")
+
+    def physics_update(self):
+        """This does not need to be called for gimbals, call `compute_rotation` instead."""
+        raise NameError(
+            "`state_update` does not need to be called for gimbals, call `compute_rotation` instead."
+        )
+
     def compute_rotation(self, gimbal_command) -> np.ndarray:
         """Returns a rotation vector after the gimbal rotation.
 
         Args:
             gimbal_command (np.ndarray): (num_gimbals, 2) array of floats between [-1, 1]
 
         Returns:
```

### Comparing `PyFlyt-0.5.3/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.6.0/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         """Gets the current state of the components.
 
         Returns:
             np.ndarray:
         """
         return np.array([surface.actuation for surface in self.surfaces])
 
-    def cmd2forces(self, cmd: np.ndarray):
+    def physics_update(self, cmd: np.ndarray):
         """Converts actuation commands into forces on the lifting surfaces.
 
         Args:
             cmd (np.ndarray): the full command array, command mapping is handled through `command_id` and `command_sign` on each surface.
         """
         assert np.all(cmd >= -1.0) and np.all(
             cmd <= 1.0
@@ -52,17 +52,17 @@
         for surface in self.surfaces:
             actuation = (
                 0.0
                 if surface.command_id is None
                 else float(cmd[surface.command_id] * surface.command_sign)
             )
 
-            surface.cmd2forces(actuation)
+            surface.physics_update(actuation)
 
-    def update_local_surface_velocities(self, rotation_matrix: np.ndarray):
+    def state_update(self, rotation_matrix: np.ndarray):
         """Updates all local surface velocities of the lifting surface, place under `update_state`.
 
         Args:
             rotation_matrix (np.ndarray): rotation_matrix of the main body
         """
         # get all the states for all the surfaces
         surface_velocities = self.p.getLinkStates(
@@ -73,15 +73,15 @@
         surface_velocities = np.array([item[-2] for item in surface_velocities])
 
         # convert all to local velocities
         surface_velocities = np.matmul(rotation_matrix, surface_velocities.T).T
 
         # update the velocities of all surfaces
         for surface, velocity in zip(self.surfaces, surface_velocities):
-            surface.update_local_surface_velocity(velocity)
+            surface.state_update(velocity)
 
 
 class LiftingSurface:
     """LiftingSurface."""
 
     def __init__(
         self,
@@ -90,83 +90,68 @@
         np_random: np.random.RandomState,
         uav_id: int,
         surface_id: int,
         command_id: None | int,
         command_sign: float,
         lifting_unit: np.ndarray,
         forward_unit: np.ndarray,
-        aerofoil_params: dict,
+        Cl_alpha_2D: float,
+        chord: float,
+        span: float,
+        flap_to_chord: float,
+        eta: float,
+        alpha_0_base: float,
+        alpha_stall_P_base: float,
+        alpha_stall_N_base: float,
+        Cd_0: float,
+        deflection_limit: float,
+        tau: float,
     ):
         """Used for simulating a single lifting surface.
 
         Args:
             p (bullet_client.BulletClient): p
             physics_period (float): physics_period
             np_random (np.random.RandomState): np_random
             uav_id (int): uav_id
             surface_id (int): surface_id
             command_id (None | int): command_id, for convenience
             command_sign (float): command_sign, for convenience
             lifting_unit (np.ndarray): (3,) unit vector representing the direction of lift
             forward_unit (np.ndarray): (3,) unit vector representing the direction of travel
-            aerofoil_params (dict): aerofoil_params, see below
-
-        Aerofoil params must have these components (everything is in degrees and is a float):
-            - Cl_alpha_2D
-            - chord
-            - span
-            - flap_to_chord
-            - eta
-            - alpha_0_base
-            - alpha_stall_P_base
-            - alpha_stall_N_base
-            - Cd_0
-            - deflection_limit
-            - tau
+            Cl_alpha_2D (float): float
+            chord (float): float
+            span (float): float
+            flap_to_chord (float): float
+            eta (float): float
+            alpha_0_base (float): float
+            alpha_stall_P_base (float): float
+            alpha_stall_N_base (float): float
+            Cd_0 (float): float
+            deflection_limit (float): float
+            tau (float): float
         """
         self.p = p
         self.physics_period = physics_period
         self.np_random = np_random
 
         # store IDs
         self.uav_id = uav_id
         self.surface_id = surface_id
 
         # command inputs for referencing
         self.command_id = command_id
         self.command_sign = command_sign
 
-        # check that we have all the required params
-        params_list = [
-            "Cl_alpha_2D",
-            "chord",
-            "span",
-            "flap_to_chord",
-            "eta",
-            "alpha_0_base",
-            "alpha_stall_P_base",
-            "alpha_stall_N_base",
-            "Cd_0",
-            "deflection_limit",
-            "tau",
-        ]
-        for key in aerofoil_params:
-            if key in params_list:
-                params_list.remove(key)
-
-        assert (
-            len(params_list) == 0
-        ), f"Missing parameters: {params_list} in aerofoil_params for component {surface_id}."
-
         # some checks for the lifting and norm vectors
         assert lifting_unit.shape == (3,)
         assert forward_unit.shape == (3,)
         assert (
-            aerofoil_params["tau"] >= 0.0 / physics_period
-        ), f"Setting `tau = 1 / physics_period` is equivalent to 0, 0 is not a valid option, got {aerofoil_params['tau']}."
+            tau >= 0.0 / physics_period
+        ), f"Setting `tau = 1 / physics_period` is equivalent to 0, 0 is not a valid option, got {tau}."
         if np.linalg.norm(lifting_unit) != 1.0:
             warnings.warn(f"Norm of `{lifting_unit=}` is not 1.0, normalizing...")
             lifting_unit /= np.linalg.norm(lifting_unit)
         if np.linalg.norm(forward_unit) != 1.0:
             warnings.warn(f"Norm of `{forward_unit=}` is not 1.0, normalizing...")
             forward_unit /= np.linalg.norm(forward_unit)
         if np.dot(lifting_unit, forward_unit) != 0.0:
@@ -176,25 +161,25 @@
 
         # get the lift, drag, and torque units
         self.lift_unit = lifting_unit
         self.drag_unit = forward_unit
         self.torque_unit = np.cross(lifting_unit, forward_unit)
 
         # wing parameters
-        self.Cl_alpha_2D = float(aerofoil_params["Cl_alpha_2D"])
-        self.chord = float(aerofoil_params["chord"])
-        self.span = float(aerofoil_params["span"])
-        self.flap_to_chord = float(aerofoil_params["flap_to_chord"])
-        self.eta = float(aerofoil_params["eta"])
-        self.alpha_0_base = float(aerofoil_params["alpha_0_base"])
-        self.alpha_stall_P_base = float(aerofoil_params["alpha_stall_P_base"])
-        self.alpha_stall_N_base = float(aerofoil_params["alpha_stall_N_base"])
-        self.Cd_0 = float(aerofoil_params["Cd_0"])
-        self.deflection_limit = float(aerofoil_params["deflection_limit"])
-        self.cmd_tau = float(aerofoil_params["tau"])
+        self.Cl_alpha_2D = Cl_alpha_2D
+        self.chord = chord
+        self.span = span
+        self.flap_to_chord = flap_to_chord
+        self.eta = eta
+        self.alpha_0_base = alpha_0_base
+        self.alpha_stall_P_base = alpha_stall_P_base
+        self.alpha_stall_N_base = alpha_stall_N_base
+        self.Cd_0 = Cd_0
+        self.deflection_limit = deflection_limit
+        self.cmd_tau = tau
 
         # precompute some constants
         self.half_rho = 0.5 * 1.225
         self.area = self.chord * self.span
         self.aspect = self.span / self.chord
         self.alpha_stall_P_base = np.deg2rad(self.alpha_stall_P_base)
         self.alpha_stall_N_base = np.deg2rad(self.alpha_stall_N_base)
@@ -209,23 +194,31 @@
         # runtime parameters
         self.local_surface_velocity = np.array([0.0, 0.0, 0.0])
 
     def reset(self):
         """Reset the lifting surfaces."""
         self.actuation = 0.0
 
-    def update_local_surface_velocity(self, surface_velocity: np.ndarray):
+    def get_states(self) -> float:
+        """Gets the current state of the components.
+
+        Returns:
+            float: the level of deflection of the surface.
+        """
+        return self.actuation
+
+    def state_update(self, surface_velocity: np.ndarray):
         """Updates the local surface velocity of the lifting surface.
 
         Args:
             surface_velocity (np.ndarray): surface_velocity
         """
         self.local_surface_velocity = surface_velocity
 
-    def cmd2forces(self, cmd: float):
+    def physics_update(self, cmd: float):
         """Converts a commanded actuation state into forces on the lifting surface.
 
         Args:
             cmd (float): normalized actuation in [-1, 1]
 
         Returns:
             tuple[np.ndarray, np.ndarray]: vec3 force, vec3 torque
```

### Comparing `PyFlyt-0.5.3/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.6.0/PyFlyt/core/abstractions/motors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """A component to simulate an array of electric propeller motors on vehicle."""
 from __future__ import annotations
 
+import warnings
+
 import numpy as np
 from pybullet_utils import bullet_client
 
 
 class Motors:
     """Motors."""
 
@@ -73,15 +75,19 @@
         """Gets the current state of the components.
 
         Returns:
             np.ndarray:
         """
         return self.throttle.flatten()
 
-    def pwm2forces(self, pwm: np.ndarray, rotation: None | np.ndarray = None):
+    def state_update(self):
+        """This does not need to be called for motors."""
+        warnings.warn("`state_update` does not need to be called for motors.")
+
+    def physics_update(self, pwm: np.ndarray, rotation: None | np.ndarray = None):
         """Converts motor PWM values to forces, this motor allows negative thrust.
 
         Args:
             pwm (np.ndarray): [num_motors, ] array defining the pwm values of each motor from -1 to 1
             rotation (np.ndarray): (num_motors, 3, 3) rotation matrices to rotate each booster's thrust axis around
         """
         assert np.all(pwm >= -1.0) and np.all(
```

### Comparing `PyFlyt-0.5.3/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.6.0/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/core/aviary.py` & `PyFlyt-0.6.0/PyFlyt/core/aviary.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,73 @@
 """The Aviary class, the core of how PyFlyt handles UAVs in the PyBullet simulation environment."""
 from __future__ import annotations
 
 import time
 from itertools import repeat
-from typing import Sequence
+from typing import Any, Sequence
 
 import numpy as np
 import pybullet as p
 import pybullet_data
 from pybullet_utils import bullet_client
 
 from .abstractions import DroneClass
-from .drones import FixedWing, QuadX, Rocket
+from .drones import Fixedwing, QuadX, Rocket
 
 DroneIndex = int
 
 
 class Aviary(bullet_client.BulletClient):
-    """Aviary class, the core of how PyFlyt handles UAVs in the PyBullet simulation environment."""
+    """Aviary class, the core of how PyFlyt handles UAVs in the PyBullet simulation environment.
+
+    The `aviary` is a handler for physics stepping, setpoint handling, collisions tracking, and much more.
+    It provides a common endpoint from where users may control drones or define tasks.
+
+    Args:
+        start_pos (np.ndarray): an `(n, 3)` array for the starting X, Y, Z positions for each drone.
+        start_orn (np.ndarray): an `(n, 3)` array for the starting orientations for each drone, in terms of Euler angles.
+        drone_type (str | Sequence[str]): a _lowercase_ string representing what type of drone to spawn.
+        drone_type_mappings (None | dict(str, DroneClass)): a dictionary mapping of `{str: DroneClass}` for spawning custom drones.
+        drone_options (dict[str, Any] | Sequence[dict[str, Any]]): dictionary mapping of custom parameters for each drone.
+        render (bool): a boolean whether to render the simulation.
+        render_FPS (int): the FPS for rendering, this helps the scheduler.
+        physics_hz (int): physics looprate (not recommended to be changed).
+        worldScale (float): how big to spawn the floor.
+        seed (None | int): optional int for seeding the simulation RNG.
+    """
 
     def __init__(
         self,
         start_pos: np.ndarray,
         start_orn: np.ndarray,
         drone_type: str | Sequence[str],
         drone_type_mappings: None | dict[str, DroneClass] = None,
+        drone_options: dict[str, Any] | Sequence[dict[str, Any]] = {},
         render: bool = False,
+        render_FPS: int = 60,
         physics_hz: int = 240,
         worldScale: float = 1.0,
-        drone_options: dict | Sequence[dict] = {},
         seed: None | int = None,
     ):
         """Initializes a PyBullet environment that hosts UAVs and other entities.
 
         The Aviary class itself inherits from a BulletClient, so any function that a PyBullet client has, this class will have.
         The Aviary also handles dealing with physics and control looprates, as well as automatic construction of several default UAVs and their corresponding cameras.
 
         Args:
-            start_pos (np.ndarray): start_pos
-            start_orn (np.ndarray): start_orn
-            drone_type (str | Sequence[str]): drone_types
-            drone_type_mappings (None | dict[str, DroneClass]): string to mapping of custom drone classes
-            render (bool): render
-            physics_hz (int): physics_hz
-            worldScale (float): worldScale
-            drone_options (dict | Sequence[dict]): drone_options
-            seed (None | int): seed
+            start_pos (np.ndarray): an `(n, 3)` array for the starting X, Y, Z positions for each drone.
+            start_orn (np.ndarray): an `(n, 3)` array for the starting orientations for each drone, in terms of Euler angles.
+            drone_type (str | Sequence[str]): a _lowercase_ string representing what type of drone to spawn.
+            drone_type_mappings (None | dict(str, DroneClass)): a dictionary mapping of `{str: DroneClass}` for spawning custom drones.
+            drone_options (dict[str, Any] | Sequence[dict[str, Any]]): dictionary mapping of custom parameters for each drone.
+            render (bool): a boolean whether to render the simulation.
+            render_FPS (int): the FPS for rendering, this helps the scheduler.
+            physics_hz (int): physics looprate (not recommended to be changed).
+            worldScale (float): how big to spawn the floor.
+            seed (None | int): optional int for seeding the simulation RNG.
         """
         super().__init__(p.GUI if render else p.DIRECT)
         print("\033[A                             \033[A")
 
         # check for starting position and orientation shapes
         assert (
             len(start_pos.shape) == 2
@@ -81,15 +99,15 @@
         # default physics looprate is 240 Hz
         self.physics_hz = physics_hz
         self.physics_period = 1.0 / physics_hz
 
         # mapping of drone type string to the constructors
         self.drone_type_mappings = dict()
         self.drone_type_mappings["quadx"] = QuadX
-        self.drone_type_mappings["fixedwing"] = FixedWing
+        self.drone_type_mappings["fixedwing"] = Fixedwing
         self.drone_type_mappings["rocket"] = Rocket
         if drone_type_mappings is not None:
             self.drone_type_mappings = {
                 **self.drone_type_mappings,
                 **drone_type_mappings,
             }
 
@@ -165,30 +183,42 @@
                     physics_hz=self.physics_hz,
                     np_random=self.np_random,
                     **drone_options,
                 )
             )
 
         # constants for tracking how many times to step depending on control hz
-        all_control_hz = [1.0 / drone.control_period for drone in self.drones]
+        all_control_hz = [int(1.0 / drone.control_period) for drone in self.drones]
         self.updates_per_step = int(self.physics_hz / np.min(all_control_hz))
         self.update_period = 1.0 / np.min(all_control_hz)
+
+        # sanity check the control looprates
+        if len(all_control_hz) > 0:
+            all_control_hz.sort()
+            all_ratios = np.array(all_control_hz)[1:] / np.array(all_control_hz)[:-1]
+            assert all(
+                r % 1.0 == 0.0 for r in all_ratios
+            ), "Looprates must form common multiples of each other."
+
+        # rtf tracking parameters
         self.now = time.time()
+        self.frame_time_elapsed = 0.0
+        self.sim_time_elapsed = 0.0
 
         # arm everything
         self.register_all_new_bodies()
         self.set_armed(True)
 
     def register_all_new_bodies(self):
         """Registers all new bodies in the environment to be able to handle collisions later.
 
         Call this when there is an update in the number of bodies in the environment.
         """
         # collision array
-        self.collision_array = np.zeros(
+        self.contact_array = np.zeros(
             (self.getNumBodies(), self.getNumBodies()), dtype=bool
         )
 
     def state(self, index: DroneIndex) -> np.ndarray:
         """Returns the state for the indexed drone.
 
         Args:
@@ -247,15 +277,15 @@
             bodies[i] = self.getBodyInfo(i)[-1].decode("UTF-8")
 
         from pprint import pprint
 
         pprint(bodies)
 
     def set_armed(self, settings: int | bool | list[int | bool]):
-        """Sets the arming state of each drone in the environment.
+        """Sets the arming state of each drone in the environment. Unarmed drones won't receive updates and will ragdoll.
 
         Args:
             settings (int | bool | list[int | bool]): arm setting
         """
         if isinstance(settings, list):
             assert len(settings) == len(
                 self.drones
@@ -263,15 +293,15 @@
             self.armed_drones = [
                 drone for (drone, arm) in zip(self.drones, settings) if arm
             ]
         else:
             self.armed_drones = [drone for drone in self.drones] if settings else []
 
     def set_mode(self, flight_modes: int | list[int]):
-        """Sets the flight mode of each drone in the environment.
+        """Sets the flight control mode of each drone in the environment.
 
         Args:
             flight_modes (int | list[int]): flight mode
         """
         if isinstance(flight_modes, list):
             assert len(flight_modes) == len(
                 self.drones
@@ -303,49 +333,52 @@
     def step(self):
         """Steps the environment, this automatically handles physics and control looprates, one step is equivalent to one control loop step."""
         # compute rtf if we're rendering
         if self.render:
             elapsed = time.time() - self.now
             self.now = time.time()
 
-            # sleep to maintain real time factor
-            time.sleep(max(0, self.update_period - elapsed))
+            self.sim_time_elapsed += self.update_period * self.updates_per_step
+            self.frame_time_elapsed += elapsed
 
-            # calculate real time factor
-            RTF = self.update_period / (elapsed + 1e-6)
+            # print RTF every 0.5 seconds, this actually adds considerable overhead
+            if self.frame_time_elapsed >= 0.5:
+                # calculate real time factor based on realtime/simtime
+                RTF = self.sim_time_elapsed / (self.frame_time_elapsed + 1e-6)
+                self.sim_time_elapsed = 0.0
+                self.frame_time_elapsed = 0.0
 
-            # handle case where sometimes elapsed becomes 0
-            if elapsed != 0.0:
                 self.rtf_debug_line = self.addUserDebugText(
-                    text=f"RTF: {str(RTF)[:7]}",
+                    text=f"RTF: {RTF:.3f}",
                     textPosition=[0, 0, 0],
                     textColorRGB=[1, 0, 0],
                     replaceItemUniqueId=self.rtf_debug_line,
                 )
 
         # reset collisions
-        self.collision_array &= False
+        self.contact_array &= False
 
         # step the environment enough times for one control loop of the slowest controller
-        physics_steps = 1
-        while physics_steps <= self.updates_per_step:
+        for physics_steps in range(self.updates_per_step):
             # update onboard avionics conditionally
             [
-                drone.update_avionics()
+                drone.update_control()
                 for drone in self.armed_drones
                 if physics_steps % drone.physics_control_ratio == 0
             ]
 
-            # compute physics
+            # update physics and state
             [drone.update_physics() for drone in self.armed_drones]
+            [drone.update_state() for drone in self.armed_drones]
 
             # advance pybullet
             self.stepSimulation()
 
             # splice out collisions
             for collision in self.getContactPoints():
-                self.collision_array[collision[1], collision[2]] = True
-                self.collision_array[collision[2], collision[1]] = True
+                self.contact_array[collision[1], collision[2]] = True
+                self.contact_array[collision[2], collision[1]] = True
 
-            physics_steps += 1
+        # update the last components of the drones, this is usually limited to cameras only
+        [drone.update_last() for drone in self.armed_drones]
 
         self.steps += 1
```

### Comparing `PyFlyt-0.5.3/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.6.0/PyFlyt/core/drones/fixedwing.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 from ..abstractions.base_drone import DroneClass
 from ..abstractions.camera import Camera
 from ..abstractions.lifting_surfaces import LiftingSurface, LiftingSurfaces
 from ..abstractions.motors import Motors
 
 
-class FixedWing(DroneClass):
-    """FixedWing instance that handles everything about a FixedWing."""
+class Fixedwing(DroneClass):
+    """Fixedwing instance that handles everything about a FixedWing."""
 
     def __init__(
         self,
         p: bullet_client.BulletClient,
         start_pos: np.ndarray,
         start_orn: np.ndarray,
         control_hz: int = 120,
@@ -79,71 +79,71 @@
                     np_random=self.np_random,
                     uav_id=self.Id,
                     surface_id=3,
                     command_id=0,
                     command_sign=+1.0,
                     lifting_unit=np.array([0.0, 0.0, 1.0]),
                     forward_unit=np.array([1.0, 0.0, 0.0]),
-                    aerofoil_params=all_params["left_wing_flapped_params"],
+                    **all_params["left_wing_flapped_params"],
                 )
             )
             surfaces.append(
                 LiftingSurface(
                     p=self.p,
                     physics_period=self.physics_period,
                     np_random=self.np_random,
                     uav_id=self.Id,
                     surface_id=4,
                     command_id=0,
                     command_sign=-1.0,
                     lifting_unit=np.array([0.0, 0.0, 1.0]),
                     forward_unit=np.array([1.0, 0.0, 0.0]),
-                    aerofoil_params=all_params["right_wing_flapped_params"],
+                    **all_params["right_wing_flapped_params"],
                 )
             )
             surfaces.append(
                 LiftingSurface(
                     p=self.p,
                     physics_period=self.physics_period,
                     np_random=self.np_random,
                     uav_id=self.Id,
                     surface_id=1,
                     command_id=1,
                     command_sign=1.0,
                     lifting_unit=np.array([0.0, 0.0, 1.0]),
                     forward_unit=np.array([1.0, 0.0, 0.0]),
-                    aerofoil_params=all_params["horizontal_tail_params"],
+                    **all_params["horizontal_tail_params"],
                 )
             )
             surfaces.append(
                 LiftingSurface(
                     p=self.p,
                     physics_period=self.physics_period,
                     np_random=self.np_random,
                     uav_id=self.Id,
                     surface_id=5,
                     command_id=None,
                     command_sign=+1.0,
                     lifting_unit=np.array([0.0, 0.0, 1.0]),
                     forward_unit=np.array([1.0, 0.0, 0.0]),
-                    aerofoil_params=all_params["main_wing_params"],
+                    **all_params["main_wing_params"],
                 )
             )
             surfaces.append(
                 LiftingSurface(
                     p=self.p,
                     physics_period=self.physics_period,
                     np_random=self.np_random,
                     uav_id=self.Id,
                     surface_id=2,
                     command_id=2,
                     command_sign=-1.0,
                     lifting_unit=np.array([0.0, 1.0, 0.0]),
                     forward_unit=np.array([1.0, 0.0, 0.0]),
-                    aerofoil_params=all_params["vertical_tail_params"],
+                    **all_params["vertical_tail_params"],
                 )
             )
             self.lifting_surfaces = LiftingSurfaces(lifting_surfaces=surfaces)
 
             # motor
             motor_params = all_params["motor_params"]
             tau = np.array([motor_params["tau"]])
@@ -197,14 +197,37 @@
         self.lifting_surfaces.reset()
         self.motors.reset()
         self.update_state()
 
         if self.use_camera:
             self.rgbaImg, self.depthImg, self.segImg = self.camera.capture_image()
 
+    def update_control(self):
+        """Runs through controllers."""
+        # the default mode
+        if self.mode == 0:
+            self.cmd = self.setpoint
+            return
+
+        # otherwise, check that we have a custom controller
+        if self.mode not in self.registered_controllers.keys():
+            raise ValueError(
+                f"Don't have other modes aside from 0, received {self.mode}."
+            )
+
+        # custom controllers run if any
+        self.cmd = self.instanced_controllers[self.mode].step(self.state, self.setpoint)
+
+    def update_physics(self):
+        """Updates the physics of the vehicle."""
+        assert self.cmd[3] >= 0.0, f"thrust `{self.cmd[3]}` must be more than 0.0."
+
+        self.lifting_surfaces.physics_update(self.cmd)
+        self.motors.physics_update(self.cmd[[3]])
+
     def update_state(self):
         """Updates the current state of the UAV.
 
         This includes: ang_vel, ang_pos, lin_vel, lin_pos.
         """
         lin_pos, ang_pos = self.p.getBasePositionAndOrientation(self.Id)
         lin_vel, ang_vel = self.p.getBaseVelocity(self.Id)
@@ -217,44 +240,18 @@
         # ang_pos in euler form
         ang_pos = self.p.getEulerFromQuaternion(ang_pos)
 
         # create the state
         self.state = np.stack([ang_vel, ang_pos, lin_vel, lin_pos], axis=0)
 
         # update all lifting surface velocities
-        self.lifting_surfaces.update_local_surface_velocities(rotation)
+        self.lifting_surfaces.state_update(rotation)
 
         # update auxiliary information
         self.aux_state = np.concatenate(
             (self.lifting_surfaces.get_states(), self.motors.get_states())
         )
 
-    def update_control(self):
-        """Runs through controllers."""
-        # the default mode
-        if self.mode == 0:
-            self.cmd = self.setpoint
-            return
-
-        # otherwise, check that we have a custom controller
-        if self.mode not in self.registered_controllers.keys():
-            raise ValueError(
-                f"Don't have other modes aside from 0, received {self.mode}."
-            )
-
-        # custom controllers run if any
-        self.cmd = self.instanced_controllers[self.mode].step(self.state, self.setpoint)
-
-    def update_physics(self):
-        """Updates the physics of the vehicle."""
-        assert self.cmd[3] >= 0.0, f"thrust `{self.cmd[3]}` must be more than 0.0."
-
-        self.update_state()
-        self.lifting_surfaces.cmd2forces(self.cmd)
-        self.motors.pwm2forces(self.cmd[[3]])
-
-    def update_avionics(self):
-        """Updates state and control."""
-        self.update_control()
-
+    def update_last(self):
+        """Updates things only at the end of `Aviary.step()`."""
         if self.use_camera:
             self.rgbaImg, self.depthImg, self.segImg = self.camera.capture_image()
```

### Comparing `PyFlyt-0.5.3/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.6.0/PyFlyt/core/drones/quadx.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,36 +362,14 @@
         assert (
             base_mode >= -1 and base_mode <= 7
         ), f"`base_mode` must be within -1 and 7, currently {base_mode}."
 
         self.registered_controllers[controller_id] = controller_constructor
         self.registered_base_modes[controller_id] = base_mode
 
-    def update_state(self):
-        """Updates the current state of the UAV.
-
-        This includes: ang_vel, ang_pos, lin_vel, lin_pos.
-        """
-        lin_pos, ang_pos = self.p.getBasePositionAndOrientation(self.Id)
-        lin_vel, ang_vel = self.p.getBaseVelocity(self.Id)
-
-        # express vels in local frame
-        rotation = np.array(self.p.getMatrixFromQuaternion(ang_pos)).reshape(3, 3).T
-        lin_vel = np.matmul(rotation, lin_vel)
-        ang_vel = np.matmul(rotation, ang_vel)
-
-        # ang_pos in euler form
-        ang_pos = self.p.getEulerFromQuaternion(ang_pos)
-
-        # create the state
-        self.state = np.stack([ang_vel, ang_pos, lin_vel, lin_pos], axis=0)
-
-        # update auxiliary information
-        self.aux_state = self.motors.get_states()
-
     def update_control(self):
         """Runs through controllers."""
         # this is the thing we cascade down controllers
         a_output = self.setpoint[:3].copy()
         z_output = self.setpoint[-1].copy()
         mode = self.mode
 
@@ -467,29 +445,47 @@
         if (high := np.max(self.pwm)) > 1.0:
             self.pwm /= high
         if (low := np.min(self.pwm)) < 0.05:
             self.pwm += (1.0 - self.pwm) / (1.0 - low) * (0.05 - low)
 
     def update_physics(self):
         """Updates the physics of the vehicle."""
-        self.update_state()
-
         # update the motors
-        self.motors.pwm2forces(self.pwm)
+        self.motors.physics_update(self.pwm)
 
         # simulate drag
         drag_pqr = -self.drag_coef_pqr * (np.array(self.state[0]) ** 2)
         drag_xyz = -self.drag_coef_xyz * (np.array(self.state[2]) ** 2)
 
         # warning, the physics is funky for bounces
         if len(self.p.getContactPoints()) == 0:
             self.p.applyExternalForce(
                 self.Id, -1, drag_xyz, [0.0, 0.0, 0.0], self.p.LINK_FRAME
             )
             self.p.applyExternalTorque(self.Id, -1, drag_pqr, self.p.LINK_FRAME)
 
-    def update_avionics(self):
-        """Updates state and control."""
-        self.update_control()
+    def update_state(self):
+        """Updates the current state of the UAV.
+
+        This includes: ang_vel, ang_pos, lin_vel, lin_pos.
+        """
+        lin_pos, ang_pos = self.p.getBasePositionAndOrientation(self.Id)
+        lin_vel, ang_vel = self.p.getBaseVelocity(self.Id)
+
+        # express vels in local frame
+        rotation = np.array(self.p.getMatrixFromQuaternion(ang_pos)).reshape(3, 3).T
+        lin_vel = np.matmul(rotation, lin_vel)
+        ang_vel = np.matmul(rotation, ang_vel)
+
+        # ang_pos in euler form
+        ang_pos = self.p.getEulerFromQuaternion(ang_pos)
+
+        # create the state
+        self.state = np.stack([ang_vel, ang_pos, lin_vel, lin_pos], axis=0)
+
+        # update auxiliary information
+        self.aux_state = self.motors.get_states()
 
+    def update_last(self):
+        """Updates things only at the end of `Aviary.step()`."""
         if self.use_camera:
             self.rgbaImg, self.depthImg, self.segImg = self.camera.capture_image()
```

### Comparing `PyFlyt-0.5.3/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.6.0/PyFlyt/core/drones/rocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                         np_random=self.np_random,
                         uav_id=self.Id,
                         surface_id=finlet_id,
                         command_id=command_id,
                         command_sign=+1.0,
                         lifting_unit=np.array([0.0, 1.0, 0.0]),
                         forward_unit=np.array([0.0, 0.0, -1.0]),
-                        aerofoil_params=all_params["finlet_params"],
+                        **all_params["finlet_params"],
                     )
                 )
             for finlet_id, command_id in zip([4, 5], [2, 3]):
                 # y axis fins
                 surfaces.append(
                     LiftingSurface(
                         p=self.p,
@@ -131,15 +131,15 @@
                         np_random=self.np_random,
                         uav_id=self.Id,
                         surface_id=finlet_id,
                         command_id=command_id,
                         command_sign=+1.0,
                         lifting_unit=np.array([1.0, 0.0, 0.0]),
                         forward_unit=np.array([0.0, 0.0, -1.0]),
-                        aerofoil_params=all_params["finlet_params"],
+                        **all_params["finlet_params"],
                     )
                 )
             self.lifting_surfaces = LiftingSurfaces(lifting_surfaces=surfaces)
 
             # mixing matrix to map finlet force command to finlet movement
             # force_x, force_y, yaw
             self.finlet_map = np.array(
@@ -221,48 +221,14 @@
         self.booster_gimbal.reset()
         self.boosters.reset(starting_fuel_ratio=self.starting_fuel_ratio)
         self.update_state()
 
         if self.use_camera:
             self.rgbaImg, self.depthImg, self.segImg = self.camera.capture_image()
 
-    def update_state(self):
-        """Updates the current state of the UAV.
-
-        This includes: ang_vel, ang_pos, lin_vel, lin_pos.
-        """
-        lin_pos, ang_pos = self.p.getBasePositionAndOrientation(self.Id)
-        lin_vel, ang_vel = self.p.getBaseVelocity(self.Id)
-
-        # express vels in local frame
-        rotation = np.array(self.p.getMatrixFromQuaternion(ang_pos)).reshape(3, 3).T
-        lin_vel = np.matmul(rotation, lin_vel)
-        ang_vel = np.matmul(rotation, ang_vel)
-
-        # ang_pos in euler form
-        ang_pos = self.p.getEulerFromQuaternion(ang_pos)
-
-        # create the state
-        self.state = np.stack([ang_vel, ang_pos, lin_vel, lin_pos], axis=0)
-
-        # update all bodies, which is just the booster here
-        self.bodies.update_local_velocity(np.expand_dims(rotation, axis=0))
-
-        # update all lifting surface velocities
-        self.lifting_surfaces.update_local_surface_velocities(rotation)
-
-        # update auxiliary information
-        self.aux_state = np.concatenate(
-            (
-                self.lifting_surfaces.get_states(),
-                self.boosters.get_states(),
-                self.booster_gimbal.get_states(),
-            )
-        )
-
     def update_control(self):
         """Runs through controllers."""
         # the default mode
         if self.mode == 0:
             # finlet mapping
             finlet_cmd = self.finlet_map @ np.expand_dims(self.setpoint[:3], axis=-1)
             finlet_cmd = np.clip(finlet_cmd, -1.0, 1.0)
@@ -278,33 +244,63 @@
             )
 
         # custom controllers run if any
         self.cmd = self.instanced_controllers[self.mode].step(self.state, self.setpoint)
 
     def update_physics(self):
         """Updates the physics of the vehicle."""
-        self.update_state()
-
         # update the forces on the main body
-        self.bodies.update_forces()
+        self.bodies.physics_update()
 
         # actuate lifting surfaces
-        self.lifting_surfaces.cmd2forces(self.cmd)
+        self.lifting_surfaces.physics_update(self.cmd)
 
         # move the booster gimbal
         rotation = self.booster_gimbal.compute_rotation(
             np.array([self.cmd[6], self.cmd[7]])
         )
 
         # update booster
-        self.boosters.settings2forces(
+        self.boosters.physics_update(
             ignition=self.cmd[[4]],
             pwm=self.cmd[[5]],
             rotation=rotation,
         )
 
-    def update_avionics(self):
-        """Updates state and control."""
-        self.update_control()
+    def update_state(self):
+        """Updates the current state of the UAV.
+
+        This includes: ang_vel, ang_pos, lin_vel, lin_pos.
+        """
+        lin_pos, ang_pos = self.p.getBasePositionAndOrientation(self.Id)
+        lin_vel, ang_vel = self.p.getBaseVelocity(self.Id)
+
+        # express vels in local frame
+        rotation = np.array(self.p.getMatrixFromQuaternion(ang_pos)).reshape(3, 3).T
+        lin_vel = np.matmul(rotation, lin_vel)
+        ang_vel = np.matmul(rotation, ang_vel)
+
+        # ang_pos in euler form
+        ang_pos = self.p.getEulerFromQuaternion(ang_pos)
+
+        # create the state
+        self.state = np.stack([ang_vel, ang_pos, lin_vel, lin_pos], axis=0)
+
+        # update all bodies, which is just the booster here
+        self.bodies.state_update(np.expand_dims(rotation, axis=0))
+
+        # update all lifting surface velocities
+        self.lifting_surfaces.state_update(rotation)
+
+        # update auxiliary information
+        self.aux_state = np.concatenate(
+            (
+                self.lifting_surfaces.get_states(),
+                self.boosters.get_states(),
+                self.booster_gimbal.get_states(),
+            )
+        )
 
+    def update_last(self):
+        """Updates things only at the end of `Aviary.step()`."""
         if self.use_camera:
             self.rgbaImg, self.depthImg, self.segImg = self.camera.capture_image()
```

### Comparing `PyFlyt-0.5.3/PyFlyt/core/load_objs.py` & `PyFlyt-0.6.0/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.6.0/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.6.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
     def compute_base_term_trunc_reward(self):
         """compute_base_term_trunc_reward."""
         # exceed step count
         if self.step_count > self.max_steps:
             self.truncation |= True
 
         # collision
-        if np.any(self.env.collision_array):
+        if np.any(self.env.contact_array):
             self.reward = -100.0
             self.info["collision"] = True
             self.termination |= True
 
         # exceed flight dome
         if np.linalg.norm(self.env.state(0)[-1]) > self.flight_dome_size:
             self.reward = -100.0
```

### Comparing `PyFlyt-0.5.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.6.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,22 +101,22 @@
         return self.state, self.info
 
     def compute_state(self):
         """Computes the state of the current timestep.
 
         This returns the observation as well as the distances to target.
         - "attitude" (Box)
-            - ang_vel (vector of 3 values)
-            - ang_pos (vector of 3/4 values)
-            - lin_vel (vector of 3 values)
-            - lin_pos (vector of 3 values)
-            - previous_action (vector of 4 values)
-            - auxiliary information (vector of 4 values)
+        ----- ang_vel (vector of 3 values)
+        ----- ang_pos (vector of 3/4 values)
+        ----- lin_vel (vector of 3 values)
+        ----- lin_pos (vector of 3 values)
+        ----- previous_action (vector of 4 values)
+        ----- auxiliary information (vector of 4 values)
         - "target_deltas" (Sequence)
-            - list of body_frame distances to target (vector of 3/4 values)
+        ----- list of body_frame distances to target (vector of 3/4 values)
         """
         ang_vel, ang_pos, lin_vel, lin_pos, quarternion = super().compute_attitude()
         aux_state = super().compute_auxiliary()
 
         # combine everything
         new_state = dict()
         if self.angle_representation == 0:
```

### Comparing `PyFlyt-0.5.3/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     def compute_base_term_trunc_reward(self):
         """compute_base_term_trunc_reward."""
         # exceed step count
         if self.step_count > self.max_steps:
             self.truncation |= True
 
         # collision
-        if np.any(self.env.collision_array):
+        if np.any(self.env.contact_array):
             self.reward = -100.0
             self.info["collision"] = True
             self.termination |= True
 
         # exceed flight dome
         if np.linalg.norm(self.env.state(0)[-1]) > self.flight_dome_size:
             self.reward = -100.0
```

### Comparing `PyFlyt-0.5.3/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.6.0/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,22 +105,22 @@
         return self.state, self.info
 
     def compute_state(self):
         """Computes the state of the current timestep.
 
         This returns the observation as well as the distances to target.
         - "attitude" (Box)
-            - ang_vel (vector of 3 values)
-            - ang_pos (vector of 3/4 values)
-            - lin_vel (vector of 3 values)
-            - lin_pos (vector of 3 values)
-            - previous_action (vector of 4 values)
-            - auxiliary information (vector of 4 values)
+        ----- ang_vel (vector of 3 values)
+        ----- ang_pos (vector of 3/4 values)
+        ----- lin_vel (vector of 3 values)
+        ----- lin_pos (vector of 3 values)
+        ----- previous_action (vector of 4 values)
+        ----- auxiliary information (vector of 4 values)
         - "target_deltas" (Sequence)
-            - list of body_frame distances to target (vector of 3/4 values)
+        ----- list of body_frame distances to target (vector of 3/4 values)
         """
         ang_vel, ang_pos, lin_vel, lin_pos, quarternion = super().compute_attitude()
         aux_state = super().compute_auxiliary()
 
         # combine everything
         new_state = dict()
         if self.angle_representation == 0:
```

### Comparing `PyFlyt-0.5.3/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.6.0/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
             collision_ignore_mask (np.ndarray | list[int]): list of ids to ignore collisions between
         """
         # exceed step count
         if self.step_count > self.max_steps:
             self.truncation = self.truncation or True
 
         # mask collisions if any
-        collision_array = self.env.collision_array.copy()
+        collision_array = self.env.contact_array.copy()
         for i, j in zip(collision_ignore_mask[1:], collision_ignore_mask[:-1]):
             collision_array[i, j] = False
             collision_array[j, i] = False
 
         # fatal collision or below ground
         if np.any(collision_array) or self.env.state(0)[-1, -1] < 0.0:
             # self.reward = -100.0
@@ -296,15 +296,15 @@
         Returns:
             state, reward, termination, truncation, info
         """
         # unsqueeze the action to be usable in aviary
         self.action = action.copy()
 
         # reset the reward and set the action
-        self.reward = -0.1
+        self.reward = 0.0
         self.env.set_setpoint(0, action)
 
         # step through env, the internal env updates a few steps before the outer env
         for _ in range(self.env_step_ratio):
             # if we've already ended, don't continue
             if self.termination or self.truncation:
                 break
```

### Comparing `PyFlyt-0.5.3/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.6.0/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Rocket Landing Environment."""
 from __future__ import annotations
 
 import os
 
 import numpy as np
+import pybullet as p
 from gymnasium.spaces import Box
 
 from .rocket_base_env import RocketBaseEnv
 
 
 class RocketLandingEnv(RocketBaseEnv):
     """Rocket Landing Environment.
@@ -22,15 +23,15 @@
     """
 
     def __init__(
         self,
         sparse_reward: bool = False,
         ceiling: float = 500.0,
         max_displacement: float = 200.0,
-        max_duration_seconds: float = 10.0,
+        max_duration_seconds: float = 30.0,
         angle_representation: str = "quaternion",
         agent_hz: int = 40,
         render_mode: None | str = None,
         render_resolution: tuple[int, int] = (480, 480),
     ):
         """__init__.
 
@@ -79,29 +80,31 @@
     def reset(self, seed=None, options=dict()):
         """Resets the environment.
 
         Args:
             seed: int
             options: None
         """
-        options = dict(randomize_drop=True, accelerate_drop=True)
+        options = dict(randomize_drop=False, accelerate_drop=True)
         drone_options = dict(starting_fuel_ratio=0.01)
 
         super().begin_reset(seed, options, drone_options)
 
         # reset the tracked parameters
-        self.ang_pos = np.zeros((3,))
+        self.landing_pad_contact = 0.0
+        self.ang_vel = np.zeros((3,))
+        self.lin_vel = np.zeros((3,))
+        self.distance = np.zeros((3,))
         self.previous_ang_vel = np.zeros((3,))
         self.previous_lin_vel = np.zeros((3,))
-        self.landing_pad_contact = 0.0
-        self.distance_to_pad = np.array([100.0, 100.0, 100.0])
+        self.previous_distance = np.zeros((3,))
 
         # randomly generate the target landing location
         theta = self.np_random.uniform(0.0, 2.0 * np.pi)
-        distance = self.np_random.uniform(0.0, 0.5 * self.max_displacement)
+        distance = self.np_random.uniform(0.0, 0.05 * self.ceiling)
         self.landing_pad_position = (
             np.array([np.cos(theta), np.sin(theta), 0.1]) * distance
         )
         self.landing_pad_id = self.env.loadURDF(
             self.targ_obj_dir,
             basePosition=self.landing_pad_position,
             useFixedBase=True,
@@ -118,101 +121,121 @@
         - ang_vel (vector of 3 values)
         - ang_pos (vector of 3/4 values)
         - lin_vel (vector of 3 values)
         - lin_pos (vector of 3 values)
         - previous_action (vector of 4 values)
         - auxiliary information (vector of 4 values)
         """
-        ang_vel, ang_pos, lin_vel, lin_pos, quarternion = super().compute_attitude()
+        # update the previous values to current values
+        self.previous_ang_vel = self.ang_vel.copy()
+        self.previous_lin_vel = self.lin_vel.copy()
+        self.previous_distance = self.distance.copy()
+
+        # update current values
+        (
+            self.ang_vel,
+            self.ang_pos,
+            self.lin_vel,
+            lin_pos,
+            quarternion,
+        ) = super().compute_attitude()
         aux_state = super().compute_auxiliary()
 
-        # store our angular position in euler
-        self.ang_pos = ang_pos
-
-        # drone to target
-        self.distance_to_pad = self.landing_pad_position - lin_pos
+        # drone to landing pad
+        # rotation = np.array(p.getMatrixFromQuaternion(quarternion)).reshape(3, 3)
+        # self.distance = np.matmul((lin_pos - self.landing_pad_position), rotation)
+        self.distance = lin_pos - self.landing_pad_position
 
         # combine everything
         if self.angle_representation == 0:
             self.state = np.array(
                 [
-                    *ang_vel,
-                    *ang_pos,
-                    *lin_vel,
+                    *self.ang_vel,
+                    *self.ang_pos,
+                    *self.lin_vel,
                     *lin_pos,
                     *self.action,
                     *aux_state,
                     self.landing_pad_contact,
-                    *self.distance_to_pad,
+                    *self.distance,
                 ]
             )
         elif self.angle_representation == 1:
             self.state = np.array(
                 [
-                    *ang_vel,
+                    *self.ang_vel,
                     *quarternion,
-                    *lin_vel,
+                    *self.lin_vel,
                     *lin_pos,
                     *self.action,
                     *aux_state,
                     self.landing_pad_contact,
-                    *self.distance_to_pad,
+                    *self.distance,
                 ]
             )
 
     def compute_term_trunc_reward(self):
         """Computes the termination, truncation, and reward of the current timestep."""
         super().compute_base_term_trunc_reward(
             collision_ignore_mask=[self.env.drones[0].Id, self.landing_pad_id]
         )
 
+        # compute reward
         if not self.sparse_reward:
-            # position, orientation, and angular velocity penalties
-            distance_to_pad = np.linalg.norm(self.distance_to_pad[:2] + 0.1)
-            self.reward += (
-                +(0.1 / np.linalg.norm(distance_to_pad))
-                - (0.1 * np.linalg.norm(distance_to_pad))
-                - (1.0 * np.linalg.norm(self.ang_pos[:2]))
-                - (0.2 * np.linalg.norm(self.state[0:3]))
+            # progress and distance to pad
+            progress_to_pad = float(  # noqa
+                np.linalg.norm(self.previous_distance[:2])
+                - np.linalg.norm(self.distance[:2])
             )
+            offset_to_pad = np.linalg.norm(self.distance[:2]) + 0.1  # noqa
 
-            # velocity penalty
-            # the closer we are to the landing pad, the more we care about velocity
-            # distance_scalar = 0.3 / np.linalg.norm(self.distance_to_pad)
-            # self.reward -= distance_scalar * np.linalg.norm(self.state[6:9])
-            #
+            # deceleration as long as we're still falling
+            deceleration_bonus = (  # noqa
+                max(
+                    (self.lin_vel[-1] < 0.0)
+                    * (self.lin_vel[-1] - self.previous_lin_vel[-1]),
+                    0.0,
+                )
+                / self.distance[-1]
+            )
+
+            # composite reward together
+            self.reward += (
+                # -5.0  # negative offset to discourage staying in the air
+                # + (1.0 / offset_to_pad)  # encourage being near the pad
+                # + (500.0 * progress_to_pad)  # encourage progress to landing pad
+                -(1.0 * abs(self.ang_vel[-1]))  # minimize spinning
+                - (1.0 * np.linalg.norm(self.ang_pos[:2]))  # penalize aggressive angles
+                # + (5.0 * deceleration_bonus)  # reward deceleration when near pad
+            )
 
         # check if we touched the landing pad
-        if not self.env.collision_array[self.env.drones[0].Id, self.landing_pad_id]:
-            # track the velocity for the next time
-            self.previous_ang_vel = self.state[0:3]
-            self.previous_lin_vel = self.state[6:9]
+        if self.env.contact_array[self.env.drones[0].Id, self.landing_pad_id]:
+            self.landing_pad_contact = 1.0
+            self.reward += 20
+        else:
             self.landing_pad_contact = 0.0
             return
 
-        # update that we touched the landing pad
-        self.landing_pad_contact = 1.0
-
         # if collision has more than 0.35 rad/s angular velocity, we dead
         # truthfully, if collision has more than 0.55 m/s linear acceleration, we dead
         # number taken from here:
         # https://cosmosmagazine.com/space/launch-land-repeat-reusable-rockets-explained/
         # but doing so is kinda impossible for RL, so I've lessened the requirement to 1.0
         if (
             np.linalg.norm(self.previous_ang_vel) > 0.35
             or np.linalg.norm(self.previous_lin_vel) > 1.0
         ):
-            # self.reward = -20.0
             self.info["fatal_collision"] = True
             self.termination |= True
             return
 
         # if our both velocities are less than 0.02 m/s and we upright, we LANDED!
         if (
             np.linalg.norm(self.previous_ang_vel) < 0.02
             and np.linalg.norm(self.previous_lin_vel) < 0.02
-            and np.linalg.norm(self.state[3:5]) < 0.1
+            and np.linalg.norm(self.ang_pos[:2]) < 0.1
         ):
-            self.reward = 100.0
+            self.reward += 500.0
             self.info["env_complete"] = True
             self.termination |= True
             return
```

### Comparing `PyFlyt-0.5.3/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.6.0/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,18 +111,18 @@
 
         Args:
             ang_pos (np.ndarray): ang_pos
             lin_pos (np.ndarray): lin_pos
             quarternion (np.ndarray): quarternion
         """
         # rotation matrix
-        rotation = np.array(self.p.getMatrixFromQuaternion(quarternion)).reshape(3, 3).T
+        rotation = np.array(self.p.getMatrixFromQuaternion(quarternion)).reshape(3, 3)
 
         # drone to target
-        target_deltas = np.matmul(rotation, (self.targets - lin_pos).T).T
+        target_deltas = np.matmul((self.targets - lin_pos), rotation)
 
         # record distance to the next target
         self.old_distance = self.new_distance
         self.new_distance = float(np.linalg.norm(target_deltas[0]))
 
         if self.use_yaw_targets:
             yaw_errors = self.yaw_targets - ang_pos[-1]
```

### Comparing `PyFlyt-0.5.3/PyFlyt/models/race_gate.urdf` & `PyFlyt-0.6.0/PyFlyt/models/race_gate.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/models/vehicles/cf2x/cf2.dae` & `PyFlyt-0.6.0/PyFlyt/models/vehicles/cf2x/cf2.dae`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/models/vehicles/cf2x/cf2x.urdf` & `PyFlyt-0.6.0/PyFlyt/models/vehicles/cf2x/cf2x.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/models/vehicles/cf2x/cf2x.yaml` & `PyFlyt-0.6.0/PyFlyt/models/vehicles/cf2x/cf2x.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf` & `PyFlyt-0.6.0/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml` & `PyFlyt-0.6.0/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf` & `PyFlyt-0.6.0/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml` & `PyFlyt-0.6.0/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/models/vehicles/quadplane/quadplane.urdf` & `PyFlyt-0.6.0/PyFlyt/models/vehicles/quadplane/quadplane.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/models/vehicles/quadplane/quadplane.yaml` & `PyFlyt-0.6.0/PyFlyt/models/vehicles/quadplane/quadplane.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt/models/vehicles/rocket/rocket.urdf` & `PyFlyt-0.6.0/PyFlyt/models/vehicles/rocket/rocket.urdf`

 * *Files 2% similar despite different names*

#### Comparing `PyFlyt-0.5.3/PyFlyt/models/vehicles/rocket/rocket.urdf` & `PyFlyt-0.6.0/PyFlyt/models/vehicles/rocket/rocket.urdf`

```diff
@@ -23,16 +23,16 @@
   </material>
   <material name="yellow">
     <color rgba="1.0 0.8 0.0 1.0"/>
   </material>
   <link name="base_link">
     <inertial>
       <origin rpy="0 0 0" xyz="0 0 0"/>
-      <mass value="69.0"/>
-      <inertia ixx="282.5" ixy="0" ixz="0" iyy="282.5" iyz="0" izz="1.18"/>
+      <mass value="91.0"/>
+      <inertia ixx="372.6" ixy="0" ixz="0" iyy="372.6" iyz="0" izz="1.55"/>
     </inertial>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
         <cylinder radius="0.185" length="4.77"/>
       </geometry>
     </collision>
@@ -60,16 +60,16 @@
     <origin rpy="0 0 0" xyz="0 0 0"/>
     <parent link="base_link"/>
     <child link="fueltank_link"/>
   </joint>
   <link name="booster_link">
     <inertial>
       <origin rpy="0 0 0" xyz="0 0 0"/>
-      <mass value="69.0"/>
-      <inertia ixx="282.5" ixy="0" ixz="0" iyy="282.5" iyz="0" izz="1.18"/>
+      <mass value="47"/>
+      <inertia ixx="192.43" ixy="0" ixz="0" iyy="192.43" iyz="0" izz="0.81"/>
     </inertial>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
         <cylinder radius="0.25" length="0.5"/>
       </geometry>
     </collision>
```

### Comparing `PyFlyt-0.5.3/PyFlyt/models/vehicles/rocket/rocket.yaml` & `PyFlyt-0.6.0/PyFlyt/models/vehicles/rocket/rocket.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.6.0/PyFlyt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.5.3
+Version: 0.6.0
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -37,16 +37,18 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![hits](https://hits.dwyl.com/jjshoots/PyFlyt.svg)](https://hits.dwyl.com/jjshoots/PyFlyt)
 [![total downloads](https://static.pepy.tech/personalized-badge/pyflyt?period=total&units=international_system&left_color=grey&right_color=green&left_text=total%20downloads)](https://pepy.tech/project/pyflyt)
 [![weekly downloads](https://static.pepy.tech/personalized-badge/pyflyt?period=week&units=international_system&left_color=grey&right_color=green&left_text=weekly%20downloads)](https://pepy.tech/project/pyflyt)
 
 # PyFlyt - UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research
 
+## [View the documentation here!](https://jjshoots.github.io/PyFlyt/documentation.html)
+
 <p align="center">
-    <img src="https://github.com/jjshoots/PyFlyt/blob/master/readme_assets/pyflyt_cover_photo.png?raw=true" width="800px"/>
+    <img src="https://github.com/jjshoots/PyFlyt/blob/master/readme_assets/pyflyt_cover_photo.png?raw=true" width="650px"/>
 </p>
 
 This is a library for testing reinforcement learning algorithms on UAVs.
 This repo is still under development.
 We are also actively looking for users and developers, if this sounds like you, don't hesitate to get in touch!
 
 PyFlyt currently supports two separate UAV platforms:
@@ -84,25 +86,23 @@
 
 ## Usage
 
 Usage is similar to any other Gymnasium and (soon) PettingZoo environment:
 
 ```py
 import gymnasium
-import PyFlyt.gym_envs
-
-env = gymnasium.make("PyFlyt/QuadX-Hover-v0")
+import PyFlyt.gym_envs # noqa
 
-# omit the below line to remove rendering and let the simulation go as fast as possible
-env.render()
+env = gymnasium.make("PyFlyt/QuadX-Hover-v0", render_mode="human")
 obs = env.reset()
 
 termination = False
 truncation = False
-while not termination and not truncation:
+
+while not termination or truncation:
     observation, reward, termination, truncation, info = env.step(env.action_space.sample())
 ```
 
 ## Environments
 
 ### `PyFlyt/QuadX-Hover-v0`
```

### Comparing `PyFlyt-0.5.3/PyFlyt.egg-info/SOURCES.txt` & `PyFlyt-0.6.0/PyFlyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/pyproject.toml` & `PyFlyt-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.5.3"
+version = "0.6.0"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `PyFlyt-0.5.3/readme.md` & `PyFlyt-0.6.0/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![hits](https://hits.dwyl.com/jjshoots/PyFlyt.svg)](https://hits.dwyl.com/jjshoots/PyFlyt)
 [![total downloads](https://static.pepy.tech/personalized-badge/pyflyt?period=total&units=international_system&left_color=grey&right_color=green&left_text=total%20downloads)](https://pepy.tech/project/pyflyt)
 [![weekly downloads](https://static.pepy.tech/personalized-badge/pyflyt?period=week&units=international_system&left_color=grey&right_color=green&left_text=weekly%20downloads)](https://pepy.tech/project/pyflyt)
 
 # PyFlyt - UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research
 
+## [View the documentation here!](https://jjshoots.github.io/PyFlyt/documentation.html)
+
 <p align="center">
-    <img src="https://github.com/jjshoots/PyFlyt/blob/master/readme_assets/pyflyt_cover_photo.png?raw=true" width="800px"/>
+    <img src="https://github.com/jjshoots/PyFlyt/blob/master/readme_assets/pyflyt_cover_photo.png?raw=true" width="650px"/>
 </p>
 
 This is a library for testing reinforcement learning algorithms on UAVs.
 This repo is still under development.
 We are also actively looking for users and developers, if this sounds like you, don't hesitate to get in touch!
 
 PyFlyt currently supports two separate UAV platforms:
@@ -49,25 +51,23 @@
 
 ## Usage
 
 Usage is similar to any other Gymnasium and (soon) PettingZoo environment:
 
 ```py
 import gymnasium
-import PyFlyt.gym_envs
-
-env = gymnasium.make("PyFlyt/QuadX-Hover-v0")
+import PyFlyt.gym_envs # noqa
 
-# omit the below line to remove rendering and let the simulation go as fast as possible
-env.render()
+env = gymnasium.make("PyFlyt/QuadX-Hover-v0", render_mode="human")
 obs = env.reset()
 
 termination = False
 truncation = False
-while not termination and not truncation:
+
+while not termination or truncation:
     observation, reward, termination, truncation, info = env.step(env.action_space.sample())
 ```
 
 ## Environments
 
 ### `PyFlyt/QuadX-Hover-v0`
```

### Comparing `PyFlyt-0.5.3/tests/test_core.py` & `PyFlyt-0.6.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.5.3/tests/test_gym_envs.py` & `PyFlyt-0.6.0/tests/test_gym_envs.py`

 * *Files identical despite different names*

