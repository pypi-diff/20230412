# Comparing `tmp/usdm-0.23.0.tar.gz` & `tmp/usdm-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usdm-0.23.0.tar", last modified: Wed Apr 12 12:54:10 2023, max compression
+gzip compressed data, was "usdm-0.24.0.tar", last modified: Wed Apr 12 18:24:16 2023, max compression
```

## Comparing `usdm-0.23.0.tar` & `usdm-0.24.0.tar`

### file list

```diff
@@ -1,124 +1,126 @@
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.384576 usdm-0.23.0/
--rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.23.0/LICENSE
--rw-r--r--   0 daveih     (501) staff       (20)    17808 2023-04-12 12:54:10.384322 usdm-0.23.0/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)    17358 2023-04-12 05:07:19.000000 usdm-0.23.0/README.md
--rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.23.0/pyproject.toml
--rw-r--r--   0 daveih     (501) staff       (20)       38 2023-04-12 12:54:10.384623 usdm-0.23.0/setup.cfg
--rw-r--r--   0 daveih     (501) staff       (20)      932 2023-04-12 12:31:13.000000 usdm-0.23.0/setup.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.279845 usdm-0.23.0/src/
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.300324 usdm-0.23.0/src/usdm.egg-info/
--rw-r--r--   0 daveih     (501) staff       (20)    17808 2023-04-12 12:54:10.000000 usdm-0.23.0/src/usdm.egg-info/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)     3866 2023-04-12 12:54:10.000000 usdm-0.23.0/src/usdm.egg-info/SOURCES.txt
--rw-r--r--   0 daveih     (501) staff       (20)        1 2023-04-12 12:54:10.000000 usdm-0.23.0/src/usdm.egg-info/dependency_links.txt
--rw-r--r--   0 daveih     (501) staff       (20)       45 2023-04-12 12:54:10.000000 usdm-0.23.0/src/usdm.egg-info/requires.txt
--rw-r--r--   0 daveih     (501) staff       (20)       32 2023-04-12 12:54:10.000000 usdm-0.23.0/src/usdm.egg-info/top_level.txt
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.318709 usdm-0.23.0/src/usdm_excel/
--rw-r--r--   0 daveih     (501) staff       (20)     1056 2023-04-12 12:34:20.000000 usdm-0.23.0/src/usdm_excel/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      269 2023-03-31 14:50:16.000000 usdm-0.23.0/src/usdm_excel/alias.py
--rw-r--r--   0 daveih     (501) staff       (20)     7697 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     3766 2023-04-05 14:21:45.000000 usdm-0.23.0/src/usdm_excel/cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      787 2023-03-31 14:50:16.000000 usdm-0.23.0/src/usdm_excel/cdisc_ct.py
--rw-r--r--   0 daveih     (501) staff       (20)     4349 2023-04-11 15:59:49.000000 usdm-0.23.0/src/usdm_excel/cdisc_ct_library.py
--rw-r--r--   0 daveih     (501) staff       (20)     1004 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/configuration_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      400 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/cross_ref.py
--rw-r--r--   0 daveih     (501) staff       (20)      337 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/ct_version_manager.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.320480 usdm-0.23.0/src/usdm_excel/data/
--rw-r--r--   0 daveih     (501) staff       (20)      927 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/data/cdisc_ct_config.yaml
--rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/data/iso_3166.json
--rw-r--r--   0 daveih     (501) staff       (20)     3453 2023-04-11 15:59:49.000000 usdm-0.23.0/src/usdm_excel/data/missing_ct.yaml
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.323398 usdm-0.23.0/src/usdm_excel/errors/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-06 07:20:00.000000 usdm-0.23.0/src/usdm_excel/errors/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      627 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/errors/error.py
--rw-r--r--   0 daveih     (501) staff       (20)      650 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/errors/errors.py
--rw-r--r--   0 daveih     (501) staff       (20)     1189 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/id_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)      737 2023-04-05 14:06:46.000000 usdm-0.23.0/src/usdm_excel/iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      111 2023-04-03 10:43:35.000000 usdm-0.23.0/src/usdm_excel/logger.py
--rw-r--r--   0 daveih     (501) staff       (20)      309 2023-03-31 14:50:16.000000 usdm-0.23.0/src/usdm_excel/ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)     3730 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/nodes_and_edges.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.325516 usdm-0.23.0/src/usdm_excel/study_design_element_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_element_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1834 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.326593 usdm-0.23.0/src/usdm_excel/study_design_encounter_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2429 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.327396 usdm-0.23.0/src/usdm_excel/study_design_estimands_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2259 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.328225 usdm-0.23.0/src/usdm_excel/study_design_ii_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_ii_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1655 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.329275 usdm-0.23.0/src/usdm_excel/study_design_objective_endpoint_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2023 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.330994 usdm-0.23.0/src/usdm_excel/study_design_population_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_population_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1631 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.339763 usdm-0.23.0/src/usdm_excel/study_design_procedure_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1590 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.340832 usdm-0.23.0/src/usdm_excel/study_design_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     5859 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.341698 usdm-0.23.0/src/usdm_excel/study_identifiers_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_identifiers_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2559 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.342963 usdm-0.23.0/src/usdm_excel/study_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     6824 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_excel/study_sheet/study_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.354113 usdm-0.23.0/src/usdm_excel/study_soa_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      637 2023-04-03 10:43:35.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/activities.py
--rw-r--r--   0 daveih     (501) staff       (20)     2899 2023-04-05 14:06:46.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      888 2023-04-05 14:06:46.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/cycle.py
--rw-r--r--   0 daveih     (501) staff       (20)     1864 2023-04-05 14:06:46.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/cycles.py
--rw-r--r--   0 daveih     (501) staff       (20)      993 2023-04-05 14:06:46.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/encounters.py
--rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/soa_column_rows.py
--rw-r--r--   0 daveih     (501) staff       (20)     4547 2023-04-11 13:28:11.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     5030 2023-04-11 15:59:49.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/timepoint.py
--rw-r--r--   0 daveih     (501) staff       (20)     2852 2023-04-05 14:06:46.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/timepoints.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.354765 usdm-0.23.0/src/usdm_info/
--rw-r--r--   0 daveih     (501) staff       (20)       59 2023-04-12 12:31:13.000000 usdm-0.23.0/src/usdm_info/__init__.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.381675 usdm-0.23.0/src/usdm_model/
--rw-r--r--   0 daveih     (501) staff       (20)     1685 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      545 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      210 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/address.py
--rw-r--r--   0 daveih     (501) staff       (20)      229 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/aliasCode.py
--rw-r--r--   0 daveih     (501) staff       (20)      229 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/alias_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      139 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/analysis_population.py
--rw-r--r--   0 daveih     (501) staff       (20)      844 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/api_base_model.py
--rw-r--r--   0 daveih     (501) staff       (20)      375 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      315 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/biomedical_concept_category.py
--rw-r--r--   0 daveih     (501) staff       (20)      394 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/biomedical_concept_property.py
--rw-r--r--   0 daveih     (501) staff       (20)      216 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/biomedical_concept_surrogate.py
--rw-r--r--   0 daveih     (501) staff       (20)      152 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/code.py
--rw-r--r--   0 daveih     (501) staff       (20)      642 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/encounter.py
--rw-r--r--   0 daveih     (501) staff       (20)      262 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/endpoint.py
--rw-r--r--   0 daveih     (501) staff       (20)      543 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/estimand.py
--rw-r--r--   0 daveih     (501) staff       (20)      224 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/indication.py
--rw-r--r--   0 daveih     (501) staff       (20)      206 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/intercurrent_event.py
--rw-r--r--   0 daveih     (501) staff       (20)      260 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/investigational_intervention.py
--rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/objective.py
--rw-r--r--   0 daveih     (501) staff       (20)      347 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/organisation.py
--rw-r--r--   0 daveih     (501) staff       (20)      274 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/procedure.py
--rw-r--r--   0 daveih     (501) staff       (20)      186 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/response_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      509 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/schedule_timeline.py
--rw-r--r--   0 daveih     (501) staff       (20)      114 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/schedule_timeline_exit.py
--rw-r--r--   0 daveih     (501) staff       (20)      738 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/scheduled_instance.py
--rw-r--r--   0 daveih     (501) staff       (20)      677 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/study.py
--rw-r--r--   0 daveih     (501) staff       (20)      296 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/study_arm.py
--rw-r--r--   0 daveih     (501) staff       (20)      380 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/study_cell.py
--rw-r--r--   0 daveih     (501) staff       (20)     1583 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/study_design.py
--rw-r--r--   0 daveih     (501) staff       (20)      351 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/study_design_population.py
--rw-r--r--   0 daveih     (501) staff       (20)      359 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/study_element.py
--rw-r--r--   0 daveih     (501) staff       (20)      401 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/study_epoch.py
--rw-r--r--   0 daveih     (501) staff       (20)      583 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/study_identifier.py
--rw-r--r--   0 daveih     (501) staff       (20)      412 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/study_protocol_version.py
--rw-r--r--   0 daveih     (501) staff       (20)      336 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/timing.py
--rw-r--r--   0 daveih     (501) staff       (20)      134 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/transition_rule.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.383877 usdm-0.23.0/tests/
--rw-r--r--   0 daveih     (501) staff       (20)    12726 2023-04-11 13:28:11.000000 usdm-0.23.0/tests/test_base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     2129 2023-04-05 14:43:30.000000 usdm-0.23.0/tests/test_cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      679 2023-04-11 13:28:11.000000 usdm-0.23.0/tests/test_error.py
--rw-r--r--   0 daveih     (501) staff       (20)     1126 2023-04-11 13:28:11.000000 usdm-0.23.0/tests/test_errors.py
--rw-r--r--   0 daveih     (501) staff       (20)      950 2023-04-05 14:06:46.000000 usdm-0.23.0/tests/test_iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      412 2023-04-05 14:06:46.000000 usdm-0.23.0/tests/test_ncit.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.807154 usdm-0.24.0/
+-rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-01-12 15:50:29.000000 usdm-0.24.0/LICENSE
+-rw-r--r--   0 daveih     (501) staff       (20)    18175 2023-04-12 18:24:16.806944 usdm-0.24.0/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)    17725 2023-04-12 18:20:23.000000 usdm-0.24.0/README.md
+-rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 15:14:44.000000 usdm-0.24.0/pyproject.toml
+-rw-r--r--   0 daveih     (501) staff       (20)       38 2023-04-12 18:24:16.807205 usdm-0.24.0/setup.cfg
+-rw-r--r--   0 daveih     (501) staff       (20)      932 2023-04-12 12:32:56.000000 usdm-0.24.0/setup.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.736124 usdm-0.24.0/src/
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.743951 usdm-0.24.0/src/usdm.egg-info/
+-rw-r--r--   0 daveih     (501) staff       (20)    18175 2023-04-12 18:24:16.000000 usdm-0.24.0/src/usdm.egg-info/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)     3928 2023-04-12 18:24:16.000000 usdm-0.24.0/src/usdm.egg-info/SOURCES.txt
+-rw-r--r--   0 daveih     (501) staff       (20)        1 2023-04-12 18:24:16.000000 usdm-0.24.0/src/usdm.egg-info/dependency_links.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       45 2023-04-12 18:24:16.000000 usdm-0.24.0/src/usdm.egg-info/requires.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       32 2023-04-12 18:24:16.000000 usdm-0.24.0/src/usdm.egg-info/top_level.txt
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.774532 usdm-0.24.0/src/usdm_excel/
+-rw-r--r--   0 daveih     (501) staff       (20)     1122 2023-04-12 17:04:52.000000 usdm-0.24.0/src/usdm_excel/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      269 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/alias.py
+-rw-r--r--   0 daveih     (501) staff       (20)     8005 2023-04-12 17:04:52.000000 usdm-0.24.0/src/usdm_excel/base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3766 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      787 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/cdisc_ct.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4349 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/cdisc_ct_library.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1366 2023-04-12 17:04:52.000000 usdm-0.24.0/src/usdm_excel/configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      400 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/cross_ref.py
+-rw-r--r--   0 daveih     (501) staff       (20)      337 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/ct_version_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.777106 usdm-0.24.0/src/usdm_excel/data/
+-rw-r--r--   0 daveih     (501) staff       (20)      927 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/data/cdisc_ct_config.yaml
+-rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/data/iso_3166.json
+-rw-r--r--   0 daveih     (501) staff       (20)     3453 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/data/missing_ct.yaml
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.782871 usdm-0.24.0/src/usdm_excel/errors/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-05 16:50:22.000000 usdm-0.24.0/src/usdm_excel/errors/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      627 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/errors/error.py
+-rw-r--r--   0 daveih     (501) staff       (20)      650 2023-04-11 18:31:21.000000 usdm-0.24.0/src/usdm_excel/errors/errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1189 2023-04-04 17:49:00.000000 usdm-0.24.0/src/usdm_excel/id_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)      737 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)      111 2023-03-31 15:48:06.000000 usdm-0.24.0/src/usdm_excel/logger.py
+-rw-r--r--   0 daveih     (501) staff       (20)      309 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3730 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/nodes_and_edges.py
+-rw-r--r--   0 daveih     (501) staff       (20)      512 2023-04-12 17:04:52.000000 usdm-0.24.0/src/usdm_excel/option_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.784535 usdm-0.24.0/src/usdm_excel/study_design_element_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_element_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1834 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.785643 usdm-0.24.0/src/usdm_excel/study_design_encounter_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2429 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.786520 usdm-0.24.0/src/usdm_excel/study_design_estimands_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2259 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.787749 usdm-0.24.0/src/usdm_excel/study_design_ii_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_ii_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1655 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.788649 usdm-0.24.0/src/usdm_excel/study_design_objective_endpoint_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2023 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.789363 usdm-0.24.0/src/usdm_excel/study_design_population_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_population_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1631 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.789855 usdm-0.24.0/src/usdm_excel/study_design_procedure_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1590 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.790292 usdm-0.24.0/src/usdm_excel/study_design_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5859 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.790763 usdm-0.24.0/src/usdm_excel/study_identifiers_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_identifiers_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2559 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.791209 usdm-0.24.0/src/usdm_excel/study_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     7158 2023-04-12 17:04:52.000000 usdm-0.24.0/src/usdm_excel/study_sheet/study_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.794033 usdm-0.24.0/src/usdm_excel/study_soa_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      637 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/activities.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2899 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      888 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/cycle.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1864 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/cycles.py
+-rw-r--r--   0 daveih     (501) staff       (20)      993 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/encounters.py
+-rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/soa_column_rows.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4547 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5048 2023-04-12 17:57:02.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/timepoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2748 2023-04-12 17:57:02.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/timepoints.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.794242 usdm-0.24.0/src/usdm_info/
+-rw-r--r--   0 daveih     (501) staff       (20)       59 2023-04-12 17:04:52.000000 usdm-0.24.0/src/usdm_info/__init__.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.804393 usdm-0.24.0/src/usdm_model/
+-rw-r--r--   0 daveih     (501) staff       (20)     1685 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      545 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      210 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/address.py
+-rw-r--r--   0 daveih     (501) staff       (20)      229 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/aliasCode.py
+-rw-r--r--   0 daveih     (501) staff       (20)      229 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/alias_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      139 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/analysis_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)      844 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/api_base_model.py
+-rw-r--r--   0 daveih     (501) staff       (20)      375 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      315 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/biomedical_concept_category.py
+-rw-r--r--   0 daveih     (501) staff       (20)      394 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/biomedical_concept_property.py
+-rw-r--r--   0 daveih     (501) staff       (20)      216 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/biomedical_concept_surrogate.py
+-rw-r--r--   0 daveih     (501) staff       (20)      152 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      642 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/encounter.py
+-rw-r--r--   0 daveih     (501) staff       (20)      262 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/endpoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)      543 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/estimand.py
+-rw-r--r--   0 daveih     (501) staff       (20)      224 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/indication.py
+-rw-r--r--   0 daveih     (501) staff       (20)      206 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/intercurrent_event.py
+-rw-r--r--   0 daveih     (501) staff       (20)      260 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/investigational_intervention.py
+-rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/objective.py
+-rw-r--r--   0 daveih     (501) staff       (20)      347 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/organisation.py
+-rw-r--r--   0 daveih     (501) staff       (20)      274 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/procedure.py
+-rw-r--r--   0 daveih     (501) staff       (20)      186 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/response_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      509 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/schedule_timeline.py
+-rw-r--r--   0 daveih     (501) staff       (20)      114 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/schedule_timeline_exit.py
+-rw-r--r--   0 daveih     (501) staff       (20)      691 2023-04-12 17:57:02.000000 usdm-0.24.0/src/usdm_model/scheduled_instance.py
+-rw-r--r--   0 daveih     (501) staff       (20)      677 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/study.py
+-rw-r--r--   0 daveih     (501) staff       (20)      296 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/study_arm.py
+-rw-r--r--   0 daveih     (501) staff       (20)      380 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/study_cell.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1583 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/study_design.py
+-rw-r--r--   0 daveih     (501) staff       (20)      351 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/study_design_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)      359 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/study_element.py
+-rw-r--r--   0 daveih     (501) staff       (20)      401 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/study_epoch.py
+-rw-r--r--   0 daveih     (501) staff       (20)      583 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/study_identifier.py
+-rw-r--r--   0 daveih     (501) staff       (20)      412 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/study_protocol_version.py
+-rw-r--r--   0 daveih     (501) staff       (20)      336 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/timing.py
+-rw-r--r--   0 daveih     (501) staff       (20)      134 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/transition_rule.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.806594 usdm-0.24.0/tests/
+-rw-r--r--   0 daveih     (501) staff       (20)    12726 2023-04-11 16:05:11.000000 usdm-0.24.0/tests/test_base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2129 2023-04-05 15:14:12.000000 usdm-0.24.0/tests/test_cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      679 2023-04-11 16:05:11.000000 usdm-0.24.0/tests/test_error.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1126 2023-04-11 16:05:11.000000 usdm-0.24.0/tests/test_errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)      950 2023-04-04 18:02:59.000000 usdm-0.24.0/tests/test_iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)      412 2023-04-04 18:04:47.000000 usdm-0.24.0/tests/test_ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)      969 2023-04-12 17:04:52.000000 usdm-0.24.0/tests/test_option_manager.py
```

### Comparing `usdm-0.23.0/LICENSE` & `usdm-0.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/PKG-INFO` & `usdm-0.24.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usdm
-Version: 0.23.0
+Version: 0.24.0
 Summary: A python package for using the CDISC TransCelerate USDM
 Author: D Iberson-Hurst
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -401,18 +401,19 @@
 #### Sheet Contents
 
 A set of rows consisting of configuration parameters. The first column is the type of configuration parameter while the second is the value. The values for specific parameters may vary in their format
 
 | Parameter | Description | Format and Values |
 | :--- | :--- | :--- |
 | CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form CT name = Version value, For example `SNOMED = 21st June 2012`|
