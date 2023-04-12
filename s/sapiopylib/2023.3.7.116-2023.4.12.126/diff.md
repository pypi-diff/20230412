# Comparing `tmp/sapiopylib-2023.3.7.116.tar.gz` & `tmp/sapiopylib-2023.4.12.126.tar.gz`

## Comparing `sapiopylib-2023.3.7.116.tar` & `sapiopylib-2023.4.12.126.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/INSTALL.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/sapio_input_config.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/sapio_input_data.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/sapio_native_tools.py
--rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/AccessionService.py
--rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/CustomReportService.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/DashboardManager.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/DataMgmtService.py
--rw-r--r--   0        0        0    39200 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/DataRecordManagerService.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/DataTypeService.py
--rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/ELNService.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/PicklistService.py
--rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/User.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/WebhookService.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/__init__.py
--rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/CustomReport.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/DataRecord.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/DataRecordPaging.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/Picklist.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/SapioAccessType.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/Sort.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/TableColumn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/__init__.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/chartdata/ChartData.py
--rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
--rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/chartdata/__init__.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/DataType.py
--rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
--rw-r--r--   0        0        0    54969 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/__init__.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
--rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
--rw-r--r--   0        0        0    21404 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/eln/__init__.py
--rw-r--r--   0        0        0    13295 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
--rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
--rw-r--r--   0        0        0     8702 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/__init__.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/DataRecordUtil.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/DataTypeCacheManager.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/FormBuilder.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/FoundationAccessioning.py
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/MultiMap.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/ProtocolUtils.py
--rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/Protocols.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/SapioDateUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/__init__.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/plates/PlatingUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/plates/__init__.py
--rw-r--r--   0        0        0    25307 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
--rw-r--r--   0        0        0    45021 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
--rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/tests/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/LICENSE
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/README.md
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/pyproject.toml
--rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 sapiopylib-2023.3.7.116/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/INSTALL.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/sapio_input_config.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/sapio_input_data.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/sapio_native_tools.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/AccessionService.py
+-rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/CustomReportService.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/DashboardManager.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/DataMgmtService.py
+-rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/DataRecordManagerService.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/DataTypeService.py
+-rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/ELNService.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/PicklistService.py
+-rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/User.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/WebhookService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/__init__.py
+-rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/CustomReport.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/DataRecord.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/DataRecordPaging.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/DateRange.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/Picklist.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/SapioAccessType.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/Sort.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/TableColumn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/__init__.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/chartdata/ChartData.py
+-rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
+-rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/chartdata/__init__.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/DataType.py
+-rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
+-rw-r--r--   0        0        0    54969 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/__init__.py
+-rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
+-rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
+-rw-r--r--   0        0        0    21404 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/eln/__init__.py
+-rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
+-rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
+-rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
+-rw-r--r--   0        0        0     8702 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/__init__.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/DataRecordUtil.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/DataTypeCacheManager.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/FormBuilder.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/FoundationAccessioning.py
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/MultiMap.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/ProtocolUtils.py
+-rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/Protocols.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/SapioDateUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/__init__.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/plates/PlatingUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/plates/__init__.py
+-rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
+-rw-r--r--   0        0        0    45312 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
+-rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/tests/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/LICENSE
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/README.md
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/pyproject.toml
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 sapiopylib-2023.4.12.126/PKG-INFO
```

### Comparing `sapiopylib-2023.3.7.116/INSTALL.md` & `sapiopylib-2023.4.12.126/INSTALL.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/sapio_input_data.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/sapio_input_data.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/sapio_native_tools.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/sapio_native_tools.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/AccessionService.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/AccessionService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/CustomReportService.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/CustomReportService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/DashboardManager.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/DashboardManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/DataMgmtService.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/DataMgmtService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/DataRecordManagerService.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/DataRecordManagerService.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Union, Any, List, Dict, IO, Callable, Optional
 from weakref import WeakValueDictionary
 
 from pandas import DataFrame
 from sapiopylib.rest.pojo.DataRecordPaging import DataRecordPojoPageCriteria, DataRecordPojoListPageResult, \
     DataRecordPojoHierarchyPageCriteria, DataRecordPojoHierarchyListPageResult
 
-from sapiopylib.rest.User import SapioUser
+from sapiopylib.rest.User import SapioUser, SapioServerException
 from sapiopylib.rest.pojo.DataRecord import from_json_record_list, to_record_json_list, DataRecord
 from sapiopylib.rest.pojo.DataRecordSideLinkPaging import DataRecordSideLinkFromPageCriteria, \
     DataRecordSideLinkFromListPageResult, DataRecordSideLinkToPageCriteria, DataRecordSideLinkToListPageResult
 from sapiopylib.rest.pojo.SapioAccessType import SapioAccessType
 
 
 class DataRecordManager:
