# Comparing `tmp/woke-3.1.0.tar.gz` & `tmp/woke-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woke-3.1.0.tar", max compression
+gzip compressed data, was "woke-3.2.0.tar", max compression
```

## Comparing `woke-3.1.0.tar` & `woke-3.2.0.tar`

### file list

```diff
@@ -1,238 +1,238 @@
--rw-r--r--   0        0        0      751 2023-03-24 22:12:38.649114 woke-3.1.0/LICENSE
--rw-r--r--   0        0        0     3423 2023-03-24 22:12:38.655781 woke-3.1.0/README.md
--rw-r--r--   0        0        0     2688 2023-03-25 09:58:41.055668 woke-3.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.672448 woke-3.1.0/woke/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.672448 woke-3.1.0/woke/analysis/__init__.py
--rw-r--r--   0        0        0    20349 2023-03-24 22:12:38.672448 woke-3.1.0/woke/analysis/cfg.py
--rw-r--r--   0        0        0     1013 2023-03-24 22:12:38.672448 woke-3.1.0/woke/analysis/detectors/__init__.py
--rw-r--r--   0        0        0    21690 2023-03-24 22:12:38.672448 woke-3.1.0/woke/analysis/detectors/api.py
--rw-r--r--   0        0        0       61 2023-03-24 22:12:38.672448 woke-3.1.0/woke/analysis/detectors/axelar/__init__.py
--rw-r--r--   0        0        0    14739 2023-03-24 22:12:38.672448 woke-3.1.0/woke/analysis/detectors/axelar/proxy_contract_id.py
--rw-r--r--   0        0        0     6292 2023-03-24 22:12:38.672448 woke-3.1.0/woke/analysis/detectors/balance_state_var.py
--rw-r--r--   0        0        0     4759 2023-03-24 22:12:38.672448 woke-3.1.0/woke/analysis/detectors/bug_empty_byte_array_copy.py
--rw-r--r--   0        0        0     1777 2023-03-24 22:12:38.672448 woke-3.1.0/woke/analysis/detectors/call_options_not_called.py
--rw-r--r--   0        0        0     4162 2023-03-24 22:12:38.672448 woke-3.1.0/woke/analysis/detectors/missing_return.py
--rw-r--r--   0        0        0     3013 2023-03-24 22:12:38.672448 woke-3.1.0/woke/analysis/detectors/msg_value_nonpayable_function.py
--rw-r--r--   0        0        0     8578 2023-03-24 22:12:38.672448 woke-3.1.0/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py
--rw-r--r--   0        0        0    17003 2023-03-24 22:12:38.675781 woke-3.1.0/woke/analysis/detectors/ownable.py
--rw-r--r--   0        0        0    23312 2023-03-24 22:12:38.675781 woke-3.1.0/woke/analysis/detectors/proxy_contract_selector_clashes.py
--rw-r--r--   0        0        0    13896 2023-03-24 22:12:38.675781 woke-3.1.0/woke/analysis/detectors/reentrancy.py
--rw-r--r--   0        0        0     2766 2023-03-24 22:12:38.675781 woke-3.1.0/woke/analysis/detectors/unchecked_return_value.py
--rw-r--r--   0        0        0     6242 2023-03-24 22:12:38.675781 woke-3.1.0/woke/analysis/detectors/unsafe_delegatecall.py
--rw-r--r--   0        0        0     1344 2023-03-24 22:12:38.675781 woke-3.1.0/woke/analysis/detectors/unsafe_selfdestruct.py
--rw-r--r--   0        0        0     5982 2023-03-24 22:12:38.675781 woke-3.1.0/woke/analysis/detectors/unsafe_tx_origin.py
--rw-r--r--   0        0        0     1397 2023-03-24 22:12:38.675781 woke-3.1.0/woke/analysis/detectors/unused_contract.py
--rw-r--r--   0        0        0    12233 2023-03-24 22:12:38.675781 woke-3.1.0/woke/analysis/detectors/utils.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/__init__.py
--rw-r--r--   0        0        0    10921 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/enums.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/__init__.py
--rw-r--r--   0        0        0     5939 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/abc.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/declaration/__init__.py
--rw-r--r--   0        0        0     5854 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/declaration/abc.py
--rw-r--r--   0        0        0    16242 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/declaration/contract_definition.py
--rw-r--r--   0        0        0     2460 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/declaration/enum_definition.py
--rw-r--r--   0        0        0     1360 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/declaration/enum_value.py
--rw-r--r--   0        0        0     4391 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/declaration/error_definition.py
--rw-r--r--   0        0        0     5162 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/declaration/event_definition.py
--rw-r--r--   0        0        0    18673 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/declaration/function_definition.py
--rw-r--r--   0        0        0    12886 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/declaration/modifier_definition.py
--rw-r--r--   0        0        0     2769 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/declaration/struct_definition.py
--rw-r--r--   0        0        0     2654 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/declaration/user_defined_value_type_definition.py
--rw-r--r--   0        0        0    17582 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/declaration/variable_declaration.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/__init__.py
--rw-r--r--   0        0        0     6583 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/abc.py
--rw-r--r--   0        0        0     3975 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/assignment.py
--rw-r--r--   0        0        0     2959 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/binary_operation.py
--rw-r--r--   0        0        0     2087 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/conditional.py
--rw-r--r--   0        0        0     1361 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/elementary_type_name_expression.py
--rw-r--r--   0        0        0     8923 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/function_call.py
--rw-r--r--   0        0        0     2132 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/function_call_options.py
--rw-r--r--   0        0        0     4446 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/identifier.py
--rw-r--r--   0        0        0     1996 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/index_access.py
--rw-r--r--   0        0        0     2661 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/index_range_access.py
--rw-r--r--   0        0        0     1437 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/literal.py
--rw-r--r--   0        0        0    18452 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/member_access.py
--rw-r--r--   0        0        0     1376 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/new_expression.py
--rw-r--r--   0        0        0     2186 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/tuple_expression.py
--rw-r--r--   0        0        0     3071 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/expression/unary_operation.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/meta/__init__.py
--rw-r--r--   0        0        0     8531 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/meta/identifier_path.py
--rw-r--r--   0        0        0     8845 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/meta/import_directive.py
--rw-r--r--   0        0        0     3751 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/meta/inheritance_specifier.py
--rw-r--r--   0        0        0     5699 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/meta/modifier_invocation.py
--rw-r--r--   0        0        0     3456 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/meta/override_specifier.py
--rw-r--r--   0        0        0     4305 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/meta/parameter_list.py
--rw-r--r--   0        0        0     1529 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/meta/pragma_directive.py
--rw-r--r--   0        0        0     9257 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/meta/source_unit.py
--rw-r--r--   0        0        0     2314 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/meta/structured_documentation.py
--rw-r--r--   0        0        0     4541 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/meta/try_catch_clause.py
--rw-r--r--   0        0        0     5698 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/meta/using_for_directive.py
--rw-r--r--   0        0        0     4849 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/reference_resolver.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/__init__.py
--rw-r--r--   0        0        0     5607 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/abc.py
--rw-r--r--   0        0        0     3130 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/block.py
--rw-r--r--   0        0        0     1610 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/break_statement.py
--rw-r--r--   0        0        0     1634 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/continue_statement.py
--rw-r--r--   0        0        0     2563 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/do_while_statement.py
--rw-r--r--   0        0        0     2452 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/emit_statement.py
--rw-r--r--   0        0        0     6016 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/expression_statement.py
--rw-r--r--   0        0        0     5735 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/for_statement.py
--rw-r--r--   0        0        0     3423 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/if_statement.py
--rw-r--r--   0        0        0    10271 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/inline_assembly.py
--rw-r--r--   0        0        0     1582 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/placeholder_statement.py
--rw-r--r--   0        0        0     3336 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/return_statement.py
--rw-r--r--   0        0        0     2608 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/revert_statement.py
--rw-r--r--   0        0        0     3129 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/try_statement.py
--rw-r--r--   0        0        0     2449 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/unchecked_block.py
--rw-r--r--   0        0        0     4325 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/variable_declaration_statement.py
--rw-r--r--   0        0        0     2596 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/statement/while_statement.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/type_name/__init__.py
--rw-r--r--   0        0        0     4932 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/type_name/abc.py
--rw-r--r--   0        0        0     4036 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/type_name/array_type_name.py
--rw-r--r--   0        0        0     5647 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/type_name/elementary_type_name.py
--rw-r--r--   0        0        0     3971 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/type_name/function_type_name.py
--rw-r--r--   0        0        0     3922 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/type_name/mapping.py
--rw-r--r--   0        0        0     8333 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/type_name/user_defined_type_name.py
--rw-r--r--   0        0        0       36 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/utils/__init__.py
--rw-r--r--   0        0        0      589 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/utils/init_tuple.py
--rw-r--r--   0        0        0      578 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/yul/__init__.py
--rw-r--r--   0        0        0      703 2023-03-25 09:49:53.164026 woke-3.1.0/woke/ast/ir/yul/abc.py
--rw-r--r--   0        0        0     1811 2023-03-25 09:49:53.164026 woke-3.1.0/woke/ast/ir/yul/assignment.py
--rw-r--r--   0        0        0     4302 2023-03-25 09:49:53.164026 woke-3.1.0/woke/ast/ir/yul/block.py
--rw-r--r--   0        0        0      300 2023-03-25 09:49:53.164026 woke-3.1.0/woke/ast/ir/yul/break_statement.py
--rw-r--r--   0        0        0     1199 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/yul/case_statement.py
--rw-r--r--   0        0        0      303 2023-03-25 09:49:53.164026 woke-3.1.0/woke/ast/ir/yul/continue_statement.py
--rw-r--r--   0        0        0     1658 2023-03-25 09:49:53.164026 woke-3.1.0/woke/ast/ir/yul/expression_statement.py
--rw-r--r--   0        0        0     1893 2023-03-25 09:49:53.164026 woke-3.1.0/woke/ast/ir/yul/for_loop.py
--rw-r--r--   0        0        0     2317 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/yul/function_call.py
--rw-r--r--   0        0        0     2288 2023-03-25 09:49:53.164026 woke-3.1.0/woke/ast/ir/yul/function_definition.py
--rw-r--r--   0        0        0     1492 2023-03-24 22:12:38.675781 woke-3.1.0/woke/ast/ir/yul/identifier.py
--rw-r--r--   0        0        0     1582 2023-03-25 09:49:53.164026 woke-3.1.0/woke/ast/ir/yul/if_statement.py
--rw-r--r--   0        0        0      300 2023-03-25 09:49:53.164026 woke-3.1.0/woke/ast/ir/yul/leave.py
--rw-r--r--   0        0        0     1780 2023-03-24 22:12:38.679114 woke-3.1.0/woke/ast/ir/yul/literal.py
--rw-r--r--   0        0        0     1796 2023-03-25 09:49:53.164026 woke-3.1.0/woke/ast/ir/yul/switch.py
--rw-r--r--   0        0        0      920 2023-03-24 22:12:38.679114 woke-3.1.0/woke/ast/ir/yul/typed_name.py
--rw-r--r--   0        0        0     2091 2023-03-25 09:49:53.164026 woke-3.1.0/woke/ast/ir/yul/variable_declaration.py
--rw-r--r--   0        0        0    37545 2023-03-24 22:12:38.679114 woke-3.1.0/woke/ast/nodes.py
--rw-r--r--   0        0        0    47040 2023-03-24 22:12:38.679114 woke-3.1.0/woke/ast/types.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.679114 woke-3.1.0/woke/cli/__init__.py
--rw-r--r--   0        0        0     3435 2023-03-24 22:12:38.679114 woke-3.1.0/woke/cli/__main__.py
--rw-r--r--   0        0        0     7942 2023-03-24 22:12:38.679114 woke-3.1.0/woke/cli/accounts.py
--rw-r--r--   0        0        0     4650 2023-03-24 22:12:38.679114 woke-3.1.0/woke/cli/compile.py
--rw-r--r--   0        0        0       54 2023-03-24 22:12:38.679114 woke-3.1.0/woke/cli/console.py
--rw-r--r--   0        0        0     3838 2023-03-24 22:12:38.679114 woke-3.1.0/woke/cli/detect.py
--rw-r--r--   0        0        0     3738 2023-03-25 09:49:53.164026 woke-3.1.0/woke/cli/fuzz.py
--rw-r--r--   0        0        0    11813 2023-03-25 09:49:53.164026 woke-3.1.0/woke/cli/init.py
--rw-r--r--   0        0        0     1081 2023-03-24 22:12:38.679114 woke-3.1.0/woke/cli/lsp.py
--rw-r--r--   0        0        0     2545 2023-03-24 22:12:38.679114 woke-3.1.0/woke/cli/run.py
--rw-r--r--   0        0        0     4922 2023-03-24 22:12:38.679114 woke-3.1.0/woke/cli/svm.py
--rw-r--r--   0        0        0     2190 2023-03-25 09:49:53.164026 woke-3.1.0/woke/cli/test.py
--rw-r--r--   0        0        0      187 2023-03-24 22:12:38.679114 woke-3.1.0/woke/compiler/__init__.py
--rw-r--r--   0        0        0     1814 2023-03-24 22:12:38.679114 woke-3.1.0/woke/compiler/build_data_model.py
--rw-r--r--   0        0        0     3078 2023-03-24 22:12:38.679114 woke-3.1.0/woke/compiler/compilation_unit.py
--rw-r--r--   0        0        0    40866 2023-03-24 22:12:38.679114 woke-3.1.0/woke/compiler/compiler.py
--rw-r--r--   0        0        0       97 2023-03-24 22:12:38.679114 woke-3.1.0/woke/compiler/exceptions.py
--rw-r--r--   0        0        0      103 2023-03-24 22:12:38.679114 woke-3.1.0/woke/compiler/solc_frontend/__init__.py
--rw-r--r--   0        0        0       48 2023-03-24 22:12:38.679114 woke-3.1.0/woke/compiler/solc_frontend/exceptions.py
--rw-r--r--   0        0        0     8554 2023-03-24 22:12:38.679114 woke-3.1.0/woke/compiler/solc_frontend/input_data_model.py
--rw-r--r--   0        0        0     8728 2023-03-24 22:12:38.679114 woke-3.1.0/woke/compiler/solc_frontend/output_data_model.py
--rw-r--r--   0        0        0     3571 2023-03-24 22:12:38.679114 woke-3.1.0/woke/compiler/solc_frontend/solc_runner.py
--rw-r--r--   0        0        0     2455 2023-03-24 22:12:38.679114 woke-3.1.0/woke/compiler/source_path_resolver.py
--rw-r--r--   0        0        0     4819 2023-03-24 22:12:38.679114 woke-3.1.0/woke/compiler/source_unit_name_resolver.py
--rw-r--r--   0        0        0     1118 2023-03-24 22:12:38.679114 woke-3.1.0/woke/config/__init__.py
--rw-r--r--   0        0        0     6685 2023-03-24 22:12:38.679114 woke-3.1.0/woke/config/data_model.py
--rw-r--r--   0        0        0    12419 2023-03-24 22:12:38.679114 woke-3.1.0/woke/config/woke_config.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.679114 woke-3.1.0/woke/contracts/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.679114 woke-3.1.0/woke/contracts/woke/__init__.py
--rw-r--r--   0        0        0    64087 2023-03-24 22:12:38.679114 woke-3.1.0/woke/contracts/woke/console.sol
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.679114 woke-3.1.0/woke/core/__init__.py
--rw-r--r--   0        0        0      360 2023-03-24 22:12:38.679114 woke-3.1.0/woke/core/enums.py
--rw-r--r--   0        0        0    24824 2023-03-24 22:12:38.679114 woke-3.1.0/woke/core/solidity_version.py
--rw-r--r--   0        0        0      663 2023-03-24 22:12:38.679114 woke-3.1.0/woke/deployment/__init__.py
--rw-r--r--   0        0        0    13302 2023-03-24 22:12:38.679114 woke-3.1.0/woke/deployment/core.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.679114 woke-3.1.0/woke/development/__init__.py
--rw-r--r--   0        0        0     4552 2023-03-24 22:12:38.679114 woke-3.1.0/woke/development/blocks.py
--rw-r--r--   0        0        0    28972 2023-03-24 22:12:38.679114 woke-3.1.0/woke/development/call_trace.py
--rw-r--r--   0        0        0    23917 2023-03-25 09:49:53.164026 woke-3.1.0/woke/development/chain_interfaces.py
--rw-r--r--   0        0        0     1132 2023-03-24 22:12:38.679114 woke-3.1.0/woke/development/constants.py
--rw-r--r--   0        0        0    94067 2023-03-25 09:49:53.167359 woke-3.1.0/woke/development/core.py
--rw-r--r--   0        0        0     2272 2023-03-25 09:49:53.167359 woke-3.1.0/woke/development/globals.py
--rw-r--r--   0        0        0   161115 2023-03-24 22:12:38.682448 woke-3.1.0/woke/development/hardhat_console.py
--rw-r--r--   0        0        0     1093 2023-03-24 22:12:38.682448 woke-3.1.0/woke/development/internal.py
--rw-r--r--   0        0        0       39 2023-03-24 22:12:38.682448 woke-3.1.0/woke/development/json_rpc/__init__.py
--rw-r--r--   0        0        0      302 2023-03-24 22:12:38.682448 woke-3.1.0/woke/development/json_rpc/abc.py
--rw-r--r--   0        0        0     2070 2023-03-24 22:12:38.682448 woke-3.1.0/woke/development/json_rpc/communicator.py
--rw-r--r--   0        0        0      821 2023-03-24 22:12:38.682448 woke-3.1.0/woke/development/json_rpc/http.py
--rw-r--r--   0        0        0     2733 2023-03-24 22:12:38.682448 woke-3.1.0/woke/development/json_rpc/ipc.py
--rw-r--r--   0        0        0      625 2023-03-24 22:12:38.682448 woke-3.1.0/woke/development/json_rpc/websocket.py
--rw-r--r--   0        0        0     6572 2023-03-24 22:12:38.682448 woke-3.1.0/woke/development/primitive_types.py
--rw-r--r--   0        0        0    87234 2023-03-24 22:12:38.682448 woke-3.1.0/woke/development/pytypes_generator.py
--rw-r--r--   0        0        0    22357 2023-03-24 22:12:38.682448 woke-3.1.0/woke/development/transactions.py
--rw-r--r--   0        0        0     5277 2023-03-24 22:12:38.682448 woke-3.1.0/woke/development/utils.py
--rw-r--r--   0        0        0       47 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/__init__.py
--rw-r--r--   0        0        0      310 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/commands/__init__.py
--rw-r--r--   0        0        0     3648 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/commands/generate_control_flow_graph.py
--rw-r--r--   0        0        0      938 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/commands/generate_imports_graph.py
--rw-r--r--   0        0        0     4247 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/commands/generate_inheritance_graph.py
--rw-r--r--   0        0        0     2163 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/commands/generate_linearized_inheritance_graph.py
--rw-r--r--   0        0        0    31330 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/common_structures.py
--rw-r--r--   0        0        0     1721 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/context.py
--rw-r--r--   0        0        0     2574 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/document_sync.py
--rw-r--r--   0        0        0      130 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/enums.py
--rw-r--r--   0        0        0      471 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/features/__init__.py
--rw-r--r--   0        0        0     9946 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/features/code_lens.py
--rw-r--r--   0        0        0    14531 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/features/completion.py
--rw-r--r--   0        0        0     9664 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/features/definition.py
--rw-r--r--   0        0        0     1446 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/features/diagnostic.py
--rw-r--r--   0        0        0     3908 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/features/document_link.py
--rw-r--r--   0        0        0     8407 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/features/document_symbol.py
--rw-r--r--   0        0        0    11205 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/features/hover.py
--rw-r--r--   0        0        0     3850 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/features/implementation.py
--rw-r--r--   0        0        0     5092 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/features/references.py
--rw-r--r--   0        0        0     8935 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/features/rename.py
--rw-r--r--   0        0        0     9505 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/features/type_definition.py
--rw-r--r--   0        0        0    11043 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/features/type_hierarchy.py
--rw-r--r--   0        0        0    37460 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/lsp_compiler.py
--rw-r--r--   0        0        0      328 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/lsp_data_model.py
--rw-r--r--   0        0        0     5551 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/methods.py
--rw-r--r--   0        0        0     1897 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/protocol_structures.py
--rw-r--r--   0        0        0     2229 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/rpc_protocol.py
--rw-r--r--   0        0        0    36478 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/server.py
--rw-r--r--   0        0        0     6541 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/server_capabilities.py
--rw-r--r--   0        0        0       86 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/utils/__init__.py
--rw-r--r--   0        0        0     1021 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/utils/position.py
--rw-r--r--   0        0        0      459 2023-03-24 22:12:38.682448 woke-3.1.0/woke/lsp/utils/uri.py
--rw-r--r--   0        0        0       50 2023-03-24 22:12:38.682448 woke-3.1.0/woke/regex_parser/__init__.py
--rw-r--r--   0        0        0     1690 2023-03-24 22:12:38.682448 woke-3.1.0/woke/regex_parser/solidity_import.py
--rw-r--r--   0        0        0     6653 2023-03-24 22:12:38.682448 woke-3.1.0/woke/regex_parser/solidity_parser.py
--rw-r--r--   0        0        0       36 2023-03-24 22:12:38.682448 woke-3.1.0/woke/svm/__init__.py
--rw-r--r--   0        0        0     1810 2023-03-24 22:12:38.682448 woke-3.1.0/woke/svm/abc.py
--rw-r--r--   0        0        0      270 2023-03-24 22:12:38.682448 woke-3.1.0/woke/svm/exceptions.py
--rw-r--r--   0        0        0    11716 2023-03-24 22:12:38.682448 woke-3.1.0/woke/svm/svm.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.682448 woke-3.1.0/woke/templates/scripts/__init__.py
--rw-r--r--   0        0        0      184 2023-03-24 22:12:38.682448 woke-3.1.0/woke/templates/scripts/deploy.py
--rw-r--r--   0        0        0        0 2023-03-24 22:12:38.682448 woke-3.1.0/woke/templates/tests/__init__.py
--rw-r--r--   0        0        0      140 2023-03-24 22:12:38.682448 woke-3.1.0/woke/templates/tests/test_default.py
--rw-r--r--   0        0        0      663 2023-03-24 22:12:38.682448 woke-3.1.0/woke/testing/__init__.py
--rw-r--r--   0        0        0    11178 2023-03-24 22:12:38.682448 woke-3.1.0/woke/testing/core.py
--rw-r--r--   0        0        0    24360 2023-03-25 09:49:53.167359 woke-3.1.0/woke/testing/coverage.py
--rw-r--r--   0        0        0      187 2023-03-24 22:12:38.682448 woke-3.1.0/woke/testing/fuzzing/__init__.py
--rw-r--r--   0        0        0     4999 2023-03-24 22:12:38.682448 woke-3.1.0/woke/testing/fuzzing/fuzz_test.py
--rw-r--r--   0        0        0     9792 2023-03-25 09:49:53.167359 woke-3.1.0/woke/testing/fuzzing/fuzzer.py
--rw-r--r--   0        0        0     5780 2023-03-24 22:12:38.682448 woke-3.1.0/woke/testing/fuzzing/generators.py
--rw-r--r--   0        0        0      298 2023-03-24 22:12:38.682448 woke-3.1.0/woke/testing/pytest_plugin.py
--rw-r--r--   0        0        0      170 2023-03-24 22:12:38.682448 woke-3.1.0/woke/utils/__init__.py
--rw-r--r--   0        0        0      560 2023-03-24 22:12:38.682448 woke-3.1.0/woke/utils/context_managers.py
--rw-r--r--   0        0        0      513 2023-03-24 22:12:38.682448 woke-3.1.0/woke/utils/decorators.py
--rw-r--r--   0        0        0      158 2023-03-24 22:12:38.682448 woke-3.1.0/woke/utils/enums.py
--rw-r--r--   0        0        0     1699 2023-03-24 22:12:38.682448 woke-3.1.0/woke/utils/file_utils.py
--rw-r--r--   0        0        0      383 2023-03-24 22:12:38.682448 woke-3.1.0/woke/utils/keyed_default_dict.py
--rw-r--r--   0        0        0      194 2023-03-24 22:12:38.682448 woke-3.1.0/woke/utils/networking.py
--rw-r--r--   0        0        0     1017 2023-03-24 22:12:38.682448 woke-3.1.0/woke/utils/openzeppelin.py
--rw-r--r--   0        0        0      630 2023-03-24 22:12:38.682448 woke-3.1.0/woke/utils/string.py
--rw-r--r--   0        0        0     1742 2023-03-24 22:12:38.682448 woke-3.1.0/woke/utils/tee.py
--rw-r--r--   0        0        0     3765 2023-03-24 22:12:38.682448 woke-3.1.0/woke/utils/threaded_child_watcher.py
--rw-r--r--   0        0        0      423 2023-03-24 22:12:38.682448 woke-3.1.0/woke/utils/version.py
--rw-r--r--   0        0        0     6061 1970-01-01 00:00:00.000000 woke-3.1.0/setup.py
--rw-r--r--   0        0        0     5959 1970-01-01 00:00:00.000000 woke-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0      751 2023-04-03 13:13:18.467843 woke-3.2.0/LICENSE
+-rw-r--r--   0        0        0     3423 2023-04-03 13:13:18.474510 woke-3.2.0/README.md
+-rw-r--r--   0        0        0     2655 2023-04-12 19:11:29.746527 woke-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.504510 woke-3.2.0/woke/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/__init__.py
+-rw-r--r--   0        0        0    20349 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/cfg.py
+-rw-r--r--   0        0        0     1013 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/__init__.py
+-rw-r--r--   0        0        0    21690 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/api.py
+-rw-r--r--   0        0        0       61 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/axelar/__init__.py
+-rw-r--r--   0        0        0    14739 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/axelar/proxy_contract_id.py
+-rw-r--r--   0        0        0     6292 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/balance_state_var.py
+-rw-r--r--   0        0        0     4759 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/bug_empty_byte_array_copy.py
+-rw-r--r--   0        0        0     1777 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/call_options_not_called.py
+-rw-r--r--   0        0        0     4162 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/missing_return.py
+-rw-r--r--   0        0        0     3013 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/msg_value_nonpayable_function.py
+-rw-r--r--   0        0        0     8578 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py
+-rw-r--r--   0        0        0    17003 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/ownable.py
+-rw-r--r--   0        0        0    23312 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/proxy_contract_selector_clashes.py
+-rw-r--r--   0        0        0    13896 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/reentrancy.py
+-rw-r--r--   0        0        0     2766 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/unchecked_return_value.py
+-rw-r--r--   0        0        0     6242 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/unsafe_delegatecall.py
+-rw-r--r--   0        0        0     1344 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/unsafe_selfdestruct.py
+-rw-r--r--   0        0        0     5982 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/unsafe_tx_origin.py
+-rw-r--r--   0        0        0     1397 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/unused_contract.py
+-rw-r--r--   0        0        0    12233 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/utils.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/__init__.py
+-rw-r--r--   0        0        0    10921 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/enums.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/__init__.py
+-rw-r--r--   0        0        0     5939 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/abc.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/__init__.py
+-rw-r--r--   0        0        0     5854 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/abc.py
+-rw-r--r--   0        0        0    16242 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/contract_definition.py
+-rw-r--r--   0        0        0     2460 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/enum_definition.py
+-rw-r--r--   0        0        0     1360 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/enum_value.py
+-rw-r--r--   0        0        0     4391 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/error_definition.py
+-rw-r--r--   0        0        0     5162 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/event_definition.py
+-rw-r--r--   0        0        0    18673 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/function_definition.py
+-rw-r--r--   0        0        0    12886 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/modifier_definition.py
+-rw-r--r--   0        0        0     2769 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/struct_definition.py
+-rw-r--r--   0        0        0     2654 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/user_defined_value_type_definition.py
+-rw-r--r--   0        0        0    17582 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/variable_declaration.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/__init__.py
+-rw-r--r--   0        0        0     6583 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/abc.py
+-rw-r--r--   0        0        0     3975 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/assignment.py
+-rw-r--r--   0        0        0     2959 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/binary_operation.py
+-rw-r--r--   0        0        0     2087 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/conditional.py
+-rw-r--r--   0        0        0     1361 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/elementary_type_name_expression.py
+-rw-r--r--   0        0        0     8923 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/function_call.py
+-rw-r--r--   0        0        0     2132 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/function_call_options.py
+-rw-r--r--   0        0        0     4446 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/identifier.py
+-rw-r--r--   0        0        0     1996 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/index_access.py
+-rw-r--r--   0        0        0     2661 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/expression/index_range_access.py
+-rw-r--r--   0        0        0     1437 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/expression/literal.py
+-rw-r--r--   0        0        0    18452 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/expression/member_access.py
+-rw-r--r--   0        0        0     1376 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/expression/new_expression.py
+-rw-r--r--   0        0        0     2186 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/expression/tuple_expression.py
+-rw-r--r--   0        0        0     3071 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/expression/unary_operation.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/__init__.py
+-rw-r--r--   0        0        0     8531 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/identifier_path.py
+-rw-r--r--   0        0        0     8845 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/import_directive.py
+-rw-r--r--   0        0        0     3751 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/inheritance_specifier.py
+-rw-r--r--   0        0        0     5699 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/modifier_invocation.py
+-rw-r--r--   0        0        0     3456 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/override_specifier.py
+-rw-r--r--   0        0        0     4305 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/parameter_list.py
+-rw-r--r--   0        0        0     1529 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/pragma_directive.py
+-rw-r--r--   0        0        0     9257 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/source_unit.py
+-rw-r--r--   0        0        0     2314 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/structured_documentation.py
+-rw-r--r--   0        0        0     4541 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/try_catch_clause.py
+-rw-r--r--   0        0        0     5698 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/using_for_directive.py
+-rw-r--r--   0        0        0     4849 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/reference_resolver.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/__init__.py
+-rw-r--r--   0        0        0     5607 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/abc.py
+-rw-r--r--   0        0        0     3130 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/block.py
+-rw-r--r--   0        0        0     1610 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/break_statement.py
+-rw-r--r--   0        0        0     1634 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/continue_statement.py
+-rw-r--r--   0        0        0     2563 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/do_while_statement.py
+-rw-r--r--   0        0        0     2452 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/emit_statement.py
+-rw-r--r--   0        0        0     6016 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/expression_statement.py
+-rw-r--r--   0        0        0     5735 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/for_statement.py
+-rw-r--r--   0        0        0     3423 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/if_statement.py
+-rw-r--r--   0        0        0    10271 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/inline_assembly.py
+-rw-r--r--   0        0        0     1582 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/placeholder_statement.py
+-rw-r--r--   0        0        0     3336 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/return_statement.py
+-rw-r--r--   0        0        0     2608 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/revert_statement.py
+-rw-r--r--   0        0        0     3129 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/try_statement.py
+-rw-r--r--   0        0        0     2449 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/unchecked_block.py
+-rw-r--r--   0        0        0     4325 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/variable_declaration_statement.py
+-rw-r--r--   0        0        0     2596 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/while_statement.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/type_name/__init__.py
+-rw-r--r--   0        0        0     4932 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/type_name/abc.py
+-rw-r--r--   0        0        0     4036 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/type_name/array_type_name.py
+-rw-r--r--   0        0        0     5647 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/type_name/elementary_type_name.py
+-rw-r--r--   0        0        0     3971 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/type_name/function_type_name.py
+-rw-r--r--   0        0        0     3922 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/type_name/mapping.py
+-rw-r--r--   0        0        0     8333 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/type_name/user_defined_type_name.py
+-rw-r--r--   0        0        0       36 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/utils/__init__.py
+-rw-r--r--   0        0        0      589 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/utils/init_tuple.py
+-rw-r--r--   0        0        0      578 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/__init__.py
+-rw-r--r--   0        0        0      703 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/abc.py
+-rw-r--r--   0        0        0     1811 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/assignment.py
+-rw-r--r--   0        0        0     4302 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/block.py
+-rw-r--r--   0        0        0      300 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/break_statement.py
+-rw-r--r--   0        0        0     1199 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/case_statement.py
+-rw-r--r--   0        0        0      303 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/continue_statement.py
+-rw-r--r--   0        0        0     1658 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/expression_statement.py
+-rw-r--r--   0        0        0     1893 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/for_loop.py
+-rw-r--r--   0        0        0     2317 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/function_call.py
+-rw-r--r--   0        0        0     2288 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/function_definition.py
+-rw-r--r--   0        0        0     1492 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/identifier.py
+-rw-r--r--   0        0        0     1582 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/if_statement.py
+-rw-r--r--   0        0        0      300 2023-04-03 13:13:18.511176 woke-3.2.0/woke/ast/ir/yul/leave.py
+-rw-r--r--   0        0        0     1780 2023-04-03 13:13:18.511176 woke-3.2.0/woke/ast/ir/yul/literal.py
+-rw-r--r--   0        0        0     1796 2023-04-03 13:13:18.511176 woke-3.2.0/woke/ast/ir/yul/switch.py
+-rw-r--r--   0        0        0      920 2023-04-03 13:13:18.511176 woke-3.2.0/woke/ast/ir/yul/typed_name.py
+-rw-r--r--   0        0        0     2091 2023-04-03 13:13:18.511176 woke-3.2.0/woke/ast/ir/yul/variable_declaration.py
+-rw-r--r--   0        0        0    37545 2023-04-03 13:13:18.511176 woke-3.2.0/woke/ast/nodes.py
+-rw-r--r--   0        0        0    47040 2023-04-03 13:13:18.511176 woke-3.2.0/woke/ast/types.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.511176 woke-3.2.0/woke/cli/__init__.py
+-rw-r--r--   0        0        0     3500 2023-04-12 19:11:06.759862 woke-3.2.0/woke/cli/__main__.py
+-rw-r--r--   0        0        0     7942 2023-04-03 13:13:18.511176 woke-3.2.0/woke/cli/accounts.py
+-rw-r--r--   0        0        0     4650 2023-04-06 18:42:41.395142 woke-3.2.0/woke/cli/compile.py
+-rw-r--r--   0        0        0       54 2023-04-03 13:13:18.511176 woke-3.2.0/woke/cli/console.py
+-rw-r--r--   0        0        0     3838 2023-04-03 13:13:18.511176 woke-3.2.0/woke/cli/detect.py
+-rw-r--r--   0        0        0     3791 2023-04-12 19:11:06.759862 woke-3.2.0/woke/cli/fuzz.py
+-rw-r--r--   0        0        0    11813 2023-04-03 13:13:18.511176 woke-3.2.0/woke/cli/init.py
+-rw-r--r--   0        0        0     1081 2023-04-03 13:13:18.511176 woke-3.2.0/woke/cli/lsp.py
+-rw-r--r--   0        0        0     3154 2023-04-12 19:11:06.759862 woke-3.2.0/woke/cli/run.py
+-rw-r--r--   0        0        0     4922 2023-04-03 13:13:18.511176 woke-3.2.0/woke/cli/svm.py
+-rw-r--r--   0        0        0     2258 2023-04-11 08:46:32.102660 woke-3.2.0/woke/cli/test.py
+-rw-r--r--   0        0        0      187 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/__init__.py
+-rw-r--r--   0        0        0     1814 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/build_data_model.py
+-rw-r--r--   0        0        0     3078 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/compilation_unit.py
+-rw-r--r--   0        0        0    40866 2023-04-10 08:07:29.589366 woke-3.2.0/woke/compiler/compiler.py
+-rw-r--r--   0        0        0       97 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/exceptions.py
+-rw-r--r--   0        0        0      103 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/solc_frontend/__init__.py
+-rw-r--r--   0        0        0       48 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/solc_frontend/exceptions.py
+-rw-r--r--   0        0        0     8554 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/solc_frontend/input_data_model.py
+-rw-r--r--   0        0        0     8728 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/solc_frontend/output_data_model.py
+-rw-r--r--   0        0        0     3571 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/solc_frontend/solc_runner.py
+-rw-r--r--   0        0        0     2455 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/source_path_resolver.py
+-rw-r--r--   0        0        0     4819 2023-04-10 08:45:44.228249 woke-3.2.0/woke/compiler/source_unit_name_resolver.py
+-rw-r--r--   0        0        0     1118 2023-04-03 13:13:18.511176 woke-3.2.0/woke/config/__init__.py
+-rw-r--r--   0        0        0     6866 2023-04-06 13:04:44.339069 woke-3.2.0/woke/config/data_model.py
+-rw-r--r--   0        0        0    12617 2023-04-05 07:53:42.584834 woke-3.2.0/woke/config/woke_config.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.511176 woke-3.2.0/woke/contracts/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.511176 woke-3.2.0/woke/contracts/woke/__init__.py
+-rw-r--r--   0        0        0    64087 2023-04-03 13:13:18.511176 woke-3.2.0/woke/contracts/woke/console.sol
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.511176 woke-3.2.0/woke/core/__init__.py
+-rw-r--r--   0        0        0      360 2023-04-03 13:13:18.511176 woke-3.2.0/woke/core/enums.py
+-rw-r--r--   0        0        0    24824 2023-04-03 13:13:18.511176 woke-3.2.0/woke/core/solidity_version.py
+-rw-r--r--   0        0        0      663 2023-04-03 13:13:18.511176 woke-3.2.0/woke/deployment/__init__.py
+-rw-r--r--   0        0        0    14322 2023-04-12 19:11:06.759862 woke-3.2.0/woke/deployment/core.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.511176 woke-3.2.0/woke/development/__init__.py
+-rw-r--r--   0        0        0     4552 2023-04-03 13:13:18.511176 woke-3.2.0/woke/development/blocks.py
+-rw-r--r--   0        0        0    28998 2023-04-12 19:11:06.763195 woke-3.2.0/woke/development/call_trace.py
+-rw-r--r--   0        0        0    26323 2023-04-11 09:25:36.391768 woke-3.2.0/woke/development/chain_interfaces.py
+-rw-r--r--   0        0        0     1132 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/constants.py
+-rw-r--r--   0        0        0    94704 2023-04-12 19:11:06.763195 woke-3.2.0/woke/development/core.py
+-rw-r--r--   0        0        0     7222 2023-04-12 19:11:06.763195 woke-3.2.0/woke/development/globals.py
+-rw-r--r--   0        0        0   161115 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/hardhat_console.py
+-rw-r--r--   0        0        0     1093 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/internal.py
+-rw-r--r--   0        0        0       39 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/json_rpc/__init__.py
+-rw-r--r--   0        0        0      302 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/json_rpc/abc.py
+-rw-r--r--   0        0        0     2070 2023-04-05 07:27:39.545655 woke-3.2.0/woke/development/json_rpc/communicator.py
+-rw-r--r--   0        0        0      821 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/json_rpc/http.py
+-rw-r--r--   0        0        0     2733 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/json_rpc/ipc.py
+-rw-r--r--   0        0        0      625 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/json_rpc/websocket.py
+-rw-r--r--   0        0        0     6572 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/primitive_types.py
+-rw-r--r--   0        0        0    88054 2023-04-12 19:11:06.763195 woke-3.2.0/woke/development/pytypes_generator.py
+-rw-r--r--   0        0        0    26578 2023-04-12 19:11:06.763195 woke-3.2.0/woke/development/transactions.py
+-rw-r--r--   0        0        0     7389 2023-04-05 07:53:42.588167 woke-3.2.0/woke/development/utils.py
+-rw-r--r--   0        0        0       47 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/__init__.py
+-rw-r--r--   0        0        0      310 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/commands/__init__.py
+-rw-r--r--   0        0        0     3648 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/commands/generate_control_flow_graph.py
+-rw-r--r--   0        0        0      938 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/commands/generate_imports_graph.py
+-rw-r--r--   0        0        0     4247 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/commands/generate_inheritance_graph.py
+-rw-r--r--   0        0        0     2163 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/commands/generate_linearized_inheritance_graph.py
+-rw-r--r--   0        0        0    31330 2023-04-10 08:45:44.228249 woke-3.2.0/woke/lsp/common_structures.py
+-rw-r--r--   0        0        0     1721 2023-04-10 08:45:44.228249 woke-3.2.0/woke/lsp/context.py
+-rw-r--r--   0        0        0     2574 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/document_sync.py
+-rw-r--r--   0        0        0      130 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/enums.py
+-rw-r--r--   0        0        0      471 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/__init__.py
+-rw-r--r--   0        0        0     9946 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/code_lens.py
+-rw-r--r--   0        0        0    14531 2023-04-10 08:45:44.228249 woke-3.2.0/woke/lsp/features/completion.py
+-rw-r--r--   0        0        0     9664 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/definition.py
+-rw-r--r--   0        0        0     1446 2023-04-06 18:43:28.740922 woke-3.2.0/woke/lsp/features/diagnostic.py
+-rw-r--r--   0        0        0     3908 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/document_link.py
+-rw-r--r--   0        0        0     8407 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/document_symbol.py
+-rw-r--r--   0        0        0    11205 2023-04-10 08:45:44.228249 woke-3.2.0/woke/lsp/features/hover.py
+-rw-r--r--   0        0        0     3850 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/implementation.py
+-rw-r--r--   0        0        0     5092 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/references.py
+-rw-r--r--   0        0        0     8935 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/rename.py
+-rw-r--r--   0        0        0     9505 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/type_definition.py
+-rw-r--r--   0        0        0    11043 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/type_hierarchy.py
+-rw-r--r--   0        0        0    37460 2023-04-09 08:21:30.944679 woke-3.2.0/woke/lsp/lsp_compiler.py
+-rw-r--r--   0        0        0      328 2023-04-03 13:13:18.517843 woke-3.2.0/woke/lsp/lsp_data_model.py
+-rw-r--r--   0        0        0     5551 2023-04-03 13:13:18.517843 woke-3.2.0/woke/lsp/methods.py
+-rw-r--r--   0        0        0     1897 2023-04-03 13:13:18.517843 woke-3.2.0/woke/lsp/protocol_structures.py
+-rw-r--r--   0        0        0     2229 2023-04-03 13:13:18.517843 woke-3.2.0/woke/lsp/rpc_protocol.py
+-rw-r--r--   0        0        0    36478 2023-04-10 08:45:44.228249 woke-3.2.0/woke/lsp/server.py
+-rw-r--r--   0        0        0     6541 2023-04-10 08:45:44.228249 woke-3.2.0/woke/lsp/server_capabilities.py
+-rw-r--r--   0        0        0       86 2023-04-03 13:13:18.517843 woke-3.2.0/woke/lsp/utils/__init__.py
+-rw-r--r--   0        0        0     1021 2023-04-03 13:13:18.517843 woke-3.2.0/woke/lsp/utils/position.py
+-rw-r--r--   0        0        0      459 2023-04-03 13:13:18.517843 woke-3.2.0/woke/lsp/utils/uri.py
+-rw-r--r--   0        0        0       50 2023-04-03 13:13:18.517843 woke-3.2.0/woke/regex_parser/__init__.py
+-rw-r--r--   0        0        0     1690 2023-04-03 13:13:18.517843 woke-3.2.0/woke/regex_parser/solidity_import.py
+-rw-r--r--   0        0        0     6653 2023-04-03 13:13:18.517843 woke-3.2.0/woke/regex_parser/solidity_parser.py
+-rw-r--r--   0        0        0       36 2023-04-03 13:13:18.517843 woke-3.2.0/woke/svm/__init__.py
+-rw-r--r--   0        0        0     1810 2023-04-03 13:13:18.517843 woke-3.2.0/woke/svm/abc.py
+-rw-r--r--   0        0        0      270 2023-04-03 13:13:18.517843 woke-3.2.0/woke/svm/exceptions.py
+-rw-r--r--   0        0        0    11716 2023-04-03 13:13:18.517843 woke-3.2.0/woke/svm/svm.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.517843 woke-3.2.0/woke/templates/scripts/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-03 13:13:18.517843 woke-3.2.0/woke/templates/scripts/deploy.py
+-rw-r--r--   0        0        0        0 2023-04-03 13:13:18.517843 woke-3.2.0/woke/templates/tests/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-03 13:13:18.517843 woke-3.2.0/woke/templates/tests/test_default.py
+-rw-r--r--   0        0        0      663 2023-04-03 13:13:18.517843 woke-3.2.0/woke/testing/__init__.py
+-rw-r--r--   0        0        0    11329 2023-04-12 19:11:06.763195 woke-3.2.0/woke/testing/core.py
+-rw-r--r--   0        0        0    24360 2023-04-03 13:13:18.517843 woke-3.2.0/woke/testing/coverage.py
+-rw-r--r--   0        0        0      187 2023-04-03 13:13:18.517843 woke-3.2.0/woke/testing/fuzzing/__init__.py
+-rw-r--r--   0        0        0     4999 2023-04-03 13:13:18.517843 woke-3.2.0/woke/testing/fuzzing/fuzz_test.py
+-rw-r--r--   0        0        0    10795 2023-04-12 19:11:06.763195 woke-3.2.0/woke/testing/fuzzing/fuzzer.py
+-rw-r--r--   0        0        0     5780 2023-04-03 13:13:18.517843 woke-3.2.0/woke/testing/fuzzing/generators.py
+-rw-r--r--   0        0        0      298 2023-04-03 13:13:18.517843 woke-3.2.0/woke/testing/pytest_plugin.py
+-rw-r--r--   0        0        0      170 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/__init__.py
+-rw-r--r--   0        0        0      560 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/context_managers.py
+-rw-r--r--   0        0        0      513 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/decorators.py
+-rw-r--r--   0        0        0      158 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/enums.py
+-rw-r--r--   0        0        0     1699 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/file_utils.py
+-rw-r--r--   0        0        0      383 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/keyed_default_dict.py
+-rw-r--r--   0        0        0      194 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/networking.py
+-rw-r--r--   0        0        0     1017 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/openzeppelin.py
+-rw-r--r--   0        0        0      630 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/string.py
+-rw-r--r--   0        0        0     1742 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/tee.py
+-rw-r--r--   0        0        0     3765 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/threaded_child_watcher.py
+-rw-r--r--   0        0        0      423 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/version.py
+-rw-r--r--   0        0        0     6058 1970-01-01 00:00:00.000000 woke-3.2.0/setup.py
+-rw-r--r--   0        0        0     5956 1970-01-01 00:00:00.000000 woke-3.2.0/PKG-INFO
```

### Comparing `woke-3.1.0/LICENSE` & `woke-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/README.md` & `woke-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/pyproject.toml` & `woke-3.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "woke"
-version = "3.1.0"
+version = "3.2.0"
 description = "Woke is a Python-based development and testing framework for Solidity."
 license = "ISC"
 authors = ["Ackee Blockchain"]
 readme = "README.md"
 homepage = "https://ackeeblockchain.com"
 repository = "https://github.com/Ackee-Blockchain/woke"
 documentation = "https://ackeeblockchain.com/woke/docs/latest"