+| SDR Prev Next | Allows for next and previous ids to be set to '' rather than null values so as to accomodate the SDR validation checks | Set to 'SDR' to use '' or leave empty to set null values |
+| SDR Root | Allows for the API specification complant JSON output to be wrpaped in a root "clinicalStudy" element so as to accomodate the SDR validation checks | Set to 'SDR' to use wrapper or leave empty to just generate the API compliant JSON |
 
 ### Content Not Suported As Yet
 
 It is intended to support all of the content in the USDM. The following features are not yet supported:
 
 - Full Arm definitions
 - Full Epoch definitions
-- Better handlingof content in timeline sheet (remove need for '-' characters)
 - BC categories
 
 See the [github issues](https://github.com/data4knowledge/usdm/issues)
```

### Comparing `usdm-0.23.0/README.md` & `usdm-0.24.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -387,18 +387,19 @@
 #### Sheet Contents
 
 A set of rows consisting of configuration parameters. The first column is the type of configuration parameter while the second is the value. The values for specific parameters may vary in their format
 
 | Parameter | Description | Format and Values |
 | :--- | :--- | :--- |
 | CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form CT name = Version value, For example `SNOMED = 21st June 2012`|
+| SDR Prev Next | Allows for next and previous ids to be set to '' rather than null values so as to accomodate the SDR validation checks | Set to 'SDR' to use '' or leave empty to set null values |
+| SDR Root | Allows for the API specification complant JSON output to be wrpaped in a root "clinicalStudy" element so as to accomodate the SDR validation checks | Set to 'SDR' to use wrapper or leave empty to just generate the API compliant JSON |
 
 ### Content Not Suported As Yet
 
 It is intended to support all of the content in the USDM. The following features are not yet supported:
 
 - Full Arm definitions
 - Full Epoch definitions
-- Better handlingof content in timeline sheet (remove need for '-' characters)
 - BC categories
 
 See the [github issues](https://github.com/data4knowledge/usdm/issues)
```

### Comparing `usdm-0.23.0/setup.py` & `usdm-0.24.0/setup.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm.egg-info/PKG-INFO` & `usdm-0.24.0/src/usdm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usdm
-Version: 0.23.0
+Version: 0.24.0
 Summary: A python package for using the CDISC TransCelerate USDM
 Author: D Iberson-Hurst
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -401,18 +401,19 @@
 #### Sheet Contents
 
 A set of rows consisting of configuration parameters. The first column is the type of configuration parameter while the second is the value. The values for specific parameters may vary in their format
 
 | Parameter | Description | Format and Values |
 | :--- | :--- | :--- |
 | CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form CT name = Version value, For example `SNOMED = 21st June 2012`|
+| SDR Prev Next | Allows for next and previous ids to be set to '' rather than null values so as to accomodate the SDR validation checks | Set to 'SDR' to use '' or leave empty to set null values |
+| SDR Root | Allows for the API specification complant JSON output to be wrpaped in a root "clinicalStudy" element so as to accomodate the SDR validation checks | Set to 'SDR' to use wrapper or leave empty to just generate the API compliant JSON |
 
 ### Content Not Suported As Yet
 
 It is intended to support all of the content in the USDM. The following features are not yet supported:
 
 - Full Arm definitions
 - Full Epoch definitions
-- Better handlingof content in timeline sheet (remove need for '-' characters)
 - BC categories
 
 See the [github issues](https://github.com/data4knowledge/usdm/issues)
```

### Comparing `usdm-0.23.0/src/usdm.egg-info/SOURCES.txt` & `usdm-0.24.0/src/usdm.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/usdm_excel/cross_ref.py
 src/usdm_excel/ct_version_manager.py
 src/usdm_excel/id_manager.py
 src/usdm_excel/iso_3166.py
 src/usdm_excel/logger.py
 src/usdm_excel/ncit.py
 src/usdm_excel/nodes_and_edges.py
+src/usdm_excel/option_manager.py
 src/usdm_excel/data/cdisc_ct_config.yaml
 src/usdm_excel/data/iso_3166.json
 src/usdm_excel/data/missing_ct.yaml
 src/usdm_excel/errors/__init__.py
 src/usdm_excel/errors/error.py
 src/usdm_excel/errors/errors.py
 src/usdm_excel/study_design_element_sheet/__init__.py
@@ -95,8 +96,9 @@
 src/usdm_model/timing.py
 src/usdm_model/transition_rule.py
 tests/test_base_sheet.py
 tests/test_cdisc_biomedical_concept.py
 tests/test_error.py
 tests/test_errors.py
 tests/test_iso_3166.py
-tests/test_ncit.py
+tests/test_ncit.py
+tests/test_option_manager.py
```

### Comparing `usdm-0.23.0/src/usdm_excel/__init__.py` & `usdm-0.24.0/src/usdm_excel/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from usdm_excel.id_manager import id_manager
 from usdm_excel.configuration_sheet import ConfigurationSheet
 from usdm_excel.study_sheet.study_sheet import StudySheet
 from usdm_excel.nodes_and_edges import NodesAndEdges
 from usdm_excel.cross_ref import cross_references
 from usdm_excel.ct_version_manager import ct_version_manager
 from usdm_excel.errors.errors import error_manager
+from usdm_excel.option_manager import *
 
 class USDMExcel():
 
   def __init__(self, file_path):
     id_manager.clear()
     cross_references.clear()
     ct_version_manager.clear()
     error_manager.clear()
+    option_manager.clear()
     self.configuration = ConfigurationSheet(file_path)
     self.study = StudySheet(file_path)
 
   def identifier(self):
     study = self.study.the_study()
     if study == None:
       return None
     else:
       return study.study_identifier()
 
   def the_study(self):
     return self.study.the_study()
   
   def to_json(self):
-    return self.study.the_study().to_json()
+    return self.study.api_root().to_json()
 
   def to_nodes_and_edges(self):
     return NodesAndEdges(self.study.the_study()).nodes_and_edges()
 
   def errors(self):
     return error_manager
```

### Comparing `usdm-0.23.0/src/usdm_excel/base_sheet.py` & `usdm-0.24.0/src/usdm_excel/base_sheet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pandas as pd
 from usdm_excel.id_manager import id_manager
 from usdm_excel.cdisc_ct import CDISCCT
 from usdm_model.code import Code
 from usdm_excel.ct_version_manager import ct_version_manager
 from usdm_excel.errors.errors import error_manager
 from usdm_excel.logger import package_logger
+from usdm_excel.option_manager import *
 
 class BaseSheet():
 
   def __init__(self, file_path, sheet_name, header=0):
     self.file_path = file_path
     self.sheet_name = sheet_name
     self.sheet = pd.read_excel(open(file_path, 'rb'), sheet_name=sheet_name, header=header)
@@ -150,20 +151,26 @@
       else:
         self._error(row_index, col_index, f"CDISC CT not found for value '{item.strip()}'.")
     return result
 
   def double_link(self, items, id, prev, next):
     for idx, item in enumerate(items):
       if idx == 0:
-        setattr(item, prev, None)
+        if option_manager.get(Options.PREVIOUS_NEXT) == PrevNextOption.NULL_STRING:
+          setattr(item, prev, "")
+        else:
+          setattr(item, prev, None)
       else:
         the_id = getattr(items[idx-1], id)
         setattr(item, prev, the_id)
       if idx == len(items)-1:  
-        setattr(item, next, None)
+        if option_manager.get(Options.PREVIOUS_NEXT) == PrevNextOption.NULL_STRING:
+          setattr(item, next, "")
+        else:
+          setattr(item, next, None)
       else:
         the_id = getattr(items[idx+1], id)
         setattr(item, next, the_id)
 
   def _decode_other_code(self, value, row_index, col_index):
     if value.strip() == "":
       return None
```

### Comparing `usdm-0.23.0/src/usdm_excel/cdisc_biomedical_concept.py` & `usdm-0.24.0/src/usdm_excel/cdisc_biomedical_concept.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/cdisc_ct.py` & `usdm-0.24.0/src/usdm_excel/cdisc_ct.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/cdisc_ct_library.py` & `usdm-0.24.0/src/usdm_excel/cdisc_ct_library.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/data/cdisc_ct_config.yaml` & `usdm-0.24.0/src/usdm_excel/data/cdisc_ct_config.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/data/iso_3166.json` & `usdm-0.24.0/src/usdm_excel/data/iso_3166.json`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/data/missing_ct.yaml` & `usdm-0.24.0/src/usdm_excel/data/missing_ct.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/errors/error.py` & `usdm-0.24.0/src/usdm_excel/errors/error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/errors/errors.py` & `usdm-0.24.0/src/usdm_excel/errors/errors.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/id_manager.py` & `usdm-0.24.0/src/usdm_excel/id_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/iso_3166.py` & `usdm-0.24.0/src/usdm_excel/iso_3166.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/nodes_and_edges.py` & `usdm-0.24.0/src/usdm_excel/nodes_and_edges.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py` & `usdm-0.24.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py` & `usdm-0.24.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py` & `usdm-0.24.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py` & `usdm-0.24.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py` & `usdm-0.24.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py` & `usdm-0.24.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py` & `usdm-0.24.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_design_sheet/study_design_sheet.py` & `usdm-0.24.0/src/usdm_excel/study_design_sheet/study_design_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py` & `usdm-0.24.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_sheet/study_sheet.py` & `usdm-0.24.0/src/usdm_excel/study_sheet/study_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,25 @@
 from usdm_excel.study_design_estimands_sheet.study_design_estimands_sheet import StudyDesignEstimandsSheet
 from usdm_excel.study_design_procedure_sheet.study_design_procedure_sheet import StudyDesignProcedureSheet
 from usdm_excel.study_design_encounter_sheet.study_design_encounter_sheet import StudyDesignEncounterSheet
 from usdm_excel.study_design_element_sheet.study_design_element_sheet import StudyDesignElementSheet
 from usdm_excel.alias import Alias
 from usdm_excel.id_manager import id_manager
 from usdm_excel.cross_ref import cross_references
+from usdm_excel.option_manager import *
+from usdm_model.api_base_model import ApiBaseModel
 from usdm_model.study import Study
 from usdm_model.study_protocol_version import StudyProtocolVersion
 import traceback
 import pandas as pd
 import datetime
 
+class SDRRoot(ApiBaseModel):
+  clinicalStudy: Study
+
 class StudySheet(BaseSheet):
 
   TITLE_ROW = 0
   VERSION_ROW = 1
   TYPE_ROW = 2
   PHASE_ROW = 3
   ACRONYM_ROW = 4
@@ -105,14 +110,21 @@
 
   def study_regulatory(self):
     return self.cdisc_code(code="C93453", decode="Study Registry")
 
   def the_study(self):
     return self.study
   
+  def api_root(self):
+    if option_manager.get(Options.ROOT) == RootOption.SDR_COMPATABLE:
+      root = SDRRoot(clinicalStudy=self.study)
+    else:
+      root = self.study
+    return root
+
   def _process_sheet(self):
     fields = [ 'briefTitle', 'officialTitle', 'publicTitle', 'scientificTitle', 'protocolVersion', 'protocolAmendment', 'protocolEffectiveDate', 'protocolStatus' ]    
     for rindex, row in self.sheet.iterrows():
       if rindex == self.TITLE_ROW:
         self.title = self.read_cell(rindex, self.PARAMS_DATA_COL)
       elif rindex == self.VERSION_ROW:
         self.version = self.read_cell(rindex, self.PARAMS_DATA_COL)
```

### Comparing `usdm-0.23.0/src/usdm_excel/study_soa_sheet/activities.py` & `usdm-0.24.0/src/usdm_excel/study_soa_sheet/activities.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_soa_sheet/activity.py` & `usdm-0.24.0/src/usdm_excel/study_soa_sheet/activity.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_soa_sheet/cycle.py` & `usdm-0.24.0/src/usdm_excel/study_soa_sheet/cycle.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_soa_sheet/cycles.py` & `usdm-0.24.0/src/usdm_excel/study_soa_sheet/cycles.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_soa_sheet/encounters.py` & `usdm-0.24.0/src/usdm_excel/study_soa_sheet/encounters.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py` & `usdm-0.24.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_excel/study_soa_sheet/timepoint.py` & `usdm-0.24.0/src/usdm_excel/study_soa_sheet/timepoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,27 +70,27 @@
 
   def _as_usdm(self):
     instance = None
     if self.timing_type in ["anchor", "next", "previous", "cycle start"]:
       timing = self._to_timing()
       instance = ScheduledActivityInstance(
         scheduledInstanceId=id_manager.build_id(ScheduledActivityInstance),
-        scheduledInstanceType=1,
+        scheduledInstanceType='ACTIVITY',
         scheduleSequenceNumber=0,
         scheduleTimelineExitId="",
         scheduledInstanceEncounterId="",
         scheduledInstanceTimings=[timing],
         scheduledInstanceTimelineId="",
         activityIds=[]
       )
       timing.relativeFromScheduledInstanceId = instance.scheduledInstanceId
     elif self.timing_type == "condition":
       instance = ScheduledDecisionInstance(
         scheduledInstanceId=id_manager.build_id(ScheduledActivityInstance),
-        scheduledInstanceType=2,
+        scheduledInstanceType='DECISION',
         scheduleSequenceNumber=0,
         scheduleTimelineExitId="",
         scheduledInstanceEncounterId="",
         scheduledInstanceTimings=[],
         scheduledInstanceTimelineId="",
         conditionAssignments=[]
       )
```

### Comparing `usdm-0.23.0/src/usdm_excel/study_soa_sheet/timepoints.py` & `usdm-0.24.0/src/usdm_excel/study_soa_sheet/timepoints.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from usdm_excel.base_sheet import BaseSheet
 from usdm_excel.study_soa_sheet.soa_column_rows import SoAColumnRows
 from usdm_excel.study_soa_sheet.timepoint import Timepoint
 from usdm_excel.id_manager import id_manager
-from usdm_model.scheduled_instance import ScheduledInstanceType
 import pandas as pd
 
 class Timepoints():
   
   def __init__(self, parent):
     #super().__init__(sheet)
     self.parent = parent
@@ -25,27 +24,27 @@
     timepoint.reference = reference
     self.items.insert(insert_at_index, timepoint)
     return timepoint
   
   def set_condition_refs(self):
     for item in self.items:
       condition = item.usdm_timepoint
-      if condition.scheduledInstanceType == ScheduledInstanceType.DECISION:
+      if condition.scheduledInstanceType == 'DECISION':
         condition_instance = self.items[item.reference].usdm_timepoint
         text = item.timing_value
         if text == "":
           text = "default, no condition set"
         condition.conditionAssignments.append([text, condition_instance.scheduledInstanceId])
     previous_item = None
     for item in self.items:
       if previous_item == None:
         previous_item = item        
         continue
       previous_condition = previous_item.usdm_timepoint
-      if previous_condition.scheduledInstanceType == ScheduledInstanceType.DECISION:
+      if previous_condition.scheduledInstanceType == 'DECISION':
         current_instance = item.usdm_timepoint
         previous_condition.conditionAssignments.append(["default", current_instance.scheduledInstanceId])        
       previous_item = item        
 
   def _build_timepoints(self):    
     for col_index in range(self.parent.sheet.shape[1]):
       if col_index >= SoAColumnRows.FIRST_VISIT_COL:
```

### Comparing `usdm-0.23.0/src/usdm_model/__init__.py` & `usdm-0.24.0/src/usdm_model/__init__.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_model/activity.py` & `usdm-0.24.0/src/usdm_model/activity.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_model/api_base_model.py` & `usdm-0.24.0/src/usdm_model/api_base_model.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_model/encounter.py` & `usdm-0.24.0/src/usdm_model/encounter.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_model/estimand.py` & `usdm-0.24.0/src/usdm_model/estimand.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_model/scheduled_instance.py` & `usdm-0.24.0/src/usdm_model/scheduled_instance.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from enum import Enum
-from typing import List, Dict, Union
+from typing import List, Dict, Union, Literal
 
 from .api_base_model import ApiBaseModel
 from .timing import Timing
 
-class ScheduledInstanceType(Enum):
-  ACTIVITY = 1
-  DECISION = 2
-
 class ScheduledInstance(ApiBaseModel):
     scheduledInstanceId: str
-    scheduledInstanceType: ScheduledInstanceType
+    scheduledInstanceType: Literal['ACTIVITY', 'DECISION']
     scheduleSequenceNumber: int
     scheduleTimelineExitId: Union[str, None] = None
     scheduledInstanceEncounterId: Union[str, None] = None
     scheduledInstanceTimings: List[Timing] = []
     scheduledInstanceTimelineId: Union[str, None] = None
 
 class ScheduledActivityInstance(ScheduledInstance):
```

### Comparing `usdm-0.23.0/src/usdm_model/study.py` & `usdm-0.24.0/src/usdm_model/study.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_model/study_design.py` & `usdm-0.24.0/src/usdm_model/study_design.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/src/usdm_model/study_identifier.py` & `usdm-0.24.0/src/usdm_model/study_identifier.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/tests/test_base_sheet.py` & `usdm-0.24.0/tests/test_base_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/tests/test_cdisc_biomedical_concept.py` & `usdm-0.24.0/tests/test_cdisc_biomedical_concept.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/tests/test_error.py` & `usdm-0.24.0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/tests/test_errors.py` & `usdm-0.24.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `usdm-0.23.0/tests/test_iso_3166.py` & `usdm-0.24.0/tests/test_iso_3166.py`

 * *Files identical despite different names*