@@ -180,23 +180,42 @@
         :param record_id_list: The list of record IDs to retrieve parents for.
         :param child_type_name: The child data type name of records in the record_id_list.
         This is only required in high-performance high-volume data retrieval.
         :param parent_type_name: The parent data type name to get for each child.
         :param paging_criteria: Optionally specify the page to retrieve for. Note the page size may be enforced in SaaS.
         :return: The current page's result.
         """
-        record_id_list.sort()
-        params = {'childTypeName': child_type_name,
-                  'parentTypeName': parent_type_name}
-        self._append_query_param(paging_criteria, params)
-        sub_path = '/datarecordlist/parents'
-        response = self.user.post(sub_path, params=params, payload=record_id_list)
-        self.user.raise_for_status(response)
-        json_dict = response.json()
-        return DataRecordPojoHierarchyListPageResult.from_json(json_dict)
+        try:
+            record_id_list.sort()
+            params = {'childTypeName': child_type_name,
+                      'parentTypeName': parent_type_name}
+            self._append_query_param(paging_criteria, params)
+            sub_path = '/datarecordlist/parents'
+            response = self.user.post(sub_path, params=params, payload=record_id_list)
+            self.user.raise_for_status(response)
+            json_dict = response.json()
+            return DataRecordPojoHierarchyListPageResult.from_json(json_dict)
+        except SapioServerException as e:
+            if e.client_error.response.status_code == 405:
+                # Method not found. Use the deprecated version to re-request
+                self.user.log_warn("""
+SAPIO PLATFORM VERSION MISMATCH. USING DEPRECATED WEBSERVICE CALL FORMAT.
+This is unsupported. Use at your own risk!
+                """)
+                params = {'recordIdList': ','.join(str(x) for x in record_id_list),
+                          'childTypeName': child_type_name,
+                          'parentTypeName': parent_type_name}
+                self._append_query_param(paging_criteria, params)
+                sub_path = '/datarecordlist/parents'
+                response = self.user.get(sub_path, params)
+                response.raise_for_status()
+                json_dict = response.json()
+                return DataRecordPojoHierarchyListPageResult.from_json(json_dict)
+            else:
+                raise e
 
     def get_children(self, record_id: int, child_type_name: str,
                      paging_criteria: Optional[DataRecordPojoPageCriteria] = None) -> DataRecordPojoListPageResult:
         """
         Get the children of the given type below the record with the given Record ID.
         :param record_id: The Record ID of the parent record.
         :param child_type_name: The data type name of the children to look for below the given Record ID.
@@ -217,22 +236,40 @@
             DataRecordPojoHierarchyListPageResult:
         """
         Get the children of the given type below the records with the given Record IDs.
         :param record_id_list: Parent Record IDs to get children of.
         :param child_type_name: The data type name of the children to look for below the given Record IDs.
         :param paging_criteria: Optionally specify the page to retrieve for. Note the page size may be enforced in SaaS.
         """
