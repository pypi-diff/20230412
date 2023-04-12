# Comparing `tmp/control-lab-ly-1.0.0a0.tar.gz` & `tmp/control-lab-ly-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-lab-ly-1.0.0a0.tar", last modified: Tue Apr 11 17:19:36 2023, max compression
+gzip compressed data, was "control-lab-ly-1.0.0b0.tar", last modified: Wed Apr 12 15:59:31 2023, max compression
```

## Comparing `control-lab-ly-1.0.0a0.tar` & `control-lab-ly-1.0.0b0.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:36.154237 control-lab-ly-1.0.0a0/
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.0a0/LICENSE.md
--rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/MANIFEST.in
--rw-rw-rw-   0        0        0    13972 2023-04-11 17:19:36.157240 control-lab-ly-1.0.0a0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.610645 control-lab-ly-1.0.0a0/docs/
--rw-rw-rw-   0        0        0     3251 2023-04-06 08:36:33.000000 control-lab-ly-1.0.0a0/docs/CHANGELOG.md
--rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.0.0a0/docs/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.0a0/docs/LICENSE.md
--rw-rw-rw-   0        0        0     9601 2023-03-10 02:06:03.000000 control-lab-ly-1.0.0a0/docs/README.md
--rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/pyproject.toml
--rw-rw-rw-   0        0        0     1542 2023-04-11 17:19:36.165240 control-lab-ly-1.0.0a0/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.0.0a0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.187089 control-lab-ly-1.0.0a0/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.715250 control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/
--rw-rw-rw-   0        0        0    13972 2023-04-11 17:19:32.000000 control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7306 2023-04-11 17:19:33.000000 control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 17:19:33.000000 control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2023-04-11 17:19:33.000000 control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 17:19:33.000000 control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.718528 control-lab-ly-1.0.0a0/src/controllably/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.721526 control-lab-ly-1.0.0a0/src/controllably/Analyse/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.732654 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.750585 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Database/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Database/__init__.py
--rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Database/database_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.814894 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/
--rw-rw-rw-   0        0        0      277 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/__init__.py
--rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/circuit_datatype.py
--rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/eis_datatype.py
--rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
--rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/eis_tests.json
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.823440 control-lab-ly-1.0.0a0/src/controllably/Analyse/Visualisation/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Visualisation/__init__.py
--rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Visualisation/visualisation_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.852140 control-lab-ly-1.0.0a0/src/controllably/Compound/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.874727 control-lab-ly-1.0.0a0/src/controllably/Compound/LiquidMover/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.903288 control-lab-ly-1.0.0a0/src/controllably/Compound/LiquidMover/Opentrons/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
--rw-rw-rw-   0        0        0      259 2023-04-11 13:56:49.000000 control-lab-ly-1.0.0a0/src/controllably/Compound/LiquidMover/__init__.py
--rw-rw-rw-   0        0        0    14057 2023-04-11 13:56:45.000000 control-lab-ly-1.0.0a0/src/controllably/Compound/LiquidMover/liquidmover_utils.py
--rw-rw-rw-   0        0        0      241 2023-04-11 13:56:26.000000 control-lab-ly-1.0.0a0/src/controllably/Compound/__init__.py
--rw-rw-rw-   0        0        0     8733 2023-04-11 13:56:17.000000 control-lab-ly-1.0.0a0/src/controllably/Compound/compound_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.907295 control-lab-ly-1.0.0a0/src/controllably/Control/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.031250 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/
--rw-rw-rw-   0        0        0      516 2023-04-11 14:00:31.000000 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/__init__.py
--rw-rw-rw-   0        0        0    30932 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/_guibuilder.py
--rw-rw-rw-   0        0        0    17704 2023-04-11 14:06:14.000000 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/gui_utils.py
--rw-rw-rw-   0        0        0      886 2023-04-11 13:59:24.000000 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/loader_panel.py
--rw-rw-rw-   0        0        0     8608 2023-04-11 13:59:13.000000 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/measurer_panel.py
--rw-rw-rw-   0        0        0    15405 2023-04-11 13:58:21.000000 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/mover_panel.py
--rw-rw-rw-   0        0        0     3624 2023-04-11 13:59:00.000000 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/viewer_panel.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.063378 control-lab-ly-1.0.0a0/src/controllably/Control/Schedule/
--rw-rw-rw-   0        0        0      147 2023-04-11 14:01:57.000000 control-lab-ly-1.0.0a0/src/controllably/Control/Schedule/__init__.py
--rw-rw-rw-   0        0        0     1868 2023-04-11 14:01:25.000000 control-lab-ly-1.0.0a0/src/controllably/Control/Schedule/schedule_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Control/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.106680 control-lab-ly-1.0.0a0/src/controllably/Make/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.146597 control-lab-ly-1.0.0a0/src/controllably/Make/Heat/
--rw-rw-rw-   0        0        0      225 2023-04-11 14:04:55.000000 control-lab-ly-1.0.0a0/src/controllably/Make/Heat/__init__.py
--rw-rw-rw-   0        0        0    10393 2023-04-11 14:39:53.000000 control-lab-ly-1.0.0a0/src/controllably/Make/Heat/peltier_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.181769 control-lab-ly-1.0.0a0/src/controllably/Make/Light/
--rw-rw-rw-   0        0        0      218 2023-04-11 14:07:39.000000 control-lab-ly-1.0.0a0/src/controllably/Make/Light/__init__.py
--rw-rw-rw-   0        0        0     9094 2023-04-11 14:08:32.000000 control-lab-ly-1.0.0a0/src/controllably/Make/Light/led_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.208516 control-lab-ly-1.0.0a0/src/controllably/Make/Mixture/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Make/Mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.239790 control-lab-ly-1.0.0a0/src/controllably/Make/ThinFilm/
--rw-rw-rw-   0        0        0      268 2023-04-11 14:09:21.000000 control-lab-ly-1.0.0a0/src/controllably/Make/ThinFilm/__init__.py
--rw-rw-rw-   0        0        0     9660 2023-04-11 14:10:14.000000 control-lab-ly-1.0.0a0/src/controllably/Make/ThinFilm/spinner_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-11 14:03:24.000000 control-lab-ly-1.0.0a0/src/controllably/Make/__init__.py
--rw-rw-rw-   0        0        0     3956 2023-04-11 14:04:05.000000 control-lab-ly-1.0.0a0/src/controllably/Make/make_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.319995 control-lab-ly-1.0.0a0/src/controllably/Measure/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.350929 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.434609 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/
--rw-rw-rw-   0        0        0      314 2023-04-11 14:50:27.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/__init__.py
--rw-rw-rw-   0        0        0    18015 2023-04-11 14:53:07.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/keithley_device.py
--rw-rw-rw-   0        0        0     7492 2023-04-11 14:52:34.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
--rw-rw-rw-   0        0        0     2102 2023-04-11 14:53:27.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.453778 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/programs/
--rw-rw-rw-   0        0        0      401 2023-04-11 14:54:22.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
--rw-rw-rw-   0        0        0    10256 2023-04-11 14:55:55.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-11 14:26:43.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/electrical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.482125 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.531624 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/
--rw-rw-rw-   0        0        0      334 2023-04-11 14:32:40.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
--rw-rw-rw-   0        0        0    10329 2023-04-11 14:40:14.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
--rw-rw-rw-   0        0        0     3163 2023-04-11 14:36:04.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
--rw-rw-rw-   0        0        0     2093 2023-04-11 14:34:20.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.569223 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
--rw-rw-rw-   0        0        0      350 2023-04-11 14:46:27.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
--rw-rw-rw-   0        0        0     3973 2023-04-11 14:48:39.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-11 14:27:13.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/mechanical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.614198 control-lab-ly-1.0.0a0/src/controllably/Measure/Physical/
--rw-rw-rw-   0        0        0      249 2023-04-11 14:29:04.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Physical/__init__.py
--rw-rw-rw-   0        0        0     7972 2023-04-11 14:40:46.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Physical/balance_utils.py
--rw-rw-rw-   0        0        0      535 2023-04-11 14:28:21.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/__init__.py
--rw-rw-rw-   0        0        0     5398 2023-04-11 14:13:18.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/instrument_utils.py
--rw-rw-rw-   0        0        0    13804 2023-04-11 14:14:10.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/measure_utils.py
--rw-rw-rw-   0        0        0     4176 2023-04-11 14:24:57.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/program_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.642989 control-lab-ly-1.0.0a0/src/controllably/Move/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.713661 control-lab-ly-1.0.0a0/src/controllably/Move/Cartesian/
--rw-rw-rw-   0        0        0      346 2023-04-11 15:42:35.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Cartesian/__init__.py
--rw-rw-rw-   0        0        0     9049 2023-04-11 15:43:28.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Cartesian/cartesian_utils.py
--rw-rw-rw-   0        0        0     3402 2023-04-11 15:44:47.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Cartesian/ender_utils.py
--rw-rw-rw-   0        0        0     2853 2023-04-11 15:45:04.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Cartesian/primitiv_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.740121 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.833086 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/
--rw-rw-rw-   0        0        0      336 2023-04-11 15:48:58.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.865186 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
--rw-rw-rw-   0        0        0    24262 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
--rw-rw-rw-   0        0        0    15851 2023-04-11 16:10:31.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/dobot_utils.py
--rw-rw-rw-   0        0        0     7030 2023-04-11 15:51:52.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
--rw-rw-rw-   0        0        0     4325 2023-04-11 15:52:41.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/mg400_utils.py
--rw-rw-rw-   0        0        0      233 2023-04-11 15:46:16.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/__init__.py
--rw-rw-rw-   0        0        0    10507 2023-04-11 15:45:49.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/jointed_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-11 15:40:54.000000 control-lab-ly-1.0.0a0/src/controllably/Move/__init__.py
--rw-rw-rw-   0        0        0    32152 2023-04-11 16:11:01.000000 control-lab-ly-1.0.0a0/src/controllably/Move/move_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.898471 control-lab-ly-1.0.0a0/src/controllably/Transfer/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.954513 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.001141 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.063594 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/
--rw-rw-rw-   0        0        0      255 2023-04-11 16:17:38.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
--rw-rw-rw-   0        0        0     3460 2023-04-11 16:21:03.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
--rw-rw-rw-   0        0        0    29831 2023-04-11 16:19:04.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
--rw-rw-rw-   0        0        0      332 2023-04-11 16:16:26.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/__init__.py
--rw-rw-rw-   0        0        0     9064 2023-04-11 16:16:52.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
--rw-rw-rw-   0        0        0     3097 2023-04-11 16:15:20.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.112849 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Sartorius/
--rw-rw-rw-   0        0        0      252 2023-04-11 16:13:12.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Sartorius/__init__.py
--rw-rw-rw-   0        0        0     3210 2023-04-11 16:12:23.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
--rw-rw-rw-   0        0        0    30582 2023-04-11 16:14:25.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
--rw-rw-rw-   0        0        0      364 2023-04-11 16:04:51.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/__init__.py
--rw-rw-rw-   0        0        0    13126 2023-04-11 16:03:59.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/liquid_utils.py
--rw-rw-rw-   0        0        0     3413 2023-04-11 16:06:49.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/syringe_lib.py
--rw-rw-rw-   0        0        0    14619 2023-04-11 16:04:45.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/syringe_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.128095 control-lab-ly-1.0.0a0/src/controllably/Transfer/Powder/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Powder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.165640 control-lab-ly-1.0.0a0/src/controllably/Transfer/Substrate/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.200245 control-lab-ly-1.0.0a0/src/controllably/Transfer/Substrate/Dobot/
--rw-rw-rw-   0        0        0      348 2023-04-11 17:00:43.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Substrate/Dobot/__init__.py
--rw-rw-rw-   0        0        0     8255 2023-04-11 17:04:17.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
--rw-rw-rw-   0        0        0      238 2023-04-11 16:59:01.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Substrate/__init__.py
--rw-rw-rw-   0        0        0     1032 2023-04-11 16:59:39.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Substrate/substrate_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/transfer_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.269947 control-lab-ly-1.0.0a0/src/controllably/View/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.308060 control-lab-ly-1.0.0a0/src/controllably/View/Classifiers/
--rw-rw-rw-   0        0        0      333 2023-04-11 16:27:05.000000 control-lab-ly-1.0.0a0/src/controllably/View/Classifiers/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-04-11 16:27:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Classifiers/classifier_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.333310 control-lab-ly-1.0.0a0/src/controllably/View/Optical/
--rw-rw-rw-   0        0        0      219 2023-04-11 16:28:38.000000 control-lab-ly-1.0.0a0/src/controllably/View/Optical/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-11 16:29:18.000000 control-lab-ly-1.0.0a0/src/controllably/View/Optical/optical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.355311 control-lab-ly-1.0.0a0/src/controllably/View/Optical/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/View/Optical/placeholders/__init__.py
--rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Optical/placeholders/optical_camera.png
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.392852 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.412779 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.559395 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/__init__.py
--rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8.py
--rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
--rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
--rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
--rw-rw-rw-   0        0        0      219 2023-04-11 16:29:59.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.592206 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/placeholders/__init__.py
--rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/placeholders/infrared_camera.png
--rw-rw-rw-   0        0        0     2983 2023-04-11 16:30:36.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/thermal_utils.py
--rw-rw-rw-   0        0        0      294 2023-04-11 16:22:53.000000 control-lab-ly-1.0.0a0/src/controllably/View/__init__.py
--rw-rw-rw-   0        0        0    15729 2023-04-11 16:25:00.000000 control-lab-ly-1.0.0a0/src/controllably/View/image_utils.py
--rw-rw-rw-   0        0        0    17366 2023-04-11 16:26:02.000000 control-lab-ly-1.0.0a0/src/controllably/View/view_utils.py
--rw-rw-rw-   0        0        0       98 2023-04-11 16:48:22.000000 control-lab-ly-1.0.0a0/src/controllably/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.759907 control-lab-ly-1.0.0a0/src/controllably/misc/
--rw-rw-rw-   0        0        0      586 2023-04-11 15:22:32.000000 control-lab-ly-1.0.0a0/src/controllably/misc/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-04-11 15:11:11.000000 control-lab-ly-1.0.0a0/src/controllably/misc/decorators.py
--rw-rw-rw-   0        0        0    10014 2023-04-11 15:09:55.000000 control-lab-ly-1.0.0a0/src/controllably/misc/factory.py
--rw-rw-rw-   0        0        0     6551 2023-04-11 15:05:56.000000 control-lab-ly-1.0.0a0/src/controllably/misc/helper.py
--rw-rw-rw-   0        0        0    17274 2023-04-11 15:02:50.000000 control-lab-ly-1.0.0a0/src/controllably/misc/layout.py
--rw-rw-rw-   0        0        0     2867 2023-04-11 15:01:48.000000 control-lab-ly-1.0.0a0/src/controllably/misc/logger.py
--rw-rw-rw-   0        0        0     4576 2023-04-11 15:00:29.000000 control-lab-ly-1.0.0a0/src/controllably/misc/misc_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.802402 control-lab-ly-1.0.0a0/src/controllably/misc/templates/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.818489 control-lab-ly-1.0.0a0/src/controllably/misc/templates/configs/
--rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.870191 control-lab-ly-1.0.0a0/src/controllably/misc/templates/configs/plugins/
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/configs/plugins/__init__.py
--rw-rw-rw-   0        0        0     1092 2023-04-11 15:28:12.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/configs/plugins/plugin_template.py
--rw-rw-rw-   0        0        0      439 2023-04-11 15:17:49.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/configs/registry.yaml
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.910020 control-lab-ly-1.0.0a0/src/controllably/misc/templates/setup/
--rw-rw-rw-   0        0        0      772 2023-04-11 15:16:54.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/setup/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-11 15:27:46.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/setup/config.yaml
--rw-rw-rw-   0        0        0      987 2023-04-11 15:24:36.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/setup/layout.json
-drwxrwxrwx   0        0        0        0 2023-04-11 17:19:36.152238 control-lab-ly-1.0.0a0/tests/
--rw-rw-rw-   0        0        0      189 2023-04-11 09:35:43.000000 control-lab-ly-1.0.0a0/tests/test_camera_optical.py
--rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_camera_thermal.py
--rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_cartesian_ender.py
--rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_cartesian_primitiv.py
--rw-rw-rw-   0        0        0      585 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_compound_liquidmover.py
--rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_compound_spin_printer.py
--rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_dobot_m1pro.py
--rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_dobot_mg400.py
--rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_electrical_keithley.py
--rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_film_spin.py
--rw-rw-rw-   0        0        0      587 2023-04-11 09:21:52.000000 control-lab-ly-1.0.0a0/tests/test_heat_peltier.py
--rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_light_led_array.py
--rw-rw-rw-   0        0        0      362 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_liquid_sartorius.py
--rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_liquid_syringe_assembly.py
--rw-rw-rw-   0        0        0      578 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_liquid_tricontinent.py
--rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_mechanical_piezorobotics.py
--rw-rw-rw-   0        0        0      268 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_panels.py
--rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_physical_balance.py
--rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_pump_peristaltic.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:31.012549 control-lab-ly-1.0.0b0/
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.0b0/LICENSE.md
+-rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/MANIFEST.in
+-rw-rw-rw-   0        0        0    17511 2023-04-12 15:59:31.012549 control-lab-ly-1.0.0b0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.487610 control-lab-ly-1.0.0b0/docs/
+-rw-rw-rw-   0        0        0     4263 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/docs/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.0.0b0/docs/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.0b0/docs/LICENSE.md
+-rw-rw-rw-   0        0        0    12128 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/docs/README.md
+-rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0     1559 2023-04-12 15:59:31.012549 control-lab-ly-1.0.0b0/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.0.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.105592 control-lab-ly-1.0.0b0/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.579377 control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/
+-rw-rw-rw-   0        0        0    17511 2023-04-12 15:59:28.000000 control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7306 2023-04-12 15:59:29.000000 control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 15:59:28.000000 control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2023-04-12 15:59:28.000000 control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 15:59:28.000000 control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.588512 control-lab-ly-1.0.0b0/src/controllably/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.596525 control-lab-ly-1.0.0b0/src/controllably/Analyse/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.596525 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.612525 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Database/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Database/__init__.py
+-rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Database/database_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.644701 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/
+-rw-rw-rw-   0        0        0      277 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/__init__.py
+-rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/circuit_datatype.py
+-rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/eis_datatype.py
+-rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
+-rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/eis_tests.json
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.661282 control-lab-ly-1.0.0b0/src/controllably/Analyse/Visualisation/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Visualisation/__init__.py
+-rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/Visualisation/visualisation_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Analyse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.677673 control-lab-ly-1.0.0b0/src/controllably/Compound/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.693863 control-lab-ly-1.0.0b0/src/controllably/Compound/LiquidMover/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.721655 control-lab-ly-1.0.0b0/src/controllably/Compound/LiquidMover/Opentrons/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
+-rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Compound/LiquidMover/__init__.py
+-rw-rw-rw-   0        0        0    14057 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Compound/LiquidMover/liquidmover_utils.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Compound/__init__.py
+-rw-rw-rw-   0        0        0     8733 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Compound/compound_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.734897 control-lab-ly-1.0.0b0/src/controllably/Control/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.810279 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/
+-rw-rw-rw-   0        0        0      516 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/__init__.py
+-rw-rw-rw-   0        0        0    30932 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/_guibuilder.py
+-rw-rw-rw-   0        0        0    17704 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/gui_utils.py
+-rw-rw-rw-   0        0        0      886 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/loader_panel.py
+-rw-rw-rw-   0        0        0     8608 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/measurer_panel.py
+-rw-rw-rw-   0        0        0    15405 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/mover_panel.py
+-rw-rw-rw-   0        0        0     3624 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Control/GUI/viewer_panel.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.835322 control-lab-ly-1.0.0b0/src/controllably/Control/Schedule/
+-rw-rw-rw-   0        0        0      147 2023-04-11 14:01:57.000000 control-lab-ly-1.0.0b0/src/controllably/Control/Schedule/__init__.py
+-rw-rw-rw-   0        0        0     1868 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Control/Schedule/schedule_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.857550 control-lab-ly-1.0.0b0/src/controllably/Make/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.894688 control-lab-ly-1.0.0b0/src/controllably/Make/Heat/
+-rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/Heat/__init__.py
+-rw-rw-rw-   0        0        0    10393 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/Heat/peltier_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.920275 control-lab-ly-1.0.0b0/src/controllably/Make/Light/
+-rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/Light/__init__.py
+-rw-rw-rw-   0        0        0     9094 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/Light/led_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.935354 control-lab-ly-1.0.0b0/src/controllably/Make/Mixture/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Make/Mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:29.950711 control-lab-ly-1.0.0b0/src/controllably/Make/ThinFilm/
+-rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/ThinFilm/__init__.py
+-rw-rw-rw-   0        0        0     9660 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/ThinFilm/spinner_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/__init__.py
+-rw-rw-rw-   0        0        0     3956 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Make/make_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.007123 control-lab-ly-1.0.0b0/src/controllably/Measure/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.025165 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.079009 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/
+-rw-rw-rw-   0        0        0      314 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/__init__.py
+-rw-rw-rw-   0        0        0    18015 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/keithley_device.py
+-rw-rw-rw-   0        0        0     7492 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
+-rw-rw-rw-   0        0        0     2102 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.099136 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/programs/
+-rw-rw-rw-   0        0        0      401 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
+-rw-rw-rw-   0        0        0    10256 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/electrical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.112969 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.140213 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/
+-rw-rw-rw-   0        0        0      334 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
+-rw-rw-rw-   0        0        0    10329 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
+-rw-rw-rw-   0        0        0     2093 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.160646 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
+-rw-rw-rw-   0        0        0      350 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
+-rw-rw-rw-   0        0        0     3973 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/mechanical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.169356 control-lab-ly-1.0.0b0/src/controllably/Measure/Physical/
+-rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Physical/__init__.py
+-rw-rw-rw-   0        0        0     7972 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/Physical/balance_utils.py
+-rw-rw-rw-   0        0        0      535 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/__init__.py
+-rw-rw-rw-   0        0        0     5398 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/instrument_utils.py
+-rw-rw-rw-   0        0        0    13804 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/measure_utils.py
+-rw-rw-rw-   0        0        0     4176 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Measure/program_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.185407 control-lab-ly-1.0.0b0/src/controllably/Move/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.211676 control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/
+-rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/__init__.py
+-rw-rw-rw-   0        0        0     9049 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/cartesian_utils.py
+-rw-rw-rw-   0        0        0     3402 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/ender_utils.py
+-rw-rw-rw-   0        0        0     2853 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/primitiv_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.228095 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.248401 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/
+-rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.264530 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/
+-rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
+-rw-rw-rw-   0        0        0    24262 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
+-rw-rw-rw-   0        0        0    15851 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/dobot_utils.py
+-rw-rw-rw-   0        0        0     7030 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+-rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/mg400_utils.py
+-rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/__init__.py
+-rw-rw-rw-   0        0        0    10507 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/jointed_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/__init__.py
+-rw-rw-rw-   0        0        0    32152 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Move/move_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.281075 control-lab-ly-1.0.0b0/src/controllably/Transfer/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.313773 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.336095 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.401096 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/
+-rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
+-rw-rw-rw-   0        0        0     3460 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
+-rw-rw-rw-   0        0        0    29831 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
+-rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/__init__.py
+-rw-rw-rw-   0        0        0     9064 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
+-rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.446322 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Sartorius/
+-rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Sartorius/__init__.py
+-rw-rw-rw-   0        0        0     3210 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
+-rw-rw-rw-   0        0        0    30582 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
+-rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/__init__.py
+-rw-rw-rw-   0        0        0    13126 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/liquid_utils.py
+-rw-rw-rw-   0        0        0     3413 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/syringe_lib.py
+-rw-rw-rw-   0        0        0    14619 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/syringe_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.460983 control-lab-ly-1.0.0b0/src/controllably/Transfer/Powder/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Powder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.513402 control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.529303 control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/Dobot/
+-rw-rw-rw-   0        0        0      348 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/Dobot/__init__.py
+-rw-rw-rw-   0        0        0     8255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
+-rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/__init__.py
+-rw-rw-rw-   0        0        0     1032 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/substrate_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/src/controllably/Transfer/transfer_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.553922 control-lab-ly-1.0.0b0/src/controllably/View/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.570365 control-lab-ly-1.0.0b0/src/controllably/View/Classifiers/
+-rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/Classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/Classifiers/classifier_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.586360 control-lab-ly-1.0.0b0/src/controllably/View/Optical/
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/Optical/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/Optical/optical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.610419 control-lab-ly-1.0.0b0/src/controllably/View/Optical/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0b0/src/controllably/View/Optical/placeholders/__init__.py
+-rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Optical/placeholders/optical_camera.png
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.618961 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.627009 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.667104 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/__init__.py
+-rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8.py
+-rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
+-rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
+-rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.683469 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/placeholders/__init__.py
+-rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/placeholders/infrared_camera.png
+-rw-rw-rw-   0        0        0     2983 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/Thermal/thermal_utils.py
+-rw-rw-rw-   0        0        0      294 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/__init__.py
+-rw-rw-rw-   0        0        0    15729 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/image_utils.py
+-rw-rw-rw-   0        0        0    17366 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/View/view_utils.py
+-rw-rw-rw-   0        0        0       98 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.748995 control-lab-ly-1.0.0b0/src/controllably/misc/
+-rw-rw-rw-   0        0        0      586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/decorators.py
+-rw-rw-rw-   0        0        0    10014 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/factory.py
+-rw-rw-rw-   0        0        0     6551 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/helper.py
+-rw-rw-rw-   0        0        0    17274 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/layout.py
+-rw-rw-rw-   0        0        0     2867 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/logger.py
+-rw-rw-rw-   0        0        0     4576 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/misc_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.756938 control-lab-ly-1.0.0b0/src/controllably/misc/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.779479 control-lab-ly-1.0.0b0/src/controllably/misc/templates/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.830516 control-lab-ly-1.0.0b0/src/controllably/misc/templates/configs/plugins/
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/configs/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/configs/plugins/plugin_template.py
+-rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/configs/registry.yaml
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:30.854517 control-lab-ly-1.0.0b0/src/controllably/misc/templates/setup/
+-rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/setup/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/setup/config.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2023-04-12 15:59:31.004546 control-lab-ly-1.0.0b0/tests/
+-rw-rw-rw-   0        0        0      189 2023-04-11 09:35:43.000000 control-lab-ly-1.0.0b0/tests/test_camera_optical.py
+-rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_camera_thermal.py
+-rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_cartesian_ender.py
+-rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_cartesian_primitiv.py
+-rw-rw-rw-   0        0        0      585 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_compound_liquidmover.py
+-rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_compound_spin_printer.py
+-rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_dobot_m1pro.py
+-rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_dobot_mg400.py
+-rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_electrical_keithley.py
+-rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_film_spin.py
+-rw-rw-rw-   0        0        0      587 2023-04-11 09:21:52.000000 control-lab-ly-1.0.0b0/tests/test_heat_peltier.py
+-rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_light_led_array.py
+-rw-rw-rw-   0        0        0      362 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_liquid_sartorius.py
+-rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_liquid_syringe_assembly.py
+-rw-rw-rw-   0        0        0      538 2023-04-12 15:51:49.000000 control-lab-ly-1.0.0b0/tests/test_liquid_tricontinent.py
+-rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_mechanical_piezorobotics.py
+-rw-rw-rw-   0        0        0      268 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_panels.py
+-rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_physical_balance.py
+-rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0b0/tests/test_pump_peristaltic.py
```

### Comparing `control-lab-ly-1.0.0a0/LICENSE.md` & `control-lab-ly-1.0.0b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/PKG-INFO` & `control-lab-ly-1.0.0b0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.0.0a0
+Version: 1.0.0b0
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -25,246 +25,291 @@
 
 # Control.lab.ly
 Lab Equipment Automation Package
 
 ## Description
 User-friendly package that enables flexible automation an reconfigurable setups for high-throughput experimentation and machine learning.
 
