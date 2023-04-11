# Comparing `tmp/polyglot_piranha-0.3.1.tar.gz` & `tmp/polyglot_piranha-0.3.2.tar.gz`

## Comparing `polyglot_piranha-0.3.1.tar` & `polyglot_piranha-0.3.2.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.1/Cargo.toml
--rw-r--r--   0     1001      123    35210 2023-04-06 19:48:46.000000 polyglot_piranha-0.3.1/Cargo.lock
--rw-r--r--   0     1001      123    11359 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/LICENSE
--rw-r--r--   0     1001      123     3091 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/README.md
--rw-r--r--   0     1001      123     1373 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java
--rw-r--r--   0     1001      123      994 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java
--rw-r--r--   0     1001      123     5517 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java
--rw-r--r--   0     1001      123     5621 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java
--rw-r--r--   0     1001      123    66915 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java
--rw-r--r--   0     1001      123    21518 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java
--rw-r--r--   0     1001      123     5106 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java
--rw-r--r--   0     1001      123      377 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaConfigurationException.java
--rw-r--r--   0     1001      123     3615 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java
--rw-r--r--   0     1001      123     5039 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java
--rw-r--r--   0     1001      123     2584 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java
--rw-r--r--   0     1001      123     2605 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java
--rw-r--r--   0     1001      123      550 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java
--rw-r--r--   0     1001      123     2456 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java
--rw-r--r--   0     1001      123    13106 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java
--rw-r--r--   0     1001      123     5875 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java
--rw-r--r--   0     1001      123    85120 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java
--rw-r--r--   0     1001      123    55188 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java
--rw-r--r--   0     1001      123    48474 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java
--rw-r--r--   0     1001      123     2304 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java
--rw-r--r--   0     1001      123    33367 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java
--rw-r--r--   0     1001      123     6780 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java
--rw-r--r--   0     1001      123     3480 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java
--rw-r--r--   0     1001      123     8540 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java
--rw-r--r--   0     1001      123     4153 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java
--rw-r--r--   0     1001      123     4326 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java
--rw-r--r--   0     1001      123     2555 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java
--rw-r--r--   0     1001      123     1490 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java
--rw-r--r--   0     1001      123     2091 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java
--rw-r--r--   0     1001      123     2194 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java
--rw-r--r--   0     1001      123     1550 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java
--rw-r--r--   0     1001      123     1618 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java
--rw-r--r--   0     1001      123     1573 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java
--rw-r--r--   0     1001      123       75 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParam.java
--rw-r--r--   0     1001      123      109 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParameter.java
--rw-r--r--   0     1001      123      175 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/OverlappingNameInterface.java
--rw-r--r--   0     1001      123      103 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/PVal.java
--rw-r--r--   0     1001      123      154 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/Parameter.java
--rw-r--r--   0     1001      123      155 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeOtherInterface.java
--rw-r--r--   0     1001      123      160 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeParamRev.java
--rw-r--r--   0     1001      123      122 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/StaticMthds.java
--rw-r--r--   0     1001      123      229 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/invalid/piranha.properties
--rw-r--r--   0     1001      123       97 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid.json
--rw-r--r--   0     1001      123      202 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_2.json
--rw-r--r--   0     1001      123      213 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_3.json
--rw-r--r--   0     1001      123      216 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_4.json
--rw-r--r--   0     1001      123      361 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_enum_no_arg.json
--rw-r--r--   0     1001      123      525 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json
--rw-r--r--   0     1001      123      526 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json
--rw-r--r--   0     1001      123      488 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name.json
--rw-r--r--   0     1001      123      489 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name_no_method_chain.json
--rw-r--r--   0     1001      123      526 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json
--rw-r--r--   0     1001      123      704 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_argument.json
--rw-r--r--   0     1001      123     1332 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json
--rw-r--r--   0     1001      123      192 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_noFlag.json
--rw-r--r--   0     1001      123      739 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json
--rw-r--r--   0     1001      123      652 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_receive.json
--rw-r--r--   0     1001      123     1896 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json
--rw-r--r--   0     1001      123      844 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_return.json
--rw-r--r--   0     1001      123     1776 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json
--rw-r--r--   0     1001      123     1932 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json
--rw-r--r--   0     1001      123     4525 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json
--rw-r--r--   0     1001      123      251 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_no_match.json
--rw-r--r--   0     1001      123      246 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_wrong_arg.json
--rw-r--r--   0     1001      123      142 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_without_enum.json
--rw-r--r--   0     1001      123     1637 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json
--rw-r--r--   0     1001      123     1304 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java
--rw-r--r--   0     1001      123     1304 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak
--rw-r--r--   0     1001      123     1107 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect
--rw-r--r--   0     1001      123     2565 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/javascript/src/config_checker.js
--rw-r--r--   0     1001      123     4304 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/javascript/src/piranha.js
--rw-r--r--   0     1001      123    27988 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/javascript/src/refactor.js
--rw-r--r--   0     1001      123     1445 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/javascript/src/source_checker.js
--rw-r--r--   0     1001      123      646 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt
--rw-r--r--   0     1001      123     1064 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/objc/src/XPFlagRefactoring/README.txt
--rw-r--r--   0     1001      123    26229 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp
--rw-r--r--   0     1001      123        0 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.exports
--rw-r--r--   0     1001      123      793 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/pyproject.toml
--rw-r--r--   0     1001      123     2043 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/cleanup_rules/go/edges.toml
--rw-r--r--   0     1001      123    11027 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/cleanup_rules/go/rules.toml
--rw-r--r--   0     1001      123     1460 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/cleanup_rules/go/scope_config.toml
--rwxr-xr-x   0     1001      123     2241 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/cleanup_rules/java/edges.toml
--rwxr-xr-x   0     1001      123    15939 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/cleanup_rules/java/rules.toml
--rwxr-xr-x   0     1001      123     3582 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/cleanup_rules/java/scope_config.toml
--rwxr-xr-x   0     1001      123     2251 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/cleanup_rules/kt/edges.toml
--rwxr-xr-x   0     1001      123    19122 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/cleanup_rules/kt/rules.toml
--rwxr-xr-x   0     1001      123     2139 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/cleanup_rules/kt/scope_config.toml
--rw-r--r--   0     1001      123     1133 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/cleanup_rules/swift/edges.toml
--rw-r--r--   0     1001      123     9296 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/cleanup_rules/swift/rules.toml
--rw-r--r--   0     1001      123     1369 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/cleanup_rules/swift/scope_config.toml
--rw-r--r--   0     1001      123     7317 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/lib.rs
--rw-r--r--   0     1001      123     1679 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/main.rs
--rw-r--r--   0     1001      123     5799 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/constraint.rs
--rw-r--r--   0     1001      123     3143 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/default_configs.rs
--rw-r--r--   0     1001      123     4915 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/edit.rs
--rw-r--r--   0     1001      123     6744 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/language.rs
--rw-r--r--   0     1001      123    11140 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/matches.rs
--rw-r--r--   0     1001      123      928 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/mod.rs
--rw-r--r--   0     1001      123     1987 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/outgoing_edges.rs
--rw-r--r--   0     1001      123    14103 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/piranha_arguments.rs
--rw-r--r--   0     1001      123     2091 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/piranha_output.rs
--rw-r--r--   0     1001      123     7916 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/rule.rs
--rw-r--r--   0     1001      123     6286 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/rule_graph.rs
--rw-r--r--   0     1001      123     5931 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/rule_store.rs
--rw-r--r--   0     1001      123     3329 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/scopes.rs
--rw-r--r--   0     1001      123    14473 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/source_code_unit.rs
--rw-r--r--   0     1001      123     1586 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/unit_tests/piranha_arguments_test.rs
--rw-r--r--   0     1001      123     8340 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/unit_tests/rule_test.rs
--rw-r--r--   0     1001      123     6061 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/unit_tests/scopes_test.rs
--rw-r--r--   0     1001      123     6996 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/models/unit_tests/source_code_unit_test.rs
--rw-r--r--   0     1001      123     8196 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/tests/mod.rs
--rw-r--r--   0     1001      123     1647 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/tests/test_piranha_go.rs
--rw-r--r--   0     1001      123    12255 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/tests/test_piranha_java.rs
--rw-r--r--   0     1001      123     1862 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/tests/test_piranha_kt.rs
--rw-r--r--   0     1001      123     2423 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/tests/test_piranha_python.rs
--rw-r--r--   0     1001      123     1833 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/tests/test_piranha_swift.rs
--rw-r--r--   0     1001      123     1138 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/tests/test_piranha_ts.rs
--rw-r--r--   0     1001      123     1281 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/tests/test_piranha_tsx.rs
--rw-r--r--   0     1001      123     5476 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/utilities/mod.rs
--rw-r--r--   0     1001      123    12743 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/utilities/tree_sitter_utilities.rs
--rw-r--r--   0     1001      123     3681 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/utilities/unit_tests/tree_sitter_utilities_test.rs
--rw-r--r--   0     1001      123     2237 2023-04-06 19:46:26.000000 polyglot_piranha-0.3.1/src/utilities/unit_tests/utilities_test.rs
--rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.2/Cargo.toml
+-rw-r--r--   0     1001      123    35211 2023-04-11 23:15:27.000000 polyglot_piranha-0.3.2/Cargo.lock
+-rw-r--r--   0     1001      123    11359 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/LICENSE
+-rw-r--r--   0     1001      123     3091 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/README.md
+-rw-r--r--   0     1001      123     1373 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java
+-rw-r--r--   0     1001      123      994 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java
+-rw-r--r--   0     1001      123     5517 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java
+-rw-r--r--   0     1001      123     5621 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java
+-rw-r--r--   0     1001      123    66915 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java
+-rw-r--r--   0     1001      123    21518 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java
+-rw-r--r--   0     1001      123     5106 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java
+-rw-r--r--   0     1001      123      377 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaConfigurationException.java
+-rw-r--r--   0     1001      123     3615 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java
+-rw-r--r--   0     1001      123     5039 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java
+-rw-r--r--   0     1001      123     2584 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java
+-rw-r--r--   0     1001      123     2605 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java
+-rw-r--r--   0     1001      123      550 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java
+-rw-r--r--   0     1001      123     2456 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java
+-rw-r--r--   0     1001      123    13106 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java
+-rw-r--r--   0     1001      123     5875 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java
+-rw-r--r--   0     1001      123    85120 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java
+-rw-r--r--   0     1001      123    55188 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java
+-rw-r--r--   0     1001      123    48474 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java
+-rw-r--r--   0     1001      123     2304 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java
+-rw-r--r--   0     1001      123    33367 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java
+-rw-r--r--   0     1001      123     6780 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java
+-rw-r--r--   0     1001      123     3480 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java
+-rw-r--r--   0     1001      123     8540 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java
+-rw-r--r--   0     1001      123     4153 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java
+-rw-r--r--   0     1001      123     4326 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java
+-rw-r--r--   0     1001      123     2555 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java
+-rw-r--r--   0     1001      123     1490 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java
+-rw-r--r--   0     1001      123     2091 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java
+-rw-r--r--   0     1001      123     2194 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java
+-rw-r--r--   0     1001      123     1550 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java
+-rw-r--r--   0     1001      123     1618 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java
+-rw-r--r--   0     1001      123     1573 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java
+-rw-r--r--   0     1001      123       75 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParam.java
+-rw-r--r--   0     1001      123      109 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParameter.java
+-rw-r--r--   0     1001      123      175 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/OverlappingNameInterface.java
+-rw-r--r--   0     1001      123      103 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/PVal.java
+-rw-r--r--   0     1001      123      154 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/Parameter.java
+-rw-r--r--   0     1001      123      155 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeOtherInterface.java
+-rw-r--r--   0     1001      123      160 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeParamRev.java
+-rw-r--r--   0     1001      123      122 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/StaticMthds.java
+-rw-r--r--   0     1001      123      229 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/invalid/piranha.properties
+-rw-r--r--   0     1001      123       97 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid.json
+-rw-r--r--   0     1001      123      202 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_2.json
+-rw-r--r--   0     1001      123      213 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_3.json
+-rw-r--r--   0     1001      123      216 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_4.json
+-rw-r--r--   0     1001      123      361 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_enum_no_arg.json
+-rw-r--r--   0     1001      123      525 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json
+-rw-r--r--   0     1001      123      526 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json
+-rw-r--r--   0     1001      123      488 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name.json
+-rw-r--r--   0     1001      123      489 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name_no_method_chain.json
+-rw-r--r--   0     1001      123      526 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json
+-rw-r--r--   0     1001      123      704 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_argument.json
+-rw-r--r--   0     1001      123     1332 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json
+-rw-r--r--   0     1001      123      192 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_noFlag.json
+-rw-r--r--   0     1001      123      739 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json
+-rw-r--r--   0     1001      123      652 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_receive.json
+-rw-r--r--   0     1001      123     1896 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json
+-rw-r--r--   0     1001      123      844 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return.json
+-rw-r--r--   0     1001      123     1776 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json
+-rw-r--r--   0     1001      123     1932 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json
+-rw-r--r--   0     1001      123     4525 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json
+-rw-r--r--   0     1001      123      251 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_no_match.json
+-rw-r--r--   0     1001      123      246 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_wrong_arg.json
+-rw-r--r--   0     1001      123      142 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_without_enum.json
+-rw-r--r--   0     1001      123     1637 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json
+-rw-r--r--   0     1001      123     1304 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java
+-rw-r--r--   0     1001      123     1304 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak
+-rw-r--r--   0     1001      123     1107 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect
+-rw-r--r--   0     1001      123     2565 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/javascript/src/config_checker.js
+-rw-r--r--   0     1001      123     4304 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/javascript/src/piranha.js
+-rw-r--r--   0     1001      123    27988 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/javascript/src/refactor.js
+-rw-r--r--   0     1001      123     1445 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/javascript/src/source_checker.js
+-rw-r--r--   0     1001      123      646 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt
+-rw-r--r--   0     1001      123     1064 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/objc/src/XPFlagRefactoring/README.txt
+-rw-r--r--   0     1001      123    26229 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp
+-rw-r--r--   0     1001      123        0 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.exports
+-rw-r--r--   0     1001      123      793 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/pyproject.toml
+-rw-r--r--   0     1001      123     2043 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/go/edges.toml
+-rw-r--r--   0     1001      123    11027 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/go/rules.toml
+-rw-r--r--   0     1001      123     1460 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/go/scope_config.toml
+-rwxr-xr-x   0     1001      123     2241 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/java/edges.toml
+-rwxr-xr-x   0     1001      123    15939 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/java/rules.toml
+-rwxr-xr-x   0     1001      123     3582 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/java/scope_config.toml
+-rwxr-xr-x   0     1001      123     2251 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/kt/edges.toml
+-rwxr-xr-x   0     1001      123    19122 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/kt/rules.toml
+-rwxr-xr-x   0     1001      123     2139 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/kt/scope_config.toml
+-rw-r--r--   0     1001      123     1133 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/swift/edges.toml
+-rw-r--r--   0     1001      123     9296 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/swift/rules.toml
+-rw-r--r--   0     1001      123     1369 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/swift/scope_config.toml
+-rw-r--r--   0     1001      123     7317 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/lib.rs
+-rw-r--r--   0     1001      123     1679 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/main.rs
+-rw-r--r--   0     1001      123     5799 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/constraint.rs
+-rw-r--r--   0     1001      123     3143 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/default_configs.rs
+-rw-r--r--   0     1001      123     4915 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/edit.rs
+-rw-r--r--   0     1001      123     6744 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/language.rs
+-rw-r--r--   0     1001      123    11140 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/matches.rs
+-rw-r--r--   0     1001      123      928 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/mod.rs
+-rw-r--r--   0     1001      123     1987 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/outgoing_edges.rs
+-rw-r--r--   0     1001      123    14202 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/piranha_arguments.rs
+-rw-r--r--   0     1001      123     2091 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/piranha_output.rs
+-rw-r--r--   0     1001      123     7916 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/rule.rs
+-rw-r--r--   0     1001      123     6286 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/rule_graph.rs
+-rw-r--r--   0     1001      123     5931 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/rule_store.rs
+-rw-r--r--   0     1001      123     3329 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/scopes.rs
+-rw-r--r--   0     1001      123    14473 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/source_code_unit.rs
+-rw-r--r--   0     1001      123     1586 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/unit_tests/piranha_arguments_test.rs
+-rw-r--r--   0     1001      123     8340 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/unit_tests/rule_test.rs
+-rw-r--r--   0     1001      123     6061 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/unit_tests/scopes_test.rs
+-rw-r--r--   0     1001      123     6996 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/unit_tests/source_code_unit_test.rs
+-rw-r--r--   0     1001      123     8196 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/mod.rs
+-rw-r--r--   0     1001      123     1647 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/test_piranha_go.rs
+-rw-r--r--   0     1001      123    12255 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/test_piranha_java.rs
+-rw-r--r--   0     1001      123     1862 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/test_piranha_kt.rs
+-rw-r--r--   0     1001      123     2423 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/test_piranha_python.rs
+-rw-r--r--   0     1001      123     1833 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/test_piranha_swift.rs
+-rw-r--r--   0     1001      123     1138 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/test_piranha_ts.rs
+-rw-r--r--   0     1001      123     1281 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/test_piranha_tsx.rs
+-rw-r--r--   0     1001      123     5476 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/utilities/mod.rs
+-rw-r--r--   0     1001      123    12743 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/utilities/tree_sitter_utilities.rs
+-rw-r--r--   0     1001      123     3681 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/utilities/unit_tests/tree_sitter_utilities_test.rs
+-rw-r--r--   0     1001      123     2237 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/utilities/unit_tests/utilities_test.rs
+-rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.2/PKG-INFO
```

### Comparing `polyglot_piranha-0.3.1/Cargo.toml` & `polyglot_piranha-0.3.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "Ameya Ketkar <ketkara@uber.com>",
   "Lazaro Clapp <lazaro@uber.com>",
   "Murali Krishna Ramanathan",
   "Uber Technologies Inc.",
 ]
 name = "piranha"
 description = "Polyglot Piranha is a library for performing structural find and replace with deep cleanup."