-        record_id_list.sort()
-        params = {'childTypeName': child_type_name}
-        self._append_query_param(paging_criteria, params)
-        sub_path = '/datarecordlist/childrenbyid'
-        response = self.user.post(sub_path, params=params, payload=record_id_list)
-        self.user.raise_for_status(response)
-        json_dict = response.json()
-        return DataRecordPojoHierarchyListPageResult.from_json(json_dict)
+        try:
+            record_id_list.sort()
+            params = {'childTypeName': child_type_name}
+            self._append_query_param(paging_criteria, params)
+            sub_path = '/datarecordlist/childrenbyid'
+            response = self.user.post(sub_path, params=params, payload=record_id_list)
+            self.user.raise_for_status(response)
+            json_dict = response.json()
+            return DataRecordPojoHierarchyListPageResult.from_json(json_dict)
+        except SapioServerException as e:
+            if e.client_error.response.status_code == 405:
+                # Method not found. Use the deprecated version to re-request
+                self.user.log_warn("""
+SAPIO PLATFORM VERSION MISMATCH. USING DEPRECATED WEBSERVICE CALL FORMAT.
+This is unsupported. Use at your own risk!
+                """)
+                params = {'recordIdList': ','.join(str(x) for x in record_id_list),
+                          'childTypeName': child_type_name}
+                self._append_query_param(paging_criteria, params)
+                sub_path = '/datarecordlist/children'
+                response = self.user.get(sub_path, params)
+                response.raise_for_status()
+                json_dict = response.json()
+                return DataRecordPojoHierarchyListPageResult.from_json(json_dict)
+            else:
+                raise e
 
     def get_ancestors(self, record_id: int, descendant_type_name: str, ancestor_type_name: str,
                       paging_criteria: Optional[DataRecordPojoPageCriteria] = None) -> DataRecordPojoListPageResult:
         """
         Get the ancestors of the given type above the records with the given Record ID.
         :param record_id: The Record ID of the descendant record.
         :param descendant_type_name: The data type name of descendants ancestors to look for above the given Record ID.
```

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/DataTypeService.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/DataTypeService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/ELNService.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/ELNService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/PicklistService.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/PicklistService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/User.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/User.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/WebhookService.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/WebhookService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/CustomReport.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/CustomReport.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/DataRecord.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/DataRecord.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/DataRecordPaging.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/DataRecordPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/Picklist.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/Picklist.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/Sort.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/Sort.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/TableColumn.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/TableColumn.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/chartdata/ChartData.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/chartdata/ChartData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/DataType.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/DataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/eln/ElnExperiment.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/eln/ElnExperiment.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 class AbstractReportEntryDataContext(ABC):
     entry_type: RbEntryType
 
     @abstractmethod
     def get_entry_type(self) -> RbEntryType:
         pass
 
+    def to_json_supply_entry_type(self, entry_type: RbEntryType) -> Dict[str, Any]:
+        return {
+            '@type': entry_type.class_name,
+            'entryType': entry_type.name
+        }
+
     def to_json(self) -> Dict[str, Any]:
         return {
             '@type': self.entry_type.class_name,
             'entryType': self.entry_type.name
         }
 
 
@@ -83,14 +89,22 @@
 
     def get_data_type_name(self) -> str:
         return self._data_type_name
 
     def get_data_field_name(self) -> str:
         return self._data_field_name
 
+    def to_json_supply_entry_type(self, entry_type: RbEntryType) -> Dict[str, Any]:
+        ret: Dict[str, Any] = super().to_json_supply_entry_type(entry_type)
+        ret['dataTypeName'] = self._data_type_name
+        ret['dataFieldName'] = self._data_field_name
+        ret['dataRecordId'] = self.data_record_id
+        ret['staticTimestamp'] = self.static_timestamp
+        return ret
+
     def to_json(self) -> Dict[str, Any]:
         ret: Dict[str, Any] = super().to_json()
         ret['dataTypeName'] = self._data_type_name
         ret['dataFieldName'] = self._data_field_name
         ret['dataRecordId'] = self.data_record_id
         ret['staticTimestamp'] = self.static_timestamp
         return ret
@@ -224,14 +238,22 @@
         self._data_field_name = _data_field_name
         self.data_record_id = data_record_id
         self.static_html = static_html
 
     def get_entry_type(self) -> RbEntryType:
         return RbEntryType.STATIC_TEXT
 
+    def to_json_supply_entry_type(self, entry_type: RbEntryType) -> Dict[str, Any]:
+        ret: Dict[str, Any] = super().to_json_supply_entry_type(entry_type)
+        ret['dataTypeName'] = self._data_type_name
+        ret['dataFieldName'] = self._data_field_name
+        ret['dataRecordId'] = self.data_record_id
+        ret['staticHtml'] = self.static_html
+        return ret
+
     def to_json(self) -> Dict[str, Any]:
         ret: Dict[str, Any] = super().to_json()
         ret['dataTypeName'] = self._data_type_name
         ret['dataFieldName'] = self._data_field_name
         ret['dataRecordId'] = self.data_record_id
         ret['staticHtml'] = self.static_html
         return ret
@@ -317,8 +339,7 @@
             data_record_id: Optional[int] = json_dct.get('dataRecordId')
             static_html: Optional[str] = json_dct.get('staticHtml')
             return StaticTextEntryDataContext(_data_type_name, _data_field_name, data_record_id, static_html)
         elif entry_type == RbEntryType.TABLE_VIEW:
             _data_type_name: str = json_dct.get('dataTypeName')
             record_id_list: Optional[List[int]] = json_dct.get('recordIds')
             return TableEntryDataContext(_data_type_name, record_id_list)
-
```

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,18 +109,18 @@
         self.entry_type = entry_type
         self.entry_data_context = entry_data_context
 
     def to_json(self) -> Dict[str, Any]:
         ret: Dict[str, Any] = dict()
         ret['entryId'] = self._entry_id
         ret['entryName'] = self.entry_name
-        if self.entry_type is not None:
-            ret['entryType'] = self.entry_type.name
-        if self.entry_data_context is not None:
-            ret['entryDataContextPojo'] = self.entry_data_context.entry_type
+        ret['entryType'] = self.entry_type.name
+        entry_data_context: Dict[str, Any] = self.entry_data_context.to_json_supply_entry_type(self.entry_type)
+        for key in entry_data_context.keys():
+            ret[key] = entry_data_context[key]
         return ret
 
 
 class ReportDataContext:
     """
     Context object used to provide details about the data that should be added to a Report Template when
     generating a PDF.