+## Package Structure
+1. Analyse
+2. Compound
+3. Control
+4. Make
+5. Measure
+6. Move
+7. Transfer
+8. View
+
 ## Device support
 - Make
-  - Multi-channel spin-coater \[Arduino\]
   - Multi-channel LED array \[Arduino\]
+  - Multi-channel spin-coater \[Arduino\]
   - Peltier device \[Arduino\]
 - Measure
   - (Keithley) 2450 Source Measure Unit (SMU) Instrument
   - (PiezoRobotics) Dynamic Mechanical Analyser (DMA)
   - Precision mass balance \[Arduino\]
 - Move
   - (Creality) Ender-3
   - (Dobot) M1 Pro
   - (Dobot) MG400
   - Primitiv \[Arduino\]
 - Transfer
+  - (Dobot) Gripper attachments
   - (Sartorius) rLINE® dispensing modules
   - (TriContinent) C Series syringe pumps
   - Peristaltic pump and syringe system \[Arduino\]
 - View
-  - (FLIR) AX8 thermal imaging camera - full functionality in development 
+  - (FLIR) AX8 thermal imaging camera - *full functionality in development*
   - Web cameras \[General\]
 
 ## Installation
+Control.lab.ly can be found on PyPI and can be installed easily with `pip install`.
 ```shell
 $ pip install control-lab-ly
 ```
 