@@ -28,17 +28,17 @@
 eth-account = "^0.8"
 eth-utils = "^2.1"
 eth-abi = { version = "^4.0.0b2", allow-prereleases = true }
 parsimonious = "^0.9"
 eth-hash = { version = "^0.5.1", extras = ["pycryptodome"] }
 websocket-client = "^1.4"
 pywin32 = { version = ">= 302", platform = "win32" }
-watchdog = "^2.2"
+watchdog = "~2.2.0"
 pytest = "^7"
-pdbr = { version = "^0.8.0", extras = ["ipython"] }
+ipdb = "^0.13.9"
 
 pytest-asyncio = { version = "^0.17", optional = true }
 GitPython = { version = "^3.1.20", optional = true }
 
 black = { version = "^22", optional = true }
 mkdocs-material = { version = "^9", optional = true }
 mkdocstrings = { version = "^0.19", extras = ["python"], optional = true }
```

### Comparing `woke-3.1.0/woke/analysis/cfg.py` & `woke-3.2.0/woke/analysis/cfg.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/__init__.py` & `woke-3.2.0/woke/analysis/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/api.py` & `woke-3.2.0/woke/analysis/detectors/api.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/axelar/proxy_contract_id.py` & `woke-3.2.0/woke/analysis/detectors/axelar/proxy_contract_id.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/balance_state_var.py` & `woke-3.2.0/woke/analysis/detectors/balance_state_var.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/bug_empty_byte_array_copy.py` & `woke-3.2.0/woke/analysis/detectors/bug_empty_byte_array_copy.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/call_options_not_called.py` & `woke-3.2.0/woke/analysis/detectors/call_options_not_called.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/missing_return.py` & `woke-3.2.0/woke/analysis/detectors/missing_return.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/msg_value_nonpayable_function.py` & `woke-3.2.0/woke/analysis/detectors/msg_value_nonpayable_function.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py` & `woke-3.2.0/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/ownable.py` & `woke-3.2.0/woke/analysis/detectors/ownable.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/proxy_contract_selector_clashes.py` & `woke-3.2.0/woke/analysis/detectors/proxy_contract_selector_clashes.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/reentrancy.py` & `woke-3.2.0/woke/analysis/detectors/reentrancy.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/unchecked_return_value.py` & `woke-3.2.0/woke/analysis/detectors/unchecked_return_value.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/unsafe_delegatecall.py` & `woke-3.2.0/woke/analysis/detectors/unsafe_delegatecall.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/unsafe_selfdestruct.py` & `woke-3.2.0/woke/analysis/detectors/unsafe_selfdestruct.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/unsafe_tx_origin.py` & `woke-3.2.0/woke/analysis/detectors/unsafe_tx_origin.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/unused_contract.py` & `woke-3.2.0/woke/analysis/detectors/unused_contract.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/analysis/detectors/utils.py` & `woke-3.2.0/woke/analysis/detectors/utils.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/enums.py` & `woke-3.2.0/woke/ast/enums.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/abc.py` & `woke-3.2.0/woke/ast/ir/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/declaration/abc.py` & `woke-3.2.0/woke/ast/ir/declaration/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/declaration/contract_definition.py` & `woke-3.2.0/woke/ast/ir/declaration/contract_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/declaration/enum_definition.py` & `woke-3.2.0/woke/ast/ir/declaration/enum_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/declaration/enum_value.py` & `woke-3.2.0/woke/ast/ir/declaration/enum_value.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/declaration/error_definition.py` & `woke-3.2.0/woke/ast/ir/declaration/error_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/declaration/event_definition.py` & `woke-3.2.0/woke/ast/ir/declaration/event_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/declaration/function_definition.py` & `woke-3.2.0/woke/ast/ir/declaration/function_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/declaration/modifier_definition.py` & `woke-3.2.0/woke/ast/ir/declaration/modifier_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/declaration/struct_definition.py` & `woke-3.2.0/woke/ast/ir/declaration/struct_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/declaration/user_defined_value_type_definition.py` & `woke-3.2.0/woke/ast/ir/declaration/user_defined_value_type_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/declaration/variable_declaration.py` & `woke-3.2.0/woke/ast/ir/declaration/variable_declaration.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/abc.py` & `woke-3.2.0/woke/ast/ir/expression/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/assignment.py` & `woke-3.2.0/woke/ast/ir/expression/assignment.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/binary_operation.py` & `woke-3.2.0/woke/ast/ir/expression/binary_operation.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/conditional.py` & `woke-3.2.0/woke/ast/ir/expression/conditional.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/elementary_type_name_expression.py` & `woke-3.2.0/woke/ast/ir/expression/elementary_type_name_expression.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/function_call.py` & `woke-3.2.0/woke/ast/ir/expression/function_call.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/function_call_options.py` & `woke-3.2.0/woke/ast/ir/expression/function_call_options.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/identifier.py` & `woke-3.2.0/woke/ast/ir/expression/identifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/index_access.py` & `woke-3.2.0/woke/ast/ir/expression/index_access.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/index_range_access.py` & `woke-3.2.0/woke/ast/ir/expression/index_range_access.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/literal.py` & `woke-3.2.0/woke/ast/ir/expression/literal.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/member_access.py` & `woke-3.2.0/woke/ast/ir/expression/member_access.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/new_expression.py` & `woke-3.2.0/woke/ast/ir/expression/new_expression.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/tuple_expression.py` & `woke-3.2.0/woke/ast/ir/expression/tuple_expression.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/expression/unary_operation.py` & `woke-3.2.0/woke/ast/ir/expression/unary_operation.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/meta/identifier_path.py` & `woke-3.2.0/woke/ast/ir/meta/identifier_path.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/meta/import_directive.py` & `woke-3.2.0/woke/ast/ir/meta/import_directive.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/meta/inheritance_specifier.py` & `woke-3.2.0/woke/ast/ir/meta/inheritance_specifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/meta/modifier_invocation.py` & `woke-3.2.0/woke/ast/ir/meta/modifier_invocation.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/meta/override_specifier.py` & `woke-3.2.0/woke/ast/ir/meta/override_specifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/meta/parameter_list.py` & `woke-3.2.0/woke/ast/ir/meta/parameter_list.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/meta/pragma_directive.py` & `woke-3.2.0/woke/ast/ir/meta/pragma_directive.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/meta/source_unit.py` & `woke-3.2.0/woke/ast/ir/meta/source_unit.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/meta/structured_documentation.py` & `woke-3.2.0/woke/ast/ir/meta/structured_documentation.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/meta/try_catch_clause.py` & `woke-3.2.0/woke/ast/ir/meta/try_catch_clause.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/meta/using_for_directive.py` & `woke-3.2.0/woke/ast/ir/meta/using_for_directive.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/reference_resolver.py` & `woke-3.2.0/woke/ast/ir/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/abc.py` & `woke-3.2.0/woke/ast/ir/statement/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/block.py` & `woke-3.2.0/woke/ast/ir/statement/block.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/break_statement.py` & `woke-3.2.0/woke/ast/ir/statement/break_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/continue_statement.py` & `woke-3.2.0/woke/ast/ir/statement/continue_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/do_while_statement.py` & `woke-3.2.0/woke/ast/ir/statement/do_while_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/emit_statement.py` & `woke-3.2.0/woke/ast/ir/statement/emit_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/expression_statement.py` & `woke-3.2.0/woke/ast/ir/statement/expression_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/for_statement.py` & `woke-3.2.0/woke/ast/ir/statement/for_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/if_statement.py` & `woke-3.2.0/woke/ast/ir/statement/if_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/inline_assembly.py` & `woke-3.2.0/woke/ast/ir/statement/inline_assembly.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/placeholder_statement.py` & `woke-3.2.0/woke/ast/ir/statement/placeholder_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/return_statement.py` & `woke-3.2.0/woke/ast/ir/statement/return_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/revert_statement.py` & `woke-3.2.0/woke/ast/ir/statement/revert_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/try_statement.py` & `woke-3.2.0/woke/ast/ir/statement/try_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/unchecked_block.py` & `woke-3.2.0/woke/ast/ir/statement/unchecked_block.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/variable_declaration_statement.py` & `woke-3.2.0/woke/ast/ir/statement/variable_declaration_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/statement/while_statement.py` & `woke-3.2.0/woke/ast/ir/statement/while_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/type_name/abc.py` & `woke-3.2.0/woke/ast/ir/type_name/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/type_name/array_type_name.py` & `woke-3.2.0/woke/ast/ir/type_name/array_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/type_name/elementary_type_name.py` & `woke-3.2.0/woke/ast/ir/type_name/elementary_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/type_name/function_type_name.py` & `woke-3.2.0/woke/ast/ir/type_name/function_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/type_name/mapping.py` & `woke-3.2.0/woke/ast/ir/type_name/mapping.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/type_name/user_defined_type_name.py` & `woke-3.2.0/woke/ast/ir/type_name/user_defined_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/utils/init_tuple.py` & `woke-3.2.0/woke/ast/ir/utils/init_tuple.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/__init__.py` & `woke-3.2.0/woke/ast/ir/yul/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/abc.py` & `woke-3.2.0/woke/ast/ir/yul/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/assignment.py` & `woke-3.2.0/woke/ast/ir/yul/assignment.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/block.py` & `woke-3.2.0/woke/ast/ir/yul/block.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/case_statement.py` & `woke-3.2.0/woke/ast/ir/yul/case_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/expression_statement.py` & `woke-3.2.0/woke/ast/ir/yul/expression_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/for_loop.py` & `woke-3.2.0/woke/ast/ir/yul/for_loop.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/function_call.py` & `woke-3.2.0/woke/ast/ir/yul/function_call.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/function_definition.py` & `woke-3.2.0/woke/ast/ir/yul/function_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/identifier.py` & `woke-3.2.0/woke/ast/ir/yul/identifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/if_statement.py` & `woke-3.2.0/woke/ast/ir/yul/if_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/literal.py` & `woke-3.2.0/woke/ast/ir/yul/literal.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/switch.py` & `woke-3.2.0/woke/ast/ir/yul/switch.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/typed_name.py` & `woke-3.2.0/woke/ast/ir/yul/typed_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/ir/yul/variable_declaration.py` & `woke-3.2.0/woke/ast/ir/yul/variable_declaration.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/nodes.py` & `woke-3.2.0/woke/ast/nodes.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/ast/types.py` & `woke-3.2.0/woke/ast/types.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/cli/__main__.py` & `woke-3.2.0/woke/cli/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import logging
+import os
 import platform
 from pathlib import Path
 from typing import Optional
 
 import rich.traceback
 import rich_click as click
 from click.core import Context