-version = "0.3.1"
+version = "0.3.2"
 edition = "2021"
 include = ["pyproject.toml", "src/"]
 exclude = ["legacy"]
 license-file = "LICENSE"
 categories = [
   "structural find-replace",
   "find-replace",
```

### Comparing `polyglot_piranha-0.3.1/Cargo.lock` & `polyglot_piranha-0.3.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 version = "4.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9644cd56d6b87dbe899ef8b053e331c0637664e9e21a33dfcdc36093f5c5c4"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.14",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
@@ -199,17 +199,17 @@
  "crossbeam-epoch",
  "crossbeam-queue",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.7"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf2b3e8478797446514c91ef04bafcb59faba183e621ad488df88983cc14128c"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
@@ -349,21 +349,21 @@
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
 name = "errno"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d6a0976c999d473fe89ad888d5a284e55366d9dc9038b1ba2aa15128c4afa0"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -627,15 +627,15 @@
  "redox_syscall",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "piranha"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "assert_cmd",
  "cc",
  "clap",
  "colored",
  "derive_builder",
  "env_logger",
@@ -905,17 +905,17 @@
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.8"
+version = "0.37.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1aef160324be24d31a62147fae491c14d2204a3865c7ca8c3b0d7f7bcb3ea635"
+checksum = "85597d61f83914ddeba6a47b3b8ffe7365107221c2e557ed94426489fefb5f77"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
@@ -931,27 +931,27 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 
 [[package]]
 name = "serde_derive"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.14",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
@@ -991,17 +991,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.13"
+version = "2.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
+checksum = "fcf316d5356ed6847742d036f8a39c3b8435cac10bd528a4bd461928a6ab34d5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `polyglot_piranha-0.3.1/LICENSE` & `polyglot_piranha-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/README.md` & `polyglot_piranha-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_argument.json` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_receive.json` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_receive.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_return.json` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json` & `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java` & `polyglot_piranha-0.3.2/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak` & `polyglot_piranha-0.3.2/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect` & `polyglot_piranha-0.3.2/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/javascript/src/config_checker.js` & `polyglot_piranha-0.3.2/legacy/javascript/src/config_checker.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/javascript/src/piranha.js` & `polyglot_piranha-0.3.2/legacy/javascript/src/piranha.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/javascript/src/refactor.js` & `polyglot_piranha-0.3.2/legacy/javascript/src/refactor.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/javascript/src/source_checker.js` & `polyglot_piranha-0.3.2/legacy/javascript/src/source_checker.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt` & `polyglot_piranha-0.3.2/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/objc/src/XPFlagRefactoring/README.txt` & `polyglot_piranha-0.3.2/legacy/objc/src/XPFlagRefactoring/README.txt`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp` & `polyglot_piranha-0.3.2/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/pyproject.toml` & `polyglot_piranha-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/cleanup_rules/go/edges.toml` & `polyglot_piranha-0.3.2/src/cleanup_rules/go/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/cleanup_rules/go/rules.toml` & `polyglot_piranha-0.3.2/src/cleanup_rules/go/rules.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/cleanup_rules/go/scope_config.toml` & `polyglot_piranha-0.3.2/src/cleanup_rules/go/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/cleanup_rules/java/edges.toml` & `polyglot_piranha-0.3.2/src/cleanup_rules/java/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/cleanup_rules/java/rules.toml` & `polyglot_piranha-0.3.2/src/cleanup_rules/java/rules.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/cleanup_rules/java/scope_config.toml` & `polyglot_piranha-0.3.2/src/cleanup_rules/java/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/cleanup_rules/kt/edges.toml` & `polyglot_piranha-0.3.2/src/cleanup_rules/kt/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/cleanup_rules/kt/rules.toml` & `polyglot_piranha-0.3.2/src/cleanup_rules/kt/rules.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/cleanup_rules/kt/scope_config.toml` & `polyglot_piranha-0.3.2/src/cleanup_rules/kt/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/cleanup_rules/swift/edges.toml` & `polyglot_piranha-0.3.2/src/cleanup_rules/swift/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/cleanup_rules/swift/rules.toml` & `polyglot_piranha-0.3.2/src/cleanup_rules/swift/rules.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/cleanup_rules/swift/scope_config.toml` & `polyglot_piranha-0.3.2/src/cleanup_rules/swift/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/lib.rs` & `polyglot_piranha-0.3.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/main.rs` & `polyglot_piranha-0.3.2/src/main.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/constraint.rs` & `polyglot_piranha-0.3.2/src/models/constraint.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/default_configs.rs` & `polyglot_piranha-0.3.2/src/models/default_configs.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/edit.rs` & `polyglot_piranha-0.3.2/src/models/edit.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/language.rs` & `polyglot_piranha-0.3.2/src/models/language.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/matches.rs` & `polyglot_piranha-0.3.2/src/models/matches.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/mod.rs` & `polyglot_piranha-0.3.2/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/outgoing_edges.rs` & `polyglot_piranha-0.3.2/src/models/outgoing_edges.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/piranha_arguments.rs` & `polyglot_piranha-0.3.2/src/models/piranha_arguments.rs`

 * *Files 1% similar despite different names*

```diff
@@ -160,25 +160,30 @@
   /// * global_tag_prefix (string): the prefix for global tags
   /// * delete_file_if_empty (bool): User option that determines whether an empty file will be deleted
   /// * path_to_output_summary : Path to the file where the Piranha output summary should be persisted
   /// * allow_dirty_ast : Allows syntax errors in the input source code
   /// Returns PiranhaArgument.
   #[new]
   fn py_new(
-    language: String, substitutions: &PyDict, path_to_configurations: Option<String>,
+    language: String, substitutions: Option<&PyDict>, path_to_configurations: Option<String>,
     rule_graph: Option<RuleGraph>, path_to_codebase: Option<String>, code_snippet: Option<String>,
     dry_run: Option<bool>, cleanup_comments: Option<bool>, cleanup_comments_buffer: Option<i32>,
     number_of_ancestors_in_parent_scope: Option<u8>, delete_consecutive_new_lines: Option<bool>,
     global_tag_prefix: Option<String>, delete_file_if_empty: Option<bool>,
     path_to_output_summary: Option<String>, allow_dirty_ast: Option<bool>,
   ) -> Self {
-    let subs = substitutions
-      .iter()
-      .map(|(k, v)| (k.to_string(), v.to_string()))
-      .collect_vec();
+    let subs = if substitutions.is_some() {
+      substitutions
+        .unwrap()
+        .iter()
+        .map(|(k, v)| (k.to_string(), v.to_string()))
+        .collect_vec()
+    } else {
+      vec![]
+    };
 
     let rg = rule_graph.unwrap_or_else(|| RuleGraphBuilder::default().build());
     piranha_arguments! {
       path_to_codebase = path_to_codebase.unwrap_or_else(default_path_to_codebase),
       path_to_configurations = path_to_configurations.unwrap_or_else(default_path_to_configurations),
       rule_graph = rg,
       code_snippet = code_snippet.unwrap_or_else(default_code_snippet),
```

### Comparing `polyglot_piranha-0.3.1/src/models/piranha_output.rs` & `polyglot_piranha-0.3.2/src/models/piranha_output.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/rule.rs` & `polyglot_piranha-0.3.2/src/models/rule.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/rule_graph.rs` & `polyglot_piranha-0.3.2/src/models/rule_graph.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/rule_store.rs` & `polyglot_piranha-0.3.2/src/models/rule_store.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/scopes.rs` & `polyglot_piranha-0.3.2/src/models/scopes.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/source_code_unit.rs` & `polyglot_piranha-0.3.2/src/models/source_code_unit.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/unit_tests/piranha_arguments_test.rs` & `polyglot_piranha-0.3.2/src/models/unit_tests/piranha_arguments_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/unit_tests/rule_test.rs` & `polyglot_piranha-0.3.2/src/models/unit_tests/rule_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/unit_tests/scopes_test.rs` & `polyglot_piranha-0.3.2/src/models/unit_tests/scopes_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/models/unit_tests/source_code_unit_test.rs` & `polyglot_piranha-0.3.2/src/models/unit_tests/source_code_unit_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/tests/mod.rs` & `polyglot_piranha-0.3.2/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/tests/test_piranha_go.rs` & `polyglot_piranha-0.3.2/src/tests/test_piranha_go.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/tests/test_piranha_java.rs` & `polyglot_piranha-0.3.2/src/tests/test_piranha_java.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/tests/test_piranha_kt.rs` & `polyglot_piranha-0.3.2/src/tests/test_piranha_kt.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/tests/test_piranha_python.rs` & `polyglot_piranha-0.3.2/src/tests/test_piranha_python.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/tests/test_piranha_swift.rs` & `polyglot_piranha-0.3.2/src/tests/test_piranha_swift.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/tests/test_piranha_ts.rs` & `polyglot_piranha-0.3.2/src/tests/test_piranha_ts.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/tests/test_piranha_tsx.rs` & `polyglot_piranha-0.3.2/src/tests/test_piranha_tsx.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/utilities/mod.rs` & `polyglot_piranha-0.3.2/src/utilities/mod.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/utilities/tree_sitter_utilities.rs` & `polyglot_piranha-0.3.2/src/utilities/tree_sitter_utilities.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/utilities/unit_tests/tree_sitter_utilities_test.rs` & `polyglot_piranha-0.3.2/src/utilities/unit_tests/tree_sitter_utilities_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/src/utilities/unit_tests/utilities_test.rs` & `polyglot_piranha-0.3.2/src/utilities/unit_tests/utilities_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.1/PKG-INFO` & `polyglot_piranha-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: polyglot_piranha
-Version: 0.3.1
+Version: 0.3.2
 License-File: LICENSE
 License-File: LICENSE
 License-File: NOTICE
 Summary: Polyglot Piranha is a library for performing structural find and replace with deep cleanup.
 Keywords: refactoring,code update,structural find-replace,structural search and replace,structural search
 Author: Uber Technologies Inc.
 Author-email: Ameya Ketkar <ketkara@uber.com>, Lazaro Clapp <lazaro@uber.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: documentation, https://github.com/uber/piranha
 Project-URL: repository, https://github.com/uber/piranha
 Project-URL: homepage, https://github.com/uber/piranha
+Project-URL: documentation, https://github.com/uber/piranha
 
 # Piranha
 
 [![Join the chat at https://gitter.im/uber/piranha](https://badges.gitter.im/uber/piranha.svg)](https://gitter.im/uber/piranha?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 Feature flags are commonly used to enable gradual rollout or experiment with new features. In a few cases, even after the purpose of the flag is accomplished, the code pertaining to the feature flag is not removed. We refer to such flags as stale flags. The presence of code pertaining to stale flags can have the following drawbacks: 
 - Unnecessary code clutter increases the overall complexity w.r.t maintenance resulting in reduced developer productivity
```

