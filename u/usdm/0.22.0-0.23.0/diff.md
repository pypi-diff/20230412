# Comparing `tmp/usdm-0.22.0.tar.gz` & `tmp/usdm-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usdm-0.22.0.tar", last modified: Tue Apr 11 16:09:48 2023, max compression
+gzip compressed data, was "usdm-0.23.0.tar", last modified: Wed Apr 12 12:54:10 2023, max compression
```

## Comparing `usdm-0.22.0.tar` & `usdm-0.23.0.tar`

### file list

```diff
@@ -1,122 +1,124 @@
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.119456 usdm-0.22.0/
--rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-01-12 15:50:29.000000 usdm-0.22.0/LICENSE
--rw-r--r--   0 daveih     (501) staff       (20)    17709 2023-04-11 16:09:48.119241 usdm-0.22.0/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)    17259 2023-04-04 16:09:15.000000 usdm-0.22.0/README.md
--rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 15:14:44.000000 usdm-0.22.0/pyproject.toml
--rw-r--r--   0 daveih     (501) staff       (20)       38 2023-04-11 16:09:48.119503 usdm-0.22.0/setup.cfg
--rw-r--r--   0 daveih     (501) staff       (20)      823 2023-04-11 16:04:30.000000 usdm-0.22.0/setup.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.076887 usdm-0.22.0/src/
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.080763 usdm-0.22.0/src/usdm.egg-info/
--rw-r--r--   0 daveih     (501) staff       (20)    17709 2023-04-11 16:09:48.000000 usdm-0.22.0/src/usdm.egg-info/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)     3840 2023-04-11 16:09:48.000000 usdm-0.22.0/src/usdm.egg-info/SOURCES.txt
--rw-r--r--   0 daveih     (501) staff       (20)        1 2023-04-11 16:09:48.000000 usdm-0.22.0/src/usdm.egg-info/dependency_links.txt
--rw-r--r--   0 daveih     (501) staff       (20)       45 2023-04-11 16:09:48.000000 usdm-0.22.0/src/usdm.egg-info/requires.txt
--rw-r--r--   0 daveih     (501) staff       (20)       22 2023-04-11 16:09:48.000000 usdm-0.22.0/src/usdm.egg-info/top_level.txt
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.086929 usdm-0.22.0/src/usdm_excel/
--rw-r--r--   0 daveih     (501) staff       (20)     1030 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      269 2023-04-05 16:39:25.000000 usdm-0.22.0/src/usdm_excel/alias.py
--rw-r--r--   0 daveih     (501) staff       (20)     7697 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     3766 2023-04-05 16:39:25.000000 usdm-0.22.0/src/usdm_excel/cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      787 2023-04-05 16:39:25.000000 usdm-0.22.0/src/usdm_excel/cdisc_ct.py
--rw-r--r--   0 daveih     (501) staff       (20)     4349 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/cdisc_ct_library.py
--rw-r--r--   0 daveih     (501) staff       (20)     1004 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/configuration_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      400 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/cross_ref.py
--rw-r--r--   0 daveih     (501) staff       (20)      337 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/ct_version_manager.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.088203 usdm-0.22.0/src/usdm_excel/data/
--rw-r--r--   0 daveih     (501) staff       (20)      927 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/data/cdisc_ct_config.yaml
--rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/data/iso_3166.json
--rw-r--r--   0 daveih     (501) staff       (20)     3453 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/data/missing_ct.yaml
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.089403 usdm-0.22.0/src/usdm_excel/errors/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-05 16:50:22.000000 usdm-0.22.0/src/usdm_excel/errors/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      627 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/errors/error.py
--rw-r--r--   0 daveih     (501) staff       (20)      650 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/errors/errors.py
--rw-r--r--   0 daveih     (501) staff       (20)     1189 2023-04-04 17:49:00.000000 usdm-0.22.0/src/usdm_excel/id_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)      737 2023-04-05 16:39:25.000000 usdm-0.22.0/src/usdm_excel/iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      111 2023-03-31 15:48:06.000000 usdm-0.22.0/src/usdm_excel/logger.py
--rw-r--r--   0 daveih     (501) staff       (20)      309 2023-04-05 16:39:25.000000 usdm-0.22.0/src/usdm_excel/ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)     3730 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/nodes_and_edges.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.090226 usdm-0.22.0/src/usdm_excel/study_design_element_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/study_design_element_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1834 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.091003 usdm-0.22.0/src/usdm_excel/study_design_encounter_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2429 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.091687 usdm-0.22.0/src/usdm_excel/study_design_estimands_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2259 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.092412 usdm-0.22.0/src/usdm_excel/study_design_ii_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/study_design_ii_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1655 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.093376 usdm-0.22.0/src/usdm_excel/study_design_objective_endpoint_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2023 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.094602 usdm-0.22.0/src/usdm_excel/study_design_population_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/study_design_population_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1631 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.095524 usdm-0.22.0/src/usdm_excel/study_design_procedure_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1590 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.096223 usdm-0.22.0/src/usdm_excel/study_design_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/study_design_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     5859 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.096937 usdm-0.22.0/src/usdm_excel/study_identifiers_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/study_identifiers_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2559 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.097635 usdm-0.22.0/src/usdm_excel/study_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/study_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     6824 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/study_sheet/study_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.101112 usdm-0.22.0/src/usdm_excel/study_soa_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/study_soa_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      637 2023-04-05 16:39:25.000000 usdm-0.22.0/src/usdm_excel/study_soa_sheet/activities.py
--rw-r--r--   0 daveih     (501) staff       (20)     2899 2023-04-05 16:39:25.000000 usdm-0.22.0/src/usdm_excel/study_soa_sheet/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      888 2023-04-05 16:39:25.000000 usdm-0.22.0/src/usdm_excel/study_soa_sheet/cycle.py
--rw-r--r--   0 daveih     (501) staff       (20)     1864 2023-04-05 16:39:25.000000 usdm-0.22.0/src/usdm_excel/study_soa_sheet/cycles.py
--rw-r--r--   0 daveih     (501) staff       (20)      993 2023-04-05 16:39:25.000000 usdm-0.22.0/src/usdm_excel/study_soa_sheet/encounters.py
--rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_excel/study_soa_sheet/soa_column_rows.py
--rw-r--r--   0 daveih     (501) staff       (20)     4547 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     5030 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_excel/study_soa_sheet/timepoint.py
--rw-r--r--   0 daveih     (501) staff       (20)     2852 2023-04-05 16:39:25.000000 usdm-0.22.0/src/usdm_excel/study_soa_sheet/timepoints.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.116914 usdm-0.22.0/src/usdm_model/
--rw-r--r--   0 daveih     (501) staff       (20)     1685 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      545 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_model/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      210 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_model/address.py
--rw-r--r--   0 daveih     (501) staff       (20)      229 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_model/aliasCode.py
--rw-r--r--   0 daveih     (501) staff       (20)      229 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/alias_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      139 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/analysis_population.py
--rw-r--r--   0 daveih     (501) staff       (20)      844 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/api_base_model.py
--rw-r--r--   0 daveih     (501) staff       (20)      375 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      315 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/biomedical_concept_category.py
--rw-r--r--   0 daveih     (501) staff       (20)      394 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/biomedical_concept_property.py
--rw-r--r--   0 daveih     (501) staff       (20)      216 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/biomedical_concept_surrogate.py
--rw-r--r--   0 daveih     (501) staff       (20)      152 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/code.py
--rw-r--r--   0 daveih     (501) staff       (20)      642 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/encounter.py
--rw-r--r--   0 daveih     (501) staff       (20)      262 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/endpoint.py
--rw-r--r--   0 daveih     (501) staff       (20)      543 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/estimand.py
--rw-r--r--   0 daveih     (501) staff       (20)      224 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/indication.py
--rw-r--r--   0 daveih     (501) staff       (20)      206 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/intercurrent_event.py
--rw-r--r--   0 daveih     (501) staff       (20)      260 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/investigational_intervention.py
--rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/objective.py
--rw-r--r--   0 daveih     (501) staff       (20)      347 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/organisation.py
--rw-r--r--   0 daveih     (501) staff       (20)      274 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_model/procedure.py
--rw-r--r--   0 daveih     (501) staff       (20)      186 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/response_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      509 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_model/schedule_timeline.py
--rw-r--r--   0 daveih     (501) staff       (20)      114 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/schedule_timeline_exit.py
--rw-r--r--   0 daveih     (501) staff       (20)      738 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_model/scheduled_instance.py
--rw-r--r--   0 daveih     (501) staff       (20)      677 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/study.py
--rw-r--r--   0 daveih     (501) staff       (20)      296 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_model/study_arm.py
--rw-r--r--   0 daveih     (501) staff       (20)      380 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/study_cell.py
--rw-r--r--   0 daveih     (501) staff       (20)     1583 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_model/study_design.py
--rw-r--r--   0 daveih     (501) staff       (20)      351 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/study_design_population.py
--rw-r--r--   0 daveih     (501) staff       (20)      359 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/study_element.py
--rw-r--r--   0 daveih     (501) staff       (20)      401 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/study_epoch.py
--rw-r--r--   0 daveih     (501) staff       (20)      583 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/study_identifier.py
--rw-r--r--   0 daveih     (501) staff       (20)      412 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/study_protocol_version.py
--rw-r--r--   0 daveih     (501) staff       (20)      336 2023-04-11 16:05:11.000000 usdm-0.22.0/src/usdm_model/timing.py
--rw-r--r--   0 daveih     (501) staff       (20)      134 2023-03-31 15:14:44.000000 usdm-0.22.0/src/usdm_model/transition_rule.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-11 16:09:48.118800 usdm-0.22.0/tests/
--rw-r--r--   0 daveih     (501) staff       (20)    12726 2023-04-11 16:05:11.000000 usdm-0.22.0/tests/test_base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     2129 2023-04-05 15:14:12.000000 usdm-0.22.0/tests/test_cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      679 2023-04-11 16:05:11.000000 usdm-0.22.0/tests/test_error.py
--rw-r--r--   0 daveih     (501) staff       (20)     1126 2023-04-11 16:05:11.000000 usdm-0.22.0/tests/test_errors.py
--rw-r--r--   0 daveih     (501) staff       (20)      950 2023-04-04 18:02:59.000000 usdm-0.22.0/tests/test_iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      412 2023-04-04 18:04:47.000000 usdm-0.22.0/tests/test_ncit.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.384576 usdm-0.23.0/
+-rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.23.0/LICENSE
+-rw-r--r--   0 daveih     (501) staff       (20)    17808 2023-04-12 12:54:10.384322 usdm-0.23.0/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)    17358 2023-04-12 05:07:19.000000 usdm-0.23.0/README.md
+-rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.23.0/pyproject.toml
+-rw-r--r--   0 daveih     (501) staff       (20)       38 2023-04-12 12:54:10.384623 usdm-0.23.0/setup.cfg
+-rw-r--r--   0 daveih     (501) staff       (20)      932 2023-04-12 12:31:13.000000 usdm-0.23.0/setup.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.279845 usdm-0.23.0/src/
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.300324 usdm-0.23.0/src/usdm.egg-info/
+-rw-r--r--   0 daveih     (501) staff       (20)    17808 2023-04-12 12:54:10.000000 usdm-0.23.0/src/usdm.egg-info/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)     3866 2023-04-12 12:54:10.000000 usdm-0.23.0/src/usdm.egg-info/SOURCES.txt
+-rw-r--r--   0 daveih     (501) staff       (20)        1 2023-04-12 12:54:10.000000 usdm-0.23.0/src/usdm.egg-info/dependency_links.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       45 2023-04-12 12:54:10.000000 usdm-0.23.0/src/usdm.egg-info/requires.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       32 2023-04-12 12:54:10.000000 usdm-0.23.0/src/usdm.egg-info/top_level.txt
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.318709 usdm-0.23.0/src/usdm_excel/
+-rw-r--r--   0 daveih     (501) staff       (20)     1056 2023-04-12 12:34:20.000000 usdm-0.23.0/src/usdm_excel/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      269 2023-03-31 14:50:16.000000 usdm-0.23.0/src/usdm_excel/alias.py
+-rw-r--r--   0 daveih     (501) staff       (20)     7697 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3766 2023-04-05 14:21:45.000000 usdm-0.23.0/src/usdm_excel/cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      787 2023-03-31 14:50:16.000000 usdm-0.23.0/src/usdm_excel/cdisc_ct.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4349 2023-04-11 15:59:49.000000 usdm-0.23.0/src/usdm_excel/cdisc_ct_library.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1004 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      400 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/cross_ref.py
+-rw-r--r--   0 daveih     (501) staff       (20)      337 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/ct_version_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.320480 usdm-0.23.0/src/usdm_excel/data/
+-rw-r--r--   0 daveih     (501) staff       (20)      927 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/data/cdisc_ct_config.yaml
+-rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/data/iso_3166.json
+-rw-r--r--   0 daveih     (501) staff       (20)     3453 2023-04-11 15:59:49.000000 usdm-0.23.0/src/usdm_excel/data/missing_ct.yaml
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.323398 usdm-0.23.0/src/usdm_excel/errors/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-06 07:20:00.000000 usdm-0.23.0/src/usdm_excel/errors/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      627 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/errors/error.py
+-rw-r--r--   0 daveih     (501) staff       (20)      650 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/errors/errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1189 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/id_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)      737 2023-04-05 14:06:46.000000 usdm-0.23.0/src/usdm_excel/iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)      111 2023-04-03 10:43:35.000000 usdm-0.23.0/src/usdm_excel/logger.py
+-rw-r--r--   0 daveih     (501) staff       (20)      309 2023-03-31 14:50:16.000000 usdm-0.23.0/src/usdm_excel/ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3730 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/nodes_and_edges.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.325516 usdm-0.23.0/src/usdm_excel/study_design_element_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_element_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1834 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.326593 usdm-0.23.0/src/usdm_excel/study_design_encounter_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2429 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.327396 usdm-0.23.0/src/usdm_excel/study_design_estimands_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2259 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.328225 usdm-0.23.0/src/usdm_excel/study_design_ii_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_ii_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1655 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.329275 usdm-0.23.0/src/usdm_excel/study_design_objective_endpoint_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2023 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.330994 usdm-0.23.0/src/usdm_excel/study_design_population_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_population_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1631 2023-04-11 13:28:10.000000 usdm-0.23.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.339763 usdm-0.23.0/src/usdm_excel/study_design_procedure_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1590 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.340832 usdm-0.23.0/src/usdm_excel/study_design_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_design_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5859 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.341698 usdm-0.23.0/src/usdm_excel/study_identifiers_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_identifiers_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2559 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.342963 usdm-0.23.0/src/usdm_excel/study_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     6824 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_excel/study_sheet/study_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.354113 usdm-0.23.0/src/usdm_excel/study_soa_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      637 2023-04-03 10:43:35.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/activities.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2899 2023-04-05 14:06:46.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      888 2023-04-05 14:06:46.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/cycle.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1864 2023-04-05 14:06:46.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/cycles.py
+-rw-r--r--   0 daveih     (501) staff       (20)      993 2023-04-05 14:06:46.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/encounters.py
+-rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/soa_column_rows.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4547 2023-04-11 13:28:11.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5030 2023-04-11 15:59:49.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/timepoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2852 2023-04-05 14:06:46.000000 usdm-0.23.0/src/usdm_excel/study_soa_sheet/timepoints.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.354765 usdm-0.23.0/src/usdm_info/
+-rw-r--r--   0 daveih     (501) staff       (20)       59 2023-04-12 12:31:13.000000 usdm-0.23.0/src/usdm_info/__init__.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.381675 usdm-0.23.0/src/usdm_model/
+-rw-r--r--   0 daveih     (501) staff       (20)     1685 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      545 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      210 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/address.py
+-rw-r--r--   0 daveih     (501) staff       (20)      229 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/aliasCode.py
+-rw-r--r--   0 daveih     (501) staff       (20)      229 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/alias_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      139 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/analysis_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)      844 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/api_base_model.py
+-rw-r--r--   0 daveih     (501) staff       (20)      375 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      315 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/biomedical_concept_category.py
+-rw-r--r--   0 daveih     (501) staff       (20)      394 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/biomedical_concept_property.py
+-rw-r--r--   0 daveih     (501) staff       (20)      216 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/biomedical_concept_surrogate.py
+-rw-r--r--   0 daveih     (501) staff       (20)      152 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      642 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/encounter.py
+-rw-r--r--   0 daveih     (501) staff       (20)      262 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/endpoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)      543 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/estimand.py
+-rw-r--r--   0 daveih     (501) staff       (20)      224 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/indication.py
+-rw-r--r--   0 daveih     (501) staff       (20)      206 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/intercurrent_event.py
+-rw-r--r--   0 daveih     (501) staff       (20)      260 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/investigational_intervention.py
+-rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/objective.py
+-rw-r--r--   0 daveih     (501) staff       (20)      347 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/organisation.py
+-rw-r--r--   0 daveih     (501) staff       (20)      274 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/procedure.py
+-rw-r--r--   0 daveih     (501) staff       (20)      186 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/response_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      509 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/schedule_timeline.py
+-rw-r--r--   0 daveih     (501) staff       (20)      114 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/schedule_timeline_exit.py
+-rw-r--r--   0 daveih     (501) staff       (20)      738 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/scheduled_instance.py
+-rw-r--r--   0 daveih     (501) staff       (20)      677 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/study.py
+-rw-r--r--   0 daveih     (501) staff       (20)      296 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/study_arm.py
+-rw-r--r--   0 daveih     (501) staff       (20)      380 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/study_cell.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1583 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/study_design.py
+-rw-r--r--   0 daveih     (501) staff       (20)      351 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/study_design_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)      359 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/study_element.py
+-rw-r--r--   0 daveih     (501) staff       (20)      401 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/study_epoch.py
+-rw-r--r--   0 daveih     (501) staff       (20)      583 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/study_identifier.py
+-rw-r--r--   0 daveih     (501) staff       (20)      412 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/study_protocol_version.py
+-rw-r--r--   0 daveih     (501) staff       (20)      336 2023-04-11 13:59:38.000000 usdm-0.23.0/src/usdm_model/timing.py
+-rw-r--r--   0 daveih     (501) staff       (20)      134 2023-03-31 13:46:27.000000 usdm-0.23.0/src/usdm_model/transition_rule.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 12:54:10.383877 usdm-0.23.0/tests/
+-rw-r--r--   0 daveih     (501) staff       (20)    12726 2023-04-11 13:28:11.000000 usdm-0.23.0/tests/test_base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2129 2023-04-05 14:43:30.000000 usdm-0.23.0/tests/test_cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      679 2023-04-11 13:28:11.000000 usdm-0.23.0/tests/test_error.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1126 2023-04-11 13:28:11.000000 usdm-0.23.0/tests/test_errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)      950 2023-04-05 14:06:46.000000 usdm-0.23.0/tests/test_iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)      412 2023-04-05 14:06:46.000000 usdm-0.23.0/tests/test_ncit.py
```

### Comparing `usdm-0.22.0/LICENSE` & `usdm-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/PKG-INFO` & `usdm-0.23.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usdm
-Version: 0.22.0
+Version: 0.23.0
 Summary: A python package for using the CDISC TransCelerate USDM
 Author: D Iberson-Hurst
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -342,18 +342,20 @@
 #### Sheet Contents
 
 A header row in row 1 followed by repeating rows from row 2, containing procedure definitions.
 
 | Column | Column Name | Description | Format and Values |
 | :--- | :--- | :--- | :--- |
 | A | xref | Identifier | Text string |