@@ -63,14 +64,16 @@
     ctx.obj["debug"] = debug
 
     if platform.system() == "Windows":
         asyncio.set_event_loop_policy(asyncio.WindowsProactorEventLoopPolicy())
     else:
         asyncio.get_event_loop_policy().set_child_watcher(ThreadedChildWatcher())
 
+    os.environ["PYTHONBREAKPOINT"] = "ipdb.set_trace"
+
 
 main.add_command(run_accounts)
 main.add_command(run_compile)
 main.add_command(run_detect)
 main.add_command(run_fuzz)
 main.add_command(run_init)
 main.add_command(run_lsp)
```

### Comparing `woke-3.1.0/woke/cli/accounts.py` & `woke-3.2.0/woke/cli/accounts.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/cli/compile.py` & `woke-3.2.0/woke/cli/compile.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/cli/detect.py` & `woke-3.2.0/woke/cli/detect.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/cli/fuzz.py` & `woke-3.2.0/woke/cli/fuzz.py`

 * *Files 12% similar despite different names*

```diff
@@ -90,35 +90,34 @@
         module_spec = importlib.util.spec_from_file_location(module_name, file)
         if module_spec is None or module_spec.loader is None:
             raise ValueError()
         module = importlib.util.module_from_spec(module_spec)
         sys.modules[module_name] = module
         module_spec.loader.exec_module(module)
 