-## Usage
-### Import package
-```python
-import controllably as lab
-```
-
-### [Optional] Set safety level for session
-```python
-lab.set_safety('high')  # Pauses for input before every move action
-lab.set_safety('low')   # Waits for countdown before every move action
-```
+## Basic Usage
+Simple start-up guide for basic usage of the package.
 
 ### Import desired class
 ```python
 from controllably.Move.Cartesian import Ender
 mover = Ender(...)
 mover.safeMoveTo((x,y,z))
 ```
 
 More details for each class / module / package can be explored by using the `help` function.
-
 ```python
 help(controllably.Move)   # help on package
 help(Ender)               # help on class
 help(mover)               # help on instance/object
 ```
 
 Alternatively, you can use the native `pydoc` documentation generator.
-
 ```shell
 $ python -m pydoc controllably.Move
-$ python -m pydoc controllably.Move.Cartesian.Ender
 ```
 
 >Tip: when using Interactive Python (IPython) (e.g. Jupyter notebooks), add a exclamation mark (`!`) in front of the shell command
 ```python
->>> !python -m pydoc controllably
+>>> !python -m pydoc controllably.Move
+>>> !python -m pydoc -b                 # Generates a static HTML site to browse package documentation
+```
+For basic usage, this is all you need to know. Check the documentation for more details on each respective class.
+
+---
+
+## Advanced Usage
+For more advanced uses, Control.lab.ly provides a host of tools to streamline the development of lab equipment automation.
+
+### 0. Import package
+The convention is to import Control-lab-ly as `lab`.
+```python
+import controllably as lab
 ```
 
-### Create new project
+### Contents
+1. Projects
+2. Setups
+3. Decks
+4. Safety measures
+5. Plugins
+
+### 1. Creating a new project
 Create a `/configs` folder in the base folder of your project repository to store all configuration related files from which the package will read from.\
 This only has to be done once when you first set up the project folder.
-
 ```python
 lab.create_configs()
 ```
 
 A different address may be used by different machines for the same device. To manage the different addresses used by different machines, you first need your machine's unique identifier.
-
 ```python
 # Get your machine's ID
 print(lab.Helper.get_node())
 ```
 
 A template of `registry.yaml` has also been added to the folder to hold the machine-specific addresses of your connected devices (i.e. COM ports).\
 Populate the YAML file in the format shown below.
-
 ```yaml
 ### registry.yaml ###
-'0123456789ABCDE':              # insert your machine's ID here (from the above step)
+'012345678901234':              # insert your machine's 15-digit ID here (from the above step)
     cam_index:                  # camera index of the connected imaging devices
       __cam_01__: 1             # keep the leading and trailing double underscores
       __cam_02__: 0
     port:                       # addresses of serial COM ports
       __device_01__: COM3       # keep the leading and trailing double underscores
       __device_02__: COM16
 ```
 
-To find the COM port address(es) of the device(s) that is/are currently connected to your machine, use
-
+To find the COM port address(es) of the device(s) that is/are currently connected to your machine, use:
 ```python
 lab.Helper.get_ports()
 ```
 