@@ -230,8 +230,7 @@
         report_entry_pojo_list: List[Dict[str, Any]] = json_dct.get('reportEntryInfoPojos')
         report_entry_info_list: List[ReportEntryInfo] = [VeloxReportBuilderParser.parse_report_entry_info(x)
                                                          for x in report_entry_pojo_list]
         report_data_context: ReportDataContext = VeloxReportBuilderParser.parse_report_data_context(
             json_dct.get('reportDataContextPojo'))
         return RbTemplatePopulatorData(template_info, report_entry_info_list, report_data_context)
 
-
```

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     Request the user to upload multiple files. User will be asked fo upload one or more files.
     """
     dialog_title: str
     show_image_editor: bool
     file_extension: Optional[str]
     show_camera_button: bool
 
-    def __init__(self, dialog_title: str, show_image_editor: bool, file_extension: Optional[str],
-                 show_camera_button: bool):
+    def __init__(self, dialog_title: str, show_image_editor: bool = False, file_extension: Optional[str] = None,
+                 show_camera_button: bool = False):
         """
         Request the user to upload multiple files.
         :param dialog_title: The title of the file prompt
         :param show_image_editor: Whether the user will see an image editor when image is uploaded in this file prompt.
         :param show_camera_button: Whether the user will be able to use camera to take a picture as an upload request,
         rather than selecting an existing file.
         :param file_extension: The acceptable file extensions for the file prompt. Comma separated.
@@ -270,14 +270,16 @@
         ret['fieldMapList'] = self.field_map_list
         return ret
 
 
 class WriteFileRequest(AbstractClientCallbackRequest):
     """
     Write a short amount of file data onto the client. The user will download this file from browser.
+
+    The return object from server is of type WriteFileResult, which you can use to check if user has cancelled.
     Note: file data will be stored in RAM in this operation.
 
     file_bytes: The file data to write.
     file_path: The filename of the written file.
     """
     file_bytes: bytes
     file_path: str
@@ -288,9 +290,67 @@
 
     def get_callback_type(self) -> CallbackType:
         return CallbackType.WRITE_FILE
 
     def to_json(self) -> Dict[str, Any]:
         ret: Dict[str, Any] = super().to_json()
         ret['filePath'] = self.file_path
-        ret['fileBytes'] = base64.b64encode(self.file_bytes)
+        encoded_data: bytes = base64.b64encode(self.file_bytes)
+        ret['fileBytes'] = encoded_data.decode("utf-8")
+        return ret
+
+
+class MultiFileRequest(AbstractClientCallbackRequest):
+    """
+    Write multiple files to the user browser all at once. To fill the request, you can use it like a dictionary.
+
+    The return object from server is of type WriteFileResult, which you can use to check if user has cancelled.
+    """
+
+    json_built: Dict[str, str]
+
+    def __init__(self, initial_data: Dict[str, bytes] = None):
+        self.json_built = dict()
+        if initial_data is not None:
+            for key, value in initial_data.items():
+                self.put(key, value)
+
+    def __setitem__(self, key: str, value: bytes):
+        self.put(key, value)
+
+    def __getitem__(self, key: str):
+        return self.json_built.get(key)
+
+    def __iter__(self):
+        return self.json_built.__iter__()
+
+    def __hash__(self):
+        return hash(self.json_built)
+
+    def __eq__(self, other):
+        if not isinstance(other, MultiFileRequest):
+            return False
+        return self.json_built == other.json_built
+
+    def __len__(self):
+        return len(self.json_built)
+
+    def put(self, file_name: str, file_data: bytes) -> None:
+        """
+        Add a file to upload into this request.
+        :param file_name: The file name to upload
+        :param file_data: The file data to upload.
+        """
+        if not file_name or not file_data:
+            return
+        encoded_data: bytes = base64.b64encode(file_data)
+        if not encoded_data:
+            return
+        self.json_built[file_name] = encoded_data.decode("utf-8")
+
+    def get_callback_type(self) -> CallbackType:
+        return CallbackType.WRITE_FILE
+
+    def to_json(self) -> Dict[str, Any]:
+        ret: Dict[str, Any] = super().to_json()
+        ret['files'] = self.json_built
         return ret
```

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,18 +172,26 @@
         user_cancelled: bool = json_dct.get('userCancelled')
         callback_type = CallbackType[json_dct.get('callbackType')]
         if callback_type == CallbackType.DATA_RECORD_SELECTION:
             selected_field_map_list: Optional[List[Dict[str, Any]]] = \
                 json_dct.get('selectedFieldMapList')
             return DataRecordSelectionResult(user_cancelled, selected_field_map_list=selected_field_map_list)
         elif callback_type == CallbackType.MULTI_FILE_PROMPT:
-            files: Optional[Dict[str, bytes]] = json_dct.get('files')
+            encoded: Optional[Dict[str, str]] = json_dct.get('files')
+            files: Optional[Dict[str, bytes]] = dict()
+            if encoded:
+                for key, value in encoded.items():
+                    if key and value:
+                        decoded_value: bytes = base64.b64decode(value.encode('utf-8'))
+                        files[key] = decoded_value
             return MultiFilePromptResult(user_cancelled, files)
         elif callback_type == CallbackType.FILE_PROMPT:
-            file_bytes: Optional[bytes] = base64.b64decode(json_dct.get('fileBytes'))
+            file_bytes: Optional[bytes] = None
+            if json_dct.get('fileBytes'):
+                file_bytes = base64.b64decode(json_dct.get('fileBytes'))
             file_path: Optional[str] = json_dct.get('filePath')
             return FilePromptResult(user_cancelled, file_bytes=file_bytes, file_path=file_path)
         elif callback_type == CallbackType.FORM_ENTRY_DIALOG:
             user_response_map: Optional[Dict[str, Any]] = json_dct.get('userResponseMap')
             return FormEntryDialogResult(user_cancelled, user_response_map=user_response_map)
         elif callback_type == CallbackType.LIST_DIALOG:
             selected_options_list: Optional[List[str]] = json_dct.get('selectedOptionList')