-        functions: Iterable[Callable] = (
-            func
-            for _, func in inspect.getmembers(module, inspect.isfunction)
-            if func.__module__ == module_name and func.__name__.startswith("test")
+        functions: Iterable[Tuple[str, Callable]] = (
+            (func_name, func)
+            for func_name, func in inspect.getmembers(module, inspect.isfunction)
+            if func.__module__ == module_name and func_name.startswith("test")
         )
-        for func in functions:
-            console.print(
-                f"Found '{func.__name__}' function in '{func.__module__}' file."
-            )
-            fuzz_functions.append(func)
+        for func_name, func in functions:
+            console.print(f"Found '{func_name}' function in '{func.__module__}' file.")
+            fuzz_functions.append((func_name, func))
 
     logs_dir = config.project_root_path / ".woke-logs" / "fuzz"
     shutil.rmtree(logs_dir, ignore_errors=True)
     logs_dir.mkdir(parents=True, exist_ok=True)
 
     try:
-        for func in fuzz_functions:
+        for func_name, func in fuzz_functions:
             console.print("\n\n")
-            console.print(f"Fuzzing '{func.__name__}' in '{func.__module__}'.")
+            console.print(f"Fuzzing '{func_name}' in '{func.__module__}'.")
             fuzz(
                 config,
+                func_name,
                 func,
                 process_count,
                 random_seeds,
                 logs_dir,
                 passive,
                 coverage,
                 False,
```

### Comparing `woke-3.1.0/woke/cli/init.py` & `woke-3.2.0/woke/cli/init.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/cli/lsp.py` & `woke-3.2.0/woke/cli/lsp.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/cli/run.py` & `woke-3.2.0/woke/cli/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,32 +10,55 @@
 
 
 @click.command(name="run")
 @click.argument("paths", nargs=-1, type=click.Path(exists=True))
 @click.option(
     "--debug", "-d", is_flag=True, default=False, help="Attach debugger on exception."
 )
-def run_run(paths: Tuple[str, ...], debug: bool) -> None:
+@click.option(
+    "--ask/--no-ask",
+    is_flag=True,
+    default=True,
+    help="Confirm transaction before execution.",
+)
+@click.option(
+    "--silent/--no-silent",
+    is_flag=True,
+    default=False,
+    help="Do not print transaction info.",
+)
+def run_run(paths: Tuple[str, ...], debug: bool, ask: bool, silent: bool) -> None:
     """Run a Woke script."""
 
     import importlib.util
     import inspect
     import sys
 
     from woke.config import WokeConfig
     from woke.development.globals import (
         attach_debugger,
+        chain_interfaces_manager,
+        get_config,
         reset_exception_handled,
         set_exception_handler,
     )
 
     from .console import console
 
     config = WokeConfig()
     config.load_configs()
+    get_config().update(
+        {
+            "deployment": {
+                "confirm_transactions": ask,
+                "silent": silent,
+            }
+        },
+        [],
+    )
 
     if len(paths) == 0:
         paths = (str(config.project_root_path / "scripts"),)
 
     py_files = set()
 
     for path in paths:
@@ -72,14 +95,17 @@
     if debug:
         set_exception_handler(attach_debugger)
 
     if len(run_functions) == 0:
         console.print("[yellow]No 'main' functions found in scripts.[/]")
         return
 
-    for func in run_functions:
-        console.print(f"Running {func.__module__}...")
-        try:
-            func()
-        finally:
-            if debug:
-                reset_exception_handled()
+    try:
+        for func in run_functions:
+            console.print(f"Running {func.__module__}...")
+            try:
+                func()
+            finally:
+                if debug:
+                    reset_exception_handled()
+    finally:
+        chain_interfaces_manager.close_all()
```

### Comparing `woke-3.1.0/woke/cli/svm.py` & `woke-3.2.0/woke/cli/svm.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/cli/test.py` & `woke-3.2.0/woke/cli/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     coverage: bool,
     pytest_args: Tuple[str, ...],
 ) -> None:
     """Execute Woke tests using pytest."""
     import pytest
 
     from woke.config import WokeConfig
-    from woke.development.globals import set_config
+    from woke.development.globals import chain_interfaces_manager, set_config
     from woke.testing.pytest_plugin import PytestWokePlugin
 
     config = WokeConfig()
     config.load_configs()  # load ~/.woke/config.toml and ./woke.toml
 
     set_config(config)
 
@@ -78,8 +78,10 @@
 
         coverage_handler = get_coverage_handler()
         assert coverage_handler is not None
 
         c = export_merged_ide_coverage([coverage_handler.get_contract_ide_coverage()])
         write_coverage(c, config.project_root_path / "woke-coverage.cov")
 
+    chain_interfaces_manager.close_all()
+
     sys.exit(ret)
```

### Comparing `woke-3.1.0/woke/compiler/build_data_model.py` & `woke-3.2.0/woke/compiler/build_data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/compiler/compilation_unit.py` & `woke-3.2.0/woke/compiler/compilation_unit.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/compiler/compiler.py` & `woke-3.2.0/woke/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/compiler/solc_frontend/input_data_model.py` & `woke-3.2.0/woke/compiler/solc_frontend/input_data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/compiler/solc_frontend/output_data_model.py` & `woke-3.2.0/woke/compiler/solc_frontend/output_data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/compiler/solc_frontend/solc_runner.py` & `woke-3.2.0/woke/compiler/solc_frontend/solc_runner.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/compiler/source_path_resolver.py` & `woke-3.2.0/woke/compiler/source_path_resolver.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/compiler/source_unit_name_resolver.py` & `woke-3.2.0/woke/compiler/source_unit_name_resolver.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/config/__init__.py` & `woke-3.2.0/woke/config/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/config/data_model.py` & `woke-3.2.0/woke/config/data_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,19 +200,25 @@
     cmd: str = "anvil"
     timeout: float = 5
     anvil: AnvilConfig = Field(default_factory=AnvilConfig)
     ganache: GanacheConfig = Field(default_factory=GanacheConfig)
     hardhat: HardhatConfig = Field(default_factory=HardhatConfig)
 
 
+class DeploymentConfig(WokeConfigModel):
+    confirm_transactions: bool = True
+    silent: bool = False
+
+
 class TopLevelConfig(WokeConfigModel):
     subconfigs: List[Path] = []
     api_keys: Dict[str, str] = {}
     compiler: CompilerConfig = Field(default_factory=CompilerConfig)
     detectors: DetectorsConfig = Field(default_factory=DetectorsConfig)
     generator: GeneratorConfig = Field(default_factory=GeneratorConfig)
     lsp: LspConfig = Field(default_factory=LspConfig)
     testing: TestingConfig = Field(default_factory=TestingConfig)
+    deployment: DeploymentConfig = Field(default_factory=DeploymentConfig)
 
     @validator("subconfigs", pre=True, each_item=True)
     def set_subconfig(cls, v):
         return Path(v).resolve()
```

### Comparing `woke-3.1.0/woke/config/woke_config.py` & `woke-3.2.0/woke/config/woke_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import tomli
 
 from woke.utils import change_cwd
 
 from ..core.solidity_version import SolidityVersion
 from .data_model import (
     CompilerConfig,
+    DeploymentConfig,
     DetectorsConfig,
     GeneratorConfig,
     LspConfig,
     TestingConfig,
     TopLevelConfig,
 )
 
@@ -357,7 +358,14 @@
 
     @property
     def testing(self) -> TestingConfig:
         """
         Return testing framework-specific config options.
         """
         return self.__config.testing
+
+    @property
+    def deployment(self) -> DeploymentConfig:
+        """
+        Return deployment-specific config options.
+        """
+        return self.__config.deployment
```

### Comparing `woke-3.1.0/woke/contracts/woke/console.sol` & `woke-3.2.0/woke/contracts/woke/console.sol`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/core/solidity_version.py` & `woke-3.2.0/woke/core/solidity_version.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/deployment/__init__.py` & `woke-3.2.0/woke/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/deployment/core.py` & `woke-3.2.0/woke/deployment/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from contextlib import contextmanager
+from contextlib import contextmanager, nullcontext
 from typing import Any, Dict, Iterable, Optional, Union, cast
 
 import eth_utils
 from rich.console import Group
 from rich.pretty import pprint
 from rich.progress import BarColumn, Progress, TextColumn, TimeElapsedColumn
 from rich.prompt import Confirm
@@ -19,14 +19,15 @@
     RequestType,
     RevertToSnapshotFailedError,
     TransactionConfirmationFailedError,
     Wei,
     check_connected,
     fix_library_abi,
 )
+from woke.development.globals import chain_interfaces_manager, get_config
 from woke.development.json_rpc.communicator import JsonRpcError
 from woke.development.transactions import (
     Eip1559Transaction,
     Eip2930Transaction,
     LegacyTransaction,
     TransactionAbc,
     TransactionStatusEnum,
@@ -65,44 +66,44 @@
         if min_gas_price is not None:
             try:
                 self._chain_interface.set_min_gas_price(min_gas_price)
             except JsonRpcError:
                 pass
 
     def _connect_finalize(self) -> None:
-        pass
+        chain_interfaces_manager.close(self._chain_interface)
 
     def _update_nonce(self, address: Address, nonce: int) -> None:
         # nothing to do
         pass
 
     @check_connected
     def snapshot(self) -> str:
         snapshot_id = self._chain_interface.snapshot()
 
         self._snapshots[snapshot_id] = {
             "accounts": self._accounts.copy(),
             "default_call_account": self._default_call_account,
             "default_tx_account": self._default_tx_account,
-            "txs": dict(self._txs),
+            "txs": dict(self._txs._transactions),
             "blocks": dict(self._blocks._blocks),
         }
         return snapshot_id
 
     @check_connected
     def revert(self, snapshot_id: str) -> None:
         reverted = self._chain_interface.revert(snapshot_id)
         if not reverted:
             raise RevertToSnapshotFailedError()
 
         snapshot = self._snapshots[snapshot_id]
         self._accounts = snapshot["accounts"]
         self._default_call_account = snapshot["default_call_account"]
         self._default_tx_account = snapshot["default_tx_account"]
-        self._txs = snapshot["txs"]
+        self._txs._transactions = snapshot["txs"]
         self._blocks._blocks = snapshot["blocks"]
         del self._snapshots[snapshot_id]
 
     @property
     @check_connected
     def block_gas_limit(self) -> int:
         return self._blocks["pending"].gas_limit
@@ -286,15 +287,15 @@
         return tx
 
     def _wait_for_transaction(
         self, tx: TransactionAbc, confirmations: Optional[int]
     ) -> None:
         def get_pending_text():
             if tx.chain.chain_id in chain_explorer_urls:
-                text = f"Waiting for transaction [link={chain_explorer_urls[tx.chain.chain_id]}/tx/{tx.tx_hash}]{tx.tx_hash}[/link] to be mined\n"
+                text = f"Waiting for transaction [link={chain_explorer_urls[tx.chain.chain_id].url}/tx/{tx.tx_hash}]{tx.tx_hash}[/link] to be mined\n"
             else:
                 text = f"Waiting for transaction {tx.tx_hash} to be mined\n"
 
             t = Table("", "Set in transaction", "Current recommended")
 
             if isinstance(tx, Eip1559Transaction):
                 recommended_priority_fee = (
@@ -325,48 +326,76 @@
             return Group(text, t)
 
         if confirmations == 0:
             return
         elif confirmations is None:
             confirmations = self.default_tx_confirmations
 
-        with console.status(get_pending_text()) as status:
+        config = get_config()
+
+        ctx_manager = (
+            console.status(get_pending_text())
+            if not config.deployment.silent
+            else nullcontext()
+        )
+
+        with ctx_manager as status:
             while tx.status == TransactionStatusEnum.PENDING:
                 time.sleep(0.5)
-                status.update(get_pending_text())
+                if status is not None:
+                    status.update(get_pending_text())
 
-        if tx.chain.chain_id in chain_explorer_urls:
-            console.print(
-                f"Transaction [link={chain_explorer_urls[tx.chain.chain_id]}/tx/{tx.tx_hash}]{tx.tx_hash}[/link] mined in block {tx.block.number}"
-            )
-        else:
-            console.print(f"Transaction {tx.tx_hash} mined in block {tx.block.number}")
+        if not config.deployment.silent:
+            if tx.chain.chain_id in chain_explorer_urls:
+                console.print(
+                    f"Transaction [link={chain_explorer_urls[tx.chain.chain_id].url}/tx/{tx.tx_hash}]{tx.tx_hash}[/link] mined in block {tx.block.number}"
+                )
+            else:
+                console.print(
+                    f"Transaction {tx.tx_hash} mined in block {tx.block.number}"
+                )
 
         latest_block_number = self.chain_interface.get_block_number()
 
-        with Progress(
-            TextColumn("[progress.description]{task.description}"),
-            BarColumn(),
-            TextColumn("{task.completed} of {task.total}"),
-            TimeElapsedColumn(),
-            console=console,
-        ) as progress:
-            task_id = progress.add_task(
-                "Confirmations",
-                total=confirmations,
-                completed=(latest_block_number - tx.block.number + 1),
+        ctx_manager = (
+            Progress(
+                TextColumn("[progress.description]{task.description}"),
+                BarColumn(),
+                TextColumn("{task.completed} of {task.total}"),
+                TimeElapsedColumn(),
+                console=console,
             )
+            if not config.deployment.silent
+            else nullcontext()
+        )
+
+        with ctx_manager as progress:
+            if progress is not None:
+                task_id = progress.add_task(
+                    "Confirmations",
+                    total=confirmations,
+                    completed=(latest_block_number - tx.block.number + 1),
+                )
             while latest_block_number - tx.block.number < confirmations - 1:
                 time.sleep(1)
                 latest_block_number = self.chain_interface.get_block_number()
-                progress.update(
-                    task_id, completed=(latest_block_number - tx.block.number + 1)
-                )
+                if progress is not None:
+                    progress.update(
+                        task_id,
+                        completed=(
+                            latest_block_number - tx.block.number + 1
+                        ),  # pyright: reportUnboundVariable=false
+                    )
 
     def _confirm_transaction(self, tx: TxParams) -> None:
+        config = get_config()
+        if config.deployment.silent:
+            return
         pprint(tx, console=console, max_string=200)
-        confirm = Confirm.ask("Sign and send transaction?")
-        if not confirm:
-            raise TransactionConfirmationFailedError()
+
+        if config.deployment.confirm_transactions:
+            confirm = Confirm.ask("Sign and send transaction?")
+            if not confirm:
+                raise TransactionConfirmationFailedError()
 
 
 default_chain = Chain()
```

### Comparing `woke-3.1.0/woke/development/blocks.py` & `woke-3.2.0/woke/development/blocks.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/development/call_trace.py` & `woke-3.2.0/woke/development/call_trace.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
             value = tx_params["value"]
 
         explorer_info = None
         precompiled_info = None
         if (
             origin_fqn is None or origin_fqn not in contracts_by_fqn
         ) and tx.to is not None:
-            if tx.to.address <= Address(9):
+            if Address(0) < tx.to.address <= Address(9):
                 precompiled_info = get_precompiled_info(
                     tx.to.address, b"" if "data" not in tx_params else tx_params["data"]
                 )
             elif tx.chain._fork is not None:
                 explorer_info = get_contract_info_from_explorer(
                     tx.to.address, tx.chain.chain_id
                 )
@@ -562,15 +562,15 @@
                     fqn = get_fqn_from_address(addr, tx.block.number - 1, tx.chain)
 
                 explorer_info = None
                 precompiled_info = None
                 if fqn is None and addr != Address(
                     "0x000000000000000000636F6e736F6c652e6c6f67"
                 ):
-                    if addr <= Address(9):
+                    if Address(0) < addr <= Address(9):
                         precompiled_info = get_precompiled_info(addr, data)
                     elif tx.chain._fork is not None:
                         explorer_info = get_contract_info_from_explorer(
                             addr, tx.chain.chain_id
                         )
 
                 if fqn is None and explorer_info is None and precompiled_info is None:
```

### Comparing `woke-3.1.0/woke/development/chain_interfaces.py` & `woke-3.2.0/woke/development/chain_interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Union
 from urllib.error import URLError
 
 from typing_extensions import Literal, TypedDict
 
 from woke.config import WokeConfig
-from woke.development.globals import get_config
 from woke.utils.networking import get_free_port
 
 from .json_rpc.communicator import JsonRpcCommunicator
 
 TxParams = TypedDict(
     "TxParams",
     {
@@ -88,22 +87,21 @@
             return block_identifier
         else:
             raise TypeError("block identifier must be either int or str")
 
     @classmethod
     def launch(
         cls,
+        config: WokeConfig,
         *,
         accounts: Optional[int] = None,
         chain_id: Optional[int] = None,
         fork: Optional[str] = None,
         hardfork: Optional[str] = None,
     ) -> ChainInterfaceAbc:
-        config = get_config()
-
         if config.testing.cmd == "anvil":
             args = ["anvil"] + config.testing.anvil.cmd_args.split()
             constructor = AnvilChainInterface
         elif config.testing.cmd == "ganache":
             args = ["ganache"] + config.testing.ganache.cmd_args.split()
             constructor = GanacheChainInterface
         elif config.testing.cmd == "hardhat":
@@ -214,28 +212,31 @@
                 try:
                     process.communicate(timeout=5)
                 except subprocess.TimeoutExpired:
                     process.kill()
             raise
 
     @classmethod
-    def connect(cls, uri: str) -> ChainInterfaceAbc:
-        config = get_config()
+    def connect(cls, config: WokeConfig, uri: str) -> ChainInterfaceAbc:
         communicator = JsonRpcCommunicator(config, uri)
         communicator.__enter__()
         try:
-            client_version = communicator.send_request("web3_clientVersion").lower()
+            client_version: str = communicator.send_request(
+                "web3_clientVersion"
+            ).lower()
             if "anvil" in client_version:
                 return AnvilChainInterface(config, communicator)
             elif "hardhat" in client_version:
                 return HardhatChainInterface(config, communicator)
             elif "ethereumjs" in client_version:
                 return GanacheChainInterface(config, communicator)
-            elif "geth" in client_version:
+            elif client_version.startswith(("geth", "bor", "nitro")):
                 return GethChainInterface(config, communicator)
+            elif "hermez" in client_version:
+                return HermezChainInterface(config, communicator)
             else:
                 raise NotImplementedError(
                     f"Client version {client_version} not supported"
                 )
         except Exception:
             communicator.__exit__(None, None, None)
             raise
@@ -266,17 +267,14 @@
         return bytes.fromhex(
             self._communicator.send_request(
                 "eth_getCode",
                 [address, self._encode_block_identifier(block_identifier)],
             )[2:]
         )
 
-    def get_accounts(self) -> List[str]:
-        return self._communicator.send_request("eth_accounts")
-
     def get_coinbase(self) -> str:
         return self._communicator.send_request("eth_coinbase")
 
     def get_block(
         self, block_identifier: Union[int, str], include_transactions: bool = False
     ) -> Dict[str, Any]:
         return self._communicator.send_request(
@@ -351,22 +349,29 @@
         self, tx_hash: str, options: Optional[Dict] = None
     ) -> Dict[str, Any]:
         return self._communicator.send_request(
             "debug_traceTransaction",
             [tx_hash, options] if options is not None else [tx_hash],
         )
 
-    def debug_trace_call(self, params: TxParams, block_identifier: Union[int, str] = "latest", options: Optional[Dict] = None) -> Dict[str, Any]:
+    def debug_trace_call(
+        self,
+        params: TxParams,
+        block_identifier: Union[int, str] = "latest",
+        options: Optional[Dict] = None,
+    ) -> Dict[str, Any]:
         return self._communicator.send_request(
             "debug_traceCall",
             [
                 self._encode_tx_params(params),
                 self._encode_block_identifier(block_identifier),
                 options,
-            ] if options is not None else [
+            ]
+            if options is not None
+            else [
                 self._encode_tx_params(params),
                 self._encode_block_identifier(block_identifier),
             ],
         )
 
     def snapshot(self) -> str:
         return self._communicator.send_request("evm_snapshot")
@@ -407,14 +412,18 @@
             ],
         )
 
     def trace_transaction(self, tx_hash: str) -> List:
         return self._communicator.send_request("trace_transaction", [tx_hash])
 
     @abstractmethod
+    def get_accounts(self) -> List[str]:
+        ...
+
+    @abstractmethod
     def get_automine(self) -> bool:
         ...
 
     @abstractmethod
     def set_automine(self, value: bool) -> None:
         ...
 
@@ -456,14 +465,17 @@
 
     @abstractmethod
     def set_min_gas_price(self, value: int) -> None:
         ...
 
 
 class HardhatChainInterface(ChainInterfaceAbc):
+    def get_accounts(self) -> List[str]:
+        return self._communicator.send_request("eth_accounts")
+
     def set_balance(self, address: str, value: int) -> None:
         self._communicator.send_request("hardhat_setBalance", [address, hex(value)])
 
     def impersonate_account(self, address: str) -> None:
         self._communicator.send_request("hardhat_impersonateAccount", [address])
 
     def stop_impersonating_account(self, address: str) -> None:
@@ -508,14 +520,17 @@
         )
 
     def set_min_gas_price(self, value: int) -> None:
         self._communicator.send_request("hardhat_setMinGasPrice", [hex(value)])
 
 
 class AnvilChainInterface(ChainInterfaceAbc):