-### Create new setup
-Create a new folder for the configuration files of your new setup. If you had skipped the previous step of creating a project, calling `lab.create_setup` will also generate the required file structure. However, be sure to populate your machine ID and device addresses in the `registry.yaml` file.
+### 2. Creating a new setup
+Create a new folder for the configuration files of your new setup. If you had skipped the previous step of creating a project, calling `lab.create_setup()` will also generate the required file structure. However, be sure to populate your machine ID and device addresses in the `registry.yaml` file.
 
 ```python
-lab.create_setup(setup_name = "Setup01")
-# replace "Setup01" with the desired name for your setup
+lab.create_setup(setup_name = "_Setup01_")
+# replace "_Setup01_" with the desired name for your setup
 ```
+This creates a `/_Setup01_` folder that holds the configuration files for the setup, which includes `config.yaml` and `layout.json`.
 
-This creates a `/Setup01` folder that holds the configuration files for the setup, which includes `config.yaml` and `layout.json`.
-
-#### `config.yaml`
+#### 2.1 `config.yaml`
 Configuration and calibration values for your devices is stored in `config.yaml`.\
 Each configuration starts with the `name` of your device, then its `module`, `class`, and `settings`.
-
 ```yaml
-### config.yaml ###
-Device01:                                         # name of simple device (user-defined)
-  module: __module_name_01__                      # device module
-  class: __submodule_1A__.__class_1A__            # device class
+_Device01_:                                     # name of simple device (user-defined)
+  module: _module_name_01_                      # device module
+  class: _submodule_1A_._class_1A_              # device class
   settings:
-    port: __device_01__                           # port addresses defined in registry.yaml
-    __setting_A__: {'tuple': [300,0,200]}         # use keys to define the type of iterable
-    __setting_B__: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
+    port: __device_01__                         # port addresses defined in registry.yaml
+    _setting_A_: {'tuple': [300,0,200]}         # use keys to define the type of iterable
+    _setting_B_: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
 ```
 
 `Compound` devices are similarly configured. The configuration values for its component devices are defined under the `component_config` setting. The structure of the configuration values for the component devices are similar to that shown above, except indented to fall under the indentation of the `component_config` setting.
-
 ```yaml
-### config.yaml ###
-Device02:                                     # name of 'Compound' device (user-defined)
+_Device02_:                                     # name of 'Compound' device (user-defined)
   module: Compound                            
-  class: __submodule_2A__.__class_2A__
+  class: _submodule_2A_._class_2A_
   settings:
-    __setting_C__: 1                          # other settings for your 'Compound' device
-    component_config:                         # nest component configuration settings here
-      Component01:                            # name of component
-        module: __module_name_03__
-        class: __submodule_3A__.__class_3A__
+    _setting_C_: 1                              # other settings for your 'Compound' device
+    component_config:                           # nest component configuration settings here
+      _Component01_:                            # name of component
+        module: _module_name_03_
+        class: _submodule_3A_._class_3A_
         settings:
-          ip_address: '192.0.0.1'             # IP addresses do not vary between machines
-      Component02: 
-        module: __module_name_04__
-        class: __submodule_4A__.__class_4A__
+          ip_address: '192.0.0.1'               # IP addresses do not vary between machines
+      _Component02_: 
+        module: _module_name_04_
+        class: _submodule_4A_._class_4A_
         settings:
-          __setting_D__: 2                    # settings for your component device
+          _setting_D_: 2                        # settings for your component device
 ```
 
 Lastly, you can define shortcuts to quickly access components of `Compound` devices.
 ```yaml
-### config.yaml ###
 SHORTCUTS:
-  robot_arm: myCompoundDevice.mover
-  Nickname1: Device02.Component01
-  Nickname2: Device02.Component02
+  _Nickname1_: '_Device02_._Component01_'
+  _Nickname2_: '_Device02_._Component02_'
 ```
 
-#### `layout.json`
-Layout configuration of your physical workspace (`Deck`) will be stored in `layout.json`. This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block/module.
-
-This file is optional if your setup does not involve moving objects around in a pre-defined workspace, and hence a layout configuration may not be required.
+#### 2.2 `layout.json`
+Layout configuration of your physical workspace (`Deck`) will be stored in `layout.json`. This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block/object.
 
+*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a layout configuration may not be required.*
 ```json
 {
   "reference_points":{
     "1": ["_x01_","_y01_","_z01_"],
     "2": ["_x02_","_y02_","_z02_"]
   },
   "slots":{
     "1": {
-      "name": "Labware01",
+      "name": "_Labware01_",
       "exclusion_height": -1,
-      "filepath": "REPO/.../Labware01.json"
+      "filepath": "_repo_/.../_Labware01_.json"
     },
     "2": {
-      "name": "Labware02",
+      "name": "_Labware02_",
       "exclusion_height": 0,
-      "filepath": "REPO/.../Labware02.json"
+      "filepath": "_repo_/.../_Labware02_.json"
     },
     "3": {
-      "name": "Labware03",
+      "name": "_Labware03_",
       "exclusion_height": 10,
-      "filepath": "REPO/.../Labware03.json"
+      "filepath": "_repo_/.../_Labware03_.json"
     }
   }
 }
 ```
-
 In `reference_points`, the bottom-left coordinates of each slot in the workspace are defined. Slots are positions where Labware blocks may be placed.
 
-In `slots`, the name of each slot and the file reference for Labware block that occupies that slot are defined. The filepath starts with the repository's base folder name.\
+In `slots`, the name of each slot and the file reference for Labware block that occupies that slot are defined. The filepath starts with the repository's base folder name.
+
 The `exclusion_height` is the height (in mm) above the dimensions of the Labware block to steer clear from when performing move actions. Defaults to -1 (i.e. do not avoid).\
-\[Note: only applies to final coordinates. Does not guarantee avoidance when using point-to-point move actions. Use `safeMoveTo` instead.\]
+*(Note: only applies to final coordinates (i.e. destination). Does not guarantee collision avoidance when using point-to-point move actions. Use* `safeMoveTo()` *instead.)*
 
-### Load setup
-The initialisation of the setup occurs during the import `SETUP` from within `configs/Setup01`.
+#### 2.3 Load setup
+The initialisation of the setup occurs during the import `setup` from within `configs/_Setup01_`.
 
 ```python
 # Add repository folder to sys.path
 from pathlib import Path
 import sys
-REPO = 'REPO'
+REPO = '_repo_' 
+# replace "_repo_" with your base directory for the project
 ROOT = str(Path().absolute()).split(REPO)[0]
 sys.path.append(f'{ROOT}{REPO}')
 
 # Import the initialised setup
-from configs.Setup01 import SETUP
-this = SETUP
+from configs._Setup01_ import setup
+this = setup
+this._Device01_
+this._Nickname2_
 ```
-
 With `this`, you can access all the devices that you have defined in `configs.yaml`.
+
+### 3. Managing a deck
+*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a* `Deck` *may not be required.*
+
+#### 3.1 Loading a deck
+To load the `Deck` from the layout file, use the `loadDeck()` function.
 ```python
-this.myCompoundDevice
-this.robot_arm
-```
+from configs._Setup01_ import LAYOUT_FILE
+this._Device02_.loadDeck(LAYOUT_FILE)
+deck = this._Device02.deck
+``` 
 
-### Load deck
-To load the `Deck` from the layout file, use the `lab.load_deck` function.
+#### 3.2 Loading a Labware
+To load the `Labware` into the `Deck`, use the `load_labware()` method.
 ```python
-from configs.Setup01 import LAYOUT_FILE
-lab.load_deck(this.DeviceWithDeck, LAYOUT_FILE)
+deck.load_labware(...)
 ``` 
 
-## Package Structure
-1. Analyse
-2. Compound
-3. Control
-4. Make
-5. Measure
-6. Move
-7. Transfer
-8. View
+### 4. Setting up safety measures
+You can optionally set the safety policy for session. This has to be done before importing any of the classes.
+```python
+lab.set_safety('high')  # Pauses for input before every move action
+lab.set_safety('low')   # Waits for countdown before every move action
+# Import other classes from control-lab-ly only after setting the safety policy
+```
+
+### 5. Using plugins
+User-defined plugins can be integrated into Control.lab.ly without making additions or modifications to the package itself. All classes and functions can be found in `lab.modules`.
+```python
+print(lab.modules)  
+# view the entire package (only those that have been imported during the session)
+lab.modules.Make.Something.Good.myClass
+# this expression returns the registered class
+```
+
+#### 5.1 Directly registering a Class or Function
+You can import the class and register the object using the `Factory.register()` function.
+```python
+from my_module import myClass
+lab.Factory.register(myClass, "Make.Something.Good")
+```
+
+#### 5.2 Registering a Python module
+Alternatively, you can automatically register all Classes and Functions in a Python module just by importing it.\
+Declare a `__where__` global variable to indicate where to register the module.
+```python
+### my_module.py
+__where__ = "Make.Something.Good"                 # Where to register this module to
+def myClass:                                      # Main body of code goes here
+  ...
+from controllably import include_this_module
+include_this_module()                             # Registers only the Classes and Functions defined above in this .py file
+```
+At the end of the .py file, import and call  the `include_this_module()` function.
+
+---
 
 ## Dependencies
 - Dash (>=2.7.1)
 - Impedance (>=1.4.1)
 - Imutils (>=0.5.4)
 - Matplotlib (>=3.3.4)
 - Nest-asyncio (>=1.5.1)
@@ -288,46 +333,68 @@
 
 ## How to Contribute
 [Issues](https://github.com/kylejeanlewis/control-lab-le/issues) and feature requests are welcome!
 
 ## License
 This project is distributed under the [MIT License](https://github.com/kylejeanlewis/control-lab-le/blob/main/LICENSE).
 
+---
 # Change Log
 
 ## Unreleased
 *Items under development*
 
+## 1.0.0.x
+Major overhaul in package structure. Standardisation of methods and consolidation of common methods. First released 12 Apr 2023.
+### Added
+#### 1.0.0
+- Usage of Abstract Base Classes (ABCs) to define a base class with abstract methods that needs to be implemented through sub-classing
+- Usage of Protocols to provide an interface between different classes of objects
+- Usage of Dataclasses to store complex data 
+- Usage of decorators to modify methods
+- Introduced different functions to parse the program docstring and find program parameters
+### Changed
+#### 1.0.0
+- Standardised methods and consolidated common methods
+- Added type hints
+- Moved Dobot attachments from Mover to Transfer.Substrate
+- Split GUI Panels into individual files
+- Split Dobot arms into individual files
+- Split functions/methods in `misc.py` into individual files.
+- Changed `_flags` to a public attribute `flags`
+- Update documentation
+### Removed
+#### 1.0.0
+- Unnecessary commented-out blocks of code
+
 ## 0.0.4.x
 Introduced control for Peltier device and TriContinent Series C syringe pumps. First released 10 Mar 2023.
 ### Added
 #### 0.0.4
 - Added control for `Peltier`
   - set and get temperatures
   - hold temperatures for desired duration
   - checks if target temperature has been reached by checking power level lower than a threshold or time passed over a predefined duration, once the temperature is within tolerance
   - ability to record temperatures and timestamps 
 - Added control for `TriContinent` and `TriContinentEnsemble`
   - single actions such as `empty`, `fill`, `initialise`, move actions, set speeds and valves, and wait
   - compound actions such as `aspirate`, `dispense`, and `prime`
-
 ### Changed
 #### 0.0.4
 - Update documentation
 
 ## 0.0.3.x
 Minor changes to movement robot safety and pipette control. Introduced control for LED array. First released 08 Mar 2023.
 ### Added
 #### 0.0.3
 - Added safety measures for movement actions
   - In `Deck`, added exclusion zones when reading the `layout.json` file and new method `is_excluded()` to check if target coordinate is within the exclusion zone
   - In `Mover`, update `isFeasible()` method to check if target coordinates violates the deck's exclusion zone
   - New function `set_safety()` defines safety modes when starting a new session to pause for input (in "high" safety setting) and to wait for safety countdown (in "low" safety setting)
 - `Make.Light.LEDArray` for controlling LEDs in the photo-reactor, as well as timing the LED "on" durations
-
 ### Changed
 #### 0.0.3.1
 - Update documentation
 #### 0.0.3
 - `Sartorius`
   - made the blowout/home optional for the dispense method upon emptying the pipette
 - Update documentation
@@ -337,15 +404,14 @@
 ### Added
 #### 0.0.2.2
 - Added import of `CompoundSetup` class
 #### 0.0.2
 - `Deck.at()` method for directly referencing slots using either index numbers or names
 - New `CompoundSetup` class for common methods of `Compound` devices
 - New `load_deck()` function to load `Deck` after initialisation
-
 ### Changed
 #### 0.0.2.1
 - Changed template files for `lab.create_setup()`
 #### 0.0.2
 - Update documentation
 
 ## 0.0.1.x
```