-| B | procedureType	| Type | Text string |
-| C | procedureCode	| Code reference | External CT reference  |
-| D | procedureIsConditional | Conditional flag | Boolean |
-| E | procedureIsConditionalReason | Reason | Text string |
+| B | procedureName	| Type | Text string |
+| C | procedureDescription	| Type | Text string |
+| D | procedureType	| Type | Text string |
+| E | procedureCode	| Code reference | External CT reference  |
+| F | procedureIsConditional | Conditional flag | Boolean |
+| G | procedureIsConditionalReason | Reason | Text string |
 
 ### Study Design Encounters sheet
 
 #### Sheet Name
 
 `studyDesignEncounters`
```

### Comparing `usdm-0.22.0/README.md` & `usdm-0.23.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -328,18 +328,20 @@
 #### Sheet Contents
 
 A header row in row 1 followed by repeating rows from row 2, containing procedure definitions.
 
 | Column | Column Name | Description | Format and Values |
 | :--- | :--- | :--- | :--- |
 | A | xref | Identifier | Text string |
-| B | procedureType	| Type | Text string |
-| C | procedureCode	| Code reference | External CT reference  |
-| D | procedureIsConditional | Conditional flag | Boolean |
-| E | procedureIsConditionalReason | Reason | Text string |
+| B | procedureName	| Type | Text string |
+| C | procedureDescription	| Type | Text string |
+| D | procedureType	| Type | Text string |
+| E | procedureCode	| Code reference | External CT reference  |
+| F | procedureIsConditional | Conditional flag | Boolean |
+| G | procedureIsConditionalReason | Reason | Text string |
 
 ### Study Design Encounters sheet
 
 #### Sheet Name
 
 `studyDesignEncounters`