+    def get_accounts(self) -> List[str]:
+        return self._communicator.send_request("eth_accounts")
+
     def set_balance(self, address: str, value: int) -> None:
         self._communicator.send_request("anvil_setBalance", [address, hex(value)])
 
     def impersonate_account(self, address: str) -> None:
         self._communicator.send_request("anvil_impersonateAccount", [address])
 
     def stop_impersonating_account(self, address: str) -> None:
@@ -559,14 +574,17 @@
         self._communicator.send_request("anvil_setMinGasPrice", [hex(value)])
 
     def node_info(self) -> Dict[str, Any]:
         return self._communicator.send_request("anvil_nodeInfo")
 
 
 class GanacheChainInterface(ChainInterfaceAbc):
+    def get_accounts(self) -> List[str]:
+        return self._communicator.send_request("eth_accounts")
+
     def set_balance(self, address: str, value: int) -> None:
         self._communicator.send_request("evm_setAccountBalance", [address, hex(value)])
 
     def add_account(self, address: str, passphrase: str) -> bool:
         return self._communicator.send_request(
             "evm_addAccount", [address, passphrase]
         ) and self._communicator.send_request(
@@ -612,14 +630,17 @@
         )
 
     def set_min_gas_price(self, value: int) -> None:
         self._communicator.send_request("miner_setGasPrice", [hex(value)])
 
 
 class GethChainInterface(ChainInterfaceAbc):
+    def get_accounts(self) -> List[str]:
+        return self._communicator.send_request("eth_accounts")
+
     def get_automine(self) -> bool:
         raise NotImplementedError("Geth does not support automine")
 
     def set_automine(self, value: bool) -> None:
         raise NotImplementedError("Geth does not support automine")
 
     def reset(self, options: Optional[Dict] = None) -> None:
@@ -649,7 +670,54 @@
     def set_next_block_base_fee_per_gas(self, value: int) -> None:
         raise NotImplementedError(
             "Geth does not support setting next block base fee per gas"
         )
 
     def set_min_gas_price(self, value: int) -> None:
         raise NotImplementedError("Geth does not support setting min gas price")