### Comparing `control-lab-ly-1.0.0a0/docs/CODE_OF_CONDUCT.md` & `control-lab-ly-1.0.0b0/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/docs/LICENSE.md` & `control-lab-ly-1.0.0b0/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/docs/README.md` & `control-lab-ly-1.0.0b0/docs/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,245 +1,290 @@
 # Control.lab.ly
 Lab Equipment Automation Package
 
 ## Description
 User-friendly package that enables flexible automation an reconfigurable setups for high-throughput experimentation and machine learning.
 
+## Package Structure
+1. Analyse
+2. Compound
+3. Control
+4. Make
+5. Measure
+6. Move
+7. Transfer
+8. View
+
 ## Device support
 - Make
-  - Multi-channel spin-coater \[Arduino\]
   - Multi-channel LED array \[Arduino\]
+  - Multi-channel spin-coater \[Arduino\]
   - Peltier device \[Arduino\]
 - Measure
   - (Keithley) 2450 Source Measure Unit (SMU) Instrument
   - (PiezoRobotics) Dynamic Mechanical Analyser (DMA)
   - Precision mass balance \[Arduino\]
 - Move
   - (Creality) Ender-3
   - (Dobot) M1 Pro
   - (Dobot) MG400
   - Primitiv \[Arduino\]
 - Transfer
+  - (Dobot) Gripper attachments
   - (Sartorius) rLINE® dispensing modules
   - (TriContinent) C Series syringe pumps
   - Peristaltic pump and syringe system \[Arduino\]
 - View
-  - (FLIR) AX8 thermal imaging camera - full functionality in development 
+  - (FLIR) AX8 thermal imaging camera - *full functionality in development*
   - Web cameras \[General\]
 
 ## Installation
+Control.lab.ly can be found on PyPI and can be installed easily with `pip install`.
 ```shell
 $ pip install control-lab-ly
 ```
 
-## Usage
-### Import package
-```python
-import controllably as lab
-```
-
-### [Optional] Set safety level for session
-```python
-lab.set_safety('high')  # Pauses for input before every move action
-lab.set_safety('low')   # Waits for countdown before every move action
-```
+## Basic Usage
+Simple start-up guide for basic usage of the package.
 
 ### Import desired class
 ```python
 from controllably.Move.Cartesian import Ender
 mover = Ender(...)
 mover.safeMoveTo((x,y,z))
 ```
 
 More details for each class / module / package can be explored by using the `help` function.
-
 ```python
 help(controllably.Move)   # help on package
 help(Ender)               # help on class
 help(mover)               # help on instance/object
 ```
 
 Alternatively, you can use the native `pydoc` documentation generator.
-
 ```shell
 $ python -m pydoc controllably.Move
-$ python -m pydoc controllably.Move.Cartesian.Ender
 ```
 
 >Tip: when using Interactive Python (IPython) (e.g. Jupyter notebooks), add a exclamation mark (`!`) in front of the shell command
 ```python
->>> !python -m pydoc controllably
+>>> !python -m pydoc controllably.Move
+>>> !python -m pydoc -b                 # Generates a static HTML site to browse package documentation
 ```
+For basic usage, this is all you need to know. Check the documentation for more details on each respective class.
 
-### Create new project
+---
+
+## Advanced Usage
+For more advanced uses, Control.lab.ly provides a host of tools to streamline the development of lab equipment automation.
+
+### 0. Import package
+The convention is to import Control-lab-ly as `lab`.
+```python
+import controllably as lab
+```
+
+### Contents
+1. Projects
+2. Setups
+3. Decks
+4. Safety measures
+5. Plugins
+
+### 1. Creating a new project
 Create a `/configs` folder in the base folder of your project repository to store all configuration related files from which the package will read from.\
 This only has to be done once when you first set up the project folder.
-
 ```python
 lab.create_configs()
 ```
 
 A different address may be used by different machines for the same device. To manage the different addresses used by different machines, you first need your machine's unique identifier.
-
 ```python
 # Get your machine's ID
 print(lab.Helper.get_node())
 ```
 
 A template of `registry.yaml` has also been added to the folder to hold the machine-specific addresses of your connected devices (i.e. COM ports).\
 Populate the YAML file in the format shown below.
-
 ```yaml
 ### registry.yaml ###
-'0123456789ABCDE':              # insert your machine's ID here (from the above step)
+'012345678901234':              # insert your machine's 15-digit ID here (from the above step)
     cam_index:                  # camera index of the connected imaging devices
       __cam_01__: 1             # keep the leading and trailing double underscores
       __cam_02__: 0
     port:                       # addresses of serial COM ports
       __device_01__: COM3       # keep the leading and trailing double underscores
       __device_02__: COM16
 ```
 
-To find the COM port address(es) of the device(s) that is/are currently connected to your machine, use
-
+To find the COM port address(es) of the device(s) that is/are currently connected to your machine, use:
 ```python
 lab.Helper.get_ports()
 ```
 
-### Create new setup
-Create a new folder for the configuration files of your new setup. If you had skipped the previous step of creating a project, calling `lab.create_setup` will also generate the required file structure. However, be sure to populate your machine ID and device addresses in the `registry.yaml` file.
+### 2. Creating a new setup
+Create a new folder for the configuration files of your new setup. If you had skipped the previous step of creating a project, calling `lab.create_setup()` will also generate the required file structure. However, be sure to populate your machine ID and device addresses in the `registry.yaml` file.
 
 ```python
-lab.create_setup(setup_name = "Setup01")
-# replace "Setup01" with the desired name for your setup
+lab.create_setup(setup_name = "_Setup01_")
+# replace "_Setup01_" with the desired name for your setup
 ```
+This creates a `/_Setup01_` folder that holds the configuration files for the setup, which includes `config.yaml` and `layout.json`.
 
-This creates a `/Setup01` folder that holds the configuration files for the setup, which includes `config.yaml` and `layout.json`.
-
-#### `config.yaml`
+#### 2.1 `config.yaml`
 Configuration and calibration values for your devices is stored in `config.yaml`.\
 Each configuration starts with the `name` of your device, then its `module`, `class`, and `settings`.
-
 ```yaml
-### config.yaml ###
-Device01:                                         # name of simple device (user-defined)
-  module: __module_name_01__                      # device module
-  class: __submodule_1A__.__class_1A__            # device class
+_Device01_:                                     # name of simple device (user-defined)
+  module: _module_name_01_                      # device module
+  class: _submodule_1A_._class_1A_              # device class
   settings:
-    port: __device_01__                           # port addresses defined in registry.yaml
-    __setting_A__: {'tuple': [300,0,200]}         # use keys to define the type of iterable
-    __setting_B__: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
+    port: __device_01__                         # port addresses defined in registry.yaml
+    _setting_A_: {'tuple': [300,0,200]}         # use keys to define the type of iterable
+    _setting_B_: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
 ```
 
 `Compound` devices are similarly configured. The configuration values for its component devices are defined under the `component_config` setting. The structure of the configuration values for the component devices are similar to that shown above, except indented to fall under the indentation of the `component_config` setting.
-
 ```yaml
-### config.yaml ###
-Device02:                                     # name of 'Compound' device (user-defined)
+_Device02_:                                     # name of 'Compound' device (user-defined)
   module: Compound                            
-  class: __submodule_2A__.__class_2A__
+  class: _submodule_2A_._class_2A_
   settings:
-    __setting_C__: 1                          # other settings for your 'Compound' device
-    component_config:                         # nest component configuration settings here
-      Component01:                            # name of component
-        module: __module_name_03__
-        class: __submodule_3A__.__class_3A__
+    _setting_C_: 1                              # other settings for your 'Compound' device
+    component_config:                           # nest component configuration settings here
+      _Component01_:                            # name of component
+        module: _module_name_03_
+        class: _submodule_3A_._class_3A_
         settings:
-          ip_address: '192.0.0.1'             # IP addresses do not vary between machines
-      Component02: 
-        module: __module_name_04__
-        class: __submodule_4A__.__class_4A__
+          ip_address: '192.0.0.1'               # IP addresses do not vary between machines
+      _Component02_: 
+        module: _module_name_04_
+        class: _submodule_4A_._class_4A_
         settings:
-          __setting_D__: 2                    # settings for your component device
+          _setting_D_: 2                        # settings for your component device
 ```
 
 Lastly, you can define shortcuts to quickly access components of `Compound` devices.
 ```yaml
-### config.yaml ###
 SHORTCUTS:
-  robot_arm: myCompoundDevice.mover
-  Nickname1: Device02.Component01
-  Nickname2: Device02.Component02
+  _Nickname1_: '_Device02_._Component01_'
+  _Nickname2_: '_Device02_._Component02_'
 ```
 
-#### `layout.json`
-Layout configuration of your physical workspace (`Deck`) will be stored in `layout.json`. This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block/module.
-
-This file is optional if your setup does not involve moving objects around in a pre-defined workspace, and hence a layout configuration may not be required.
+#### 2.2 `layout.json`
+Layout configuration of your physical workspace (`Deck`) will be stored in `layout.json`. This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block/object.
 