```

### Comparing `usdm-0.22.0/setup.py` & `usdm-0.23.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
+version = {}
+with open("src/usdm_info/__init__.py") as fp:
+  exec(fp.read(), version)
+
 setuptools.setup(
   name="usdm",
-  version="0.22.0",
+  version=version['__package_version__'],
   author="D Iberson-Hurst",
   author_email="",
   description="A python package for using the CDISC TransCelerate USDM",
   long_description=long_description,
   long_description_content_type="text/markdown",
   install_requires=['pandas', 'openpyxl', 'pydantic', 'requests', 'stringcase'],
   packages=setuptools.find_packages(where="src"),
```

### Comparing `usdm-0.22.0/src/usdm.egg-info/PKG-INFO` & `usdm-0.23.0/src/usdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usdm
-Version: 0.22.0
+Version: 0.23.0
 Summary: A python package for using the CDISC TransCelerate USDM
 Author: D Iberson-Hurst
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -342,18 +342,20 @@
 #### Sheet Contents
 
 A header row in row 1 followed by repeating rows from row 2, containing procedure definitions.
 
 | Column | Column Name | Description | Format and Values |
 | :--- | :--- | :--- | :--- |
 | A | xref | Identifier | Text string |
-| B | procedureType	| Type | Text string |
-| C | procedureCode	| Code reference | External CT reference  |
-| D | procedureIsConditional | Conditional flag | Boolean |
-| E | procedureIsConditionalReason | Reason | Text string |
+| B | procedureName	| Type | Text string |
+| C | procedureDescription	| Type | Text string |
+| D | procedureType	| Type | Text string |
+| E | procedureCode	| Code reference | External CT reference  |
+| F | procedureIsConditional | Conditional flag | Boolean |
+| G | procedureIsConditionalReason | Reason | Text string |
 
 ### Study Design Encounters sheet
 
 #### Sheet Name
 
 `studyDesignEncounters`
```

### Comparing `usdm-0.22.0/src/usdm.egg-info/SOURCES.txt` & `usdm-0.23.0/src/usdm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 src/usdm_excel/study_soa_sheet/cycle.py
 src/usdm_excel/study_soa_sheet/cycles.py
 src/usdm_excel/study_soa_sheet/encounters.py
 src/usdm_excel/study_soa_sheet/soa_column_rows.py
 src/usdm_excel/study_soa_sheet/study_soa_sheet.py
 src/usdm_excel/study_soa_sheet/timepoint.py
 src/usdm_excel/study_soa_sheet/timepoints.py
+src/usdm_info/__init__.py
 src/usdm_model/__init__.py
 src/usdm_model/activity.py
 src/usdm_model/address.py
 src/usdm_model/aliasCode.py
 src/usdm_model/alias_code.py
 src/usdm_model/analysis_population.py
 src/usdm_model/api_base_model.py
```

### Comparing `usdm-0.22.0/src/usdm_excel/__init__.py` & `usdm-0.23.0/src/usdm_excel/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 class USDMExcel():
 
   def __init__(self, file_path):
     id_manager.clear()
     cross_references.clear()
     ct_version_manager.clear()
+    error_manager.clear()
     self.configuration = ConfigurationSheet(file_path)
     self.study = StudySheet(file_path)
 
   def identifier(self):
     study = self.study.the_study()
     if study == None:
       return None
```

### Comparing `usdm-0.22.0/src/usdm_excel/base_sheet.py` & `usdm-0.23.0/src/usdm_excel/base_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/cdisc_biomedical_concept.py` & `usdm-0.23.0/src/usdm_excel/cdisc_biomedical_concept.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/cdisc_ct.py` & `usdm-0.23.0/src/usdm_excel/cdisc_ct.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/cdisc_ct_library.py` & `usdm-0.23.0/src/usdm_excel/cdisc_ct_library.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/configuration_sheet.py` & `usdm-0.23.0/src/usdm_excel/configuration_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/data/cdisc_ct_config.yaml` & `usdm-0.23.0/src/usdm_excel/data/cdisc_ct_config.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/data/iso_3166.json` & `usdm-0.23.0/src/usdm_excel/data/iso_3166.json`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/data/missing_ct.yaml` & `usdm-0.23.0/src/usdm_excel/data/missing_ct.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/errors/error.py` & `usdm-0.23.0/src/usdm_excel/errors/error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/errors/errors.py` & `usdm-0.23.0/src/usdm_excel/errors/errors.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/id_manager.py` & `usdm-0.23.0/src/usdm_excel/id_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/iso_3166.py` & `usdm-0.23.0/src/usdm_excel/iso_3166.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/nodes_and_edges.py` & `usdm-0.23.0/src/usdm_excel/nodes_and_edges.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py` & `usdm-0.23.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py` & `usdm-0.23.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py` & `usdm-0.23.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py` & `usdm-0.23.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py` & `usdm-0.23.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py` & `usdm-0.23.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py` & `usdm-0.23.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_design_sheet/study_design_sheet.py` & `usdm-0.23.0/src/usdm_excel/study_design_sheet/study_design_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py` & `usdm-0.23.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_sheet/study_sheet.py` & `usdm-0.23.0/src/usdm_excel/study_sheet/study_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_soa_sheet/activities.py` & `usdm-0.23.0/src/usdm_excel/study_soa_sheet/activities.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_soa_sheet/activity.py` & `usdm-0.23.0/src/usdm_excel/study_soa_sheet/activity.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_soa_sheet/cycle.py` & `usdm-0.23.0/src/usdm_excel/study_soa_sheet/cycle.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_soa_sheet/cycles.py` & `usdm-0.23.0/src/usdm_excel/study_soa_sheet/cycles.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_soa_sheet/encounters.py` & `usdm-0.23.0/src/usdm_excel/study_soa_sheet/encounters.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py` & `usdm-0.23.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_soa_sheet/timepoint.py` & `usdm-0.23.0/src/usdm_excel/study_soa_sheet/timepoint.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_excel/study_soa_sheet/timepoints.py` & `usdm-0.23.0/src/usdm_excel/study_soa_sheet/timepoints.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_model/__init__.py` & `usdm-0.23.0/src/usdm_model/__init__.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_model/activity.py` & `usdm-0.23.0/src/usdm_model/activity.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_model/api_base_model.py` & `usdm-0.23.0/src/usdm_model/api_base_model.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_model/encounter.py` & `usdm-0.23.0/src/usdm_model/encounter.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_model/estimand.py` & `usdm-0.23.0/src/usdm_model/estimand.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_model/scheduled_instance.py` & `usdm-0.23.0/src/usdm_model/scheduled_instance.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_model/study.py` & `usdm-0.23.0/src/usdm_model/study.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_model/study_design.py` & `usdm-0.23.0/src/usdm_model/study_design.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/src/usdm_model/study_identifier.py` & `usdm-0.23.0/src/usdm_model/study_identifier.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/tests/test_base_sheet.py` & `usdm-0.23.0/tests/test_base_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/tests/test_cdisc_biomedical_concept.py` & `usdm-0.23.0/tests/test_cdisc_biomedical_concept.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/tests/test_error.py` & `usdm-0.23.0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/tests/test_errors.py` & `usdm-0.23.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `usdm-0.22.0/tests/test_iso_3166.py` & `usdm-0.23.0/tests/test_iso_3166.py`

 * *Files identical despite different names*