+
+
+class HermezChainInterface(ChainInterfaceAbc):
+    def get_accounts(self) -> List[str]:
+        return []
+
+    def get_automine(self) -> bool:
+        raise NotImplementedError("Hermez does not support automine")
+
+    def set_automine(self, value: bool) -> None:
+        raise NotImplementedError("Hermez does not support automine")
+
+    def reset(self, options: Optional[Dict] = None) -> None:
+        raise NotImplementedError("Hermez does not support resetting the chain")
+
+    def set_coinbase(self, address: str) -> None:
+        raise NotImplementedError("Hermez does not support setting coinbase")
+
+    def set_balance(self, address: str, value: int) -> None:
+        raise NotImplementedError("Hermez does not support setting balance")
+
+    def set_block_gas_limit(self, gas_limit: int) -> None:
+        raise NotImplementedError("Hermez does not support setting block gas limit")
+
+    def set_code(self, address: str, value: bytes) -> None:
+        raise NotImplementedError("Hermez does not support setting code")
+
+    def set_nonce(self, address: str, value: int) -> None:
+        raise NotImplementedError("Hermez does not support setting nonce")
+
+    def set_next_block_timestamp(self, timestamp: int) -> None:
+        raise NotImplementedError(
+            "Hermez does not support setting next block timestamp"
+        )
+
+    def send_unsigned_transaction(self, params: TxParams) -> str:
+        raise NotImplementedError(
+            "Hermez does not support sending unsigned transactions"
+        )
+
+    def set_next_block_base_fee_per_gas(self, value: int) -> None:
+        raise NotImplementedError(
+            "Hermez does not support setting next block base fee per gas"
+        )
+
+    def set_min_gas_price(self, value: int) -> None:
+        raise NotImplementedError("Hermez does not support setting min gas price")
```

### Comparing `woke-3.1.0/woke/development/constants.py` & `woke-3.2.0/woke/development/constants.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/development/core.py` & `woke-3.2.0/woke/development/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from bdb import BdbQuit
 from collections import ChainMap, defaultdict
 from contextlib import contextmanager
 from copy import deepcopy
 from enum import Enum, IntEnum
 from os import PathLike
 from pathlib import Path
-from types import MappingProxyType
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     DefaultDict,
     Dict,
     Iterable,
@@ -55,23 +54,29 @@
 from .blocks import ChainBlocks
 from .chain_interfaces import (
     AnvilChainInterface,
     ChainInterfaceAbc,
     GanacheChainInterface,
     GethChainInterface,
     HardhatChainInterface,
+    HermezChainInterface,
     TxParams,
 )
-from .globals import get_config, get_coverage_handler, get_exception_handler
+from .globals import (
+    chain_interfaces_manager,
+    get_config,
+    get_coverage_handler,
+    get_exception_handler,
+)
 from .internal import UnknownEvent, read_from_memory
 from .json_rpc.communicator import JsonRpcError
 from .primitive_types import Length, ValueRange
 
 if TYPE_CHECKING:
-    from .transactions import TransactionAbc
+    from .transactions import ChainTransactions, TransactionAbc
 
 
 # selector => (contract_fqn => pytypes_object)
 errors: Dict[bytes, Dict[str, Any]] = {}
 # selector => (contract_fqn => pytypes_object)
 events: Dict[bytes, Dict[str, Any]] = {}
 # contract_fqn => contract type
@@ -444,17 +449,20 @@
             self._chain._labels[self._address] = value
 
     @property
     def balance(self) -> Wei:
         return Wei(self._chain.chain_interface.get_balance(str(self._address)))
 
     @balance.setter
-    def balance(self, value: int) -> None:
+    def balance(self, value: Union[int, str]) -> None:
+        if isinstance(value, str):
+            value = Wei.from_str(value)
+
         if not isinstance(value, int):
-            raise TypeError("value must be an integer")
+            raise TypeError("value must be an integer or string")
         if value < 0:
             raise ValueError("value must be non-negative")
         self._chain.chain_interface.set_balance(str(self.address), value)
 
     @property
     def code(self) -> bytes:
         return self._chain.chain_interface.get_code(str(self._address))
@@ -1032,15 +1040,15 @@
     _default_access_list_account: Optional[Account]
     _default_tx_type: int
     _default_tx_confirmations: int
     _deployed_libraries: DefaultDict[bytes, List[Library]]
     _single_source_errors: Set[bytes]
     _snapshots: Dict[str, Dict]
     _blocks: ChainBlocks
-    _txs: Dict[str, TransactionAbc]
+    _txs: ChainTransactions
     _chain_id: int
     _labels: Dict[Address, str]
     _private_keys: Dict[Address, bytes]
     _require_signed_txs: bool
     _fork: Optional[str]
     _debug_trace_call_supported: bool
 
@@ -1151,46 +1159,33 @@
             raise AlreadyConnectedError("Already connected to a chain")
 
         if isinstance(min_gas_price, str):
             min_gas_price = Wei.from_str(min_gas_price)
         if isinstance(block_base_fee_per_gas, str):
             block_base_fee_per_gas = Wei.from_str(block_base_fee_per_gas)
 
-        if uri is None:
-            self._chain_interface = ChainInterfaceAbc.launch(
-                accounts=accounts,
-                chain_id=chain_id,
-                fork=fork,
-                hardfork=hardfork,
-            )
-        else:
-            if (
-                accounts is not None
-                or chain_id is not None
-                or fork is not None
-                or hardfork is not None
-            ):
-                raise ValueError(
-                    "Cannot specify accounts, chain_id, fork or hardfork when connecting to a running chain"
-                )
-            self._chain_interface = ChainInterfaceAbc.connect(uri)
+        self._chain_interface = chain_interfaces_manager.get_or_create(
+            uri, accounts=accounts, chain_id=chain_id, fork=fork, hardfork=hardfork
+        )
 
         try:
             self._connected = True
 
             try:
                 self._chain_interface.debug_trace_call(
                     {
                         "type": 0,
                     }
                 )
                 self._debug_trace_call_supported = True
             except JsonRpcError:
                 self._debug_trace_call_supported = False
 
+            self._chain_id = self._chain_interface.get_chain_id()
+
             # determine the chain hardfork to set the default tx type
             if isinstance(self._chain_interface, AnvilChainInterface):
                 hardfork = self._chain_interface.node_info()["hardFork"]
                 if hardfork in {
                     "FRONTIER",
                     "HOMESTEAD",
                     "TANGERINE",
@@ -1203,35 +1198,45 @@
                 }:
                     self._default_tx_type = 0
                 elif hardfork == "BERLIN":
                     self._default_tx_type = 1
                 else:
                     self._default_tx_type = 2
             elif isinstance(
-                self._chain_interface, (GethChainInterface, HardhatChainInterface)
+                self._chain_interface,
+                (GethChainInterface, HardhatChainInterface, HermezChainInterface),
             ):
-                try:
-                    self._chain_interface.call(
-                        {
-                            "type": 2,
-                            "maxPriorityFeePerGas": 0,
-                        }
-                    )
-                    self._default_tx_type = 2
-                except JsonRpcError:
+                if self._chain_id in {56, 97}:
+                    # BSC clients do not fail on the calls below
+                    self._default_tx_type = 1
+                else:
+                    # TODO this is not the correct flow for Hermez:
+                    # EIP-1559 txs should be supported
+                    # access lists should not be supported
+                    # `type` field in txs should not be used
+                    # because Hermez does not implement eth_maxPriorityFeePerGas, fallback to legacy txs
                     try:
                         self._chain_interface.call(
                             {
-                                "type": 1,
-                                "accessList": [],
+                                "type": 2,
+                                "maxPriorityFeePerGas": 0,
                             }
                         )
-                        self._default_tx_type = 1
+                        self._default_tx_type = 2
                     except JsonRpcError:
-                        self._default_tx_type = 0
+                        try:
+                            self._chain_interface.call(
+                                {
+                                    "type": 1,
+                                    "accessList": [],
+                                }
+                            )
+                            self._default_tx_type = 1
+                        except JsonRpcError:
+                            self._default_tx_type = 0
             elif isinstance(self._chain_interface, GanacheChainInterface):
                 self._default_tx_type = 0
             else:
                 raise NotImplementedError(
                     f"Unknown chain interface type: {type(self._chain_interface)}"
                 )
 
@@ -1241,29 +1246,31 @@
                 try:
                     self._chain_interface.set_next_block_base_fee_per_gas(
                         block_base_fee_per_gas
                     )
                 except JsonRpcError:
                     pass
 
+            from .transactions import ChainTransactions
+
+            self._txs = ChainTransactions(self)
+
             self._accounts = [
                 Account(acc, self) for acc in self._chain_interface.get_accounts()
             ]
             self._accounts_set = set(self._accounts)
-            self._chain_id = self._chain_interface.get_chain_id()
             self._snapshots = {}
             self._deployed_libraries = defaultdict(list)
             self._default_call_account = (
                 self._accounts[0] if len(self._accounts) > 0 else None
             )
             self._default_tx_account = None
             self._default_estimate_account = None
             self._default_access_list_account = None
             self._default_tx_confirmations = 1