+*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a layout configuration may not be required.*
 ```json
 {
   "reference_points":{
     "1": ["_x01_","_y01_","_z01_"],
     "2": ["_x02_","_y02_","_z02_"]
   },
   "slots":{
     "1": {
-      "name": "Labware01",
+      "name": "_Labware01_",
       "exclusion_height": -1,
-      "filepath": "REPO/.../Labware01.json"
+      "filepath": "_repo_/.../_Labware01_.json"
     },
     "2": {
-      "name": "Labware02",
+      "name": "_Labware02_",
       "exclusion_height": 0,
-      "filepath": "REPO/.../Labware02.json"
+      "filepath": "_repo_/.../_Labware02_.json"
     },
     "3": {
-      "name": "Labware03",
+      "name": "_Labware03_",
       "exclusion_height": 10,
-      "filepath": "REPO/.../Labware03.json"
+      "filepath": "_repo_/.../_Labware03_.json"
     }
   }
 }
 ```
-
 In `reference_points`, the bottom-left coordinates of each slot in the workspace are defined. Slots are positions where Labware blocks may be placed.
 
-In `slots`, the name of each slot and the file reference for Labware block that occupies that slot are defined. The filepath starts with the repository's base folder name.\
+In `slots`, the name of each slot and the file reference for Labware block that occupies that slot are defined. The filepath starts with the repository's base folder name.
+
 The `exclusion_height` is the height (in mm) above the dimensions of the Labware block to steer clear from when performing move actions. Defaults to -1 (i.e. do not avoid).\
-\[Note: only applies to final coordinates. Does not guarantee avoidance when using point-to-point move actions. Use `safeMoveTo` instead.\]
+*(Note: only applies to final coordinates (i.e. destination). Does not guarantee collision avoidance when using point-to-point move actions. Use* `safeMoveTo()` *instead.)*
 
-### Load setup
-The initialisation of the setup occurs during the import `SETUP` from within `configs/Setup01`.
+#### 2.3 Load setup
+The initialisation of the setup occurs during the import `setup` from within `configs/_Setup01_`.
 
 ```python
 # Add repository folder to sys.path
 from pathlib import Path
 import sys
-REPO = 'REPO'
+REPO = '_repo_' 
+# replace "_repo_" with your base directory for the project
 ROOT = str(Path().absolute()).split(REPO)[0]
 sys.path.append(f'{ROOT}{REPO}')
 
 # Import the initialised setup
-from configs.Setup01 import SETUP
-this = SETUP
+from configs._Setup01_ import setup
+this = setup
+this._Device01_
+this._Nickname2_
 ```
-
 With `this`, you can access all the devices that you have defined in `configs.yaml`.
+
+### 3. Managing a deck
+*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a* `Deck` *may not be required.*
+
+#### 3.1 Loading a deck
+To load the `Deck` from the layout file, use the `loadDeck()` function.
 ```python
-this.myCompoundDevice
-this.robot_arm
-```
+from configs._Setup01_ import LAYOUT_FILE
+this._Device02_.loadDeck(LAYOUT_FILE)
+deck = this._Device02.deck
+``` 
 
-### Load deck
-To load the `Deck` from the layout file, use the `lab.load_deck` function.
+#### 3.2 Loading a Labware
+To load the `Labware` into the `Deck`, use the `load_labware()` method.
 ```python
-from configs.Setup01 import LAYOUT_FILE
-lab.load_deck(this.DeviceWithDeck, LAYOUT_FILE)
+deck.load_labware(...)
 ``` 
 
-## Package Structure
-1. Analyse
-2. Compound
-3. Control
-4. Make
-5. Measure
-6. Move
-7. Transfer
-8. View
+### 4. Setting up safety measures
+You can optionally set the safety policy for session. This has to be done before importing any of the classes.
+```python
+lab.set_safety('high')  # Pauses for input before every move action
+lab.set_safety('low')   # Waits for countdown before every move action
+# Import other classes from control-lab-ly only after setting the safety policy
+```
+
+### 5. Using plugins
+User-defined plugins can be integrated into Control.lab.ly without making additions or modifications to the package itself. All classes and functions can be found in `lab.modules`.
+```python
+print(lab.modules)  
+# view the entire package (only those that have been imported during the session)
+lab.modules.Make.Something.Good.myClass
+# this expression returns the registered class
+```
+
+#### 5.1 Directly registering a Class or Function
+You can import the class and register the object using the `Factory.register()` function.
+```python
+from my_module import myClass
+lab.Factory.register(myClass, "Make.Something.Good")
+```
+
+#### 5.2 Registering a Python module
+Alternatively, you can automatically register all Classes and Functions in a Python module just by importing it.\
+Declare a `__where__` global variable to indicate where to register the module.
+```python
+### my_module.py
+__where__ = "Make.Something.Good"                 # Where to register this module to
+def myClass:                                      # Main body of code goes here
+  ...
+from controllably import include_this_module
+include_this_module()                             # Registers only the Classes and Functions defined above in this .py file
+```
+At the end of the .py file, import and call  the `include_this_module()` function.
+
+---
 
 ## Dependencies
 - Dash (>=2.7.1)
 - Impedance (>=1.4.1)
 - Imutils (>=0.5.4)
 - Matplotlib (>=3.3.4)
 - Nest-asyncio (>=1.5.1)
@@ -262,7 +307,9 @@
 
 
 ## How to Contribute
 [Issues](https://github.com/kylejeanlewis/control-lab-le/issues) and feature requests are welcome!
 
 ## License
 This project is distributed under the [MIT License](https://github.com/kylejeanlewis/control-lab-le/blob/main/LICENSE).
+
+---
```

### Comparing `control-lab-ly-1.0.0a0/setup.cfg` & `control-lab-ly-1.0.0b0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6e 7472 6f6c 2d6c 6162 2d6c   = control-lab-l
 00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e30  y..version = 1.0
-00000030: 2e30 2d61 0d0a 6465 7363 7269 7074 696f  .0-a..descriptio
+00000030: 2e30 2d62 0d0a 6465 7363 7269 7074 696f  .0-b..descriptio
 00000040: 6e20 3d20 4c61 6220 4571 7569 706d 656e  n = Lab Equipmen
 00000050: 7420 4175 746f 6d61 7469 6f6e 2050 6163  t Automation Pac
 00000060: 6b61 6765 0d0a 6c6f 6e67 5f64 6573 6372  kage..long_descr
 00000070: 6970 7469 6f6e 203d 2066 696c 653a 2064  iption = file: d
 00000080: 6f63 732f 5245 4144 4d45 2e6d 642c 2064  ocs/README.md, d
 00000090: 6f63 732f 4348 414e 4745 4c4f 472e 6d64  ocs/CHANGELOG.md
 000000a0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