```

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/VeloxRules.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/VeloxRules.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/WebhookContext.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/WebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/pojo/webhook/WebhookResult.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/pojo/webhook/WebhookResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/DataRecordUtil.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/DataRecordUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/DataTypeCacheManager.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/DataTypeCacheManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/FormBuilder.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/FormBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/FoundationAccessioning.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/FoundationAccessioning.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/MultiMap.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/MultiMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/ProtocolUtils.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/ProtocolUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/Protocols.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/Protocols.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/SapioDateUtils.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/SapioDateUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/plates/PlatingUtils.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/plates/PlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,21 +94,17 @@
             self._model, field_name, old_value, field_value))
         # Handle for side links.
         dt_cache_man: DataTypeCacheManager = self._model.record_model_manager.data_type_cache_manager
         if dt_cache_man.is_side_link_field(self._model.data_type_name, field_name):
             if field_value is None:
                 self._model.record_model_manager.event_bus.fire_side_link_changed_event(self, field_name, None)
             else:
-                target_model: Optional[PyRecordModel] = self._model.record_model_manager.instance_manager. \
-                    get_known_record_with_record_id(int(field_value))
-                if target_model is None:
-                    raise SapioRecordModelException("Side Link Target Record Model with Record ID " +
-                                                    str(field_value) + " was not loaded.", self._model)
+                target_record_id: int = int(field_value)
                 self._model.record_model_manager.event_bus.fire_side_link_changed_event(self._model,
-                                                                                        field_name, target_model)
+                                                                                        field_name, target_record_id)
 
     def __delitem__(self, field_name: str):
         if field_name not in self._model_fields:
             return
         old_value = self._model_fields.get(field_name)
         del self._model_fields[field_name]
         from sapiopylib.rest.utils.recordmodel.RecordModelEvents import FieldChangeEvent
@@ -150,15 +146,15 @@
     _model_fields: RecordModelFieldMap
     __is_deleted: bool
 
     _children_types_loaded: Set[str]
     _parent_types_loaded: Set[str]
     _children_models_by_type: SetMultimap[str, PyRecordModel]
     _parent_models_by_type: SetMultimap[str, PyRecordModel]
-    _forward_side_link_cache: Dict[str, Optional[PyRecordModel]]
+    _forward_side_link_cache: Dict[str, Optional[int]]
     _loaded_forward_side_link_field_names: Set[str]
     _reverse_side_link_cache: SetMultimap[RecordModelReverseSideLinkCacheKey, PyRecordModel]
     _loaded_reverse_side_links: Set[RecordModelReverseSideLinkCacheKey]
 
     _non_loaded_removed_parents: Set[PyRecordModel]
     _non_loaded_removed_children: Set[PyRecordModel]
     _non_loaded_removed_forward_links: Set[str]
@@ -303,26 +299,26 @@
         """
         self._parent_types_loaded.add(parent_type_name)
         for parent in parents_loaded:
             if parent in self._non_loaded_removed_parents:
                 continue
             self._parent_models_by_type.put(parent_type_name, parent)
 
-    def _mark_forward_side_link_loaded(self, field_name: str, target_model: Optional[PyRecordModel]):
+    def _mark_forward_side_link_loaded(self, field_name: str, target_record_id: Optional[int]):
         """
         Load a forward link for a particular field name and mark the field as loaded for this record.
         """
         # Mark as loaded
         self._loaded_forward_side_link_field_names.add(field_name)
         # Update cache data
-        if target_model is not None and target_model in self._non_loaded_removed_forward_links:
+        if target_record_id is not None and field_name in self._non_loaded_removed_forward_links:
             self._forward_side_link_cache[field_name] = None
             self._non_loaded_removed_forward_links.remove(field_name)
         else:
-            self._forward_side_link_cache[field_name] = target_model
+            self._forward_side_link_cache[field_name] = target_record_id
 
     def _mark_reverse_side_link_loaded(self, back_side_link_dt_name: str,
                                        back_side_link_field_name: str, loaded_side_links: List[PyRecordModel]):
         """
         Load a reverse link for a particular data type and field name and mark this key as loaded.
         """
         # Mark as loaded
@@ -428,15 +424,15 @@
     def set_side_link(self, field_name: str, link_to: Optional[PyRecordModel]) -> None:
         """
         Change the forward side link on this record's field to another record.
         """
         if link_to is None:
             self.set_field_value(field_name, None)
         elif link_to.is_new:
-            self.record_model_manager.event_bus.fire_side_link_changed_event(self, field_name, link_to)
+            self.record_model_manager.event_bus.fire_side_link_changed_event(self, field_name, link_to.record_id)
         else:
             self.set_field_value(field_name, link_to.record_id)
 
     def delete(self) -> None:
         """
         Flag the current record model to be deleted on commit.
         """
@@ -508,45 +504,55 @@
     def get_forward_side_link(self, field_name: str) -> Optional[PyRecordModel]:
         """
         Get the current forward side links. If the side links have not been loaded, throw an exception.
         :param field_name: The forward link field on this record to load its reference for.
         """
         if not self.is_forward_side_link_loaded(field_name):
             raise SapioRecordModelException("Forward link on field " + field_name + " was not loaded.", self)
-        return self._forward_side_link_cache.get(field_name)
+        target_record_id: Optional[int] = self._forward_side_link_cache.get(field_name)
+        if target_record_id is None:
+            return None
+        ret: Optional[PyRecordModel] = self._record_model_manager.instance_manager.\
+            get_known_record_with_record_id(target_record_id)
+        if ret is None:
+            raise SapioRecordModelException("Forward link on field " + field_name + " was not loaded.", self)
+        return ret
 
     def get_reverse_side_link(self, reverse_side_link_data_type_name: str, reverse_side_link_field_name: str) \
             -> List[PyRecordModel]:
         """
         Get currently loaded reverse side link models. This will throw exception if it has not been loaded before.
         """
         cache_key = RecordModelReverseSideLinkCacheKey(link_data_type_name=reverse_side_link_data_type_name,
                                                        link_data_field_name=reverse_side_link_field_name)
         if not self.is_reverse_side_link_loaded_key(cache_key):
             raise SapioRecordModelException("Reverse link on field " + reverse_side_link_data_type_name +
                                             "." + reverse_side_link_field_name + " was not loaded.", self)
         return list(self._reverse_side_link_cache.get(cache_key))
 
-    def _update_side_link_cache(self, field_name, new_target_model: Optional[PyRecordModel]) -> None:
+    def _update_side_link_cache(self, field_name, target_record_id: Optional[int]) -> None:
         """
         Update the side link cache so that both sides are consistent. This should only be called from forward direction.
         :param field_name: The field name of which the side link cache has been modified on this record.
-        :param new_target_model: The new target record linked on the field.
+        :param target_record_id: The new target record ID linked on the field.
         """
         cache_key = RecordModelReverseSideLinkCacheKey(self.data_type_name, field_name)
         old_side_link: Optional[PyRecordModel] = self.get_forward_side_link(field_name)
         # Update forward links
-        self._mark_forward_side_link_loaded(field_name, new_target_model)
+        self._mark_forward_side_link_loaded(field_name, target_record_id)
         # Update reverse links
         if old_side_link is not None:
             old_side_link._reverse_side_link_cache.pop(cache_key, None)
             if not old_side_link.is_reverse_side_link_loaded_key(cache_key):
                 old_side_link._non_loaded_removed_reverse_links.put(cache_key, self)
-        if new_target_model is not None:
-            new_target_model._reverse_side_link_cache.put(cache_key, self)
+        if target_record_id:
+            new_target_model: Optional[PyRecordModel] = self.\
+                _record_model_manager.instance_manager.get_known_record_with_record_id(target_record_id)
+            if new_target_model is not None:
+                new_target_model._reverse_side_link_cache.put(cache_key, self)
 
     def do_rollback(self):
         """
         This method is called by instance manager for referencable record models when a rollback event is fired.
         This is an internal method.
         """
         self.__is_deleted = False
```

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Optional
-
 from buslane.events import EventBus, EventHandler
 
 from sapiopylib.rest.utils.recordmodel.RecordModelEvents import *
 
 
 class RecordModelEventBus:
     """
@@ -95,13 +93,13 @@
     def subscribe_record_delete_event(self, handler: EventHandler[RecordDeletedEvent]):
         """
         Subscribes an event handler to listen to deletion of existing records that are fired from this event bus.
         """
         self._publisher.register(handler)
 
     def fire_side_link_changed_event(self, source_model: PyRecordModel, field_name: str,
-                                     target_model: Optional[PyRecordModel]):
+                                     target_record_id: Optional[int]):
         self._publisher.publish(SideLinkChangedEvent(source_model=source_model,
-                                                     link_field_name=field_name, target_model=target_model))
+                                                     link_field_name=field_name, target_record_id=target_record_id))
 
     def subscribe_side_link_changed_event(self, handler: EventHandler[SideLinkChangedEvent]):
         self._publisher.register(handler)
```

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py`

 * *Files 10% similar despite different names*

```diff
@@ -119,25 +119,25 @@
 
 class SideLinkChangedEvent(Event):
     """
     This event is fired when a side link has been modified.
     """
     __source_model: PyRecordModel
     __link_field_name: str
-    __target_model: Optional[PyRecordModel]
+    __target_record_id: Optional[int]
 
-    def __init__(self, source_model: PyRecordModel, link_field_name: str, target_model: Optional[PyRecordModel]):
+    def __init__(self, source_model: PyRecordModel, link_field_name: str, target_record_id: Optional[int]):
         self.__source_model = source_model
         self.__link_field_name = link_field_name
-        self.__target_model = target_model
+        self.__target_record_id = target_record_id
 
     @property
     def source_model(self) -> PyRecordModel:
         return self.__source_model
 
     @property
     def link_field_name(self) -> str:
         return self.__link_field_name
 
     @property
-    def target_model(self) -> Optional[PyRecordModel]:
-        return self.__target_model
+    def target_record_id(self) -> Optional[int]:
+        return self.__target_record_id
```

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,15 +450,15 @@
             for desc, links in result_map.items():
                 source_model: PyRecordModel = inst_man.get_known_record_with_record_id(desc.record_id)
                 if links:
                     link_rec: DataRecord = links[0]
                     # noinspection PyProtectedMember
                     link = inst_man._get_or_add_record(link_rec)
                     # noinspection PyProtectedMember
-                    source_model._mark_forward_side_link_loaded(field_name, link)
+                    source_model._mark_forward_side_link_loaded(field_name, link.record_id)
                 else:
                     # noinspection PyProtectedMember
                     source_model._mark_forward_side_link_loaded(field_name, None)
 
     def load_reverse_side_links_of_type(self, records: List[WrappedRecordModel],
                                         reverse_link_type: Type[WrappedRecordModel],
                                         reverse_link_field_name: str) -> None:
@@ -652,17 +652,17 @@
 
     def __init__(self, rel_man: RecordModelRelationshipManager):
         self._rel_man = rel_man
 
     def handle(self, event: SideLinkChangedEvent) -> None:
         source_model: PyRecordModel = event.source_model
         field_name: str = event.link_field_name
-        target_model: Optional[PyRecordModel] = event.target_model
+        target_record_id: Optional[int] = event.target_record_id
         # noinspection PyProtectedMember
-        source_model._update_side_link_cache(field_name, target_model)
+        source_model._update_side_link_cache(field_name, target_record_id)
 
 
 class RecordModelTransactionManager:
     """
     Holds the transaction properties for batch calls to Sapio server.
     """
     _record_model_manager: RecordModelManager
@@ -886,16 +886,20 @@
             return
         if (parent_record, child_record) in self._children_added:
             self._children_added.discard((parent_record, child_record))
         else:
             self._children_removed.add((parent_record, child_record))
 
     def _on_side_link_changed(self, source_model: PyRecordModel,
-                              side_link_field_name: str, target_model: PyRecordModel):
-        if target_model.record_id > 0:
+                              side_link_field_name: str, target_record_id: Optional[int]):
+        if target_record_id is None or target_record_id > 0:
+            return
+        target_model: Optional[PyRecordModel] = self._record_model_manager.instance_manager\
+            .get_known_record_with_record_id(target_record_id)
+        if target_model is None:
             return
         if source_model not in self._side_links_to_set:
             self._side_links_to_set[source_model] = dict()
         self._side_links_to_set[source_model][side_link_field_name] = target_model
 
 
 class _TransactionChildAddedHandler(EventHandler[ChildAddedEvent]):
@@ -926,14 +930,15 @@
     def __init__(self, trans_man: RecordModelTransactionManager):
         self._trans_man = trans_man
 
     def handle(self, event: FieldChangeEvent) -> None:
         record = event.record
         field_name = event.field_name
         new_value = event.new_value
+        # noinspection PyProtectedMember
         self._trans_man._add_field_change(record, field_name, new_value)
 
 
 class _TransactionDeletedHandler(EventHandler[RecordDeletedEvent]):
     _trans_man: RecordModelTransactionManager
 
     def __init__(self, trans_man: RecordModelTransactionManager):
@@ -959,8 +964,8 @@
     _trans_man: RecordModelTransactionManager
 
     def __init__(self, trans_man: RecordModelTransactionManager):
         self._trans_man = trans_man
 
     def handle(self, event: SideLinkChangedEvent) -> None:
         # noinspection PyProtectedMember
-        self._trans_man._on_side_link_changed(event.source_model, event.link_field_name, event.target_model)
+        self._trans_man._on_side_link_changed(event.source_model, event.link_field_name, event.target_record_id)
```

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         This method will throw exception when the values are not unique.
         """
         ret: Dict[Any, PyRecordModel] = dict()
         for model in models:
             value = model.get_field_value(field_name)
             if value in ret and model != ret.get(value):
                 raise SapioRecordModelException("Duplicated value " +
-                                                str(value) + " found when processing key " + str(model))
+                                                str(value) + " found when processing key " + str(model), model)
             ret[value] = model
         return ret
 
     @staticmethod
     def multi_map_model_by_field_value(models: Iterable[PyRecordModel], field_name: str) -> \
             ListMultimap[Any, PyRecordModel]:
         """
```

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     _field_type: FieldType
 
     @property
     def field_name(self) -> str:
         """
         The name of the data field represented in this object of the Sapio data type.
         """
-        return self.field_name
+        return self._field_name
 
     @property
     def field_type(self) -> FieldType:
         """
         The data field's type for the data type's data field with the object's field name in Sapio.
         """
         return self._field_type
```

### Comparing `sapiopylib-2023.3.7.116/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py` & `sapiopylib-2023.4.12.126/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/LICENSE` & `sapiopylib-2023.4.12.126/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/README.md` & `sapiopylib-2023.4.12.126/README.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.3.7.116/pyproject.toml` & `sapiopylib-2023.4.12.126/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopylib"
-version='2023.03.07.116'
+version='2023.04.12.126'
 authors = [
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Informatics Platform Python API"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -20,15 +20,15 @@
     "Intended Audience :: Science/Research",
     "Intended Audience :: Healthcare Industry",
     "Programming Language :: Python :: 3.7",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Software Development :: Libraries :: Python Modules",
-    'Development Status :: 4 - Beta',
+    'Development Status :: 5 - Production/Stable',
 ]
 homepage = "https://www.sapiosciences.com/"
 keywords = ["lims", "eln", "rest", "sapio"]
 
 [project.urls]
 "Homepage" = "https://github.com/sapiosciences"
 "Bug Tracker" = "https://github.com/sapiosciences/sapio-py-tutorials/issues"
```

### Comparing `sapiopylib-2023.3.7.116/PKG-INFO` & `sapiopylib-2023.4.12.126/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sapiopylib
-Version: 2023.3.7.116
+Version: 2023.4.12.126
 Summary: Official Sapio Informatics Platform Python API
 Project-URL: Homepage, https://github.com/sapiosciences
 Project-URL: Bug Tracker, https://github.com/sapiosciences/sapio-py-tutorials/issues
 Author-email: Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