-            self._txs = {}
             self._blocks = ChainBlocks(self)
             self._labels = {}
             self._private_keys = {}
             self._fork = fork
 
             self._single_source_errors = {
                 selector
@@ -1280,15 +1287,14 @@
             if not isinstance(e, BdbQuit):
                 exception_handler = get_exception_handler()
                 if exception_handler is not None:
                     exception_handler(e)
                 raise
         finally:
             self._connect_finalize()
-            self._chain_interface.close()
             self._connected = False
 
     @property
     def connected(self) -> bool:
         return self._connected
 
     @property
@@ -1304,16 +1310,16 @@
     @property
     @check_connected
     def accounts(self) -> Tuple[Account, ...]:
         return tuple(self._accounts)
 
     @property
     @check_connected
-    def txs(self) -> MappingProxyType[str, TransactionAbc]:
-        return MappingProxyType(self._txs)
+    def txs(self) -> ChainTransactions:
+        return self._txs
 
     @property
     @check_connected
     def default_call_account(self) -> Optional[Account]:
         return self._default_call_account
 
     @default_call_account.setter
@@ -1689,15 +1695,15 @@
             if selector.startswith("0x"):
                 selector = selector[2:]
             selector = bytes.fromhex(selector.zfill(64))
 
             if selector not in events:
                 continue
 
-            if len(events[selector]) > 1:
+            if len({source for source in events[selector].values()}) > 1:
                 non_unique = True
                 break
 
         if non_unique:
             debug_trace = self._chain_interface.debug_trace_transaction(
                 tx.tx_hash, {"enableMemory": True}
             )
@@ -1736,15 +1742,15 @@
 
             selector = topics[0]
 
             if selector not in events:
                 generated_events.append(UnknownEvent(topics, data))
                 continue
 
-            if len(events[selector]) > 1:
+            if len({source for source in events[selector].values()}) > 1:
                 assert traced_selector == selector
 
                 if fqn is None:
                     generated_events.append(UnknownEvent(topics, data))
                     continue
 
                 found = False
@@ -1863,25 +1869,31 @@
             revert_data = e.data["data"]
         elif (
             isinstance(self._chain_interface, HardhatChainInterface)
             and e.data["code"] == -32603
         ):
             revert_data = e.data["data"]["data"]
         else:
+            # Hermez does not provide revert data for estimate
             raise e from None
 
         if revert_data.startswith("0x"):
             revert_data = revert_data[2:]
 
         self._process_revert_data(None, bytes.fromhex(revert_data))
 
     def _send_transaction(self, tx_params: TxParams) -> str:
         assert "from" in tx_params
         assert "nonce" in tx_params
 
+        if self._chain_id in {56, 97}:
+            # BSC doesn't support access lists and tx type
+            del tx_params["type"]
+            del tx_params["accessList"]
+
         self._confirm_transaction(tx_params)
 
         if self.require_signed_txs:
             key = self._private_keys.get(Address(tx_params["from"]), None)
             tx_params["from"] = eth_utils.to_checksum_address(tx_params["from"])
 
             if "to" in tx_params:
@@ -2037,15 +2049,14 @@
         tx = tx_type(
             tx_hash,
             tx_params,
             abi,
             return_type,
             self,
         )
-        self._txs[tx_hash] = tx
 
         coverage_handler = get_coverage_handler()
         if coverage_handler is not None:
             tx._fetch_debug_trace_transaction()
             coverage_handler.add_coverage(tx_params, self, tx._debug_trace_transaction)
 
         if confirmations != 0:
@@ -2128,14 +2139,18 @@
     metadata = code[-53:]
     if metadata in contracts_by_metadata:
         return contracts_by_metadata[metadata]
     else:
         return None
 
 
+def get_contract_from_fqn(fqn: str):
+    return contracts_by_fqn[fqn]
+
+
 def process_debug_trace_for_fqn_overrides(
     tx: TransactionAbc,
     debug_trace: Dict[str, Any],
     fqn_overrides: ChainMap[Address, Optional[str]],
 ) -> None:
     if tx.status == 0:
         return
```

### Comparing `woke-3.1.0/woke/development/hardhat_console.py` & `woke-3.2.0/woke/development/hardhat_console.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/development/internal.py` & `woke-3.2.0/woke/development/internal.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/development/json_rpc/communicator.py` & `woke-3.2.0/woke/development/json_rpc/communicator.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/development/json_rpc/http.py` & `woke-3.2.0/woke/development/json_rpc/http.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/development/json_rpc/ipc.py` & `woke-3.2.0/woke/development/json_rpc/ipc.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/development/json_rpc/websocket.py` & `woke-3.2.0/woke/development/json_rpc/websocket.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/development/primitive_types.py` & `woke-3.2.0/woke/development/primitive_types.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/development/pytypes_generator.py` & `woke-3.2.0/woke/development/pytypes_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,15 @@
     __errors_index: Dict[bytes, Dict[str, Any]]
     __events_index: Dict[bytes, Dict[str, Any]]
     __contracts_by_metadata_index: Dict[bytes, str]
     __contracts_inheritance_index: Dict[str, Tuple[str, ...]]
     __contracts_revert_index: Dict[str, Set[int]]
     __creation_code_index: List[Tuple[Tuple[Tuple[int, bytes], ...], str]]
     __line_indexes: Dict[Path, List[Tuple[bytes, int]]]
+    __tx_return_types: DefaultDict[str, Dict[str, str]]
 
     def __init__(self, config: WokeConfig, return_tx_obj: bool):
         self.__config = config
         self.__return_tx_obj = return_tx_obj
         self.__source_unit_types = ""
         self.__already_generated_contracts = set()
         self.__source_units = {}
@@ -190,14 +191,15 @@
         self.__errors_index = {}
         self.__events_index = {}
         self.__contracts_by_metadata_index = {}
         self.__contracts_inheritance_index = {}
         self.__contracts_revert_index = {}
         self.__creation_code_index = []
         self.__line_indexes = {}
+        self.__tx_return_types = defaultdict(dict)
 
         # built-in Error(str) and Panic(uint256) errors
         error_abi = {
             "name": "Error",
             "type": "error",
             "inputs": [{"internalType": "string", "name": "message", "type": "string"}],
         }
@@ -601,17 +603,20 @@
                         break
                 assert (
                     event_decl is not None
                 ), f"Could not find event {item['name']} in contract {fqn} or its bases"
 
                 if selector not in self.__events_index:
                     self.__events_index[selector] = {}
+                event_module_name = "pytypes." + _make_path_alphanum(
+                    event_decl.parent.parent.source_unit_name[:-3]
+                ).replace("/", ".")
                 self.__events_index[selector][fqn] = (
-                    module_name,
-                    (self.get_name(contract), self.get_name(event_decl)),
+                    event_module_name,
+                    (self.get_name(event_decl.parent), self.get_name(event_decl)),
                 )
             elif item["type"] in {"constructor", "fallback", "receive"}:
                 abi_by_selector[item["type"]] = item
             else:
                 raise Exception(f"Unexpected ABI item type: {item['type']}")
         self.add_str_to_types(1, f"_abi = {abi_by_selector}", 1)
         self.add_str_to_types(
@@ -1270,14 +1275,19 @@
         if len(returns) == 0:
             return_types = "NoneType"
         elif len(returns) == 1:
             return_types = returns[0][0]
         else:
             return_types = f"Tuple[{', '.join(map(itemgetter(0), returns))}]"
 
+        assert isinstance(declaration.parent, ContractDefinition)
+        self.__tx_return_types[self.get_name(declaration.parent)][
+            self.get_name(declaration)
+        ] = return_types
+
         assert declaration.function_selector is not None
         fn_selector = declaration.function_selector.hex()
         self.add_str_to_types(
             2,
             f'return self._execute(self.chain, request_type, "{fn_selector}", [{", ".join(map(itemgetter(0), param_names))}], True if request_type == "tx" else False, {return_types}, from_, to if to is not None else str(self.address), value, gas_limit, gas_price, max_fee_per_gas, max_priority_fee_per_gas, access_list, type, block, confirmations)',
             2,
         )
@@ -1452,14 +1462,21 @@
                     )
 
         for fn_name, selector in selector_assignments:
             self.add_str_to_types(
                 0, f"{self.get_name(contract)}.{fn_name}.selector = {selector}", 1
             )
 
+        for contract_name in self.__tx_return_types.keys():
+            for fn_name, return_type in self.__tx_return_types[contract_name].items():
+                self.add_str_to_types(
+                    0, f"{contract_name}.{fn_name}.return_type = {return_type}", 1
+                )
+        self.__tx_return_types.clear()
+
     def generate_types_source_unit(self, unit: SourceUnit) -> None:
         self.generate_types_struct(unit.structs, 0)
         self.generate_types_enum(unit.enums, 0)
         self.generate_types_error(unit.errors, 0)
         for contract in unit.contracts:
             self.generate_types_contract(contract)
```

### Comparing `woke-3.1.0/woke/development/transactions.py` & `woke-3.2.0/woke/development/transactions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import functools
+import importlib
 import inspect
 from abc import ABC, abstractmethod
 from contextlib import AbstractContextManager, contextmanager
 from dataclasses import dataclass, field, fields
 from enum import IntEnum
 from typing import (
     TYPE_CHECKING,
@@ -24,17 +25,26 @@
 
 from .call_trace import CallTrace
 from .chain_interfaces import (
     AnvilChainInterface,
     GanacheChainInterface,
     GethChainInterface,
     HardhatChainInterface,
+    HermezChainInterface,
     TxParams,
 )
-from .core import Account, Chain, Wei
+from .core import (
+    Account,
+    Address,
+    Chain,
+    Wei,
+    get_contract_from_fqn,
+    get_fqn_from_address,
+    get_fqn_from_creation_code,
+)
 from .internal import UnknownEvent, read_from_memory
 from .json_rpc import JsonRpcError
 
 T = TypeVar("T")
 
 
 class TransactionStatusEnum(IntEnum):
@@ -66,14 +76,103 @@
             self.wait()
         assert self._tx_receipt is not None
         return f(self)
 
     return wrapper
 
 
+class ChainTransactions:
+    _chain: Chain
+    _transactions: Dict[str, TransactionAbc]
+
+    def __init__(self, chain: Chain):
+        self._chain = chain
+        self._transactions = {}
+
+    def __getitem__(self, key: str) -> TransactionAbc:
+        if not key.startswith("0x"):
+            key = "0x" + key
+        key = key.lower()
+        if key in self._transactions:
+            return self._transactions[key]
+
+        tx_data = self._chain.chain_interface.get_transaction(key)
+        type = int(tx_data["type"], 16)
+
+        tx_params: TxParams = {
+            "nonce": int(tx_data["nonce"], 16),
+            "from": tx_data["from"],
+            "gas": int(tx_data["gas"], 16),
+            "value": int(tx_data["value"], 16),
+            "data": bytes.fromhex(tx_data["input"][2:]),
+        }
+
+        if "to" in tx_data and tx_data["to"] is not None:
+            tx_params["to"] = tx_data["to"]
+            try:
+                fqn = get_fqn_from_address(
+                    Address(tx_params["to"]),
+                    int(tx_data["blockNumber"], 16) - 1
+                    if "blockNumber" in tx_data
+                    else "latest",
+                    self._chain,
+                )
+                module_name, attrs = get_contract_from_fqn(fqn)
+                obj = getattr(importlib.import_module(module_name), attrs[0])
+                for attr in attrs[1:]:
+                    obj = getattr(obj, attr)
+                selector = tx_params["data"][:4]
+                abi = obj._abi[selector]
+                method = next(
+                    getattr(obj, m)
+                    for m in dir(obj)
+                    if hasattr(getattr(obj, m), "selector")
+                    and getattr(obj, m).selector == selector
+                )
+                return_type = method.return_type
+            except (KeyError, StopIteration):
+                abi = None
+                return_type = bytearray
+        else:
+            try:
+                fqn = get_fqn_from_creation_code(tx_params["data"])[0]
+                module_name, attrs = get_contract_from_fqn(fqn)
+                obj = getattr(importlib.import_module(module_name), attrs[0])
+                for attr in attrs[1:]:
+                    obj = getattr(obj, attr)
+                if "constructor" in obj._abi:
+                    abi = obj._abi["constructor"]
+                else:
+                    abi = None
+                return_type = obj
+            except (KeyError, ValueError):
+                abi = None
+                return_type = Account
+
+        if type == 0:
+            tx_params["gasPrice"] = int(tx_data["gasPrice"], 16)
+            tx = LegacyTransaction(key, tx_params, abi, return_type, self._chain)
+        elif type == 1:
+            tx_params["gasPrice"] = int(tx_data["gasPrice"], 16)
+            tx_params["accessList"] = tx_data["accessList"]
+            tx_params["chainId"] = 1
+            tx = Eip2930Transaction(key, tx_params, abi, return_type, self._chain)
+        elif type == 2:
+            tx_params["maxFeePerGas"] = int(tx_data["maxFeePerGas"], 16)
+            tx_params["maxPriorityFeePerGas"] = int(tx_data["maxPriorityFeePerGas"], 16)
+            tx_params["accessList"] = tx_data["accessList"]
+            tx_params["chainId"] = 2
+            tx = Eip1559Transaction(key, tx_params, abi, return_type, self._chain)
+        else:
+            raise ValueError(f"Unknown transaction type {type}")
+
+        self._transactions[key] = tx
+        return tx
+
+
 class TransactionAbc(ABC, Generic[T]):
     _tx_hash: str
     _tx_params: TxParams
     _chain: Chain
     _abi: Optional[Dict]
     _return_type: Type
     _tx_data: Optional[Dict[str, Any]]
@@ -233,15 +332,15 @@
             chain_interface, (GanacheChainInterface, HardhatChainInterface)
         ):
             self._fetch_debug_trace_transaction()
             assert self._debug_trace_transaction is not None
             return self._chain._process_console_logs_from_debug_trace(
                 self._debug_trace_transaction
             )
-        elif isinstance(chain_interface, GethChainInterface):
+        elif isinstance(chain_interface, (GethChainInterface, HermezChainInterface)):
             try:
                 self._fetch_trace_transaction()
                 assert self._trace_transaction is not None
                 return self._chain._process_console_logs(self._trace_transaction)
             except JsonRpcError as e:
                 # TODO make assertions about error.code?
                 try:
@@ -338,15 +437,15 @@
                 length = int(trace["stack"][-2], 16)
 
                 revert_data = bytes(read_from_memory(offset, length, trace["memory"]))
         elif isinstance(chain_interface, HardhatChainInterface):
             self._fetch_debug_trace_transaction()
             assert self._debug_trace_transaction is not None
             revert_data = bytes.fromhex(self._debug_trace_transaction["returnValue"])  # type: ignore
-        elif isinstance(chain_interface, GethChainInterface):
+        elif isinstance(chain_interface, (GethChainInterface, HermezChainInterface)):
             try:
                 self._fetch_trace_transaction()
                 assert self._trace_transaction is not None
                 revert_data = bytes.fromhex(
                     self._trace_transaction[0]["result"]["output"][2:]
                 )
             except JsonRpcError as e:
@@ -366,28 +465,47 @@
         self._raw_error = UnknownTransactionRevertedError(revert_data)
         self._raw_error.tx = self
         return self._raw_error
 
     @property
     @_fetch_tx_receipt
     def return_value(self) -> T:
+        raw_value = self.raw_return_value
+
+        if self._return_type is type(None):
+            return None
+
+        if isinstance(raw_value, Account):
+            return self._return_type(raw_value.address, self._chain)
+        elif isinstance(raw_value, bytearray):
+            if self._abi is None:
+                return self._return_type(raw_value)
+
+            return self._chain._process_return_data(
+                self, bytes(raw_value), self._abi, self._return_type
+            )
+        else:
+            raise TypeError(
+                f"Unexpected return type from transaction {self.tx_hash}: {type(raw_value)}"
+            )
+
+    @property
+    @_fetch_tx_receipt
+    def raw_return_value(self) -> Union[Account, bytearray]:
         if self.status != TransactionStatusEnum.SUCCESS:
             e = self.error
             assert e is not None
             raise e
 
         assert self._tx_receipt is not None
         if (
             "contractAddress" in self._tx_receipt
             and self._tx_receipt["contractAddress"] is not None
         ):
-            return self._return_type(self._tx_receipt["contractAddress"], self._chain)
-
-        if self._return_type is type(None):
-            return None
+            return Account(self._tx_receipt["contractAddress"], self._chain)
 
         chain_interface = self._chain.chain_interface
         if isinstance(chain_interface, AnvilChainInterface):
             self._fetch_trace_transaction()
             assert self._trace_transaction is not None
             output = bytes.fromhex(self._trace_transaction[0]["result"]["output"][2:])
         elif isinstance(chain_interface, GanacheChainInterface):
@@ -402,15 +520,15 @@
                 length = int(trace["stack"][-2], 16)
 
                 output = read_from_memory(offset, length, trace["memory"])
         elif isinstance(chain_interface, HardhatChainInterface):
             self._fetch_debug_trace_transaction()
             assert self._debug_trace_transaction is not None
             output = bytes.fromhex(self._debug_trace_transaction["returnValue"])  # type: ignore
-        elif isinstance(chain_interface, GethChainInterface):
+        elif isinstance(chain_interface, (GethChainInterface, HermezChainInterface)):
             try:
                 self._fetch_trace_transaction()
                 assert self._trace_transaction is not None
                 output = bytes.fromhex(
                     self._trace_transaction[0]["result"]["output"][2:]
                 )
             except JsonRpcError as e:
@@ -423,20 +541,15 @@
                     # TODO make assertions about error.code?
                     raise RuntimeError(
                         f"Could not get return value for transaction {self.tx_hash} as trace_transaction and debug_trace_transaction are both unavailable"
                     )
         else:
             raise NotImplementedError
 
-        if self._abi is None:
-            return self._return_type(output)
-
-        return self._chain._process_return_data(
-            self, output, self._abi, self._return_type
-        )
+        return bytearray(output)
 
     @property
     @_fetch_tx_receipt
     def call_trace(self) -> CallTrace:
         if self._debug_trace_transaction is None:
             self._fetch_debug_trace_transaction()
         assert self._debug_trace_transaction is not None
```

### Comparing `woke-3.1.0/woke/lsp/commands/generate_control_flow_graph.py` & `woke-3.2.0/woke/lsp/commands/generate_control_flow_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/commands/generate_imports_graph.py` & `woke-3.2.0/woke/lsp/commands/generate_imports_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/commands/generate_inheritance_graph.py` & `woke-3.2.0/woke/lsp/commands/generate_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/commands/generate_linearized_inheritance_graph.py` & `woke-3.2.0/woke/lsp/commands/generate_linearized_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/common_structures.py` & `woke-3.2.0/woke/lsp/common_structures.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/context.py` & `woke-3.2.0/woke/lsp/context.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/document_sync.py` & `woke-3.2.0/woke/lsp/document_sync.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/features/code_lens.py` & `woke-3.2.0/woke/lsp/features/code_lens.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/features/completion.py` & `woke-3.2.0/woke/lsp/features/completion.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/features/definition.py` & `woke-3.2.0/woke/lsp/features/definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/features/diagnostic.py` & `woke-3.2.0/woke/lsp/features/diagnostic.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/features/document_link.py` & `woke-3.2.0/woke/lsp/features/document_link.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/features/document_symbol.py` & `woke-3.2.0/woke/lsp/features/document_symbol.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/features/hover.py` & `woke-3.2.0/woke/lsp/features/hover.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/features/implementation.py` & `woke-3.2.0/woke/lsp/features/implementation.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/features/references.py` & `woke-3.2.0/woke/lsp/features/references.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/features/rename.py` & `woke-3.2.0/woke/lsp/features/rename.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/features/type_definition.py` & `woke-3.2.0/woke/lsp/features/type_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/features/type_hierarchy.py` & `woke-3.2.0/woke/lsp/features/type_hierarchy.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/lsp_compiler.py` & `woke-3.2.0/woke/lsp/lsp_compiler.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/methods.py` & `woke-3.2.0/woke/lsp/methods.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/protocol_structures.py` & `woke-3.2.0/woke/lsp/protocol_structures.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/rpc_protocol.py` & `woke-3.2.0/woke/lsp/rpc_protocol.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/server.py` & `woke-3.2.0/woke/lsp/server.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/server_capabilities.py` & `woke-3.2.0/woke/lsp/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/lsp/utils/position.py` & `woke-3.2.0/woke/lsp/utils/position.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/regex_parser/solidity_import.py` & `woke-3.2.0/woke/regex_parser/solidity_import.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/regex_parser/solidity_parser.py` & `woke-3.2.0/woke/regex_parser/solidity_parser.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/svm/abc.py` & `woke-3.2.0/woke/svm/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/svm/svm.py` & `woke-3.2.0/woke/svm/svm.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/testing/__init__.py` & `woke-3.2.0/woke/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/testing/core.py` & `woke-3.2.0/woke/testing/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     Address,
     RequestType,
     RevertToSnapshotFailedError,
     Wei,
     check_connected,
     fix_library_abi,
 )
+from woke.development.globals import chain_interfaces_manager
 from woke.development.json_rpc import JsonRpcError
 
 from ..development.chain_interfaces import AnvilChainInterface
 from ..development.transactions import TransactionAbc, TransactionStatusEnum
 from ..utils.keyed_default_dict import KeyedDefaultDict
 
 
@@ -82,29 +83,30 @@
             except JsonRpcError:
                 pass
         else:
             self.gas_price = self._chain_interface.get_gas_price()
 
     def _connect_finalize(self) -> None:
         connected_chains.remove(self)
+        chain_interfaces_manager.free(self._chain_interface)
 
     def _update_nonce(self, address: Address, nonce: int) -> None:
         self._nonces[address] = nonce
 
     @check_connected
     def snapshot(self) -> str:
         snapshot_id = self._chain_interface.snapshot()
 
         self._snapshots[snapshot_id] = {
             "nonces": self._nonces.copy(),
             "accounts": self._accounts.copy(),
             "default_call_account": self._default_call_account,
             "default_tx_account": self._default_tx_account,
             "block_gas_limit": self._block_gas_limit,
-            "txs": dict(self._txs),
+            "txs": dict(self._txs._transactions),
             "blocks": dict(self._blocks._blocks),
         }
         return snapshot_id
 
     @check_connected
     def revert(self, snapshot_id: str) -> None:
         reverted = self._chain_interface.revert(snapshot_id)
@@ -113,15 +115,15 @@
 
         snapshot = self._snapshots[snapshot_id]
         self._nonces = snapshot["nonces"]
         self._accounts = snapshot["accounts"]
         self._default_call_account = snapshot["default_call_account"]
         self._default_tx_account = snapshot["default_tx_account"]
         self._block_gas_limit = snapshot["block_gas_limit"]
-        self._txs = snapshot["txs"]
+        self._txs._transactions = snapshot["txs"]
         self._blocks._blocks = snapshot["blocks"]
         del self._snapshots[snapshot_id]
 
     @property
     @check_connected
     def block_gas_limit(self) -> int:
         return self._block_gas_limit
```

### Comparing `woke-3.1.0/woke/testing/coverage.py` & `woke-3.2.0/woke/testing/coverage.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/testing/fuzzing/fuzz_test.py` & `woke-3.2.0/woke/testing/fuzzing/fuzz_test.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/testing/fuzzing/fuzzer.py` & `woke-3.2.0/woke/testing/fuzzing/fuzzer.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from rich.traceback import Traceback
 from tblib import pickling_support
 
 from woke.cli.console import console
 from woke.config import WokeConfig
 from woke.development.globals import (
     attach_debugger,
+    chain_interfaces_manager,
     set_coverage_handler,
     set_exception_handler,
 )
 from woke.testing.coverage import (
     CoverageHandler,
     IdeFunctionCoverageRecord,
     IdePosition,
@@ -68,15 +69,22 @@
     coverage: Optional[CoverageHandler],
 ):
     def exception_handler(e: Exception) -> None:
         for ctx_manager in ctx_managers:
             ctx_manager.__exit__(None, None, None)
         ctx_managers.clear()
 
-        err_child_conn.send(pickle.dumps(sys.exc_info()))
+        exc_info = sys.exc_info()
+        try:
+            pickled = pickle.dumps(exc_info)
+        except Exception:
+            pickled = pickle.dumps(
+                (exc_info[0], Exception(repr(exc_info[1])), exc_info[2])
+            )
+        err_child_conn.send(pickled)
         finished_event.set()
 
         try:
             attach: bool = err_child_conn.recv()
             if attach:
                 sys.stdin = os.fdopen(0)
                 attach_debugger(e)
@@ -124,14 +132,15 @@
             err_child_conn,
             cov_child_conn,
             coverage,
         )
     except Exception:
         pass
     finally:
+        chain_interfaces_manager.close_all()
         for ctx_manager in ctx_managers:
             ctx_manager.__exit__(None, None, None)
 
 
 def _compute_coverage_per_function(
     ide_cov: Dict[str, List[Dict[str, Any]]]
 ) -> Dict[str, int]:
@@ -150,14 +159,15 @@
                 funcs_cov[fn_rec["name"]] = fn_rec["coverageHits"]
 
     return funcs_cov
 
 
 def fuzz(
     config: WokeConfig,
+    func_name: str,
     fuzz_test: types.FunctionType,
     process_count: int,
     seeds: Iterable[bytes],
     logs_dir: Path,
     passive: bool,
     cov_proc_num: int,
     verbose_coverage: bool,
@@ -177,15 +187,15 @@
     for i, seed in zip(range(process_count), random_seeds):
         console.print(f"Using seed '{seed.hex()}' for process #{i}")
         finished_event = multiprocessing.Event()
         err_parent_conn, err_child_con = multiprocessing.Pipe()
         cov_parent_conn, cov_child_con = multiprocessing.Pipe()
 
         log_path = logs_dir / sanitize_filename(
-            f"{fuzz_test.__module__}.{fuzz_test.__name__}_{i}.ansi"
+            f"{fuzz_test.__module__}.{func_name}_{i}.ansi"
         )
 
         p = multiprocessing.Process(
             target=_run,
             args=(
                 fuzz_test,
                 i,
@@ -197,103 +207,115 @@
                 cov_child_con,
                 empty_coverage if i < cov_proc_num else None,
             ),
         )
         processes[i] = (p, finished_event, err_parent_conn, cov_parent_conn)
         p.start()
 
-    with rich.progress.Progress(
-        rich.progress.SpinnerColumn(finished_text="[green]⠿"),
-        "[progress.description][yellow]{task.description}, "
-        "[green]{task.fields[thr_rem]}[yellow] "
-        "processes remaining{task.fields[coverage_info]}",
-    ) as progress:
-        exported_coverages: Dict[
-            int, Dict[Path, Dict[IdePosition, IdeFunctionCoverageRecord]]
-        ] = {}
-
-        if passive:
-            progress.stop()
-        task = progress.add_task(
-            "Fuzzing", thr_rem=len(processes), coverage_info="", total=1
-        )
+    try:
+        with rich.progress.Progress(
+            rich.progress.SpinnerColumn(finished_text="[green]⠿"),
+            "[progress.description][yellow]{task.description}, "
+            "[green]{task.fields[thr_rem]}[yellow] "
+            "processes remaining{task.fields[coverage_info]}",
+        ) as progress:
+            exported_coverages: Dict[
+                int, Dict[Path, Dict[IdePosition, IdeFunctionCoverageRecord]]
+            ] = {}
+
+            if passive:
+                progress.stop()
+            task = progress.add_task(
+                "Fuzzing", thr_rem=len(processes), coverage_info="", total=1
+            )
+
+            while len(processes):
+                to_be_removed = []
+                for i, (p, e, err_parent_conn, cov_parent_conn) in processes.items():
+                    finished = e.wait(0.125)
+                    if finished:
+                        to_be_removed.append(i)
+
+                        exception_info = err_parent_conn.recv()
+                        if exception_info is not None:
+                            exception_info = pickle.loads(exception_info)
+
+                        if exception_info is not None:
+                            if not passive or i == 0:
+                                tb = Traceback.from_exception(
+                                    exception_info[0],
+                                    exception_info[1],
+                                    exception_info[2],
+                                )
 
-        while len(processes):
-            to_be_removed = []
-            for i, (p, e, err_parent_conn, cov_parent_conn) in processes.items():
-                finished = e.wait(0.125)
-                if finished:
-                    to_be_removed.append(i)
-
-                    exception_info = err_parent_conn.recv()
-                    if exception_info is not None:
-                        exception_info = pickle.loads(exception_info)
-
-                    if exception_info is not None:
-                        if not passive or i == 0:
-                            tb = Traceback.from_exception(
-                                exception_info[0], exception_info[1], exception_info[2]
-                            )
+                                if not passive:
+                                    progress.stop()
 
-                            if not passive:
-                                progress.stop()
+                                console.print(tb)
+                                console.print(
+                                    f"Process #{i} failed with an exception above."
+                                )
 
-                            console.print(tb)
-                            console.print(
-                                f"Process #{i} failed with an exception above."
-                            )
+                                attach = None
+                                while attach is None:
+                                    response = input(
+                                        "Would you like to attach the debugger? [y/n] "
+                                    )
+                                    if response == "y":
+                                        attach = True
+                                    elif response == "n":
+                                        attach = False
+                            else:
+                                attach = False
+
+                            e.clear()
+                            err_parent_conn.send(attach)
+                            e.wait()
+                            if not passive:
+                                progress.start()
 
-                            attach = None
-                            while attach is None:
-                                response = input(
-                                    "Would you like to attach the debugger? [y/n] "
-                                )
-                                if response == "y":
-                                    attach = True
-                                elif response == "n":
-                                    attach = False
-                        else:
-                            attach = False
-
-                        e.clear()
-                        err_parent_conn.send(attach)
-                        e.wait()
-                        if not passive:
+                        progress.update(
+                            task, thr_rem=len(processes) - len(to_be_removed)
+                        )
+                        if i == 0:
                             progress.start()
 
-                    progress.update(task, thr_rem=len(processes) - len(to_be_removed))
-                    if i == 0:
-                        progress.start()
-
-                tmp = None
-                while cov_parent_conn.poll(0):
-                    try:
-                        tmp = cov_parent_conn.recv()
-                    except EOFError:
-                        break
-                if tmp is not None:
-                    exported_coverages[i] = tmp
-                    res = export_merged_ide_coverage(list(exported_coverages.values()))
-                    if res:
-                        write_coverage(
-                            res, config.project_root_path / "woke-coverage.cov"
-                        )
-                    cov_info = ""
-                    if not passive and verbose_coverage:
-                        cov_info = "\n[dark_goldenrod]" + "\n".join(
-                            [
-                                f"{fn_name}: [green]{fn_calls}[dark_goldenrod]"
-                                for (fn_name, fn_calls) in sorted(
-                                    _compute_coverage_per_function(res).items(),
-                                    key=lambda x: x[1],
-                                    reverse=True,
-                                )
-                            ]
+                    tmp = None
+                    while cov_parent_conn.poll(0):
+                        try:
+                            tmp = cov_parent_conn.recv()
+                        except EOFError:
+                            break
+                    if tmp is not None:
+                        exported_coverages[i] = tmp
+                        res = export_merged_ide_coverage(
+                            list(exported_coverages.values())
                         )
-                    progress.update(task, coverage_info=cov_info)
-                if finished:
-                    cov_parent_conn.close()
+                        if res:
+                            write_coverage(
+                                res, config.project_root_path / "woke-coverage.cov"
+                            )
+                        cov_info = ""
+                        if not passive and verbose_coverage:
+                            cov_info = "\n[dark_goldenrod]" + "\n".join(
+                                [
+                                    f"{fn_name}: [green]{fn_calls}[dark_goldenrod]"
+                                    for (fn_name, fn_calls) in sorted(
+                                        _compute_coverage_per_function(res).items(),
+                                        key=lambda x: x[1],
+                                        reverse=True,
+                                    )
+                                ]
+                            )
+                        progress.update(task, coverage_info=cov_info)
+                    if finished:
+                        cov_parent_conn.close()
 
-            for i in to_be_removed:
-                processes.pop(i)
+                for i in to_be_removed:
+                    processes.pop(i)
 
-        progress.update(task, description="Finished", completed=1)
+            progress.update(task, description="Finished", completed=1)
+    finally:
+        for i, (p, e, err_parent_conn, cov_parent_conn) in processes.items():
+            if p.is_alive():
+                p.terminate()
+            p.join()
```

### Comparing `woke-3.1.0/woke/testing/fuzzing/generators.py` & `woke-3.2.0/woke/testing/fuzzing/generators.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/utils/context_managers.py` & `woke-3.2.0/woke/utils/context_managers.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/utils/decorators.py` & `woke-3.2.0/woke/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/utils/file_utils.py` & `woke-3.2.0/woke/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/utils/openzeppelin.py` & `woke-3.2.0/woke/utils/openzeppelin.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/utils/string.py` & `woke-3.2.0/woke/utils/string.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/utils/tee.py` & `woke-3.2.0/woke/utils/tee.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/woke/utils/threaded_child_watcher.py` & `woke-3.2.0/woke/utils/threaded_child_watcher.py`

 * *Files identical despite different names*

### Comparing `woke-3.1.0/setup.py` & `woke-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,26 +46,26 @@
  'click>=8,<9',
  'eth-abi>=4.0.0b2,<5.0.0',
  'eth-account>=0.8,<0.9',
  'eth-hash[pycryptodome]>=0.5.1,<0.6.0',
  'eth-utils>=2.1,<3.0',
  'graphviz>=0.19,<0.20',
  'intervaltree>=3.1,<4.0',
+ 'ipdb>=0.13.9,<0.14.0',
  'networkx>=2.5,<3.0',
  'parsimonious>=0.9,<0.10',
  'pathvalidate>=2.5,<3.0',
- 'pdbr[ipython]>=0.8.0,<0.9.0',
  'pydantic>=1.9.1,<2.0.0',
  'pytest>=7,<8',
  'rich-click>=1.6,<2.0',
  'rich>=13.3.2,<14.0.0',
  'tblib>=1.7,<2.0',
  'tomli>=2,<3',
  'typing-extensions>=4,<5',
- 'watchdog>=2.2,<3.0',
+ 'watchdog>=2.2.0,<2.3.0',
  'websocket-client>=1.4,<2.0']
 
 extras_require = \
 {':sys_platform == "win32"': ['pywin32>=302'],
  'dev': ['black>=22,<23',
          'mkdocs-material>=9,<10',
          'mkdocstrings[python]>=0.19,<0.20',
@@ -78,15 +78,15 @@
 
 entry_points = \
 {'console_scripts': ['woke = woke.cli.__main__:main',
                      'woke-solc = woke.cli.__main__:woke_solc']}
 
 setup_kwargs = {
     'name': 'woke',
-    'version': '3.1.0',
+    'version': '3.2.0',
     'description': 'Woke is a Python-based development and testing framework for Solidity.',
     'long_description': '# Woke\n\nWoke is a Python-based development and testing framework for Solidity.\n\nFeatures:\n\n- **Testing framework** - a testing framework for Solidity smart contracts with Python-native equivalents of Solidity types and blazing fast execution.\n\n- **Fuzzer** - a property-based fuzzer for Solidity smart contracts that allows testers to write their fuzz tests in Python.\n\n- **Vulnerability detectors**\n\n- **LSP server**\n\n## Dependencies\n\n- [Python](https://www.python.org/downloads/release/python-3910/) (version 3.7 or higher)\n\n> :warning: Python 3.11 is experimentally supported.\n\n## Installation\n\nvia `pip`\n\n```shell\npip3 install woke\n```\n\n## Documentation & Contribution\n\nWoke documentation can be found [here](https://ackeeblockchain.com/woke/docs/latest).\n\nThere you can also find a section on [contributing](https://ackeeblockchain.com/woke/docs/latest/contributing/).\n\n## Features\n\n### Testing framework\n\nSee [examples](examples/testing) and [documentation](https://ackeeblockchain.com/woke/docs/latest/testing-framework/overview) for more information.\n\nWriting tests is as simple as:\n\n```python\nfrom woke.testing import *\nfrom pytypes.contracts.Counter import Counter\n\n@default_chain.connect()\ndef test_counter():\n    default_chain.set_default_accounts(default_chain.accounts[0])\n\n    counter = Counter.deploy()\n    assert counter.count() == 0\n\n    counter.increment()\n    assert counter.count() == 1\n```\n\n### Fuzzer\n\nFuzzer builds on top of the testing framework and allows efficient fuzz testing of Solidity smart contracts.\n\n```python\nfrom woke.testing import *\nfrom woke.testing.fuzzing import *\nfrom pytypes.contracts.Counter import Counter\n\nclass CounterTest(FuzzTest):\n    def pre_sequence(self) -> None:\n        self.counter = Counter.deploy()\n        self.count = 0\n\n    @flow()\n    def increment(self) -> None:\n        self.counter.increment()\n        self.count += 1\n\n    @flow()\n    def decrement(self) -> None:\n        with may_revert(Panic(PanicCodeEnum.UNDERFLOW_OVERFLOW)) as e:\n            self.counter.decrement()\n\n        if e.value is not None:\n            assert self.count == 0\n        else:\n            self.count -= 1\n\n    @invariant(period=10)\n    def count(self) -> None:\n        assert self.counter.count() == self.count\n\n@default_chain.connect()\ndef test_counter():\n    default_chain.set_default_accounts(default_chain.accounts[0])\n    CounterTest().run(sequences_count=30, flows_count=100)\n```\n\n### Vulnerability detectors\n\nVulnerability detectors can be run using:\n```shell\nwoke detect\n```\n\n### LSP server\n\nWoke implements an [LSP](https://microsoft.github.io/language-server-protocol/) server for Solidity. The only currently supported communication channel is TCP.\n\nWoke LSP server can be run using:\n\n```shell\nwoke lsp\n```\n\nOr with an optional --port argument:\n\n```shell\nwoke lsp --port 1234\n```\n\nAll LSP server features can be found in the [documentation](https://ackeeblockchain.com/woke/docs/latest/language-server/).\n\n## License\n\nThis project is licensed under the [ISC license](https://github.com/Ackee-Blockchain/woke/blob/main/LICENSE).\n\n## Partners\n\nRockawayX             |  Coinbase\n:-------------------------:|:-------------------------:\n[![](https://github.com/Ackee-Blockchain/woke/blob/main/images/rockawayx.jpg?raw=true)](https://rockawayx.com/)  |  [![](https://github.com/Ackee-Blockchain/woke/blob/main/images/coinbase.png?raw=true)](https://www.coinbase.com/)\n\n\n\n\n\n\n',
     'author': 'Ackee Blockchain',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ackeeblockchain.com',
```

### Comparing `woke-3.1.0/PKG-INFO` & `woke-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woke
-Version: 3.1.0
+Version: 3.2.0
 Summary: Woke is a Python-based development and testing framework for Solidity.
 Home-page: https://ackeeblockchain.com
 License: ISC
 Keywords: ethereum,solidity,security,testing,development,framework,audit
 Author: Ackee Blockchain
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: License :: OSI Approved
@@ -23,34 +23,34 @@
 Requires-Dist: click (>=8,<9)
 Requires-Dist: eth-abi (>=4.0.0b2,<5.0.0)
 Requires-Dist: eth-account (>=0.8,<0.9)
 Requires-Dist: eth-hash[pycryptodome] (>=0.5.1,<0.6.0)
 Requires-Dist: eth-utils (>=2.1,<3.0)
 Requires-Dist: graphviz (>=0.19,<0.20)
 Requires-Dist: intervaltree (>=3.1,<4.0)
+Requires-Dist: ipdb (>=0.13.9,<0.14.0)
 Requires-Dist: isort (>=5,<6) ; extra == "dev"
 Requires-Dist: mkdocs-material (>=9,<10) ; extra == "dev"
 Requires-Dist: mkdocstrings[python] (>=0.19,<0.20) ; extra == "dev"
 Requires-Dist: networkx (>=2.5,<3.0)
 Requires-Dist: parsimonious (>=0.9,<0.10)
 Requires-Dist: pathvalidate (>=2.5,<3.0)
-Requires-Dist: pdbr[ipython] (>=0.8.0,<0.9.0)
 Requires-Dist: pillow (>=9,<10) ; extra == "dev"
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pygments (>=2,<3) ; extra == "dev"
 Requires-Dist: pymdown-extensions (>=9,<10) ; extra == "dev"
 Requires-Dist: pytest (>=7,<8)
 Requires-Dist: pytest-asyncio (>=0.17,<0.18) ; extra == "tests"
 Requires-Dist: pywin32 (>=302) ; sys_platform == "win32"
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: rich-click (>=1.6,<2.0)
 Requires-Dist: tblib (>=1.7,<2.0)
 Requires-Dist: tomli (>=2,<3)
 Requires-Dist: typing-extensions (>=4,<5)
-Requires-Dist: watchdog (>=2.2,<3.0)
+Requires-Dist: watchdog (>=2.2.0,<2.3.0)
 Requires-Dist: websocket-client (>=1.4,<2.0)
 Project-URL: Announcement, https://ackeeblockchain.com/blog/woke-our-development-and-testing-framework-for-solidity/
 Project-URL: Documentation, https://ackeeblockchain.com/woke/docs/latest
 Project-URL: Repository, https://github.com/Ackee-Blockchain/woke
 Project-URL: VS Code Extension, https://marketplace.visualstudio.com/items?itemName=AckeeBlockchain.tools-for-solidity
 Description-Content-Type: text/markdown
```