@@ -84,14 +84,15 @@
 00000530: 7079 7365 7269 616c 3e3d 332e 350d 0a09  pyserial>=3.5...
 00000540: 5079 5369 6d70 6c65 4755 493e 3d34 2e36  PySimpleGUI>=4.6
 00000550: 300d 0a09 5079 5649 5341 3e3d 312e 3132  0...PyVISA>=1.12
 00000560: 0d0a 0950 7959 414d 4c3e 3d36 2e30 0d0a  ...PyYAML>=6.0..
 00000570: 0973 6369 7079 3e3d 312e 360d 0a0d 0a5b  .scipy>=1.6....[
 00000580: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
 00000590: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-000005a0: 7372 630d 0a0d 0a5b 6f70 7469 6f6e 732e  src....[options.
-000005b0: 7061 636b 6167 655f 6461 7461 5d0d 0a2a  package_data]..*
-000005c0: 203d 202a 2e6a 736f 6e2c 202a 2e79 616d   = *.json, *.yam
-000005d0: 6c2c 202a 2e70 6e67 0d0a 0d0a 5b65 6767  l, *.png....[egg
-000005e0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-000005f0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000600: 2030 0d0a 0d0a                            0....
+000005a0: 7372 630d 0a65 7863 6c75 6465 203d 2074  src..exclude = t
+000005b0: 6573 7473 0d0a 0d0a 5b6f 7074 696f 6e73  ests....[options
+000005c0: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
+000005d0: 2a20 3d20 2a2e 6a73 6f6e 2c20 2a2e 7961  * = *.json, *.ya
+000005e0: 6d6c 2c20 2a2e 706e 670d 0a0d 0a5b 6567  ml, *.png....[eg
+000005f0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000600: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000610: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/PKG-INFO` & `control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.0.0a0
+Version: 1.0.0b0
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -25,246 +25,291 @@
 
 # Control.lab.ly
 Lab Equipment Automation Package
 
 ## Description
 User-friendly package that enables flexible automation an reconfigurable setups for high-throughput experimentation and machine learning.
 
+## Package Structure
+1. Analyse
+2. Compound
+3. Control
+4. Make
+5. Measure
+6. Move
+7. Transfer
+8. View
+
 ## Device support
 - Make
-  - Multi-channel spin-coater \[Arduino\]
   - Multi-channel LED array \[Arduino\]
+  - Multi-channel spin-coater \[Arduino\]
   - Peltier device \[Arduino\]
 - Measure
   - (Keithley) 2450 Source Measure Unit (SMU) Instrument
   - (PiezoRobotics) Dynamic Mechanical Analyser (DMA)
   - Precision mass balance \[Arduino\]
 - Move
   - (Creality) Ender-3
   - (Dobot) M1 Pro
   - (Dobot) MG400
   - Primitiv \[Arduino\]
 - Transfer
+  - (Dobot) Gripper attachments
   - (Sartorius) rLINE® dispensing modules
   - (TriContinent) C Series syringe pumps
   - Peristaltic pump and syringe system \[Arduino\]
 - View
-  - (FLIR) AX8 thermal imaging camera - full functionality in development 
+  - (FLIR) AX8 thermal imaging camera - *full functionality in development*
   - Web cameras \[General\]
 
 ## Installation
+Control.lab.ly can be found on PyPI and can be installed easily with `pip install`.
 ```shell
 $ pip install control-lab-ly
 ```
 
-## Usage
-### Import package
-```python
-import controllably as lab
-```
-
-### [Optional] Set safety level for session
-```python
-lab.set_safety('high')  # Pauses for input before every move action
-lab.set_safety('low')   # Waits for countdown before every move action
-```
+## Basic Usage
+Simple start-up guide for basic usage of the package.
 
 ### Import desired class
 ```python
 from controllably.Move.Cartesian import Ender
 mover = Ender(...)
 mover.safeMoveTo((x,y,z))
 ```
 
 More details for each class / module / package can be explored by using the `help` function.
-
 ```python
 help(controllably.Move)   # help on package
 help(Ender)               # help on class
 help(mover)               # help on instance/object
 ```
 
 Alternatively, you can use the native `pydoc` documentation generator.
-
 ```shell
 $ python -m pydoc controllably.Move
-$ python -m pydoc controllably.Move.Cartesian.Ender
 ```
 
 >Tip: when using Interactive Python (IPython) (e.g. Jupyter notebooks), add a exclamation mark (`!`) in front of the shell command
 ```python
->>> !python -m pydoc controllably
+>>> !python -m pydoc controllably.Move
+>>> !python -m pydoc -b                 # Generates a static HTML site to browse package documentation
+```
+For basic usage, this is all you need to know. Check the documentation for more details on each respective class.
+
+---
+
+## Advanced Usage
+For more advanced uses, Control.lab.ly provides a host of tools to streamline the development of lab equipment automation.
+
+### 0. Import package
+The convention is to import Control-lab-ly as `lab`.
+```python
+import controllably as lab
 ```
 
-### Create new project
+### Contents
+1. Projects
+2. Setups
+3. Decks
+4. Safety measures
+5. Plugins
+
+### 1. Creating a new project
 Create a `/configs` folder in the base folder of your project repository to store all configuration related files from which the package will read from.\
 This only has to be done once when you first set up the project folder.
-
 ```python
 lab.create_configs()
 ```
 
 A different address may be used by different machines for the same device. To manage the different addresses used by different machines, you first need your machine's unique identifier.
-
 ```python
 # Get your machine's ID
 print(lab.Helper.get_node())
 ```
 
 A template of `registry.yaml` has also been added to the folder to hold the machine-specific addresses of your connected devices (i.e. COM ports).\
 Populate the YAML file in the format shown below.
-
 ```yaml
 ### registry.yaml ###
-'0123456789ABCDE':              # insert your machine's ID here (from the above step)
+'012345678901234':              # insert your machine's 15-digit ID here (from the above step)
     cam_index:                  # camera index of the connected imaging devices
       __cam_01__: 1             # keep the leading and trailing double underscores
       __cam_02__: 0
     port:                       # addresses of serial COM ports
       __device_01__: COM3       # keep the leading and trailing double underscores
       __device_02__: COM16
 ```
 
-To find the COM port address(es) of the device(s) that is/are currently connected to your machine, use
-
+To find the COM port address(es) of the device(s) that is/are currently connected to your machine, use:
 ```python
 lab.Helper.get_ports()
 ```
 
-### Create new setup
-Create a new folder for the configuration files of your new setup. If you had skipped the previous step of creating a project, calling `lab.create_setup` will also generate the required file structure. However, be sure to populate your machine ID and device addresses in the `registry.yaml` file.
+### 2. Creating a new setup
+Create a new folder for the configuration files of your new setup. If you had skipped the previous step of creating a project, calling `lab.create_setup()` will also generate the required file structure. However, be sure to populate your machine ID and device addresses in the `registry.yaml` file.
 
 ```python
-lab.create_setup(setup_name = "Setup01")
-# replace "Setup01" with the desired name for your setup
+lab.create_setup(setup_name = "_Setup01_")
+# replace "_Setup01_" with the desired name for your setup
 ```
+This creates a `/_Setup01_` folder that holds the configuration files for the setup, which includes `config.yaml` and `layout.json`.
 
-This creates a `/Setup01` folder that holds the configuration files for the setup, which includes `config.yaml` and `layout.json`.
-
-#### `config.yaml`
+#### 2.1 `config.yaml`
 Configuration and calibration values for your devices is stored in `config.yaml`.\
 Each configuration starts with the `name` of your device, then its `module`, `class`, and `settings`.
-
 ```yaml
-### config.yaml ###
-Device01:                                         # name of simple device (user-defined)
-  module: __module_name_01__                      # device module
-  class: __submodule_1A__.__class_1A__            # device class
+_Device01_:                                     # name of simple device (user-defined)
+  module: _module_name_01_                      # device module
+  class: _submodule_1A_._class_1A_              # device class
   settings:
-    port: __device_01__                           # port addresses defined in registry.yaml
-    __setting_A__: {'tuple': [300,0,200]}         # use keys to define the type of iterable
-    __setting_B__: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
+    port: __device_01__                         # port addresses defined in registry.yaml
+    _setting_A_: {'tuple': [300,0,200]}         # use keys to define the type of iterable
+    _setting_B_: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
 ```
 
 `Compound` devices are similarly configured. The configuration values for its component devices are defined under the `component_config` setting. The structure of the configuration values for the component devices are similar to that shown above, except indented to fall under the indentation of the `component_config` setting.
-
 ```yaml
-### config.yaml ###
-Device02:                                     # name of 'Compound' device (user-defined)
+_Device02_:                                     # name of 'Compound' device (user-defined)
   module: Compound                            
-  class: __submodule_2A__.__class_2A__
+  class: _submodule_2A_._class_2A_
   settings:
-    __setting_C__: 1                          # other settings for your 'Compound' device
-    component_config:                         # nest component configuration settings here
-      Component01:                            # name of component
-        module: __module_name_03__
-        class: __submodule_3A__.__class_3A__
+    _setting_C_: 1                              # other settings for your 'Compound' device
+    component_config:                           # nest component configuration settings here
+      _Component01_:                            # name of component
+        module: _module_name_03_
+        class: _submodule_3A_._class_3A_
         settings:
-          ip_address: '192.0.0.1'             # IP addresses do not vary between machines
-      Component02: 
-        module: __module_name_04__
-        class: __submodule_4A__.__class_4A__
+          ip_address: '192.0.0.1'               # IP addresses do not vary between machines
+      _Component02_: 
+        module: _module_name_04_
+        class: _submodule_4A_._class_4A_
         settings:
-          __setting_D__: 2                    # settings for your component device
+          _setting_D_: 2                        # settings for your component device
 ```
 
 Lastly, you can define shortcuts to quickly access components of `Compound` devices.
 ```yaml
-### config.yaml ###
 SHORTCUTS:
-  robot_arm: myCompoundDevice.mover
-  Nickname1: Device02.Component01
-  Nickname2: Device02.Component02
+  _Nickname1_: '_Device02_._Component01_'
+  _Nickname2_: '_Device02_._Component02_'
 ```
 
-#### `layout.json`
-Layout configuration of your physical workspace (`Deck`) will be stored in `layout.json`. This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block/module.
-
-This file is optional if your setup does not involve moving objects around in a pre-defined workspace, and hence a layout configuration may not be required.
+#### 2.2 `layout.json`
+Layout configuration of your physical workspace (`Deck`) will be stored in `layout.json`. This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block/object.
 
+*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a layout configuration may not be required.*
 ```json
 {
   "reference_points":{
     "1": ["_x01_","_y01_","_z01_"],
     "2": ["_x02_","_y02_","_z02_"]
   },
   "slots":{
     "1": {
-      "name": "Labware01",
+      "name": "_Labware01_",
       "exclusion_height": -1,
-      "filepath": "REPO/.../Labware01.json"
+      "filepath": "_repo_/.../_Labware01_.json"
     },
     "2": {
-      "name": "Labware02",
+      "name": "_Labware02_",
       "exclusion_height": 0,
-      "filepath": "REPO/.../Labware02.json"
+      "filepath": "_repo_/.../_Labware02_.json"
     },
     "3": {
-      "name": "Labware03",
+      "name": "_Labware03_",
       "exclusion_height": 10,
-      "filepath": "REPO/.../Labware03.json"
+      "filepath": "_repo_/.../_Labware03_.json"
     }
   }
 }
 ```
-
 In `reference_points`, the bottom-left coordinates of each slot in the workspace are defined. Slots are positions where Labware blocks may be placed.
 
-In `slots`, the name of each slot and the file reference for Labware block that occupies that slot are defined. The filepath starts with the repository's base folder name.\
+In `slots`, the name of each slot and the file reference for Labware block that occupies that slot are defined. The filepath starts with the repository's base folder name.
+
 The `exclusion_height` is the height (in mm) above the dimensions of the Labware block to steer clear from when performing move actions. Defaults to -1 (i.e. do not avoid).\
-\[Note: only applies to final coordinates. Does not guarantee avoidance when using point-to-point move actions. Use `safeMoveTo` instead.\]
+*(Note: only applies to final coordinates (i.e. destination). Does not guarantee collision avoidance when using point-to-point move actions. Use* `safeMoveTo()` *instead.)*
 
-### Load setup
-The initialisation of the setup occurs during the import `SETUP` from within `configs/Setup01`.
+#### 2.3 Load setup
+The initialisation of the setup occurs during the import `setup` from within `configs/_Setup01_`.
 
 ```python
 # Add repository folder to sys.path
 from pathlib import Path
 import sys
-REPO = 'REPO'
+REPO = '_repo_' 
+# replace "_repo_" with your base directory for the project
 ROOT = str(Path().absolute()).split(REPO)[0]
 sys.path.append(f'{ROOT}{REPO}')
 
 # Import the initialised setup
-from configs.Setup01 import SETUP
-this = SETUP
+from configs._Setup01_ import setup
+this = setup
+this._Device01_
+this._Nickname2_
 ```
-
 With `this`, you can access all the devices that you have defined in `configs.yaml`.
+
+### 3. Managing a deck
+*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a* `Deck` *may not be required.*
+
+#### 3.1 Loading a deck
+To load the `Deck` from the layout file, use the `loadDeck()` function.
 ```python
-this.myCompoundDevice
-this.robot_arm
-```
+from configs._Setup01_ import LAYOUT_FILE
+this._Device02_.loadDeck(LAYOUT_FILE)
+deck = this._Device02.deck
+``` 
 
-### Load deck
-To load the `Deck` from the layout file, use the `lab.load_deck` function.
+#### 3.2 Loading a Labware
+To load the `Labware` into the `Deck`, use the `load_labware()` method.
 ```python
-from configs.Setup01 import LAYOUT_FILE
-lab.load_deck(this.DeviceWithDeck, LAYOUT_FILE)
+deck.load_labware(...)
 ``` 
 
-## Package Structure
-1. Analyse
-2. Compound
-3. Control
-4. Make
-5. Measure
-6. Move
-7. Transfer
-8. View
+### 4. Setting up safety measures
+You can optionally set the safety policy for session. This has to be done before importing any of the classes.
+```python
+lab.set_safety('high')  # Pauses for input before every move action
+lab.set_safety('low')   # Waits for countdown before every move action
+# Import other classes from control-lab-ly only after setting the safety policy
+```
+
+### 5. Using plugins
+User-defined plugins can be integrated into Control.lab.ly without making additions or modifications to the package itself. All classes and functions can be found in `lab.modules`.
+```python
+print(lab.modules)  
+# view the entire package (only those that have been imported during the session)
+lab.modules.Make.Something.Good.myClass
+# this expression returns the registered class
+```
+
+#### 5.1 Directly registering a Class or Function
+You can import the class and register the object using the `Factory.register()` function.
+```python
+from my_module import myClass
+lab.Factory.register(myClass, "Make.Something.Good")
+```
+
+#### 5.2 Registering a Python module
+Alternatively, you can automatically register all Classes and Functions in a Python module just by importing it.\
+Declare a `__where__` global variable to indicate where to register the module.
+```python
+### my_module.py
+__where__ = "Make.Something.Good"                 # Where to register this module to
+def myClass:                                      # Main body of code goes here
+  ...
+from controllably import include_this_module
+include_this_module()                             # Registers only the Classes and Functions defined above in this .py file
+```
+At the end of the .py file, import and call  the `include_this_module()` function.
+
+---
 
 ## Dependencies
 - Dash (>=2.7.1)
 - Impedance (>=1.4.1)
 - Imutils (>=0.5.4)
 - Matplotlib (>=3.3.4)
 - Nest-asyncio (>=1.5.1)
@@ -288,46 +333,68 @@
 
 ## How to Contribute
 [Issues](https://github.com/kylejeanlewis/control-lab-le/issues) and feature requests are welcome!
 
 ## License
 This project is distributed under the [MIT License](https://github.com/kylejeanlewis/control-lab-le/blob/main/LICENSE).
 
+---
 # Change Log
 
 ## Unreleased
 *Items under development*
 
+## 1.0.0.x
+Major overhaul in package structure. Standardisation of methods and consolidation of common methods. First released 12 Apr 2023.
+### Added
+#### 1.0.0
+- Usage of Abstract Base Classes (ABCs) to define a base class with abstract methods that needs to be implemented through sub-classing
+- Usage of Protocols to provide an interface between different classes of objects
+- Usage of Dataclasses to store complex data 
+- Usage of decorators to modify methods
+- Introduced different functions to parse the program docstring and find program parameters
+### Changed
+#### 1.0.0
+- Standardised methods and consolidated common methods
+- Added type hints
+- Moved Dobot attachments from Mover to Transfer.Substrate
+- Split GUI Panels into individual files
+- Split Dobot arms into individual files
+- Split functions/methods in `misc.py` into individual files.
+- Changed `_flags` to a public attribute `flags`
+- Update documentation
+### Removed
+#### 1.0.0
+- Unnecessary commented-out blocks of code
+
 ## 0.0.4.x
 Introduced control for Peltier device and TriContinent Series C syringe pumps. First released 10 Mar 2023.
 ### Added
 #### 0.0.4
 - Added control for `Peltier`
   - set and get temperatures
   - hold temperatures for desired duration
   - checks if target temperature has been reached by checking power level lower than a threshold or time passed over a predefined duration, once the temperature is within tolerance
   - ability to record temperatures and timestamps 
 - Added control for `TriContinent` and `TriContinentEnsemble`
   - single actions such as `empty`, `fill`, `initialise`, move actions, set speeds and valves, and wait
   - compound actions such as `aspirate`, `dispense`, and `prime`
-
 ### Changed
 #### 0.0.4
 - Update documentation
 
 ## 0.0.3.x
 Minor changes to movement robot safety and pipette control. Introduced control for LED array. First released 08 Mar 2023.
 ### Added
 #### 0.0.3
 - Added safety measures for movement actions
   - In `Deck`, added exclusion zones when reading the `layout.json` file and new method `is_excluded()` to check if target coordinate is within the exclusion zone
   - In `Mover`, update `isFeasible()` method to check if target coordinates violates the deck's exclusion zone
   - New function `set_safety()` defines safety modes when starting a new session to pause for input (in "high" safety setting) and to wait for safety countdown (in "low" safety setting)
 - `Make.Light.LEDArray` for controlling LEDs in the photo-reactor, as well as timing the LED "on" durations
-
 ### Changed
 #### 0.0.3.1
 - Update documentation
 #### 0.0.3
 - `Sartorius`
   - made the blowout/home optional for the dispense method upon emptying the pipette
 - Update documentation
@@ -337,15 +404,14 @@
 ### Added
 #### 0.0.2.2
 - Added import of `CompoundSetup` class
 #### 0.0.2
 - `Deck.at()` method for directly referencing slots using either index numbers or names
 - New `CompoundSetup` class for common methods of `Compound` devices
 - New `load_deck()` function to load `Deck` after initialisation
-
 ### Changed
 #### 0.0.2.1
 - Changed template files for `lab.create_setup()`
 #### 0.0.2
 - Update documentation
 
 ## 0.0.1.x
```

### Comparing `control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/SOURCES.txt` & `control-lab-ly-1.0.0b0/src/control_lab_ly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Database/database_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Database/database_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/circuit_datatype.py` & `control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/circuit_datatype.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/eis_datatype.py` & `control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/eis_datatype.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml` & `control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/eis_tests.json` & `control-lab-ly-1.0.0b0/src/controllably/Analyse/Data/Types/eis_tests.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Analyse/Visualisation/visualisation_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Analyse/Visualisation/visualisation_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Compound/LiquidMover/liquidmover_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Compound/LiquidMover/liquidmover_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Compound/compound_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Compound/compound_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Control/GUI/__init__.py` & `control-lab-ly-1.0.0b0/src/controllably/Control/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Control/GUI/_guibuilder.py` & `control-lab-ly-1.0.0b0/src/controllably/Control/GUI/_guibuilder.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Control/GUI/gui_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Control/GUI/gui_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Control/GUI/loader_panel.py` & `control-lab-ly-1.0.0b0/src/controllably/Control/GUI/loader_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Control/GUI/measurer_panel.py` & `control-lab-ly-1.0.0b0/src/controllably/Control/GUI/measurer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Control/GUI/mover_panel.py` & `control-lab-ly-1.0.0b0/src/controllably/Control/GUI/mover_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Control/GUI/viewer_panel.py` & `control-lab-ly-1.0.0b0/src/controllably/Control/GUI/viewer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Control/Schedule/schedule_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Control/Schedule/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Make/Heat/peltier_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Make/Heat/peltier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Make/Light/led_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Make/Light/led_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Make/ThinFilm/spinner_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Make/ThinFilm/spinner_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Make/make_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Make/make_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/keithley_device.py` & `control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/keithley_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py` & `control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py` & `control-lab-ly-1.0.0b0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py` & `control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py` & `control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py` & `control-lab-ly-1.0.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Measure/Physical/balance_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Measure/Physical/balance_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Measure/__init__.py` & `control-lab-ly-1.0.0b0/src/controllably/Measure/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Measure/instrument_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Measure/instrument_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Measure/measure_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Measure/measure_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Measure/program_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Measure/program_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Move/Cartesian/cartesian_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/cartesian_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Move/Cartesian/ender_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/ender_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Move/Cartesian/primitiv_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Move/Cartesian/primitiv_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py` & `control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/dobot_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/dobot_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/mg400_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/Dobot/mg400_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/jointed_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Move/Jointed/jointed_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Move/move_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Move/move_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py` & `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py` & `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/liquid_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/liquid_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/syringe_lib.py` & `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/syringe_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/syringe_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Transfer/Liquid/syringe_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py` & `control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/Transfer/Substrate/substrate_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/Transfer/Substrate/substrate_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/View/Classifiers/classifier_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/View/Classifiers/classifier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/View/Optical/optical_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/View/Optical/optical_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/View/Optical/placeholders/optical_camera.png` & `control-lab-ly-1.0.0b0/src/controllably/View/Optical/placeholders/optical_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8.py` & `control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py` & `control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py` & `control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/View/Thermal/placeholders/infrared_camera.png` & `control-lab-ly-1.0.0b0/src/controllably/View/Thermal/placeholders/infrared_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/View/Thermal/thermal_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/View/Thermal/thermal_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/View/image_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/View/image_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/View/view_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/View/view_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/misc/__init__.py` & `control-lab-ly-1.0.0b0/src/controllably/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/misc/decorators.py` & `control-lab-ly-1.0.0b0/src/controllably/misc/decorators.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/misc/factory.py` & `control-lab-ly-1.0.0b0/src/controllably/misc/factory.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/misc/helper.py` & `control-lab-ly-1.0.0b0/src/controllably/misc/helper.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/misc/layout.py` & `control-lab-ly-1.0.0b0/src/controllably/misc/layout.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/misc/logger.py` & `control-lab-ly-1.0.0b0/src/controllably/misc/logger.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/misc/misc_utils.py` & `control-lab-ly-1.0.0b0/src/controllably/misc/misc_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/misc/templates/configs/plugins/plugin_template.py` & `control-lab-ly-1.0.0b0/src/controllably/misc/templates/configs/plugins/plugin_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Functions:
     my_function
 
 Other constants and variables:
     MY_CONSTANT (str)
     my_variable (str)
 """
-__where__ = "Create.Something.Good"                 # Where to register this module to
+__where__ = "Make.Something.Good"                 # Where to register this module to
 
 # ================================================\ Define your plugin classes and functions in this section
 class MyClass:
     """This is a summary of my class."""
     @classmethod
     def say(cls, words:str):
         """
@@ -33,8 +33,8 @@
     return
 
 MY_CONSTANT = 'MY_CONSTANT'
 my_variable = 'my_variable'
 # ================================================/
 
 from controllably import include_this_module
-include_this_module()                               # Registers only the Classes and Functions defined above in this py file
+include_this_module()                               # Registers only the Classes and Functions defined above in this .py file
```

### Comparing `control-lab-ly-1.0.0a0/src/controllably/misc/templates/setup/__init__.py` & `control-lab-ly-1.0.0b0/src/controllably/misc/templates/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/src/controllably/misc/templates/setup/config.yaml` & `control-lab-ly-1.0.0b0/src/controllably/misc/templates/setup/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 _Device01_:                                     # name of simple device (user-defined)
   module: _module_name_01_                      # device module
   class: _submodule_1A_._class_1A_              # device class
   settings:
-    port: _device_01_                           # port addresses defined in registry.yaml
+    port: __device_01__                         # port addresses defined in registry.yaml
     _setting_A_: {'tuple': [300,0,200]}         # use keys to define the type of iterable
     _setting_B_: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
 
 _Device02_:                                     # name of 'Compound' device (user-defined)
   module: Compound                            
   class: _submodule_2A_._class_2A_
   settings:
```

### Comparing `control-lab-ly-1.0.0a0/src/controllably/misc/templates/setup/layout.json` & `control-lab-ly-1.0.0b0/src/controllably/misc/templates/setup/layout.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/tests/test_compound_liquidmover.py` & `control-lab-ly-1.0.0b0/tests/test_compound_liquidmover.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/tests/test_compound_spin_printer.py` & `control-lab-ly-1.0.0b0/tests/test_compound_spin_printer.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/tests/test_dobot_m1pro.py` & `control-lab-ly-1.0.0b0/tests/test_dobot_m1pro.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/tests/test_dobot_mg400.py` & `control-lab-ly-1.0.0b0/tests/test_dobot_mg400.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/tests/test_heat_peltier.py` & `control-lab-ly-1.0.0b0/tests/test_heat_peltier.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.0a0/tests/test_liquid_tricontinent.py` & `control-lab-ly-1.0.0b0/tests/test_liquid_tricontinent.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # %%
 me.setCurrentChannel(2)
 # %%
 me.prime(1)
 # %%
 me.move(40, up=False, channel=1)
 # %%
-me.moveBy(150, channel=2) # FIXME: channel parameter does not work
+me.moveBy(1000, channel=2)
 # %%
 me.moveTo(1500)
 # %%
 me.aspirate(20, channel=1)
 # %%
 me.dispense(500)
 # %%
```

