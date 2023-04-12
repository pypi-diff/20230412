# Comparing `tmp/obsinfo-0.111.0.tar.gz` & `tmp/obsinfo-0.111b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsinfo-0.111.0.tar", last modified: Wed Apr 12 06:33:07 2023, max compression
+gzip compressed data, was "obsinfo-0.111b1.tar", last modified: Wed Apr 12 06:31:11 2023, max compression
```

## Comparing `obsinfo-0.111.0.tar` & `obsinfo-0.111b1.tar`

### file list

```diff
@@ -1,301 +1,301 @@
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.493633 obsinfo-0.111.0/
--rw-r--r--   0 crawford   (501) admin       (80)    35148 2021-10-18 08:41:35.000000 obsinfo-0.111.0/LICENSE.txt
--rw-r--r--   0 crawford   (501) admin       (80)      140 2021-10-18 08:41:35.000000 obsinfo-0.111.0/MANIFEST.in
--rw-r--r--   0 crawford   (501) admin       (80)     1919 2023-04-12 06:33:07.493813 obsinfo-0.111.0/PKG-INFO
--rw-r--r--   0 crawford   (501) admin       (80)     1032 2021-10-18 08:41:35.000000 obsinfo-0.111.0/README.rst
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.370440 obsinfo-0.111.0/obsinfo/
--rw-r--r--   0 crawford   (501) admin       (80)       17 2021-09-09 21:44:08.000000 obsinfo-0.111.0/obsinfo/__init__.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.373545 obsinfo-0.111.0/obsinfo/_examples/
--rw-r--r--   0 crawford   (501) admin       (80)    10244 2023-02-06 14:21:22.000000 obsinfo-0.111.0/obsinfo/_examples/.DS_Store
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.374966 obsinfo-0.111.0/obsinfo/_examples/Information_Files/
--rw-r--r--   0 crawford   (501) admin       (80)    12292 2023-04-10 11:11:33.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      828 2023-02-06 14:15:15.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/README.rst
--rw-r--r--   0 crawford   (501) admin       (80)       90 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/README.txt
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.375563 obsinfo-0.111.0/obsinfo/_examples/Information_Files/campaigns/
--rw-r--r--   0 crawford   (501) admin       (80)     2053 2023-04-10 16:23:16.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/campaigns/SPOBS.campaign.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.376057 obsinfo-0.111.0/obsinfo/_examples/Information_Files/datacites/
--rw-r--r--   0 crawford   (501) admin       (80)     1731 2023-04-10 16:23:16.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/datacites/EMSO-MOMAR_OBS.datacite.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.377185 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/
--rw-r--r--   0 crawford   (501) admin       (80)     1763 2023-03-22 08:38:06.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/ADS1281.datalogger_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     5880 2023-03-22 08:38:32.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/LC2000.datalogger_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.381939 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 18:40:52.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      729 2023-04-11 18:33:44.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/CS5321_FIR1.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      618 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      605 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.with-delay.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      556 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR3.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      592 2023-02-28 16:43:08.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_100sps-SINC.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      596 2023-02-28 16:43:14.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_200sps-SINC.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      436 2023-02-28 16:43:36.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR1.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      435 2023-02-28 16:43:35.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR2.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      443 2023-02-28 16:43:29.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR3_LINEAR.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      443 2023-02-28 16:43:33.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR4_LINEAR.stage_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.384204 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/filters/
--rw-r--r--   0 crawford   (501) admin       (80)      480 2023-02-28 16:44:38.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR2.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2412 2023-02-28 16:44:43.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR3.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      283 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR1.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      268 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR2.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      578 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR3-linear.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1118 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR4-linear.filter.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.384997 obsinfo-0.111.0/obsinfo/_examples/Information_Files/experiments/
--rw-r--r--   0 crawford   (501) admin       (80)    16208 2023-03-01 16:50:51.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/experiments/MAYOBS.experiment.yaml
--rw-r--r--   0 crawford   (501) admin       (80)    19366 2023-04-10 16:23:16.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/experiments/MOMAR.experiment.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.389372 obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-12 12:33:43.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)     3594 2023-04-12 06:20:50.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/BBOBS1_2012+.instrumentation_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2189 2023-04-11 21:33:49.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/BBOBS1_pre2012.instrumentation_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     4527 2023-03-22 08:38:31.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/GURALP_CP.instrumentation_base.yaml_error.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1084 2023-03-07 15:14:40.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/HYDROCT1.instrumentation_base.yaml_error.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1265 2023-03-07 15:14:50.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/SPOBS1.instrumentation_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1451 2023-03-07 15:15:08.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/SPOBS2.instrumentation_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1732 2023-03-07 15:20:23.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/SPOBS3-for-channel-mod-testing.instrumentation_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1554 2023-03-07 15:20:21.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/WBOBS1.instrumentation_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1885 2023-03-07 15:14:30.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/empty.instrumentation_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.390140 obsinfo-0.111.0/obsinfo/_examples/Information_Files/location_bases/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 16:53:33.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/location_bases/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)     1356 2023-02-27 22:12:01.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/location_bases/INSU-IPGP.location_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.391082 obsinfo-0.111.0/obsinfo/_examples/Information_Files/networks/
--rw-r--r--   0 crawford   (501) admin       (80)      329 2023-04-11 08:09:43.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/networks/EMSO-AZORES.network.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      413 2023-04-11 08:09:59.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/networks/RHUM-RUM.network.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.391935 obsinfo-0.111.0/obsinfo/_examples/Information_Files/operators/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-11-30 17:19:05.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/operators/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      345 2023-02-28 16:41:26.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/operators/INSU-IPGP.operator.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.393700 obsinfo-0.111.0/obsinfo/_examples/Information_Files/persons/
--rw-r--r--   0 crawford   (501) admin       (80)      159 2023-02-28 16:46:55.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/persons/Kevin_Canjamale.person.yaml
--rw-r--r--   0 crawford   (501) admin       (80)       98 2023-02-28 16:47:13.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/persons/Romuald_Daniel.person.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      100 2023-02-28 16:47:05.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/persons/Simon_Besancon.person.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      166 2023-02-28 16:46:47.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/persons/Wayne_Crawford.person.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.396372 obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/
--rw-r--r--   0 crawford   (501) admin       (80)      643 2023-02-27 22:11:57.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_BBOBS.preamplifier_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      448 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_DPG.preamplifier_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      811 2023-02-27 22:11:40.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_GEOPHONE.preamplifier_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      797 2023-02-27 22:11:34.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO-no_redundancy.preamplifier_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      797 2023-02-27 22:11:25.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.398714 obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/stages/
--rw-r--r--   0 crawford   (501) admin       (80)      451 2023-02-27 22:11:22.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_BBOBS_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      662 2023-02-27 22:11:20.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_geophone_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      698 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/stages/SIO-LDEO_DPG-Card_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      821 2023-02-27 22:11:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/stages/Scripps_SPOBS_HydroL22_theoretical.stage_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.403109 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/
--rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-02-06 14:13:53.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      661 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/HITECH_HTI04-PLC-ULF.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      752 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/HITECH_HTI90U.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2341 2023-04-11 21:38:03.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240__theoretical.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1425 2023-02-27 22:11:14.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240_plusDates.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      835 2023-04-11 14:10:42.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_TCOMPACT_theoretical.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      652 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/SERCEL_L22.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      698 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/SERCEL_L28.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2009 2023-02-27 22:11:07.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/SIO_DPG.sensor_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.408220 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/
--rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-02-06 14:13:53.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      430 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-04-PLC-ULF_voltage-mode_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1341 2023-01-09 11:31:34.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-90U_SIO-preamp_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      536 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5004_calibrated.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      527 2023-04-11 13:55:08.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5018_calibrated.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      382 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_generic_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      485 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L22D_LCHEAPO_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      537 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L28LB_LCHEAPO_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1233 2023-02-27 22:11:02.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/Trillium_T240__theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      586 2023-02-27 22:11:00.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/Trillium_TCompact__theoretical.stage_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.415808 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2023-01-09 11:32:20.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      280 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/HiTech_HTI-04-PLC-ULF_voltage-mode_theoretical.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      310 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__5004_2007.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      306 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__5017_2007.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      364 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__generic.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      383 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/Sercel_L22D_C510-S2000_generic.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      236 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/Sercel_L28LB-obs_C395-S2490_generic.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      728 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN1-399_generic.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      873 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN400-_generic.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      547 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_TCompact__generic.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      854 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/test---attributes-poleszeros.filter.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.421729 obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2023-04-11 10:41:26.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)        5 2022-12-19 08:46:18.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/.obsinfo
--rw-r--r--   0 crawford   (501) admin       (80)     3690 2023-04-11 08:10:25.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP.subnetwork.yaml_error.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     3429 2023-04-11 21:13:12.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP_with_gain_mods.subnetwork.yaml_error.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2798 2023-04-11 10:40:05.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/EMPTY-INSTRUMENTATION.INSU-IPGP.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2835 2023-04-12 06:00:16.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2211 2023-04-11 08:10:30.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential_noRefs.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1890 2023-04-11 21:46:11.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/LEAP_SECOND.INSU-IPGP.subnetwork.yaml_error.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     3197 2023-04-11 18:07:50.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/ORIENTED.INSU-IPGP.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     3092 2023-04-11 18:07:24.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/SPOBS.INSU-IPGP.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2699 2023-04-11 18:07:16.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/SPOBS_noAnchors.INSU-IPGP.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2017 2023-04-11 18:44:22.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/TEST.subnetwork.yaml_error.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.423258 obsinfo-0.111.0/obsinfo/_examples/Information_Files/timing_bases/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 16:53:33.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/timing_bases/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      252 2023-01-17 15:49:59.000000 obsinfo-0.111.0/obsinfo/_examples/Information_Files/timing_bases/Seascan_GNSS.timing_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.363194 obsinfo-0.111.0/obsinfo/_examples/Training/
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.426720 obsinfo-0.111.0/obsinfo/_examples/Training/templates/
--rw-r--r--   0 crawford   (501) admin       (80)     1308 2023-04-11 08:12:26.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/BBOBS-train.network.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     3185 2023-04-11 08:12:46.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/BBOBS.INSU-IPGP.network.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1501 2023-01-17 18:01:07.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/BBOBS1.instrumentation.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1625 2023-01-17 18:00:12.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/BBOBS1_2012+.instrumentation.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      573 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/CS5322.stage.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1047 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/T240.stage.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.428419 obsinfo-0.111.0/obsinfo/_examples/Training/templates/components/
--rw-r--r--   0 crawford   (501) admin       (80)     3049 2023-03-22 08:38:30.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/components/LC2000-1.datalogger.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     3053 2023-03-22 08:38:26.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/components/LC2000.datalogger.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      907 2023-03-21 09:43:56.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/components/preamplifier.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1257 2023-03-21 09:44:03.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/components/sensor.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.432671 obsinfo-0.111.0/obsinfo/_examples/Training/templates/filters/
--rw-r--r--   0 crawford   (501) admin       (80)      263 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/filters/AD_Conversion.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      673 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/filters/CirrusLogic_FIR.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      607 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/filters/ExampleFIR.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      409 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/filters/HiTechPZ.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      416 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/filters/HiTech_PolesZeros.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      191 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/filters/analog.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      390 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/filters/coefficients.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      310 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/filters/digital.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      379 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/filters/response_list.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2175 2023-04-11 08:12:58.000000 obsinfo-0.111.0/obsinfo/_examples/Training/templates/network.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.435105 obsinfo-0.111.0/obsinfo/_examples/scripts/
--rw-r--r--   0 crawford   (501) admin       (80)      292 2021-09-09 21:44:08.000000 obsinfo-0.111.0/obsinfo/_examples/scripts/README.rst
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.436390 obsinfo-0.111.0/obsinfo/_examples/scripts/add_ons/
--rw-r--r--   0 crawford   (501) admin       (80)      331 2021-09-09 21:44:08.000000 obsinfo-0.111.0/obsinfo/_examples/scripts/add_ons/README.rst
--rw-r--r--   0 crawford   (501) admin       (80)      952 2021-09-09 21:44:08.000000 obsinfo-0.111.0/obsinfo/_examples/scripts/add_ons/make_data_process_scripts.sh
--rwxr-xr-x   0 crawford   (501) admin       (80)      376 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/scripts/make_stationXML.sh
--rwxr-xr-x   0 crawford   (501) admin       (80)      420 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/scripts/print_info_files.sh
--rwxr-xr-x   0 crawford   (501) admin       (80)     1646 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/scripts/validate_all.sh
--rwxr-xr-x   0 crawford   (501) admin       (80)      315 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/_examples/scripts/validate_files.sh
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.439297 obsinfo-0.111.0/obsinfo/addons/
--rw-r--r--   0 crawford   (501) admin       (80)     9904 2023-01-05 14:22:59.000000 obsinfo-0.111.0/obsinfo/addons/LC2SDS.py
--rw-r--r--   0 crawford   (501) admin       (80)    10899 2023-01-05 14:26:17.000000 obsinfo-0.111.0/obsinfo/addons/LCHEAPO.py
--rw-r--r--   0 crawford   (501) admin       (80)     9134 2023-04-11 08:13:40.000000 obsinfo-0.111.0/obsinfo/addons/OCA.py
--rw-r--r--   0 crawford   (501) admin       (80)    15899 2023-04-11 08:13:46.000000 obsinfo-0.111.0/obsinfo/addons/SDPCHAIN.py
--rw-r--r--   0 crawford   (501) admin       (80)       64 2021-09-09 21:44:08.000000 obsinfo-0.111.0/obsinfo/addons/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     2481 2023-01-05 14:20:29.000000 obsinfo-0.111.0/obsinfo/addons/infodump.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.442339 obsinfo-0.111.0/obsinfo/console_scripts/
--rw-r--r--   0 crawford   (501) admin       (80)      104 2023-04-11 12:05:29.000000 obsinfo-0.111.0/obsinfo/console_scripts/__init__.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    63491 2023-03-22 08:38:16.000000 obsinfo-0.111.0/obsinfo/console_scripts/_test.py
--rw-r--r--   0 crawford   (501) admin       (80)     7941 2023-04-12 05:49:55.000000 obsinfo-0.111.0/obsinfo/console_scripts/makeStationXML.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     8399 2023-04-12 05:27:13.000000 obsinfo-0.111.0/obsinfo/console_scripts/print.py
--rw-r--r--   0 crawford   (501) admin       (80)      289 2022-06-20 07:21:38.000000 obsinfo-0.111.0/obsinfo/console_scripts/print_version.py
--rw-r--r--   0 crawford   (501) admin       (80)     8160 2023-04-12 05:54:26.000000 obsinfo-0.111.0/obsinfo/console_scripts/setup.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    17057 2023-04-12 05:58:43.000000 obsinfo-0.111.0/obsinfo/console_scripts/validate.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.364413 obsinfo-0.111.0/obsinfo/data/
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.451007 obsinfo-0.111.0/obsinfo/data/schemas/
--rw-r--r--   0 crawford   (501) admin       (80)     8861 2023-03-03 09:25:57.000000 obsinfo-0.111.0/obsinfo/data/schemas/datacite.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     5514 2023-03-25 15:00:10.000000 obsinfo-0.111.0/obsinfo/data/schemas/datalogger_base.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)    10023 2023-04-11 15:24:46.000000 obsinfo-0.111.0/obsinfo/data/schemas/definitions.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-04-11 08:14:23.000000 obsinfo-0.111.0/obsinfo/data/schemas/experiment.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)    13582 2023-04-06 17:48:52.000000 obsinfo-0.111.0/obsinfo/data/schemas/filter.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     8241 2023-04-11 10:28:57.000000 obsinfo-0.111.0/obsinfo/data/schemas/instrumentation_base.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     1378 2022-11-30 17:16:16.000000 obsinfo-0.111.0/obsinfo/data/schemas/iris_units.json
--rw-r--r--   0 crawford   (501) admin       (80)     6575 2023-04-11 15:31:38.000000 obsinfo-0.111.0/obsinfo/data/schemas/location_base.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     1922 2023-04-11 08:14:35.000000 obsinfo-0.111.0/obsinfo/data/schemas/network.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     1407 2023-04-06 14:54:32.000000 obsinfo-0.111.0/obsinfo/data/schemas/operator.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     1735 2023-02-28 08:30:05.000000 obsinfo-0.111.0/obsinfo/data/schemas/person.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     4650 2023-03-25 15:00:19.000000 obsinfo-0.111.0/obsinfo/data/schemas/preamplifier_base.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     6472 2023-03-25 15:00:00.000000 obsinfo-0.111.0/obsinfo/data/schemas/sensor_base.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     8193 2023-04-06 17:50:39.000000 obsinfo-0.111.0/obsinfo/data/schemas/stage_base.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     2051 2023-03-21 13:52:11.000000 obsinfo-0.111.0/obsinfo/data/schemas/stages.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     7216 2023-04-11 10:58:00.000000 obsinfo-0.111.0/obsinfo/data/schemas/subnetwork.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     3997 2023-02-28 16:48:56.000000 obsinfo-0.111.0/obsinfo/data/schemas/timing_base.schema.json
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.451428 obsinfo-0.111.0/obsinfo/datacite/
--rw-r--r--   0 crawford   (501) admin       (80)        0 2023-01-19 09:54:12.000000 obsinfo-0.111.0/obsinfo/datacite/__init__.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.456118 obsinfo-0.111.0/obsinfo/helpers/
--rw-r--r--   0 crawford   (501) admin       (80)      729 2023-04-11 09:20:15.000000 obsinfo-0.111.0/obsinfo/helpers/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     3091 2023-04-06 13:54:33.000000 obsinfo-0.111.0/obsinfo/helpers/comments.py
--rw-r--r--   0 crawford   (501) admin       (80)     1565 2023-04-06 13:06:26.000000 obsinfo-0.111.0/obsinfo/helpers/external_references.py
--rw-r--r--   0 crawford   (501) admin       (80)     3089 2023-04-12 05:45:13.000000 obsinfo-0.111.0/obsinfo/helpers/float_with_uncert.py
--rw-r--r--   0 crawford   (501) admin       (80)     1518 2023-04-11 16:29:35.000000 obsinfo-0.111.0/obsinfo/helpers/functions.py
--rw-r--r--   0 crawford   (501) admin       (80)     1506 2023-04-11 09:14:43.000000 obsinfo-0.111.0/obsinfo/helpers/identifiers.py
--rw-r--r--   0 crawford   (501) admin       (80)     6469 2023-04-05 13:41:46.000000 obsinfo-0.111.0/obsinfo/helpers/location.py
--rw-r--r--   0 crawford   (501) admin       (80)     3401 2023-04-11 14:33:07.000000 obsinfo-0.111.0/obsinfo/helpers/obsinfo_class_list.py
--rw-r--r--   0 crawford   (501) admin       (80)     3622 2023-04-02 23:37:37.000000 obsinfo-0.111.0/obsinfo/helpers/oi_date.py
--rw-r--r--   0 crawford   (501) admin       (80)     2621 2023-04-11 14:26:19.000000 obsinfo-0.111.0/obsinfo/helpers/person.py
--rw-r--r--   0 crawford   (501) admin       (80)     7685 2023-04-06 07:43:07.000000 obsinfo-0.111.0/obsinfo/helpers/phone.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.465132 obsinfo-0.111.0/obsinfo/instrumentation/
--rw-r--r--   0 crawford   (501) admin       (80)      830 2023-04-11 10:13:55.000000 obsinfo-0.111.0/obsinfo/instrumentation/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    11457 2023-04-12 05:43:58.000000 obsinfo-0.111.0/obsinfo/instrumentation/channel.py
--rw-r--r--   0 crawford   (501) admin       (80)     4969 2023-04-11 15:24:42.000000 obsinfo-0.111.0/obsinfo/instrumentation/equipment.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.471003 obsinfo-0.111.0/obsinfo/instrumentation/filter/
--rw-r--r--   0 crawford   (501) admin       (80)     1850 2023-04-03 16:39:05.000000 obsinfo-0.111.0/obsinfo/instrumentation/filter/AD_conversion.py
--rw-r--r--   0 crawford   (501) admin       (80)     2814 2023-04-12 06:16:41.000000 obsinfo-0.111.0/obsinfo/instrumentation/filter/FIR.py
--rw-r--r--   0 crawford   (501) admin       (80)      506 2023-01-30 15:51:03.000000 obsinfo-0.111.0/obsinfo/instrumentation/filter/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     1555 2023-04-11 16:22:34.000000 obsinfo-0.111.0/obsinfo/instrumentation/filter/analog.py
--rw-r--r--   0 crawford   (501) admin       (80)     2353 2023-04-03 16:39:20.000000 obsinfo-0.111.0/obsinfo/instrumentation/filter/coefficients.py
--rw-r--r--   0 crawford   (501) admin       (80)     1256 2023-04-03 16:40:13.000000 obsinfo-0.111.0/obsinfo/instrumentation/filter/digital.py
--rw-r--r--   0 crawford   (501) admin       (80)     3106 2023-03-10 16:10:10.000000 obsinfo-0.111.0/obsinfo/instrumentation/filter/filter.py
--rw-r--r--   0 crawford   (501) admin       (80)     1656 2023-04-06 17:54:00.000000 obsinfo-0.111.0/obsinfo/instrumentation/filter/filter_template.py
--rw-r--r--   0 crawford   (501) admin       (80)     5290 2023-04-11 16:27:01.000000 obsinfo-0.111.0/obsinfo/instrumentation/filter/poles_zeros.py
--rw-r--r--   0 crawford   (501) admin       (80)     2442 2023-04-03 16:39:41.000000 obsinfo-0.111.0/obsinfo/instrumentation/filter/polynomial.py
--rw-r--r--   0 crawford   (501) admin       (80)     1854 2023-04-03 16:39:53.000000 obsinfo-0.111.0/obsinfo/instrumentation/filter/response_list.py
--rw-r--r--   0 crawford   (501) admin       (80)    12143 2023-04-11 22:07:58.000000 obsinfo-0.111.0/obsinfo/instrumentation/instrument.py
--rw-r--r--   0 crawford   (501) admin       (80)     9710 2023-04-11 18:45:31.000000 obsinfo-0.111.0/obsinfo/instrumentation/instrument_component.py
--rw-r--r--   0 crawford   (501) admin       (80)    10284 2023-04-11 18:01:13.000000 obsinfo-0.111.0/obsinfo/instrumentation/instrumentation.py
--rw-r--r--   0 crawford   (501) admin       (80)     5442 2023-03-27 23:26:01.000000 obsinfo-0.111.0/obsinfo/instrumentation/orientation.py
--rw-r--r--   0 crawford   (501) admin       (80)    17057 2023-04-06 17:59:14.000000 obsinfo-0.111.0/obsinfo/instrumentation/stage.py
--rw-r--r--   0 crawford   (501) admin       (80)     2771 2023-04-03 14:12:36.000000 obsinfo-0.111.0/obsinfo/instrumentation/stages.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.473651 obsinfo-0.111.0/obsinfo/misc/
--rw-r--r--   0 crawford   (501) admin       (80)        0 2022-06-24 14:31:17.000000 obsinfo-0.111.0/obsinfo/misc/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     2497 2022-06-24 14:30:50.000000 obsinfo-0.111.0/obsinfo/misc/configuration.py
--rw-r--r--   0 crawford   (501) admin       (80)      866 2022-06-24 14:29:23.000000 obsinfo-0.111.0/obsinfo/misc/const.py
--rw-r--r--   0 crawford   (501) admin       (80)     4660 2022-06-24 14:27:52.000000 obsinfo-0.111.0/obsinfo/misc/discoveryfiles.py
--rw-r--r--   0 crawford   (501) admin       (80)     3062 2023-03-21 09:50:57.000000 obsinfo-0.111.0/obsinfo/misc/printobs.py
--rw-r--r--   0 crawford   (501) admin       (80)     4026 2022-06-24 14:17:30.000000 obsinfo-0.111.0/obsinfo/misc/remoteGitLab.py
--rw-r--r--   0 crawford   (501) admin       (80)    28034 2023-04-06 17:16:02.000000 obsinfo-0.111.0/obsinfo/misc/yamlref.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.474412 obsinfo-0.111.0/obsinfo/obsMetadata/
--rw-r--r--   0 crawford   (501) admin       (80)       37 2023-02-15 09:27:51.000000 obsinfo-0.111.0/obsinfo/obsMetadata/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    25122 2023-04-11 21:42:28.000000 obsinfo-0.111.0/obsinfo/obsMetadata/obsmetadata.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.476450 obsinfo-0.111.0/obsinfo/subnetwork/
--rw-r--r--   0 crawford   (501) admin       (80)      376 2023-04-06 14:04:52.000000 obsinfo-0.111.0/obsinfo/subnetwork/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     2138 2023-04-11 10:19:15.000000 obsinfo-0.111.0/obsinfo/subnetwork/operator.py
--rw-r--r--   0 crawford   (501) admin       (80)     2094 2023-04-11 18:04:18.000000 obsinfo-0.111.0/obsinfo/subnetwork/processing.py
--rw-r--r--   0 crawford   (501) admin       (80)      654 2023-04-06 13:55:11.000000 obsinfo-0.111.0/obsinfo/subnetwork/site.py
--rw-r--r--   0 crawford   (501) admin       (80)    10316 2023-04-11 18:15:51.000000 obsinfo-0.111.0/obsinfo/subnetwork/station.py
--rw-r--r--   0 crawford   (501) admin       (80)     6326 2023-04-11 10:58:08.000000 obsinfo-0.111.0/obsinfo/subnetwork/subnetwork.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.479395 obsinfo-0.111.0/obsinfo/template_specifications/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-12 12:14:05.000000 obsinfo-0.111.0/obsinfo/template_specifications/.DS_Store
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.481788 obsinfo-0.111.0/obsinfo/template_specifications/components/
--rw-r--r--   0 crawford   (501) admin       (80)     1439 2023-03-22 08:38:14.000000 obsinfo-0.111.0/obsinfo/template_specifications/components/datalogger.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1076 2023-03-21 09:51:15.000000 obsinfo-0.111.0/obsinfo/template_specifications/components/preamplifier.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1438 2023-03-21 09:51:26.000000 obsinfo-0.111.0/obsinfo/template_specifications/components/sensor.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.484062 obsinfo-0.111.0/obsinfo/template_specifications/filters/
--rw-r--r--   0 crawford   (501) admin       (80)      276 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/template_specifications/filters/AD_Conversion.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      449 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/template_specifications/filters/FIR.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      603 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/template_specifications/filters/PolesZeros.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      194 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/template_specifications/filters/analog.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      410 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/template_specifications/filters/coefficients.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      320 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/template_specifications/filters/digital.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      401 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/template_specifications/filters/response_list.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1419 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/template_specifications/instrumentation.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2483 2023-04-11 08:15:35.000000 obsinfo-0.111.0/obsinfo/template_specifications/network.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1113 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/template_specifications/stage.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.485543 obsinfo-0.111.0/obsinfo/templates/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-12 12:14:05.000000 obsinfo-0.111.0/obsinfo/templates/.DS_Store
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.486623 obsinfo-0.111.0/obsinfo/templates/components/
--rw-r--r--   0 crawford   (501) admin       (80)     1265 2023-03-22 08:38:17.000000 obsinfo-0.111.0/obsinfo/templates/components/datalogger.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      907 2023-03-21 09:51:36.000000 obsinfo-0.111.0/obsinfo/templates/components/preamplifier.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1257 2023-03-21 09:51:42.000000 obsinfo-0.111.0/obsinfo/templates/components/sensor.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.489542 obsinfo-0.111.0/obsinfo/templates/filters/
--rw-r--r--   0 crawford   (501) admin       (80)      263 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/templates/filters/AD_Conversion.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      435 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/templates/filters/FIR.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      561 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/templates/filters/PolesZeros.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      191 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/templates/filters/analog.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      390 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/templates/filters/coefficients.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      310 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/templates/filters/digital.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      379 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/templates/filters/response_list.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1327 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/templates/instrumentation.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2176 2023-04-11 08:15:41.000000 obsinfo-0.111.0/obsinfo/templates/network.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1055 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/templates/stage.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.493276 obsinfo-0.111.0/obsinfo/tests/
--rw-r--r--   0 crawford   (501) admin       (80)     2880 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/tests/CompareXMLTree.py
--rw-r--r--   0 crawford   (501) admin       (80)       17 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/tests/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     1159 2021-10-18 08:41:35.000000 obsinfo-0.111.0/obsinfo/tests/remoteGithub.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    74280 2023-03-25 15:32:18.000000 obsinfo-0.111.0/obsinfo/tests/run_test_script.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    35142 2023-03-25 15:32:14.000000 obsinfo-0.111.0/obsinfo/tests/test_datapath.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    54029 2023-03-25 15:30:33.000000 obsinfo-0.111.0/obsinfo/tests/test_infofile.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     2148 2023-02-15 16:43:20.000000 obsinfo-0.111.0/obsinfo/tests/test_main.py
--rw-r--r--   0 crawford   (501) admin       (80)       24 2023-04-12 06:32:56.000000 obsinfo-0.111.0/obsinfo/version.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:33:07.373111 obsinfo-0.111.0/obsinfo.egg-info/
--rw-r--r--   0 crawford   (501) admin       (80)     1919 2023-04-12 06:33:06.000000 obsinfo-0.111.0/obsinfo.egg-info/PKG-INFO
--rw-r--r--   0 crawford   (501) admin       (80)    14855 2023-04-12 06:33:07.000000 obsinfo-0.111.0/obsinfo.egg-info/SOURCES.txt
--rw-r--r--   0 crawford   (501) admin       (80)        1 2023-04-12 06:33:06.000000 obsinfo-0.111.0/obsinfo.egg-info/dependency_links.txt
--rw-r--r--   0 crawford   (501) admin       (80)      586 2023-04-12 06:33:07.000000 obsinfo-0.111.0/obsinfo.egg-info/entry_points.txt
--rw-r--r--   0 crawford   (501) admin       (80)       85 2023-04-12 06:33:07.000000 obsinfo-0.111.0/obsinfo.egg-info/requires.txt
--rw-r--r--   0 crawford   (501) admin       (80)        8 2023-04-12 06:33:07.000000 obsinfo-0.111.0/obsinfo.egg-info/top_level.txt
--rw-r--r--   0 crawford   (501) admin       (80)      104 2021-10-18 08:41:35.000000 obsinfo-0.111.0/pyproject.toml
--rw-r--r--   0 crawford   (501) admin       (80)       63 2023-04-12 06:33:07.494458 obsinfo-0.111.0/setup.cfg
--rw-r--r--   0 crawford   (501) admin       (80)     2261 2023-04-12 05:54:29.000000 obsinfo-0.111.0/setup.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.575257 obsinfo-0.111b1/
+-rw-r--r--   0 crawford   (501) admin       (80)    35148 2021-10-18 08:41:35.000000 obsinfo-0.111b1/LICENSE.txt
+-rw-r--r--   0 crawford   (501) admin       (80)      140 2021-10-18 08:41:35.000000 obsinfo-0.111b1/MANIFEST.in
+-rw-r--r--   0 crawford   (501) admin       (80)     1919 2023-04-12 06:31:11.575447 obsinfo-0.111b1/PKG-INFO
+-rw-r--r--   0 crawford   (501) admin       (80)     1032 2021-10-18 08:41:35.000000 obsinfo-0.111b1/README.rst
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.481113 obsinfo-0.111b1/obsinfo/
+-rw-r--r--   0 crawford   (501) admin       (80)       17 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/__init__.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.483686 obsinfo-0.111b1/obsinfo/_examples/
+-rw-r--r--   0 crawford   (501) admin       (80)    10244 2023-02-06 14:21:22.000000 obsinfo-0.111b1/obsinfo/_examples/.DS_Store
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.484720 obsinfo-0.111b1/obsinfo/_examples/Information_Files/
+-rw-r--r--   0 crawford   (501) admin       (80)    12292 2023-04-10 11:11:33.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      828 2023-02-06 14:15:15.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/README.rst
+-rw-r--r--   0 crawford   (501) admin       (80)       90 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/README.txt
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.485116 obsinfo-0.111b1/obsinfo/_examples/Information_Files/campaigns/
+-rw-r--r--   0 crawford   (501) admin       (80)     2053 2023-04-10 16:23:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/campaigns/SPOBS.campaign.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.485576 obsinfo-0.111b1/obsinfo/_examples/Information_Files/datacites/
+-rw-r--r--   0 crawford   (501) admin       (80)     1731 2023-04-10 16:23:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/datacites/EMSO-MOMAR_OBS.datacite.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.486341 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/
+-rw-r--r--   0 crawford   (501) admin       (80)     1763 2023-03-22 08:38:06.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/ADS1281.datalogger_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     5880 2023-03-22 08:38:32.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/LC2000.datalogger_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.490625 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 18:40:52.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      729 2023-04-11 18:33:44.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5321_FIR1.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      618 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      605 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.with-delay.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      556 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR3.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      592 2023-02-28 16:43:08.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_100sps-SINC.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      596 2023-02-28 16:43:14.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_200sps-SINC.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      436 2023-02-28 16:43:36.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR1.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      435 2023-02-28 16:43:35.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR2.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      443 2023-02-28 16:43:29.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR3_LINEAR.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      443 2023-02-28 16:43:33.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR4_LINEAR.stage_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.492895 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)      480 2023-02-28 16:44:38.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR2.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2412 2023-02-28 16:44:43.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR3.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      283 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR1.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      268 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR2.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      578 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR3-linear.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1118 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR4-linear.filter.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.493597 obsinfo-0.111b1/obsinfo/_examples/Information_Files/experiments/
+-rw-r--r--   0 crawford   (501) admin       (80)    16208 2023-03-01 16:50:51.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/experiments/MAYOBS.experiment.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)    19366 2023-04-10 16:23:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/experiments/MOMAR.experiment.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.497398 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-12 12:33:43.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)     3594 2023-04-12 06:20:50.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/BBOBS1_2012+.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2189 2023-04-11 21:33:49.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/BBOBS1_pre2012.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     4527 2023-03-22 08:38:31.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/GURALP_CP.instrumentation_base.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1084 2023-03-07 15:14:40.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/HYDROCT1.instrumentation_base.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1265 2023-03-07 15:14:50.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/SPOBS1.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1451 2023-03-07 15:15:08.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/SPOBS2.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1732 2023-03-07 15:20:23.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/SPOBS3-for-channel-mod-testing.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1554 2023-03-07 15:20:21.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/WBOBS1.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1885 2023-03-07 15:14:30.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/empty.instrumentation_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.498130 obsinfo-0.111b1/obsinfo/_examples/Information_Files/location_bases/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 16:53:33.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/location_bases/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)     1356 2023-02-27 22:12:01.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/location_bases/INSU-IPGP.location_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.499002 obsinfo-0.111b1/obsinfo/_examples/Information_Files/networks/
+-rw-r--r--   0 crawford   (501) admin       (80)      329 2023-04-11 08:09:43.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/networks/EMSO-AZORES.network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      413 2023-04-11 08:09:59.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/networks/RHUM-RUM.network.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.499765 obsinfo-0.111b1/obsinfo/_examples/Information_Files/operators/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-11-30 17:19:05.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/operators/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      345 2023-02-28 16:41:26.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/operators/INSU-IPGP.operator.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.501222 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/
+-rw-r--r--   0 crawford   (501) admin       (80)      159 2023-02-28 16:46:55.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/Kevin_Canjamale.person.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)       98 2023-02-28 16:47:13.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/Romuald_Daniel.person.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      100 2023-02-28 16:47:05.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/Simon_Besancon.person.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      166 2023-02-28 16:46:47.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/Wayne_Crawford.person.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.503298 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/
+-rw-r--r--   0 crawford   (501) admin       (80)      643 2023-02-27 22:11:57.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_BBOBS.preamplifier_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      448 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_DPG.preamplifier_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      811 2023-02-27 22:11:40.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_GEOPHONE.preamplifier_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      797 2023-02-27 22:11:34.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO-no_redundancy.preamplifier_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      797 2023-02-27 22:11:25.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.504754 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/
+-rw-r--r--   0 crawford   (501) admin       (80)      451 2023-02-27 22:11:22.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_BBOBS_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      662 2023-02-27 22:11:20.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_geophone_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      698 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/SIO-LDEO_DPG-Card_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      821 2023-02-27 22:11:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/Scripps_SPOBS_HydroL22_theoretical.stage_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.508004 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/
+-rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-02-06 14:13:53.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      661 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/HITECH_HTI04-PLC-ULF.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      752 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/HITECH_HTI90U.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2341 2023-04-11 21:38:03.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240__theoretical.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1425 2023-02-27 22:11:14.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240_plusDates.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      835 2023-04-11 14:10:42.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_TCOMPACT_theoretical.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      652 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SERCEL_L22.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      698 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SERCEL_L28.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2009 2023-02-27 22:11:07.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SIO_DPG.sensor_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.512065 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/
+-rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-02-06 14:13:53.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      430 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-04-PLC-ULF_voltage-mode_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1341 2023-01-09 11:31:34.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-90U_SIO-preamp_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      536 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5004_calibrated.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      527 2023-04-11 13:55:08.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5018_calibrated.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      382 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_generic_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      485 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L22D_LCHEAPO_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      537 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L28LB_LCHEAPO_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1233 2023-02-27 22:11:02.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Trillium_T240__theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      586 2023-02-27 22:11:00.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Trillium_TCompact__theoretical.stage_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.516249 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2023-01-09 11:32:20.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      280 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/HiTech_HTI-04-PLC-ULF_voltage-mode_theoretical.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      310 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__5004_2007.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      306 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__5017_2007.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      364 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      383 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Sercel_L22D_C510-S2000_generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      236 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Sercel_L28LB-obs_C395-S2490_generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      728 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN1-399_generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      873 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN400-_generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      547 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_TCompact__generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      854 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/test---attributes-poleszeros.filter.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.521703 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2023-04-11 10:41:26.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)        5 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/.obsinfo
+-rw-r--r--   0 crawford   (501) admin       (80)     3690 2023-04-11 08:10:25.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP.subnetwork.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3429 2023-04-11 21:13:12.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP_with_gain_mods.subnetwork.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2798 2023-04-11 10:40:05.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EMPTY-INSTRUMENTATION.INSU-IPGP.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2835 2023-04-12 06:00:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2211 2023-04-11 08:10:30.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential_noRefs.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1890 2023-04-11 21:46:11.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/LEAP_SECOND.INSU-IPGP.subnetwork.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3197 2023-04-11 18:07:50.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/ORIENTED.INSU-IPGP.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3092 2023-04-11 18:07:24.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/SPOBS.INSU-IPGP.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2699 2023-04-11 18:07:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/SPOBS_noAnchors.INSU-IPGP.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2017 2023-04-11 18:44:22.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/TEST.subnetwork.yaml_error.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.522621 obsinfo-0.111b1/obsinfo/_examples/Information_Files/timing_bases/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 16:53:33.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/timing_bases/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      252 2023-01-17 15:49:59.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/timing_bases/Seascan_GNSS.timing_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.473509 obsinfo-0.111b1/obsinfo/_examples/Training/
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.525281 obsinfo-0.111b1/obsinfo/_examples/Training/templates/
+-rw-r--r--   0 crawford   (501) admin       (80)     1308 2023-04-11 08:12:26.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS-train.network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3185 2023-04-11 08:12:46.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS.INSU-IPGP.network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1501 2023-01-17 18:01:07.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS1.instrumentation.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1625 2023-01-17 18:00:12.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS1_2012+.instrumentation.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      573 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/CS5322.stage.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1047 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/T240.stage.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.526768 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/
+-rw-r--r--   0 crawford   (501) admin       (80)     3049 2023-03-22 08:38:30.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/LC2000-1.datalogger.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3053 2023-03-22 08:38:26.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/LC2000.datalogger.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      907 2023-03-21 09:43:56.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/preamplifier.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1257 2023-03-21 09:44:03.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/sensor.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.530043 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)      263 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/AD_Conversion.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      673 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/CirrusLogic_FIR.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      607 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/ExampleFIR.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      409 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/HiTechPZ.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      416 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/HiTech_PolesZeros.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      191 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/analog.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      390 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/coefficients.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      310 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/digital.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      379 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/response_list.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2175 2023-04-11 08:12:58.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/network.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.531754 obsinfo-0.111b1/obsinfo/_examples/scripts/
+-rw-r--r--   0 crawford   (501) admin       (80)      292 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/README.rst
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.532400 obsinfo-0.111b1/obsinfo/_examples/scripts/add_ons/
+-rw-r--r--   0 crawford   (501) admin       (80)      331 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/add_ons/README.rst
+-rw-r--r--   0 crawford   (501) admin       (80)      952 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/add_ons/make_data_process_scripts.sh
+-rwxr-xr-x   0 crawford   (501) admin       (80)      376 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/make_stationXML.sh
+-rwxr-xr-x   0 crawford   (501) admin       (80)      420 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/print_info_files.sh
+-rwxr-xr-x   0 crawford   (501) admin       (80)     1646 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/validate_all.sh
+-rwxr-xr-x   0 crawford   (501) admin       (80)      315 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/validate_files.sh
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.534403 obsinfo-0.111b1/obsinfo/addons/
+-rw-r--r--   0 crawford   (501) admin       (80)     9904 2023-01-05 14:22:59.000000 obsinfo-0.111b1/obsinfo/addons/LC2SDS.py
+-rw-r--r--   0 crawford   (501) admin       (80)    10899 2023-01-05 14:26:17.000000 obsinfo-0.111b1/obsinfo/addons/LCHEAPO.py
+-rw-r--r--   0 crawford   (501) admin       (80)     9134 2023-04-11 08:13:40.000000 obsinfo-0.111b1/obsinfo/addons/OCA.py
+-rw-r--r--   0 crawford   (501) admin       (80)    15899 2023-04-11 08:13:46.000000 obsinfo-0.111b1/obsinfo/addons/SDPCHAIN.py
+-rw-r--r--   0 crawford   (501) admin       (80)       64 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/addons/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2481 2023-01-05 14:20:29.000000 obsinfo-0.111b1/obsinfo/addons/infodump.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.537195 obsinfo-0.111b1/obsinfo/console_scripts/
+-rw-r--r--   0 crawford   (501) admin       (80)      104 2023-04-11 12:05:29.000000 obsinfo-0.111b1/obsinfo/console_scripts/__init__.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    63491 2023-03-22 08:38:16.000000 obsinfo-0.111b1/obsinfo/console_scripts/_test.py
+-rw-r--r--   0 crawford   (501) admin       (80)     7941 2023-04-12 05:49:55.000000 obsinfo-0.111b1/obsinfo/console_scripts/makeStationXML.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     8399 2023-04-12 05:27:13.000000 obsinfo-0.111b1/obsinfo/console_scripts/print.py
+-rw-r--r--   0 crawford   (501) admin       (80)      289 2022-06-20 07:21:38.000000 obsinfo-0.111b1/obsinfo/console_scripts/print_version.py
+-rw-r--r--   0 crawford   (501) admin       (80)     8160 2023-04-12 05:54:26.000000 obsinfo-0.111b1/obsinfo/console_scripts/setup.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    17057 2023-04-12 05:58:43.000000 obsinfo-0.111b1/obsinfo/console_scripts/validate.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.475272 obsinfo-0.111b1/obsinfo/data/
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.544142 obsinfo-0.111b1/obsinfo/data/schemas/
+-rw-r--r--   0 crawford   (501) admin       (80)     8861 2023-03-03 09:25:57.000000 obsinfo-0.111b1/obsinfo/data/schemas/datacite.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     5514 2023-03-25 15:00:10.000000 obsinfo-0.111b1/obsinfo/data/schemas/datalogger_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)    10023 2023-04-11 15:24:46.000000 obsinfo-0.111b1/obsinfo/data/schemas/definitions.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-04-11 08:14:23.000000 obsinfo-0.111b1/obsinfo/data/schemas/experiment.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)    13582 2023-04-06 17:48:52.000000 obsinfo-0.111b1/obsinfo/data/schemas/filter.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     8241 2023-04-11 10:28:57.000000 obsinfo-0.111b1/obsinfo/data/schemas/instrumentation_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     1378 2022-11-30 17:16:16.000000 obsinfo-0.111b1/obsinfo/data/schemas/iris_units.json
+-rw-r--r--   0 crawford   (501) admin       (80)     6575 2023-04-11 15:31:38.000000 obsinfo-0.111b1/obsinfo/data/schemas/location_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     1922 2023-04-11 08:14:35.000000 obsinfo-0.111b1/obsinfo/data/schemas/network.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     1407 2023-04-06 14:54:32.000000 obsinfo-0.111b1/obsinfo/data/schemas/operator.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     1735 2023-02-28 08:30:05.000000 obsinfo-0.111b1/obsinfo/data/schemas/person.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     4650 2023-03-25 15:00:19.000000 obsinfo-0.111b1/obsinfo/data/schemas/preamplifier_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     6472 2023-03-25 15:00:00.000000 obsinfo-0.111b1/obsinfo/data/schemas/sensor_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     8193 2023-04-06 17:50:39.000000 obsinfo-0.111b1/obsinfo/data/schemas/stage_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     2051 2023-03-21 13:52:11.000000 obsinfo-0.111b1/obsinfo/data/schemas/stages.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     7216 2023-04-11 10:58:00.000000 obsinfo-0.111b1/obsinfo/data/schemas/subnetwork.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     3997 2023-02-28 16:48:56.000000 obsinfo-0.111b1/obsinfo/data/schemas/timing_base.schema.json
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.544468 obsinfo-0.111b1/obsinfo/datacite/
+-rw-r--r--   0 crawford   (501) admin       (80)        0 2023-01-19 09:54:12.000000 obsinfo-0.111b1/obsinfo/datacite/__init__.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.548405 obsinfo-0.111b1/obsinfo/helpers/
+-rw-r--r--   0 crawford   (501) admin       (80)      729 2023-04-11 09:20:15.000000 obsinfo-0.111b1/obsinfo/helpers/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3091 2023-04-06 13:54:33.000000 obsinfo-0.111b1/obsinfo/helpers/comments.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1565 2023-04-06 13:06:26.000000 obsinfo-0.111b1/obsinfo/helpers/external_references.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3089 2023-04-12 05:45:13.000000 obsinfo-0.111b1/obsinfo/helpers/float_with_uncert.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1518 2023-04-11 16:29:35.000000 obsinfo-0.111b1/obsinfo/helpers/functions.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1506 2023-04-11 09:14:43.000000 obsinfo-0.111b1/obsinfo/helpers/identifiers.py
+-rw-r--r--   0 crawford   (501) admin       (80)     6469 2023-04-05 13:41:46.000000 obsinfo-0.111b1/obsinfo/helpers/location.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3401 2023-04-11 14:33:07.000000 obsinfo-0.111b1/obsinfo/helpers/obsinfo_class_list.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3622 2023-04-02 23:37:37.000000 obsinfo-0.111b1/obsinfo/helpers/oi_date.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2621 2023-04-11 14:26:19.000000 obsinfo-0.111b1/obsinfo/helpers/person.py
+-rw-r--r--   0 crawford   (501) admin       (80)     7685 2023-04-06 07:43:07.000000 obsinfo-0.111b1/obsinfo/helpers/phone.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.551585 obsinfo-0.111b1/obsinfo/instrumentation/
+-rw-r--r--   0 crawford   (501) admin       (80)      830 2023-04-11 10:13:55.000000 obsinfo-0.111b1/obsinfo/instrumentation/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    11457 2023-04-12 05:43:58.000000 obsinfo-0.111b1/obsinfo/instrumentation/channel.py
+-rw-r--r--   0 crawford   (501) admin       (80)     4969 2023-04-11 15:24:42.000000 obsinfo-0.111b1/obsinfo/instrumentation/equipment.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.555415 obsinfo-0.111b1/obsinfo/instrumentation/filter/
+-rw-r--r--   0 crawford   (501) admin       (80)     1850 2023-04-03 16:39:05.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/AD_conversion.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2814 2023-04-12 06:16:41.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/FIR.py
+-rw-r--r--   0 crawford   (501) admin       (80)      506 2023-01-30 15:51:03.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1555 2023-04-11 16:22:34.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/analog.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2353 2023-04-03 16:39:20.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/coefficients.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1256 2023-04-03 16:40:13.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/digital.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3106 2023-03-10 16:10:10.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/filter.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1656 2023-04-06 17:54:00.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/filter_template.py
+-rw-r--r--   0 crawford   (501) admin       (80)     5290 2023-04-11 16:27:01.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/poles_zeros.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2442 2023-04-03 16:39:41.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/polynomial.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1854 2023-04-03 16:39:53.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/response_list.py
+-rw-r--r--   0 crawford   (501) admin       (80)    12143 2023-04-11 22:07:58.000000 obsinfo-0.111b1/obsinfo/instrumentation/instrument.py
+-rw-r--r--   0 crawford   (501) admin       (80)     9710 2023-04-11 18:45:31.000000 obsinfo-0.111b1/obsinfo/instrumentation/instrument_component.py
+-rw-r--r--   0 crawford   (501) admin       (80)    10284 2023-04-11 18:01:13.000000 obsinfo-0.111b1/obsinfo/instrumentation/instrumentation.py
+-rw-r--r--   0 crawford   (501) admin       (80)     5442 2023-03-27 23:26:01.000000 obsinfo-0.111b1/obsinfo/instrumentation/orientation.py
+-rw-r--r--   0 crawford   (501) admin       (80)    17057 2023-04-06 17:59:14.000000 obsinfo-0.111b1/obsinfo/instrumentation/stage.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2771 2023-04-03 14:12:36.000000 obsinfo-0.111b1/obsinfo/instrumentation/stages.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.557913 obsinfo-0.111b1/obsinfo/misc/
+-rw-r--r--   0 crawford   (501) admin       (80)        0 2022-06-24 14:31:17.000000 obsinfo-0.111b1/obsinfo/misc/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2497 2022-06-24 14:30:50.000000 obsinfo-0.111b1/obsinfo/misc/configuration.py
+-rw-r--r--   0 crawford   (501) admin       (80)      866 2022-06-24 14:29:23.000000 obsinfo-0.111b1/obsinfo/misc/const.py
+-rw-r--r--   0 crawford   (501) admin       (80)     4660 2022-06-24 14:27:52.000000 obsinfo-0.111b1/obsinfo/misc/discoveryfiles.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3062 2023-03-21 09:50:57.000000 obsinfo-0.111b1/obsinfo/misc/printobs.py
+-rw-r--r--   0 crawford   (501) admin       (80)     4026 2022-06-24 14:17:30.000000 obsinfo-0.111b1/obsinfo/misc/remoteGitLab.py
+-rw-r--r--   0 crawford   (501) admin       (80)    28034 2023-04-06 17:16:02.000000 obsinfo-0.111b1/obsinfo/misc/yamlref.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.558622 obsinfo-0.111b1/obsinfo/obsMetadata/
+-rw-r--r--   0 crawford   (501) admin       (80)       37 2023-02-15 09:27:51.000000 obsinfo-0.111b1/obsinfo/obsMetadata/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    25122 2023-04-11 21:42:28.000000 obsinfo-0.111b1/obsinfo/obsMetadata/obsmetadata.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.560673 obsinfo-0.111b1/obsinfo/subnetwork/
+-rw-r--r--   0 crawford   (501) admin       (80)      376 2023-04-06 14:04:52.000000 obsinfo-0.111b1/obsinfo/subnetwork/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2138 2023-04-11 10:19:15.000000 obsinfo-0.111b1/obsinfo/subnetwork/operator.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2094 2023-04-11 18:04:18.000000 obsinfo-0.111b1/obsinfo/subnetwork/processing.py
+-rw-r--r--   0 crawford   (501) admin       (80)      654 2023-04-06 13:55:11.000000 obsinfo-0.111b1/obsinfo/subnetwork/site.py
+-rw-r--r--   0 crawford   (501) admin       (80)    10316 2023-04-11 18:15:51.000000 obsinfo-0.111b1/obsinfo/subnetwork/station.py
+-rw-r--r--   0 crawford   (501) admin       (80)     6326 2023-04-11 10:58:08.000000 obsinfo-0.111b1/obsinfo/subnetwork/subnetwork.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.562051 obsinfo-0.111b1/obsinfo/template_specifications/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-12 12:14:05.000000 obsinfo-0.111b1/obsinfo/template_specifications/.DS_Store
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.563040 obsinfo-0.111b1/obsinfo/template_specifications/components/
+-rw-r--r--   0 crawford   (501) admin       (80)     1439 2023-03-22 08:38:14.000000 obsinfo-0.111b1/obsinfo/template_specifications/components/datalogger.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1076 2023-03-21 09:51:15.000000 obsinfo-0.111b1/obsinfo/template_specifications/components/preamplifier.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1438 2023-03-21 09:51:26.000000 obsinfo-0.111b1/obsinfo/template_specifications/components/sensor.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.565577 obsinfo-0.111b1/obsinfo/template_specifications/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)      276 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/AD_Conversion.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      449 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/FIR.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      603 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/PolesZeros.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      194 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/analog.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      410 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/coefficients.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      320 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/digital.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      401 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/response_list.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1419 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/instrumentation.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2483 2023-04-11 08:15:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1113 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/stage.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.567437 obsinfo-0.111b1/obsinfo/templates/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-12 12:14:05.000000 obsinfo-0.111b1/obsinfo/templates/.DS_Store
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.568612 obsinfo-0.111b1/obsinfo/templates/components/
+-rw-r--r--   0 crawford   (501) admin       (80)     1265 2023-03-22 08:38:17.000000 obsinfo-0.111b1/obsinfo/templates/components/datalogger.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      907 2023-03-21 09:51:36.000000 obsinfo-0.111b1/obsinfo/templates/components/preamplifier.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1257 2023-03-21 09:51:42.000000 obsinfo-0.111b1/obsinfo/templates/components/sensor.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.571652 obsinfo-0.111b1/obsinfo/templates/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)      263 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/AD_Conversion.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      435 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/FIR.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      561 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/PolesZeros.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      191 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/analog.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      390 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/coefficients.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      310 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/digital.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      379 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/response_list.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1327 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/instrumentation.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2176 2023-04-11 08:15:41.000000 obsinfo-0.111b1/obsinfo/templates/network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1055 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/stage.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.574845 obsinfo-0.111b1/obsinfo/tests/
+-rw-r--r--   0 crawford   (501) admin       (80)     2880 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/tests/CompareXMLTree.py
+-rw-r--r--   0 crawford   (501) admin       (80)       17 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/tests/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1159 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/tests/remoteGithub.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    74280 2023-03-25 15:32:18.000000 obsinfo-0.111b1/obsinfo/tests/run_test_script.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    35142 2023-03-25 15:32:14.000000 obsinfo-0.111b1/obsinfo/tests/test_datapath.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    54029 2023-03-25 15:30:33.000000 obsinfo-0.111b1/obsinfo/tests/test_infofile.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     2148 2023-02-15 16:43:20.000000 obsinfo-0.111b1/obsinfo/tests/test_main.py
+-rw-r--r--   0 crawford   (501) admin       (80)       24 2023-04-12 06:30:25.000000 obsinfo-0.111b1/obsinfo/version.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.483199 obsinfo-0.111b1/obsinfo.egg-info/
+-rw-r--r--   0 crawford   (501) admin       (80)     1919 2023-04-12 06:31:10.000000 obsinfo-0.111b1/obsinfo.egg-info/PKG-INFO
+-rw-r--r--   0 crawford   (501) admin       (80)    14855 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 crawford   (501) admin       (80)        1 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 crawford   (501) admin       (80)      586 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/entry_points.txt
+-rw-r--r--   0 crawford   (501) admin       (80)       85 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/requires.txt
+-rw-r--r--   0 crawford   (501) admin       (80)        8 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/top_level.txt
+-rw-r--r--   0 crawford   (501) admin       (80)      104 2021-10-18 08:41:35.000000 obsinfo-0.111b1/pyproject.toml
+-rw-r--r--   0 crawford   (501) admin       (80)       63 2023-04-12 06:31:11.576223 obsinfo-0.111b1/setup.cfg
+-rw-r--r--   0 crawford   (501) admin       (80)     2261 2023-04-12 05:54:29.000000 obsinfo-0.111b1/setup.py
```

### Comparing `obsinfo-0.111.0/LICENSE.txt` & `obsinfo-0.111b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/PKG-INFO` & `obsinfo-0.111b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsinfo
-Version: 0.111.0
+Version: 0.111b1
 Summary: Tools for documenting ocean bottom seismometer experiments and creating metadata
 Home-page: https://gitlab.com/resif/obsinfo
 Author: Wayne Crawford
 Author-email: crawford@ipgp.fr
 Keywords: seismology OBS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `obsinfo-0.111.0/README.rst` & `obsinfo-0.111b1/README.rst`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/README.rst` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/README.rst`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/campaigns/SPOBS.campaign.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/campaigns/SPOBS.campaign.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/datacites/EMSO-MOMAR_OBS.datacite.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/datacites/EMSO-MOMAR_OBS.datacite.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/ADS1281.datalogger_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/ADS1281.datalogger_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/LC2000.datalogger_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/LC2000.datalogger_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/CS5321_FIR1.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5321_FIR1.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.with-delay.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.with-delay.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR3.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR3.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_100sps-SINC.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_100sps-SINC.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_200sps-SINC.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_200sps-SINC.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR3.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR3.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR3-linear.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR3-linear.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR4-linear.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR4-linear.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/experiments/MAYOBS.experiment.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/experiments/MAYOBS.experiment.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/experiments/MOMAR.experiment.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/experiments/MOMAR.experiment.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/BBOBS1_2012+.instrumentation_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/BBOBS1_2012+.instrumentation_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/BBOBS1_pre2012.instrumentation_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/BBOBS1_pre2012.instrumentation_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/GURALP_CP.instrumentation_base.yaml_error.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/GURALP_CP.instrumentation_base.yaml_error.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/HYDROCT1.instrumentation_base.yaml_error.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/HYDROCT1.instrumentation_base.yaml_error.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/SPOBS1.instrumentation_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/SPOBS1.instrumentation_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/SPOBS2.instrumentation_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/SPOBS2.instrumentation_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/SPOBS3-for-channel-mod-testing.instrumentation_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/SPOBS3-for-channel-mod-testing.instrumentation_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/WBOBS1.instrumentation_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/WBOBS1.instrumentation_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/instrumentations/empty.instrumentation_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/empty.instrumentation_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/location_bases/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/location_bases/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/location_bases/INSU-IPGP.location_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/location_bases/INSU-IPGP.location_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/operators/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/operators/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_BBOBS.preamplifier_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_BBOBS.preamplifier_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_GEOPHONE.preamplifier_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_GEOPHONE.preamplifier_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO-no_redundancy.preamplifier_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO-no_redundancy.preamplifier_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_geophone_theoretical.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_geophone_theoretical.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/stages/SIO-LDEO_DPG-Card_theoretical.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/SIO-LDEO_DPG-Card_theoretical.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/preamplifiers/stages/Scripps_SPOBS_HydroL22_theoretical.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/Scripps_SPOBS_HydroL22_theoretical.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/HITECH_HTI04-PLC-ULF.sensor_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/HITECH_HTI04-PLC-ULF.sensor_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/HITECH_HTI90U.sensor_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/HITECH_HTI90U.sensor_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240__theoretical.sensor_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240__theoretical.sensor_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240_plusDates.sensor_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240_plusDates.sensor_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_TCOMPACT_theoretical.sensor_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_TCOMPACT_theoretical.sensor_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/SERCEL_L22.sensor_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SERCEL_L22.sensor_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/SERCEL_L28.sensor_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SERCEL_L28.sensor_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/SIO_DPG.sensor_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SIO_DPG.sensor_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-90U_SIO-preamp_theoretical.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-90U_SIO-preamp_theoretical.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5004_calibrated.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5004_calibrated.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5018_calibrated.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5018_calibrated.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L28LB_LCHEAPO_theoretical.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L28LB_LCHEAPO_theoretical.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/Trillium_T240__theoretical.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Trillium_T240__theoretical.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/Trillium_TCompact__theoretical.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Trillium_TCompact__theoretical.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN1-399_generic.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN1-399_generic.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN400-_generic.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN400-_generic.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_TCompact__generic.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_TCompact__generic.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/sensors/stages/filters/test---attributes-poleszeros.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/test---attributes-poleszeros.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP.subnetwork.yaml_error.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP.subnetwork.yaml_error.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP_with_gain_mods.subnetwork.yaml_error.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP_with_gain_mods.subnetwork.yaml_error.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/EMPTY-INSTRUMENTATION.INSU-IPGP.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EMPTY-INSTRUMENTATION.INSU-IPGP.subnetwork.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential.subnetwork.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential_noRefs.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential_noRefs.subnetwork.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/LEAP_SECOND.INSU-IPGP.subnetwork.yaml_error.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/LEAP_SECOND.INSU-IPGP.subnetwork.yaml_error.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/ORIENTED.INSU-IPGP.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/ORIENTED.INSU-IPGP.subnetwork.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/SPOBS.INSU-IPGP.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/SPOBS.INSU-IPGP.subnetwork.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/SPOBS_noAnchors.INSU-IPGP.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/SPOBS_noAnchors.INSU-IPGP.subnetwork.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/subnetworks/TEST.subnetwork.yaml_error.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/TEST.subnetwork.yaml_error.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Information_Files/timing_bases/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/timing_bases/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Training/templates/BBOBS-train.network.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS-train.network.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Training/templates/BBOBS.INSU-IPGP.network.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS.INSU-IPGP.network.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Training/templates/BBOBS1.instrumentation.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS1.instrumentation.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Training/templates/BBOBS1_2012+.instrumentation.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS1_2012+.instrumentation.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Training/templates/CS5322.stage.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/CS5322.stage.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Training/templates/T240.stage.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/T240.stage.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Training/templates/components/LC2000-1.datalogger.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/LC2000-1.datalogger.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Training/templates/components/LC2000.datalogger.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/LC2000.datalogger.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Training/templates/components/preamplifier.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/preamplifier.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Training/templates/components/sensor.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/sensor.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Training/templates/filters/CirrusLogic_FIR.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/CirrusLogic_FIR.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Training/templates/filters/ExampleFIR.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/ExampleFIR.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/Training/templates/network.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/network.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/scripts/add_ons/make_data_process_scripts.sh` & `obsinfo-0.111b1/obsinfo/_examples/scripts/add_ons/make_data_process_scripts.sh`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/_examples/scripts/validate_all.sh` & `obsinfo-0.111b1/obsinfo/_examples/scripts/validate_all.sh`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/addons/LC2SDS.py` & `obsinfo-0.111b1/obsinfo/addons/LC2SDS.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/addons/LCHEAPO.py` & `obsinfo-0.111b1/obsinfo/addons/LCHEAPO.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/addons/OCA.py` & `obsinfo-0.111b1/obsinfo/addons/OCA.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/addons/SDPCHAIN.py` & `obsinfo-0.111b1/obsinfo/addons/SDPCHAIN.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/addons/infodump.py` & `obsinfo-0.111b1/obsinfo/addons/infodump.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/console_scripts/_test.py` & `obsinfo-0.111b1/obsinfo/console_scripts/_test.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/console_scripts/makeStationXML.py` & `obsinfo-0.111b1/obsinfo/console_scripts/makeStationXML.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/console_scripts/print.py` & `obsinfo-0.111b1/obsinfo/console_scripts/print.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/console_scripts/setup.py` & `obsinfo-0.111b1/obsinfo/console_scripts/setup.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/console_scripts/validate.py` & `obsinfo-0.111b1/obsinfo/console_scripts/validate.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/datacite.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/datacite.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/datalogger_base.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/datalogger_base.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/definitions.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/definitions.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/experiment.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/experiment.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/filter.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/filter.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/instrumentation_base.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/instrumentation_base.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/iris_units.json` & `obsinfo-0.111b1/obsinfo/data/schemas/iris_units.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/location_base.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/location_base.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/network.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/network.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/operator.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/operator.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/person.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/person.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/preamplifier_base.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/preamplifier_base.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/sensor_base.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/sensor_base.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/stage_base.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/stage_base.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/stages.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/stages.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/subnetwork.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/subnetwork.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/data/schemas/timing_base.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/timing_base.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/helpers/__init__.py` & `obsinfo-0.111b1/obsinfo/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/helpers/comments.py` & `obsinfo-0.111b1/obsinfo/helpers/comments.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/helpers/external_references.py` & `obsinfo-0.111b1/obsinfo/helpers/external_references.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/helpers/float_with_uncert.py` & `obsinfo-0.111b1/obsinfo/helpers/float_with_uncert.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/helpers/functions.py` & `obsinfo-0.111b1/obsinfo/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/helpers/identifiers.py` & `obsinfo-0.111b1/obsinfo/helpers/identifiers.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/helpers/location.py` & `obsinfo-0.111b1/obsinfo/helpers/location.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/helpers/obsinfo_class_list.py` & `obsinfo-0.111b1/obsinfo/helpers/obsinfo_class_list.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/helpers/oi_date.py` & `obsinfo-0.111b1/obsinfo/helpers/oi_date.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/helpers/person.py` & `obsinfo-0.111b1/obsinfo/helpers/person.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/helpers/phone.py` & `obsinfo-0.111b1/obsinfo/helpers/phone.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/__init__.py` & `obsinfo-0.111b1/obsinfo/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/channel.py` & `obsinfo-0.111b1/obsinfo/instrumentation/channel.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/equipment.py` & `obsinfo-0.111b1/obsinfo/instrumentation/equipment.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/filter/AD_conversion.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/AD_conversion.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/filter/FIR.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/FIR.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/filter/analog.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/analog.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/filter/coefficients.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/coefficients.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/filter/digital.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/digital.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/filter/filter.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/filter.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/filter/filter_template.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/filter_template.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/filter/poles_zeros.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/poles_zeros.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/filter/polynomial.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/polynomial.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/filter/response_list.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/response_list.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/instrument.py` & `obsinfo-0.111b1/obsinfo/instrumentation/instrument.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/instrument_component.py` & `obsinfo-0.111b1/obsinfo/instrumentation/instrument_component.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/instrumentation.py` & `obsinfo-0.111b1/obsinfo/instrumentation/instrumentation.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/orientation.py` & `obsinfo-0.111b1/obsinfo/instrumentation/orientation.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/stage.py` & `obsinfo-0.111b1/obsinfo/instrumentation/stage.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/instrumentation/stages.py` & `obsinfo-0.111b1/obsinfo/instrumentation/stages.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/misc/configuration.py` & `obsinfo-0.111b1/obsinfo/misc/configuration.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/misc/const.py` & `obsinfo-0.111b1/obsinfo/misc/const.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/misc/discoveryfiles.py` & `obsinfo-0.111b1/obsinfo/misc/discoveryfiles.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/misc/printobs.py` & `obsinfo-0.111b1/obsinfo/misc/printobs.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/misc/remoteGitLab.py` & `obsinfo-0.111b1/obsinfo/misc/remoteGitLab.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/misc/yamlref.py` & `obsinfo-0.111b1/obsinfo/misc/yamlref.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/obsMetadata/obsmetadata.py` & `obsinfo-0.111b1/obsinfo/obsMetadata/obsmetadata.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/subnetwork/operator.py` & `obsinfo-0.111b1/obsinfo/subnetwork/operator.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/subnetwork/processing.py` & `obsinfo-0.111b1/obsinfo/subnetwork/processing.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/subnetwork/site.py` & `obsinfo-0.111b1/obsinfo/subnetwork/site.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/subnetwork/station.py` & `obsinfo-0.111b1/obsinfo/subnetwork/station.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/subnetwork/subnetwork.py` & `obsinfo-0.111b1/obsinfo/subnetwork/subnetwork.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/template_specifications/.DS_Store` & `obsinfo-0.111b1/obsinfo/template_specifications/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/template_specifications/components/datalogger.yaml` & `obsinfo-0.111b1/obsinfo/template_specifications/components/datalogger.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/template_specifications/components/preamplifier.yaml` & `obsinfo-0.111b1/obsinfo/template_specifications/components/preamplifier.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/template_specifications/components/sensor.yaml` & `obsinfo-0.111b1/obsinfo/template_specifications/components/sensor.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/template_specifications/filters/PolesZeros.filter.yaml` & `obsinfo-0.111b1/obsinfo/template_specifications/filters/PolesZeros.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/template_specifications/instrumentation.yaml` & `obsinfo-0.111b1/obsinfo/template_specifications/instrumentation.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/template_specifications/network.yaml` & `obsinfo-0.111b1/obsinfo/template_specifications/network.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/template_specifications/stage.yaml` & `obsinfo-0.111b1/obsinfo/template_specifications/stage.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/templates/.DS_Store` & `obsinfo-0.111b1/obsinfo/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/templates/components/datalogger.yaml` & `obsinfo-0.111b1/obsinfo/templates/components/datalogger.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/templates/components/preamplifier.yaml` & `obsinfo-0.111b1/obsinfo/templates/components/preamplifier.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/templates/components/sensor.yaml` & `obsinfo-0.111b1/obsinfo/templates/components/sensor.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/templates/filters/PolesZeros.filter.yaml` & `obsinfo-0.111b1/obsinfo/templates/filters/PolesZeros.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/templates/instrumentation.yaml` & `obsinfo-0.111b1/obsinfo/templates/instrumentation.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/templates/network.yaml` & `obsinfo-0.111b1/obsinfo/templates/network.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/templates/stage.yaml` & `obsinfo-0.111b1/obsinfo/templates/stage.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/tests/CompareXMLTree.py` & `obsinfo-0.111b1/obsinfo/tests/CompareXMLTree.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/tests/remoteGithub.py` & `obsinfo-0.111b1/obsinfo/tests/remoteGithub.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/tests/run_test_script.py` & `obsinfo-0.111b1/obsinfo/tests/run_test_script.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/tests/test_datapath.py` & `obsinfo-0.111b1/obsinfo/tests/test_datapath.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/tests/test_infofile.py` & `obsinfo-0.111b1/obsinfo/tests/test_infofile.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo/tests/test_main.py` & `obsinfo-0.111b1/obsinfo/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo.egg-info/PKG-INFO` & `obsinfo-0.111b1/obsinfo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsinfo
-Version: 0.111.0
+Version: 0.111b1
 Summary: Tools for documenting ocean bottom seismometer experiments and creating metadata
 Home-page: https://gitlab.com/resif/obsinfo
 Author: Wayne Crawford
 Author-email: crawford@ipgp.fr
 Keywords: seismology OBS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `obsinfo-0.111.0/obsinfo.egg-info/SOURCES.txt` & `obsinfo-0.111b1/obsinfo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/obsinfo.egg-info/entry_points.txt` & `obsinfo-0.111b1/obsinfo.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.0/setup.py` & `obsinfo-0.111b1/setup.py`

 * *Files identical despite different names*

