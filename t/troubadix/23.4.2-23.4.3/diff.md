# Comparing `tmp/troubadix-23.4.2.tar.gz` & `tmp/troubadix-23.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troubadix-23.4.2.tar", max compression
+gzip compressed data, was "troubadix-23.4.3.tar", max compression
```

## Comparing `troubadix-23.4.2.tar` & `troubadix-23.4.3.tar`

### file list

```diff
@@ -1,198 +1,194 @@
--rw-r--r--   0        0        0    35149 2023-04-04 04:46:59.716900 troubadix-23.4.2/LICENSE
--rw-r--r--   0        0        0     2730 2023-04-04 04:46:59.716900 troubadix-23.4.2/README.md
--rw-r--r--   0        0        0     2412 2023-04-04 04:46:59.716900 troubadix-23.4.2/pyproject.toml
--rw-r--r--   0        0        0      716 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/__init__.py
--rw-r--r--   0        0        0      716 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/helper/__init__.py
--rw-r--r--   0        0        0     8416 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/helper/test_linguistic_exception_handler.py
--rw-r--r--   0        0        0     1940 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/helper/test_patterns.py
--rw-r--r--   0        0        0     2396 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/__init__.py
--rw-r--r--   0        0        0     1012 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/fail.nasl
--rw-r--r--   0        0        0     1291 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/fail2.nasl
--rw-r--r--   0        0        0     2100 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test.nasl
--rw-r--r--   0        0        0     2061 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_badwords.py
--rw-r--r--   0        0        0     5109 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_copyright_text.py
--rw-r--r--   0        0        0     6961 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_copyright_year.py
--rw-r--r--   0        0        0     5004 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_creation_date.py
--rw-r--r--   0        0        0     5881 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_cve_format.py
--rw-r--r--   0        0        0     4914 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_cvss_format.py
--rw-r--r--   0        0        0     8970 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_dependencies.py
--rw-r--r--   0        0        0     5808 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_dependency_category_order.py
--rw-r--r--   0        0        0     5589 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_deprecated_dependency.py
--rw-r--r--   0        0        0     3049 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_deprecated_functions.py
--rw-r--r--   0        0        0     3185 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_description.py
--rw-r--r--   0        0        0     2394 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_double_end_points.py
--rw-r--r--   0        0        0     3504 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_duplicate_oid.py
--rw-r--r--   0        0        0     4686 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_duplicated_script_tags.py
--rw-r--r--   0        0        0     3906 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_encoding.py
--rw-r--r--   0        0        0     1982 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_files/fail_bad_new_line.nasl
--rw-r--r--   0        0        0      246 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_files/fail_badwords.nasl
--rw-r--r--   0        0        0     1979 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1965 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_files/fail_name_newline.nasl
--rwxr-xr-x   0        0        0     1012 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_files/fail_permissions.nasl
--rw-r--r--   0        0        0      150 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_files/fail_spelling.nasl
--rw-r--r--   0        0        0     2213 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/fail.nasl
--rw-r--r--   0        0        0      246 2023-04-04 04:46:59.716900 troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
--rw-r--r--   0        0        0     1990 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1987 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
--rw-r--r--   0        0        0     2134 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
--rw-r--r--   0        0        0     1023 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
--rw-r--r--   0        0        0     1302 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
--rw-r--r--   0        0        0     2122 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/runner/test.nasl
--rw-r--r--   0        0        0     2119 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
--rw-r--r--   0        0        0     1023 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/test.inc
--rw-r--r--   0        0        0     2122 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/test.nasl
--rw-r--r--   0        0        0     2976 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_files/nasl/warning.nasl
--rw-r--r--   0        0        0     1012 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_files/ok_permissions.nasl
--rw-r--r--   0        0        0     2100 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_files/test_oid.nasl
--rw-r--r--   0        0        0     4548 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_forking_nasl_functions.py
--rw-r--r--   0        0        0     2271 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_get_kb_on_services.py
--rw-r--r--   0        0        0     9438 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_grammar.py
--rw-r--r--   0        0        0     6936 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_http_links_in_tags.py
--rw-r--r--   0        0        0     4730 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_illegal_characters.py
--rw-r--r--   0        0        0     5965 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_log_messages.py
--rw-r--r--   0        0        0     6174 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_malformed_dependencies.py
--rw-r--r--   0        0        0    21051 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_misplaced_compare_in_if.py
--rw-r--r--   0        0        0     3585 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_missing_desc_exit.py
--rw-r--r--   0        0        0     3101 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_missing_tag_solution.py
--rw-r--r--   0        0        0     4688 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_newlines.py
--rw-r--r--   0        0        0    40813 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_overlong_script_tags.py
--rw-r--r--   0        0        0     4294 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     4594 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_qod.py
--rw-r--r--   0        0        0     5844 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_reporting_consistency.py
--rw-r--r--   0        0        0     2329 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_risk_factor.py
--rw-r--r--   0        0        0     3371 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_script_add_preference_type.py
--rw-r--r--   0        0        0     2353 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_script_calls_empty_values.py
--rw-r--r--   0        0        0     2799 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_script_calls_recommended.py
--rw-r--r--   0        0        0     2650 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_script_category.py
--rw-r--r--   0        0        0     3469 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_script_copyright.py
--rw-r--r--   0        0        0     3877 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_script_family.py
--rw-r--r--   0        0        0     3079 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_script_tag_form.py
--rw-r--r--   0        0        0     3086 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_script_tag_whitespaces.py
--rw-r--r--   0        0        0     3313 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_script_tags_mandatory.py
--rw-r--r--   0        0        0     4858 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     3016 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_script_xref_form.py
--rw-r--r--   0        0        0     2189 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_script_xref_url.py
--rw-r--r--   0        0        0     6599 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_security_messages.py
--rw-r--r--   0        0        0     3021 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_set_get_kb_calls.py
--rw-r--r--   0        0        0     7260 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_solution_text.py
--rw-r--r--   0        0        0     3306 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_solution_type.py
--rw-r--r--   0        0        0     2827 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_spelling.py
--rw-r--r--   0        0        0     1813 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_tabs.py
--rw-r--r--   0        0        0     6297 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_todo_tbd.py
--rw-r--r--   0        0        0     2398 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_trailing_spaces_tabs.py
--rw-r--r--   0        0        0     3868 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_using_display.py
--rw-r--r--   0        0        0    24134 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_valid_oid.py
--rw-r--r--   0        0        0     4154 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_valid_script_tag_names.py
--rw-r--r--   0        0        0     1947 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_vt_file_permissions.py
--rw-r--r--   0        0        0     5189 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/plugins/test_vt_placement.py
--rw-r--r--   0        0        0      716 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/__init__.py
--rw-r--r--   0        0        0      716 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/changed_packages/__init__.py
--rw-r--r--   0        0        0      716 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/changed_packages/markers/__init__.py
--rw-r--r--   0        0        0     3075 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
--rw-r--r--   0        0        0     2620 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/changed_packages/markers/test_added_release.py
--rw-r--r--   0        0        0     1792 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
--rw-r--r--   0        0        0     3258 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
--rw-r--r--   0        0        0     3584 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
--rw-r--r--   0        0        0     3780 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/changed_packages/test_changed_packages.py
--rw-r--r--   0        0        0     2427 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/changed_packages/test_package.py
--rw-r--r--   0        0        0     2977 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/test_changed_cves.py
--rw-r--r--   0        0        0     2952 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/test_changed_oid.py
--rw-r--r--   0        0        0     3962 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/test_last_modification.py
--rw-r--r--   0        0        0     7347 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/test_no_solution.py
--rw-r--r--   0        0        0     6293 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/standalone_plugins/test_version_updated.py
--rw-r--r--   0        0        0     4768 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/test_argparser.py
--rw-r--r--   0        0        0     3947 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/test_helper.py
--rw-r--r--   0        0        0     3671 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/test_naslinter.py
--rw-r--r--   0        0        0     3399 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/test_reporter.py
--rw-r--r--   0        0        0     2517 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/test_results.py
--rw-r--r--   0        0        0    17972 2023-04-04 04:46:59.720900 troubadix-23.4.2/tests/test_runner.py
--rw-r--r--   0        0        0      716 2023-04-04 04:46:59.720900 troubadix-23.4.2/troubadix/__init__.py
--rw-r--r--   0        0        0      103 2023-04-04 04:46:59.720900 troubadix-23.4.2/troubadix/__version__.py
--rw-r--r--   0        0        0     6999 2023-04-04 04:46:59.720900 troubadix-23.4.2/troubadix/argparser.py
--rw-r--r--   0        0        0      338 2023-04-04 04:46:59.720900 troubadix-23.4.2/troubadix/codespell/codespell.additions
--rw-r--r--   0        0        0   125033 2023-04-04 04:46:59.720900 troubadix-23.4.2/troubadix/codespell/codespell.exclude
--rw-r--r--   0        0        0      756 2023-04-04 04:46:59.720900 troubadix-23.4.2/troubadix/codespell/codespell.ignore
--rw-r--r--   0        0        0     1061 2023-04-04 04:46:59.720900 troubadix-23.4.2/troubadix/helper/__init__.py
--rw-r--r--   0        0        0     3105 2023-04-04 04:46:59.720900 troubadix-23.4.2/troubadix/helper/helper.py
--rw-r--r--   0        0        0     6811 2023-04-04 04:46:59.720900 troubadix-23.4.2/troubadix/helper/linguistic_exception_handler.py
--rw-r--r--   0        0        0     9370 2023-04-04 04:46:59.720900 troubadix-23.4.2/troubadix/helper/patterns.py
--rw-r--r--   0        0        0     3508 2023-04-04 04:46:59.720900 troubadix-23.4.2/troubadix/plugin.py
--rw-r--r--   0        0        0     7139 2023-04-04 04:46:59.720900 troubadix-23.4.2/troubadix/plugins/__init__.py
--rw-r--r--   0        0        0     3600 2023-04-04 04:46:59.720900 troubadix-23.4.2/troubadix/plugins/badwords.py
--rw-r--r--   0        0        0     3583 2023-04-04 04:46:59.720900 troubadix-23.4.2/troubadix/plugins/copyright_text.py
--rw-r--r--   0        0        0     3109 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/copyright_year.py
--rw-r--r--   0        0        0     3252 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/creation_date.py
--rw-r--r--   0        0        0     3295 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/cve_format.py
--rw-r--r--   0        0        0     2204 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/cvss_format.py
--rw-r--r--   0        0        0     4357 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/dependencies.py
--rw-r--r--   0        0        0     7169 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/dependency_category_order.py
--rw-r--r--   0        0        0     4032 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/deprecated_dependency.py
--rw-r--r--   0        0        0     2466 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/deprecated_functions.py
--rw-r--r--   0        0        0     1590 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/description.py
--rw-r--r--   0        0        0     2509 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/double_end_points.py
--rw-r--r--   0        0        0     2547 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/duplicate_oid.py
--rw-r--r--   0        0        0     3079 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/duplicated_script_tags.py
--rw-r--r--   0        0        0     2090 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/encoding.py
--rw-r--r--   0        0        0     6014 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/forking_nasl_functions.py
--rw-r--r--   0        0        0     3401 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/get_kb_on_services.py
--rw-r--r--   0        0        0     8348 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/grammar.py
--rw-r--r--   0        0        0     7157 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/http_links_in_tags.py
--rw-r--r--   0        0        0     4406 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/illegal_characters.py
--rw-r--r--   0        0        0     2960 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/log_messages.py
--rw-r--r--   0        0        0     3000 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/malformed_dependencies.py
--rw-r--r--   0        0        0     5330 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/misplaced_compare_in_if.py
--rw-r--r--   0        0        0     2306 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/missing_desc_exit.py
--rw-r--r--   0        0        0     2828 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/missing_tag_solution.py
--rw-r--r--   0        0        0     2788 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/newlines.py
--rw-r--r--   0        0        0     2373 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/overlong_script_tags.py
--rw-r--r--   0        0        0     4185 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     3692 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/qod.py
--rw-r--r--   0        0        0     4019 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/reporting_consistency.py
--rw-r--r--   0        0        0     1384 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/risk_factor.py
--rw-r--r--   0        0        0     3193 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/script_add_preference_type.py
--rw-r--r--   0        0        0     2407 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/script_calls_empty_values.py
--rw-r--r--   0        0        0     3032 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/script_calls_recommended.py
--rw-r--r--   0        0        0     2079 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/script_category.py
--rw-r--r--   0        0        0     2205 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/script_copyright.py
--rw-r--r--   0        0        0     3918 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/script_family.py
--rw-r--r--   0        0        0     1773 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/script_tag_form.py
--rw-r--r--   0        0        0     1861 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/script_tag_whitespaces.py
--rw-r--r--   0        0        0     2525 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/script_tags_mandatory.py
--rw-r--r--   0        0        0     6921 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     1848 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/script_xref_form.py
--rw-r--r--   0        0        0     2875 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/script_xref_url.py
--rw-r--r--   0        0        0     4708 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/security_messages.py
--rw-r--r--   0        0        0     3415 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/set_get_kb_calls.py
--rw-r--r--   0        0        0     5852 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/solution_text.py
--rw-r--r--   0        0        0     2497 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/solution_type.py
--rw-r--r--   0        0        0     9528 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/spelling.py
--rw-r--r--   0        0        0     1319 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/tabs.py
--rw-r--r--   0        0        0     1733 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/todo_tbd.py
--rw-r--r--   0        0        0     2049 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/trailing_spaces_tabs.py
--rw-r--r--   0        0        0     3948 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/using_display.py
--rw-r--r--   0        0        0    16522 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/valid_oid.py
--rw-r--r--   0        0        0     3447 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/valid_script_tag_names.py
--rw-r--r--   0        0        0     3285 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/variable_assigned_in_if.py
--rw-r--r--   0        0        0     1521 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/vt_file_permissions.py
--rw-r--r--   0        0        0     2800 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/plugins/vt_placement.py
--rw-r--r--   0        0        0     9176 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/reporter.py
--rw-r--r--   0        0        0     2632 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/results.py
--rw-r--r--   0        0        0     5172 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/runner.py
--rw-r--r--   0        0        0       22 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/__init__.py
--rw-r--r--   0        0        0     2921 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/changed_cves.py
--rw-r--r--   0        0        0     4074 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/changed_oid.py
--rw-r--r--   0        0        0     5742 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/changed_packages.py
--rw-r--r--   0        0        0      923 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/marker/__init__.py
--rw-r--r--   0        0        0     1797 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
--rw-r--r--   0        0        0     1486 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/marker/added_release.py
--rw-r--r--   0        0        0     1124 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
--rw-r--r--   0        0        0     1952 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
--rw-r--r--   0        0        0     1632 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
--rw-r--r--   0        0        0     1278 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/marker/marker.py
--rw-r--r--   0        0        0     2743 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/package.py
--rw-r--r--   0        0        0     1028 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/common.py
--rw-r--r--   0        0        0     4616 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/last_modification.py
--rw-r--r--   0        0        0     8463 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/no_solution.py
--rw-r--r--   0        0        0     3978 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/standalone_plugins/version_updated.py
--rw-r--r--   0        0        0     6045 2023-04-04 04:46:59.724900 troubadix-23.4.2/troubadix/troubadix.py
--rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 troubadix-23.4.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 15:13:31.513378 troubadix-23.4.3/LICENSE
+-rw-r--r--   0        0        0     2730 2023-04-12 15:13:31.513378 troubadix-23.4.3/README.md
+-rw-r--r--   0        0        0     2412 2023-04-12 15:13:31.517378 troubadix-23.4.3/pyproject.toml
+-rw-r--r--   0        0        0      716 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/helper/__init__.py
+-rw-r--r--   0        0        0     8416 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/helper/test_linguistic_exception_handler.py
+-rw-r--r--   0        0        0     1940 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/helper/test_patterns.py
+-rw-r--r--   0        0        0     2396 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/__init__.py
+-rw-r--r--   0        0        0     1012 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/fail.nasl
+-rw-r--r--   0        0        0     1291 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/fail2.nasl
+-rw-r--r--   0        0        0     2100 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test.nasl
+-rw-r--r--   0        0        0     2061 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_badwords.py
+-rw-r--r--   0        0        0     5109 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_copyright_text.py
+-rw-r--r--   0        0        0     6961 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_copyright_year.py
+-rw-r--r--   0        0        0     5004 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_creation_date.py
+-rw-r--r--   0        0        0     5881 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_cve_format.py
+-rw-r--r--   0        0        0     4914 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_cvss_format.py
+-rw-r--r--   0        0        0     8970 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_dependencies.py
+-rw-r--r--   0        0        0     5808 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_dependency_category_order.py
+-rw-r--r--   0        0        0     5589 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_deprecated_dependency.py
+-rw-r--r--   0        0        0     4545 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_deprecated_functions.py
+-rw-r--r--   0        0        0     2394 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_double_end_points.py
+-rw-r--r--   0        0        0     3504 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_duplicate_oid.py
+-rw-r--r--   0        0        0     4686 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_duplicated_script_tags.py
+-rw-r--r--   0        0        0     3906 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_encoding.py
+-rw-r--r--   0        0        0     1982 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/fail_bad_new_line.nasl
+-rw-r--r--   0        0        0      246 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/fail_badwords.nasl
+-rw-r--r--   0        0        0     1979 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1965 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/fail_name_newline.nasl
+-rwxr-xr-x   0        0        0     1012 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/fail_permissions.nasl
+-rw-r--r--   0        0        0      150 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/fail_spelling.nasl
+-rw-r--r--   0        0        0     2213 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/fail.nasl
+-rw-r--r--   0        0        0      246 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
+-rw-r--r--   0        0        0     1990 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1987 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
+-rw-r--r--   0        0        0     2134 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
+-rw-r--r--   0        0        0     1023 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
+-rw-r--r--   0        0        0     1302 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
+-rw-r--r--   0        0        0     2122 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/runner/test.nasl
+-rw-r--r--   0        0        0     2119 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
+-rw-r--r--   0        0        0     1023 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/test.inc
+-rw-r--r--   0        0        0     2122 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/test.nasl
+-rw-r--r--   0        0        0     2976 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/nasl/warning.nasl
+-rw-r--r--   0        0        0     1012 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/ok_permissions.nasl
+-rw-r--r--   0        0        0     2100 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_files/test_oid.nasl
+-rw-r--r--   0        0        0     4548 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_forking_nasl_functions.py
+-rw-r--r--   0        0        0     2271 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_get_kb_on_services.py
+-rw-r--r--   0        0        0     9438 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_grammar.py
+-rw-r--r--   0        0        0     6936 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_http_links_in_tags.py
+-rw-r--r--   0        0        0     4730 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_illegal_characters.py
+-rw-r--r--   0        0        0     5965 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_log_messages.py
+-rw-r--r--   0        0        0     6174 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_malformed_dependencies.py
+-rw-r--r--   0        0        0    21051 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     3585 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_missing_desc_exit.py
+-rw-r--r--   0        0        0     3101 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_missing_tag_solution.py
+-rw-r--r--   0        0        0     4688 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_newlines.py
+-rw-r--r--   0        0        0    40813 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_overlong_script_tags.py
+-rw-r--r--   0        0        0     4294 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     4594 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_qod.py
+-rw-r--r--   0        0        0     5844 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_reporting_consistency.py
+-rw-r--r--   0        0        0     3371 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_script_add_preference_type.py
+-rw-r--r--   0        0        0     2353 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_script_calls_empty_values.py
+-rw-r--r--   0        0        0     2799 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_script_calls_recommended.py
+-rw-r--r--   0        0        0     2650 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_script_category.py
+-rw-r--r--   0        0        0     3469 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_script_copyright.py
+-rw-r--r--   0        0        0     3877 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_script_family.py
+-rw-r--r--   0        0        0     3079 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_script_tag_form.py
+-rw-r--r--   0        0        0     3086 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_script_tag_whitespaces.py
+-rw-r--r--   0        0        0     3313 2023-04-12 15:13:31.517378 troubadix-23.4.3/tests/plugins/test_script_tags_mandatory.py
+-rw-r--r--   0        0        0     4858 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     3016 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_script_xref_form.py
+-rw-r--r--   0        0        0     2189 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_script_xref_url.py
+-rw-r--r--   0        0        0     6599 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_security_messages.py
+-rw-r--r--   0        0        0     3021 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_set_get_kb_calls.py
+-rw-r--r--   0        0        0     7260 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_solution_text.py
+-rw-r--r--   0        0        0     3306 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_solution_type.py
+-rw-r--r--   0        0        0     2827 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_spelling.py
+-rw-r--r--   0        0        0     1813 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_tabs.py
+-rw-r--r--   0        0        0     6297 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_todo_tbd.py
+-rw-r--r--   0        0        0     2398 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     3868 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_using_display.py
+-rw-r--r--   0        0        0    24134 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_valid_oid.py
+-rw-r--r--   0        0        0     4154 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_valid_script_tag_names.py
+-rw-r--r--   0        0        0     1947 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_vt_file_permissions.py
+-rw-r--r--   0        0        0     5189 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/plugins/test_vt_placement.py
+-rw-r--r--   0        0        0      716 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/changed_packages/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/changed_packages/markers/__init__.py
+-rw-r--r--   0        0        0     3075 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
+-rw-r--r--   0        0        0     2620 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/changed_packages/markers/test_added_release.py
+-rw-r--r--   0        0        0     1792 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
+-rw-r--r--   0        0        0     3258 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
+-rw-r--r--   0        0        0     3584 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
+-rw-r--r--   0        0        0     3780 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/changed_packages/test_changed_packages.py
+-rw-r--r--   0        0        0     2427 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/changed_packages/test_package.py
+-rw-r--r--   0        0        0     2977 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/test_changed_cves.py
+-rw-r--r--   0        0        0     2952 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/test_changed_oid.py
+-rw-r--r--   0        0        0     3962 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/test_last_modification.py
+-rw-r--r--   0        0        0     7347 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/test_no_solution.py
+-rw-r--r--   0        0        0     6293 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/standalone_plugins/test_version_updated.py
+-rw-r--r--   0        0        0     4768 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/test_argparser.py
+-rw-r--r--   0        0        0     3947 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/test_helper.py
+-rw-r--r--   0        0        0     3671 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/test_naslinter.py
+-rw-r--r--   0        0        0     3399 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/test_reporter.py
+-rw-r--r--   0        0        0     2517 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/test_results.py
+-rw-r--r--   0        0        0    17972 2023-04-12 15:13:31.521378 troubadix-23.4.3/tests/test_runner.py
+-rw-r--r--   0        0        0      716 2023-04-12 15:13:31.521378 troubadix-23.4.3/troubadix/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-12 15:13:31.521378 troubadix-23.4.3/troubadix/__version__.py
+-rw-r--r--   0        0        0     6999 2023-04-12 15:13:31.521378 troubadix-23.4.3/troubadix/argparser.py
+-rw-r--r--   0        0        0      338 2023-04-12 15:13:31.521378 troubadix-23.4.3/troubadix/codespell/codespell.additions
+-rw-r--r--   0        0        0   125039 2023-04-12 15:13:31.521378 troubadix-23.4.3/troubadix/codespell/codespell.exclude
+-rw-r--r--   0        0        0      756 2023-04-12 15:13:31.521378 troubadix-23.4.3/troubadix/codespell/codespell.ignore
+-rw-r--r--   0        0        0     1061 2023-04-12 15:13:31.521378 troubadix-23.4.3/troubadix/helper/__init__.py
+-rw-r--r--   0        0        0     3105 2023-04-12 15:13:31.521378 troubadix-23.4.3/troubadix/helper/helper.py
+-rw-r--r--   0        0        0     6811 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/helper/linguistic_exception_handler.py
+-rw-r--r--   0        0        0     9370 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/helper/patterns.py
+-rw-r--r--   0        0        0     3508 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugin.py
+-rw-r--r--   0        0        0     7013 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/__init__.py
+-rw-r--r--   0        0        0     3600 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/badwords.py
+-rw-r--r--   0        0        0     3583 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/copyright_text.py
+-rw-r--r--   0        0        0     3109 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/copyright_year.py
+-rw-r--r--   0        0        0     3252 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/creation_date.py
+-rw-r--r--   0        0        0     3295 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/cve_format.py
+-rw-r--r--   0        0        0     2204 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/cvss_format.py
+-rw-r--r--   0        0        0     4357 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/dependencies.py
+-rw-r--r--   0        0        0     7169 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/dependency_category_order.py
+-rw-r--r--   0        0        0     4032 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/deprecated_dependency.py
+-rw-r--r--   0        0        0     2568 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/deprecated_functions.py
+-rw-r--r--   0        0        0     2509 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/double_end_points.py
+-rw-r--r--   0        0        0     2547 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/duplicate_oid.py
+-rw-r--r--   0        0        0     3079 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/duplicated_script_tags.py
+-rw-r--r--   0        0        0     2090 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/encoding.py
+-rw-r--r--   0        0        0     6014 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/forking_nasl_functions.py
+-rw-r--r--   0        0        0     3401 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/get_kb_on_services.py
+-rw-r--r--   0        0        0     8348 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/grammar.py
+-rw-r--r--   0        0        0     7157 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/http_links_in_tags.py
+-rw-r--r--   0        0        0     4406 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/illegal_characters.py
+-rw-r--r--   0        0        0     2960 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/log_messages.py
+-rw-r--r--   0        0        0     3000 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/malformed_dependencies.py
+-rw-r--r--   0        0        0     5330 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     2306 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/missing_desc_exit.py
+-rw-r--r--   0        0        0     2828 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/missing_tag_solution.py
+-rw-r--r--   0        0        0     2788 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/newlines.py
+-rw-r--r--   0        0        0     2373 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/overlong_script_tags.py
+-rw-r--r--   0        0        0     4185 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     3692 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/qod.py
+-rw-r--r--   0        0        0     4019 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/reporting_consistency.py
+-rw-r--r--   0        0        0     3193 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/script_add_preference_type.py
+-rw-r--r--   0        0        0     2407 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/script_calls_empty_values.py
+-rw-r--r--   0        0        0     3032 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/script_calls_recommended.py
+-rw-r--r--   0        0        0     2079 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/script_category.py
+-rw-r--r--   0        0        0     2205 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/script_copyright.py
+-rw-r--r--   0        0        0     3918 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/script_family.py
+-rw-r--r--   0        0        0     1773 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/script_tag_form.py
+-rw-r--r--   0        0        0     1861 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/script_tag_whitespaces.py
+-rw-r--r--   0        0        0     2525 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/script_tags_mandatory.py
+-rw-r--r--   0        0        0     6921 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     1848 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/script_xref_form.py
+-rw-r--r--   0        0        0     2875 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/script_xref_url.py
+-rw-r--r--   0        0        0     4708 2023-04-12 15:13:31.525378 troubadix-23.4.3/troubadix/plugins/security_messages.py
+-rw-r--r--   0        0        0     3415 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/plugins/set_get_kb_calls.py
+-rw-r--r--   0        0        0     5852 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/plugins/solution_text.py
+-rw-r--r--   0        0        0     2497 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/plugins/solution_type.py
+-rw-r--r--   0        0        0     9528 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/plugins/spelling.py
+-rw-r--r--   0        0        0     1319 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/plugins/tabs.py
+-rw-r--r--   0        0        0     1733 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/plugins/todo_tbd.py
+-rw-r--r--   0        0        0     2049 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/plugins/trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     3948 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/plugins/using_display.py
+-rw-r--r--   0        0        0    16522 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/plugins/valid_oid.py
+-rw-r--r--   0        0        0     3447 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/plugins/valid_script_tag_names.py
+-rw-r--r--   0        0        0     3285 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/plugins/variable_assigned_in_if.py
+-rw-r--r--   0        0        0     1521 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/plugins/vt_file_permissions.py
+-rw-r--r--   0        0        0     2800 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/plugins/vt_placement.py
+-rw-r--r--   0        0        0     9176 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/reporter.py
+-rw-r--r--   0        0        0     2632 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/results.py
+-rw-r--r--   0        0        0     5172 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/runner.py
+-rw-r--r--   0        0        0       22 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0     2921 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/changed_cves.py
+-rw-r--r--   0        0        0     4074 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/changed_oid.py
+-rw-r--r--   0        0        0     5742 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/changed_packages.py
+-rw-r--r--   0        0        0      923 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/marker/__init__.py
+-rw-r--r--   0        0        0     1797 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
+-rw-r--r--   0        0        0     1486 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/marker/added_release.py
+-rw-r--r--   0        0        0     1124 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
+-rw-r--r--   0        0        0     1952 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
+-rw-r--r--   0        0        0     1632 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
+-rw-r--r--   0        0        0     1278 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/marker/marker.py
+-rw-r--r--   0        0        0     2743 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/package.py
+-rw-r--r--   0        0        0     1028 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/common.py
+-rw-r--r--   0        0        0     4616 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/last_modification.py
+-rw-r--r--   0        0        0     8463 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/no_solution.py
+-rw-r--r--   0        0        0     3978 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/standalone_plugins/version_updated.py
+-rw-r--r--   0        0        0     6045 2023-04-12 15:13:31.529378 troubadix-23.4.3/troubadix/troubadix.py
+-rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 troubadix-23.4.3/PKG-INFO
```

### Comparing `troubadix-23.4.2/LICENSE` & `troubadix-23.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/README.md` & `troubadix-23.4.3/README.md`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/pyproject.toml` & `troubadix-23.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troubadix"
-version = "23.4.2"
+version = "23.4.3"
 description = "A linting and QA check tool for NASL files"
 authors = ["Greenbone <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/greenbone/troubadix"
 homepage = "https://github.com/greenbone/troubadix"
```

### Comparing `troubadix-23.4.2/tests/__init__.py` & `troubadix-23.4.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/helper/__init__.py` & `troubadix-23.4.3/tests/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/helper/test_linguistic_exception_handler.py` & `troubadix-23.4.3/tests/helper/test_linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/helper/test_patterns.py` & `troubadix-23.4.3/tests/helper/test_patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/__init__.py` & `troubadix-23.4.3/tests/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/fail.nasl` & `troubadix-23.4.3/tests/plugins/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/fail2.nasl` & `troubadix-23.4.3/tests/plugins/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test.nasl` & `troubadix-23.4.3/tests/plugins/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_badwords.py` & `troubadix-23.4.3/tests/plugins/test_badwords.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_copyright_text.py` & `troubadix-23.4.3/tests/plugins/test_copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_copyright_year.py` & `troubadix-23.4.3/tests/plugins/test_copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_creation_date.py` & `troubadix-23.4.3/tests/plugins/test_creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_cve_format.py` & `troubadix-23.4.3/tests/plugins/test_cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_cvss_format.py` & `troubadix-23.4.3/tests/plugins/test_cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_dependencies.py` & `troubadix-23.4.3/tests/plugins/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_dependency_category_order.py` & `troubadix-23.4.3/tests/plugins/test_dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_deprecated_dependency.py` & `troubadix-23.4.3/tests/plugins/test_deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_deprecated_functions.py` & `troubadix-23.4.3/tests/plugins/test_double_end_points.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,64 +14,58 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from pathlib import Path
 
 from troubadix.plugin import LinterError
-from troubadix.plugins.deprecated_functions import CheckDeprecatedFunctions
+from troubadix.plugins.double_end_points import CheckDoubleEndPoints
 
 from . import PluginTestCase
 
 
-class CheckDeprecatedDependencyTestCase(PluginTestCase):
+class CheckDoubleEndPointsTestCase(PluginTestCase):
     def test_ok(self):
         path = Path("some/file.nasl")
         content = (
             '  script_tag(name:"cvss_base", value:"4.0");\n'
             '  script_tag(name:"summary", value:"Foo Bar.");\n'
-            "  script_category(ACT_ATTACK);\n"
         )
         fake_context = self.create_file_plugin_context(
             nasl_file=path, file_content=content
         )
-        plugin = CheckDeprecatedFunctions(fake_context)
+        plugin = CheckDoubleEndPoints(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_deprecated_functions(self):
-        deprecated_output = {
-            'script_summary(), use script_tag(name:"'
-            'summary", value:"") instead': "script_"
-            "summary('this is not okay!');",
-            "script_id(), use script_oid() with "
-            "the full OID instead": "script_id(123345);",
-            "security_note()": "security_note('nonono!');",
-            "security_warning()": "security_warning('nonono!');",
-            "security_hole()": "security_hole('nonono!');",
-            "script_description()": "script_description('stop it!')",
-            'script_tag(name:"risk_factor", value: '
-            "SEVERITY)": 'script_tag(name:"risk_factor", value: 0.1);',
-            "script_bugtraq_id()": "script_bugtraq_id('00000');",
-        }
+    def test_exclude_inc_file(self):
+        path = Path("some/file.inc")
+        fake_context = self.create_file_plugin_context(nasl_file=path)
+        plugin = CheckDoubleEndPoints(fake_context)
+
+        results = list(plugin.run())
+
+        self.assertEqual(len(results), 0)
+
+    def test_invalid(self):
         path = Path("some/file.nasl")
-        for msg, cont in deprecated_output.items():
-            content = (
-                '  script_tag(name:"cvss_base", value:"4.0");\n'
-                '  script_tag(name:"summary", value:"Foo Bar.");\n'
-                f"  script_category(ACT_ATTACK);\n{cont}\n"
-            )
-            fake_context = self.create_file_plugin_context(
-                nasl_file=path, file_content=content
-            )
-            plugin = CheckDeprecatedFunctions(fake_context)
-
-            results = list(plugin.run())
-
-            self.assertEqual(len(results), 1)
-            self.assertIsInstance(results[0], LinterError)
-            self.assertEqual(
-                f"Found a deprecated function call: {msg}",
-                results[0].message,
-            )
+        content = (
+            '  script_tag(name:"cvss_base", value:"4.0");\n'
+            '  script_tag(name:"summary", value:"Foo Bar...");\n'
+        )
+        fake_context = self.create_file_plugin_context(
+            nasl_file=path, file_content=content
+        )
+        plugin = CheckDoubleEndPoints(fake_context)
+
+        results = list(plugin.run())
+
+        self.assertEqual(len(results), 1)
+        self.assertIsInstance(results[0], LinterError)
+        self.assertEqual(
+            "The script tag 'summary' "
+            "is ending with two or more points: "
+            "'Foo Bar...'.",
+            results[0].message,
+        )
```

### Comparing `troubadix-23.4.2/tests/plugins/test_description.py` & `troubadix-23.4.3/tests/plugins/test_missing_desc_exit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,99 @@
-# Copyright (C) 2022 Greenbone AG
+#  Copyright (c) 2022 Greenbone AG
 #
-# SPDX-License-Identifier: GPL-3.0-or-later
+#  SPDX-License-Identifier: GPL-3.0-or-later
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from pathlib import Path
 
 from troubadix.plugin import LinterError
-from troubadix.plugins.description import CheckDescription
+from troubadix.plugins.missing_desc_exit import CheckMissingDescExit
 
 from . import PluginTestCase
 
 
-class CheckDescriptionTestCase(PluginTestCase):
+class CheckMissingDescExitTestCase(PluginTestCase):
     def test_ok(self):
         nasl_file = Path(__file__).parent / "test.nasl"
         content = (
-            '  script_cve_id("CVE-2021-03807");\n'
+            "if(description) {\n"
+            '  script_tag(name:"cvss_base", value:"4.0");\n'
             '  script_tag(name:"summary", value:"Foo Bar.");\n'
-            '  script_cve_id("CVE-2019-04879");\n'
+            '  script_tag(name:"solution_type", value:"VendorFix");\n'
             '  script_tag(name:"solution", value:"meh");\n'
+            "  exit(0);\n"
+            "}\n"
         )
         fake_context = self.create_file_plugin_context(
             nasl_file=nasl_file, file_content=content
         )
-        plugin = CheckDescription(fake_context)
+        plugin = CheckMissingDescExit(fake_context)
+
+        results = list(plugin.run())
+
+        self.assertEqual(len(results), 0)
+
+    def test_exclude_inc_file(self):
+        path = Path("some/file.inc")
+        fake_context = self.create_file_plugin_context(nasl_file=path)
+        plugin = CheckMissingDescExit(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_description(self):
+    def test_nok(self):
         nasl_file = Path(__file__).parent / "test.nasl"
         content = (
-            '  script_cve_id("CVE-2021-03807");\n'
+            "if(description) {\n"
+            '  script_tag(name:"cvss_base", value:"4.0");\n'
             '  script_tag(name:"summary", value:"Foo Bar.");\n'
-            '  script_cve_id("CVE-2019-04879");\n'
+            '  script_tag(name:"solution_type", value:"VendorFix");\n'
             '  script_tag(name:"solution", value:"meh");\n'
-            '  script_description("TestTest");\n'
+            "}\n"
         )
-
         fake_context = self.create_file_plugin_context(
             nasl_file=nasl_file, file_content=content
         )
-        plugin = CheckDescription(fake_context)
+        plugin = CheckMissingDescExit(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
         self.assertEqual(
-            "VT/Include is using deprecated 'script_description'",
+            "No mandatory exit(0); found in the description block.",
             results[0].message,
         )
 
-    def test_description2(self):
+    def test_nok2(self):
         nasl_file = Path(__file__).parent / "test.nasl"
         content = (
-            '  script_cve_id("CVE-2021-03807");\n'
+            '  script_tag(name:"cvss_base", value:"4.0");\n'
             '  script_tag(name:"summary", value:"Foo Bar.");\n'
-            '  TTTTTTTscrIpt_descriPtion("TestTest");\n'
-            '  script_cve_id("CVE-2019-04879");\n'
+            '  script_tag(name:"solution_type", value:"VendorFix");\n'
             '  script_tag(name:"solution", value:"meh");\n'
         )
-
         fake_context = self.create_file_plugin_context(
             nasl_file=nasl_file, file_content=content
         )
-        plugin = CheckDescription(fake_context)
+        plugin = CheckMissingDescExit(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
         self.assertEqual(
-            "VT/Include is using deprecated 'script_description'",
+            "No description block extracted/found.",
             results[0].message,
         )
```

### Comparing `troubadix-23.4.2/tests/plugins/test_double_end_points.py` & `troubadix-23.4.3/tests/plugins/test_get_kb_on_services.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,67 @@
-# Copyright (C) 2022 Greenbone AG
+#  Copyright (c) 2022 Greenbone AG
 #
-# SPDX-License-Identifier: GPL-3.0-or-later
+#  SPDX-License-Identifier: GPL-3.0-or-later
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from pathlib import Path
 
 from troubadix.plugin import LinterError
-from troubadix.plugins.double_end_points import CheckDoubleEndPoints
+from troubadix.plugins.get_kb_on_services import CheckGetKBOnServices
 
 from . import PluginTestCase
 
 
-class CheckDoubleEndPointsTestCase(PluginTestCase):
+class CheckGetKBOnServicesTestCase(PluginTestCase):
     def test_ok(self):
         path = Path("some/file.nasl")
         content = (
+            '  script_oid("1.2.3.4.5.6.78909.8.7.000000");\n'
             '  script_tag(name:"cvss_base", value:"4.0");\n'
-            '  script_tag(name:"summary", value:"Foo Bar.");\n'
         )
         fake_context = self.create_file_plugin_context(
             nasl_file=path, file_content=content
         )
-        plugin = CheckDoubleEndPoints(fake_context)
+        plugin = CheckGetKBOnServices(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
     def test_exclude_inc_file(self):
         path = Path("some/file.inc")
         fake_context = self.create_file_plugin_context(nasl_file=path)
-        plugin = CheckDoubleEndPoints(fake_context)
+        plugin = CheckGetKBOnServices(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_invalid(self):
+    def test_ok_no_script_oid(self):
         path = Path("some/file.nasl")
         content = (
             '  script_tag(name:"cvss_base", value:"4.0");\n'
-            '  script_tag(name:"summary", value:"Foo Bar...");\n'
+            'port = get_kb_item("Services/www");\n'
+            'port = get_kb_list("Services/udp/upnp");\n'
         )
+
         fake_context = self.create_file_plugin_context(
             nasl_file=path, file_content=content
         )
-        plugin = CheckDoubleEndPoints(fake_context)
+        plugin = CheckGetKBOnServices(fake_context)
 
         results = list(plugin.run())
 
-        self.assertEqual(len(results), 1)
+        self.assertEqual(len(results), 2)
         self.assertIsInstance(results[0], LinterError)
-        self.assertEqual(
-            "The script tag 'summary' "
-            "is ending with two or more points: "
-            "'Foo Bar...'.",
-            results[0].message,
-        )
```

### Comparing `troubadix-23.4.2/tests/plugins/test_duplicate_oid.py` & `troubadix-23.4.3/tests/plugins/test_duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_duplicated_script_tags.py` & `troubadix-23.4.3/tests/plugins/test_duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_encoding.py` & `troubadix-23.4.3/tests/plugins/test_encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/fail_bad_new_line.nasl` & `troubadix-23.4.3/tests/plugins/test_files/fail_bad_new_line.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/fail_name_and_copyright_newline.nasl` & `troubadix-23.4.3/tests/plugins/test_files/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/fail_name_newline.nasl` & `troubadix-23.4.3/tests/plugins/test_files/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/fail_permissions.nasl` & `troubadix-23.4.3/tests/plugins/test_files/fail_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/fail.nasl` & `troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl` & `troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl` & `troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl` & `troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/runner/fail.nasl` & `troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/runner/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl` & `troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/runner/test.nasl` & `troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/runner/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl` & `troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/test.inc` & `troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/test.inc`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/nasl/21.04/test.nasl` & `troubadix-23.4.3/tests/plugins/test_files/nasl/21.04/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/nasl/warning.nasl` & `troubadix-23.4.3/tests/plugins/test_files/nasl/warning.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/ok_permissions.nasl` & `troubadix-23.4.3/tests/plugins/test_files/ok_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_files/test_oid.nasl` & `troubadix-23.4.3/tests/plugins/test_files/test_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_forking_nasl_functions.py` & `troubadix-23.4.3/tests/plugins/test_forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_get_kb_on_services.py` & `troubadix-23.4.3/tests/plugins/test_script_tag_form.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,90 @@
-#  Copyright (c) 2022 Greenbone AG
+# Copyright (C) 2022 Greenbone AG
 #
-#  SPDX-License-Identifier: GPL-3.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 #
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from pathlib import Path
 
+from tests.plugins import PluginTestCase
 from troubadix.plugin import LinterError
-from troubadix.plugins.get_kb_on_services import CheckGetKBOnServices
+from troubadix.plugins.script_tag_form import CheckScriptTagForm
 
-from . import PluginTestCase
 
+class CheckScriptTagFormTestCase(PluginTestCase):
+    path = Path("some/file.nasl")
 
-class CheckGetKBOnServicesTestCase(PluginTestCase):
     def test_ok(self):
-        path = Path("some/file.nasl")
         content = (
-            '  script_oid("1.2.3.4.5.6.78909.8.7.000000");\n'
-            '  script_tag(name:"cvss_base", value:"4.0");\n'
+            '  script_tag(name: "foo", value:"bar");\n'
+            '  script_tag(name: "foo", value:42);\n'
         )
         fake_context = self.create_file_plugin_context(
-            nasl_file=path, file_content=content
+            nasl_file=self.path, file_content=content
         )
-        plugin = CheckGetKBOnServices(fake_context)
+        plugin = CheckScriptTagForm(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
     def test_exclude_inc_file(self):
         path = Path("some/file.inc")
         fake_context = self.create_file_plugin_context(nasl_file=path)
-        plugin = CheckGetKBOnServices(fake_context)
+        plugin = CheckScriptTagForm(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_ok_no_script_oid(self):
-        path = Path("some/file.nasl")
-        content = (
-            '  script_tag(name:"cvss_base", value:"4.0");\n'
-            'port = get_kb_item("Services/www");\n'
-            'port = get_kb_list("Services/udp/upnp");\n'
+    def test_wrong_name(self):
+        content = '  script_tag(nammmme: "foo", value:"bar");\n'
+        fake_context = self.create_file_plugin_context(
+            nasl_file=self.path, file_content=content
+        )
+        plugin = CheckScriptTagForm(fake_context)
+
+        results = list(plugin.run())
+
+        self.assertEqual(len(results), 1)
+        self.assertIsInstance(results[0], LinterError)
+        self.assertEqual(
+            'script_tag(nammmme: "foo", value:"bar");: does not conform to'
+            ' script_tag(name:"<name>", value:<value>);',
+            results[0].message,
         )
 
+    def test_wrong_value(self):
+        content = '  script_tag(name: "foo", valueeeee:"bar");\n'
+        fake_context = self.create_file_plugin_context(
+            nasl_file=self.path, file_content=content
+        )
+        plugin = CheckScriptTagForm(fake_context)
+
+        results = list(plugin.run())
+
+        self.assertEqual(len(results), 1)
+        self.assertIsInstance(results[0], LinterError)
+
+    def test_wrong_missing_parameters(self):
+        content = '  script_tag("foo", "bar");\n'
         fake_context = self.create_file_plugin_context(
-            nasl_file=path, file_content=content
+            nasl_file=self.path, file_content=content
         )
-        plugin = CheckGetKBOnServices(fake_context)
+        plugin = CheckScriptTagForm(fake_context)
 
         results = list(plugin.run())
 
-        self.assertEqual(len(results), 2)
+        self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
```

### Comparing `troubadix-23.4.2/tests/plugins/test_grammar.py` & `troubadix-23.4.3/tests/plugins/test_grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_http_links_in_tags.py` & `troubadix-23.4.3/tests/plugins/test_http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_illegal_characters.py` & `troubadix-23.4.3/tests/plugins/test_illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_log_messages.py` & `troubadix-23.4.3/tests/plugins/test_log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_malformed_dependencies.py` & `troubadix-23.4.3/tests/plugins/test_malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_misplaced_compare_in_if.py` & `troubadix-23.4.3/tests/plugins/test_misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_missing_desc_exit.py` & `troubadix-23.4.3/tests/plugins/test_valid_script_tag_names.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,87 +13,94 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from pathlib import Path
 
 from troubadix.plugin import LinterError
-from troubadix.plugins.missing_desc_exit import CheckMissingDescExit
+from troubadix.plugins.valid_script_tag_names import CheckValidScriptTagNames
 
 from . import PluginTestCase
 
 
-class CheckMissingDescExitTestCase(PluginTestCase):
-    def test_ok(self):
+class CheckValidScriptTagNamesTestCase(PluginTestCase):
+    def test_ok_nonewline(self):
         nasl_file = Path(__file__).parent / "test.nasl"
         content = (
-            "if(description) {\n"
             '  script_tag(name:"cvss_base", value:"4.0");\n'
             '  script_tag(name:"summary", value:"Foo Bar.");\n'
             '  script_tag(name:"solution_type", value:"VendorFix");\n'
             '  script_tag(name:"solution", value:"meh");\n'
-            "  exit(0);\n"
-            "}\n"
+            '  script_tag(name:"vuldetect", value:"Without newline");\n'
         )
         fake_context = self.create_file_plugin_context(
             nasl_file=nasl_file, file_content=content
         )
-        plugin = CheckMissingDescExit(fake_context)
+        plugin = CheckValidScriptTagNames(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_exclude_inc_file(self):
-        path = Path("some/file.inc")
-        fake_context = self.create_file_plugin_context(nasl_file=path)
-        plugin = CheckMissingDescExit(fake_context)
+    def test_ok_newline(self):
+        nasl_file = Path(__file__).parent / "test.nasl"
+        content = (
+            '  script_tag(name:"cvss_base", value:"4.0");\n'
+            '  script_tag(name:"summary", value:"Foo Bar.");\n'
+            '  script_tag(name:"solution_type", value:"VendorFix");\n'
+            '  script_tag(name:"solution", value:"meh");\n'
+            '  script_tag(name:"vuldetect", value:"With\nnewline");\n'
+        )
+        fake_context = self.create_file_plugin_context(
+            nasl_file=nasl_file, file_content=content
+        )
+        plugin = CheckValidScriptTagNames(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_nok(self):
+    def test_nok_nonewline(self):
         nasl_file = Path(__file__).parent / "test.nasl"
         content = (
-            "if(description) {\n"
             '  script_tag(name:"cvss_base", value:"4.0");\n'
             '  script_tag(name:"summary", value:"Foo Bar.");\n'
             '  script_tag(name:"solution_type", value:"VendorFix");\n'
             '  script_tag(name:"solution", value:"meh");\n'
-            "}\n"
+            '  script_tag(name:"vulndetect", value:"Without newline");\n'
         )
         fake_context = self.create_file_plugin_context(
             nasl_file=nasl_file, file_content=content
         )
-        plugin = CheckMissingDescExit(fake_context)
+        plugin = CheckValidScriptTagNames(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
         self.assertEqual(
-            "No mandatory exit(0); found in the description block.",
+            "The script_tag name 'vulndetect' is not allowed.",
             results[0].message,
         )
 
-    def test_nok2(self):
+    def test_nok_newline(self):
         nasl_file = Path(__file__).parent / "test.nasl"
         content = (
             '  script_tag(name:"cvss_base", value:"4.0");\n'
             '  script_tag(name:"summary", value:"Foo Bar.");\n'
             '  script_tag(name:"solution_type", value:"VendorFix");\n'
             '  script_tag(name:"solution", value:"meh");\n'
+            '  script_tag(name:"vulndetect", value:"With\nnewline");\n'
         )
         fake_context = self.create_file_plugin_context(
             nasl_file=nasl_file, file_content=content
         )
-        plugin = CheckMissingDescExit(fake_context)
+        plugin = CheckValidScriptTagNames(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
         self.assertEqual(
-            "No description block extracted/found.",
+            "The script_tag name 'vulndetect' is not allowed.",
             results[0].message,
         )
```

### Comparing `troubadix-23.4.2/tests/plugins/test_missing_tag_solution.py` & `troubadix-23.4.3/tests/plugins/test_missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_newlines.py` & `troubadix-23.4.3/tests/plugins/test_newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_overlong_script_tags.py` & `troubadix-23.4.3/tests/plugins/test_overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_prod_svc_detect_in_vulnvt.py` & `troubadix-23.4.3/tests/plugins/test_prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_qod.py` & `troubadix-23.4.3/tests/plugins/test_qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_reporting_consistency.py` & `troubadix-23.4.3/tests/plugins/test_reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_risk_factor.py` & `troubadix-23.4.3/tests/plugins/test_script_tag_whitespaces.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,53 +13,75 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from pathlib import Path
 
+from tests.plugins import PluginTestCase
 from troubadix.plugin import LinterError
-from troubadix.plugins.risk_factor import CheckRiskFactor
+from troubadix.plugins.script_tag_whitespaces import CheckScriptTagWhitespaces
 
-from . import PluginTestCase
 
+class CheckScriptTagWhitespacesTestCase(PluginTestCase):
+    path = Path("some/file.nasl")
 
-class RiskFactorTestCase(PluginTestCase):
     def test_ok(self):
-        path = Path(__file__).parent / "test.nasl"
-        content = (
-            '  script_tag(name:"cvss_base", value:"4.0");\n'
-            '  script_tag(name:"summary", value:"Foo Bar.");\n'
-            '  script_tag(name:"solution_type", value:"VendorFix");\n'
-            '  script_tag(name:"solution", value:"meh");\n'
-        )
+        content = '  script_tag(name: "foo", value:"bar");\n'
         fake_context = self.create_file_plugin_context(
-            nasl_file=path, file_content=content
+            nasl_file=self.path, file_content=content
         )
-        plugin = CheckRiskFactor(fake_context)
+        plugin = CheckScriptTagWhitespaces(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_risk_factor(self):
-        path = Path(__file__).parent / "test.nasl"
-        content = (
-            '  script_tag(name:"cvss_base", value:"4.0");\n'
-            '  script_tag(name:"summary", value:"Foo Bar.");\n'
-            '  script_tag(name:"solution_type", value:"VendorFix");\n'
-            '  script_tag(name:"risk_factor", value:"TestTest");\n'
-        )
+    def test_exclude_inc_file(self):
+        path = Path("some/file.inc")
+        fake_context = self.create_file_plugin_context(nasl_file=path)
+        plugin = CheckScriptTagWhitespaces(fake_context)
+
+        results = list(plugin.run())
+
+        self.assertEqual(len(results), 0)
+
+    def test_leading_whitespace(self):
+        content = '  script_tag(name: "foo", value:" bar");\n'
         fake_context = self.create_file_plugin_context(
-            nasl_file=path, file_content=content
+            nasl_file=self.path, file_content=content
         )
-        plugin = CheckRiskFactor(fake_context)
+        plugin = CheckScriptTagWhitespaces(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
-
         self.assertIsInstance(results[0], LinterError)
         self.assertEqual(
-            'Deprecated function "risk factor" found: TestTest',
+            'script_tag(name: "foo", value:" bar");: value contains a leading'
+            " or trailing whitespace character",
             results[0].message,
         )
+
+    def test_trailing_whitespace(self):
+        content = '  script_tag(name: "foo", value:"bar\n");\n'
+        fake_context = self.create_file_plugin_context(
+            nasl_file=self.path, file_content=content
+        )
+        plugin = CheckScriptTagWhitespaces(fake_context)
+
+        results = list(plugin.run())
+
+        self.assertEqual(len(results), 1)
+        self.assertIsInstance(results[0], LinterError)
+
+    def test_trailing_whitespace_newline(self):
+        content = '  script_tag(name: "foo", value:"foo\nbar\n");\n'
+        fake_context = self.create_file_plugin_context(
+            nasl_file=self.path, file_content=content
+        )
+        plugin = CheckScriptTagWhitespaces(fake_context)
+
+        results = list(plugin.run())
+
+        self.assertEqual(len(results), 1)
+        self.assertIsInstance(results[0], LinterError)
```

### Comparing `troubadix-23.4.2/tests/plugins/test_script_add_preference_type.py` & `troubadix-23.4.3/tests/plugins/test_script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_script_calls_empty_values.py` & `troubadix-23.4.3/tests/plugins/test_script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_script_calls_recommended.py` & `troubadix-23.4.3/tests/plugins/test_script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_script_category.py` & `troubadix-23.4.3/tests/plugins/test_script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_script_copyright.py` & `troubadix-23.4.3/tests/plugins/test_script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_script_family.py` & `troubadix-23.4.3/tests/plugins/test_script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_script_tag_form.py` & `troubadix-23.4.3/tests/plugins/test_script_xref_form.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,76 +15,73 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from pathlib import Path
 
 from tests.plugins import PluginTestCase
 from troubadix.plugin import LinterError
-from troubadix.plugins.script_tag_form import CheckScriptTagForm
+from troubadix.plugins.script_xref_form import CheckScriptXrefForm
 
 
-class CheckScriptTagFormTestCase(PluginTestCase):
+class CheckScriptXrefFormTestCase(PluginTestCase):
     path = Path("some/file.nasl")
 
     def test_ok(self):
-        content = (
-            '  script_tag(name: "foo", value:"bar");\n'
-            '  script_tag(name: "foo", value:42);\n'
-        )
+        content = '  script_xref(name: "foo", value:"bar");\n'
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptTagForm(fake_context)
+        plugin = CheckScriptXrefForm(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
     def test_exclude_inc_file(self):
         path = Path("some/file.inc")
         fake_context = self.create_file_plugin_context(nasl_file=path)
-        plugin = CheckScriptTagForm(fake_context)
+        plugin = CheckScriptXrefForm(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
     def test_wrong_name(self):
-        content = '  script_tag(nammmme: "foo", value:"bar");\n'
+        content = '  script_xref(nammmme: "foo", value:"bar");\n'
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptTagForm(fake_context)
+        plugin = CheckScriptXrefForm(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
         self.assertEqual(
-            'script_tag(nammmme: "foo", value:"bar");: does not conform to'
-            ' script_tag(name:"<name>", value:<value>);',
+            'script_xref(nammmme: "foo", value:"bar");: does not conform to'
+            ' script_xref(name:"<name>", value:<value>);',
             results[0].message,
         )
 
     def test_wrong_value(self):
-        content = '  script_tag(name: "foo", valueeeee:"bar");\n'
+        content = '  script_xref(name: "foo", valueeeee:"bar");\n'
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptTagForm(fake_context)
+        plugin = CheckScriptXrefForm(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
 
     def test_wrong_missing_parameters(self):
-        content = '  script_tag("foo", "bar");\n'
+        content = '  script_xref("foo", "bar");\n'
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptTagForm(fake_context)
+        plugin = CheckScriptXrefForm(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
```

### Comparing `troubadix-23.4.2/tests/plugins/test_script_tag_whitespaces.py` & `troubadix-23.4.3/tests/plugins/test_script_tags_mandatory.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,73 +15,81 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from pathlib import Path
 
 from tests.plugins import PluginTestCase
 from troubadix.plugin import LinterError
-from troubadix.plugins.script_tag_whitespaces import CheckScriptTagWhitespaces
+from troubadix.plugins.script_tags_mandatory import CheckScriptTagsMandatory
 
 
-class CheckScriptTagWhitespacesTestCase(PluginTestCase):
+class CheckScriptTagsMandatoryTestCase(PluginTestCase):
     path = Path("some/file.nasl")
 
     def test_ok(self):
-        content = '  script_tag(name: "foo", value:"bar");\n'
+        content = (
+            "  script_name('foo');\n"
+            "  script_version(1234-56-78T90:98:76+5432);\n"
+            "  script_category(ACT_INIT);\n"
+            "  script_family(FAMILY);\n"
+            '  script_copyright("COPYRIGHT");\n'
+            '  script_tag(name:"summary", value:"foo");\n'
+        )
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptTagWhitespaces(fake_context)
+        plugin = CheckScriptTagsMandatory(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
     def test_exclude_inc_file(self):
         path = Path("some/file.inc")
         fake_context = self.create_file_plugin_context(nasl_file=path)
-        plugin = CheckScriptTagWhitespaces(fake_context)
+        plugin = CheckScriptTagsMandatory(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_leading_whitespace(self):
-        content = '  script_tag(name: "foo", value:" bar");\n'
+    def test_missing_tags_calls(self):
+        content = '  script_xref(name: "URL", value:"");\n'
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptTagWhitespaces(fake_context)
+        plugin = CheckScriptTagsMandatory(fake_context)
 
         results = list(plugin.run())
 
-        self.assertEqual(len(results), 1)
+        self.assertEqual(len(results), 6)
         self.assertIsInstance(results[0], LinterError)
-        self.assertEqual(
-            'script_tag(name: "foo", value:" bar");: value contains a leading'
-            " or trailing whitespace character",
-            results[0].message,
-        )
 
-    def test_trailing_whitespace(self):
-        content = '  script_tag(name: "foo", value:"bar\n");\n'
+    def test_missing_tags(self):
+        content = (
+            "  script_name('foo');\n"
+            "  script_version(1234-56-78T90:98:76+5432);\n"
+            "  script_category(ACT_INIT);\n"
+            "  script_family(FAMILY);\n"
+            '  script_copyright("COPYRIGHT");\n'
+        )
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptTagWhitespaces(fake_context)
+        plugin = CheckScriptTagsMandatory(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
 
-    def test_trailing_whitespace_newline(self):
-        content = '  script_tag(name: "foo", value:"foo\nbar\n");\n'
+    def test_missing_calls(self):
+        content = '  script_tag(name:"summary", value:"foo");\n'
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptTagWhitespaces(fake_context)
+        plugin = CheckScriptTagsMandatory(fake_context)
 
         results = list(plugin.run())
 
-        self.assertEqual(len(results), 1)
+        self.assertEqual(len(results), 5)
         self.assertIsInstance(results[0], LinterError)
```

### Comparing `troubadix-23.4.2/tests/plugins/test_script_tags_mandatory.py` & `troubadix-23.4.3/tests/plugins/test_spelling.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,95 +1,83 @@
-# Copyright (C) 2022 Greenbone AG
+#  Copyright (c) 2022 Greenbone AG
 #
-# SPDX-License-Identifier: GPL-3.0-or-later
+#  SPDX-License-Identifier: GPL-3.0-or-later
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from pathlib import Path
 
-from tests.plugins import PluginTestCase
 from troubadix.plugin import LinterError
-from troubadix.plugins.script_tags_mandatory import CheckScriptTagsMandatory
+from troubadix.plugins.spelling import CheckSpelling
 
+from . import PluginTestCase
 
-class CheckScriptTagsMandatoryTestCase(PluginTestCase):
-    path = Path("some/file.nasl")
 
+class CheckSpellingTestCase(PluginTestCase):
     def test_ok(self):
-        content = (
-            "  script_name('foo');\n"
-            "  script_version(1234-56-78T90:98:76+5432);\n"
-            "  script_category(ACT_INIT);\n"
-            "  script_family(FAMILY);\n"
-            '  script_copyright("COPYRIGHT");\n'
-            '  script_tag(name:"summary", value:"foo");\n'
-        )
-        fake_context = self.create_file_plugin_context(
-            nasl_file=self.path, file_content=content
-        )
-        plugin = CheckScriptTagsMandatory(fake_context)
+        nasl_file = Path(__file__).parent / "test.nasl"
+        fake_context = self.create_files_plugin_context(nasl_files=[nasl_file])
+        plugin = CheckSpelling(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_exclude_inc_file(self):
-        path = Path("some/file.inc")
-        fake_context = self.create_file_plugin_context(nasl_file=path)
-        plugin = CheckScriptTagsMandatory(fake_context)
+    def test_nok(self):
+        nasl_file = Path(__file__).parent / "test_files" / "fail_spelling.nasl"
+        fake_context = self.create_files_plugin_context(nasl_files=[nasl_file])
+        plugin = CheckSpelling(fake_context)
 
         results = list(plugin.run())
 
-        self.assertEqual(len(results), 0)
-
-    def test_missing_tags_calls(self):
-        content = '  script_xref(name: "URL", value:"");\n'
-        fake_context = self.create_file_plugin_context(
-            nasl_file=self.path, file_content=content
-        )
-        plugin = CheckScriptTagsMandatory(fake_context)
-
-        results = list(plugin.run())
+        self.assertEqual(len(results), 3)
 
-        self.assertEqual(len(results), 6)
         self.assertIsInstance(results[0], LinterError)
-
-    def test_missing_tags(self):
-        content = (
-            "  script_name('foo');\n"
-            "  script_version(1234-56-78T90:98:76+5432);\n"
-            "  script_category(ACT_INIT);\n"
-            "  script_family(FAMILY);\n"
-            '  script_copyright("COPYRIGHT");\n'
+        self.assertEqual(
+            f"{nasl_file}:1: soltuion ==> solution",
+            results[0].message,
         )
-        fake_context = self.create_file_plugin_context(
-            nasl_file=self.path, file_content=content
+
+        self.assertIsInstance(results[1], LinterError)
+        self.assertEqual(
+            f"{nasl_file}:1: aviaalable ==> available",
+            results[1].message,
         )
-        plugin = CheckScriptTagsMandatory(fake_context)
 
-        results = list(plugin.run())
+        self.assertIsInstance(results[2], LinterError)
+        self.assertEqual(
+            f"{nasl_file}:2: upated ==> updated",
+            results[2].message,
+        )
 
-        self.assertEqual(len(results), 1)
-        self.assertIsInstance(results[0], LinterError)
+    def test_local_files_nok(self):
+        codespell_additions = Path("codespell.additions")
+        codespell_additions.write_text("", encoding="utf-8")
 
-    def test_missing_calls(self):
-        content = '  script_tag(name:"summary", value:"foo");\n'
-        fake_context = self.create_file_plugin_context(
-            nasl_file=self.path, file_content=content
-        )
-        plugin = CheckScriptTagsMandatory(fake_context)
+        nasl_file = Path(__file__).parent / "test_files" / "fail_spelling.nasl"
+        fake_context = self.create_files_plugin_context(nasl_files=[nasl_file])
+        plugin = CheckSpelling(fake_context)
 
         results = list(plugin.run())
 
-        self.assertEqual(len(results), 5)
+        codespell_additions.unlink()
+
+        self.assertEqual(len(results), 2)
         self.assertIsInstance(results[0], LinterError)
+        self.assertEqual(
+            f"{nasl_file}:1: soltuion ==> solution",
+            results[0].message,
+        )
+        self.assertEqual(
+            f"{nasl_file}:2: upated ==> updated",
+            results[1].message,
+        )
```

### Comparing `troubadix-23.4.2/tests/plugins/test_script_version_and_last_modification_tags.py` & `troubadix-23.4.3/tests/plugins/test_script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_script_xref_form.py` & `troubadix-23.4.3/tests/plugins/test_script_xref_url.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,73 +15,49 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from pathlib import Path
 
 from tests.plugins import PluginTestCase
 from troubadix.plugin import LinterError
-from troubadix.plugins.script_xref_form import CheckScriptXrefForm
+from troubadix.plugins.script_xref_url import CheckScriptXrefUrl
 
 
-class CheckScriptXrefFormTestCase(PluginTestCase):
+class CheckScriptXrefUrlTestCase(PluginTestCase):
     path = Path("some/file.nasl")
 
     def test_ok(self):
-        content = '  script_xref(name: "foo", value:"bar");\n'
+        content = '  script_xref(name:"URL", value:"http://www.example.com");\n'
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptXrefForm(fake_context)
+        plugin = CheckScriptXrefUrl(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
     def test_exclude_inc_file(self):
         path = Path("some/file.inc")
         fake_context = self.create_file_plugin_context(nasl_file=path)
-        plugin = CheckScriptXrefForm(fake_context)
+        plugin = CheckScriptXrefUrl(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_wrong_name(self):
-        content = '  script_xref(nammmme: "foo", value:"bar");\n'
+    def test_invalid_url(self):
+        content = '  script_xref(name:"URL", value:"www.example.com");\n'
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptXrefForm(fake_context)
+        plugin = CheckScriptXrefUrl(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
         self.assertEqual(
-            'script_xref(nammmme: "foo", value:"bar");: does not conform to'
-            ' script_xref(name:"<name>", value:<value>);',
+            'script_xref(name:"URL", value:"www.example.com");: Invalid URL'
+            " value",
             results[0].message,
         )
-
-    def test_wrong_value(self):
-        content = '  script_xref(name: "foo", valueeeee:"bar");\n'
-        fake_context = self.create_file_plugin_context(
-            nasl_file=self.path, file_content=content
-        )
-        plugin = CheckScriptXrefForm(fake_context)
-
-        results = list(plugin.run())
-
-        self.assertEqual(len(results), 1)
-        self.assertIsInstance(results[0], LinterError)
-
-    def test_wrong_missing_parameters(self):
-        content = '  script_xref("foo", "bar");\n'
-        fake_context = self.create_file_plugin_context(
-            nasl_file=self.path, file_content=content
-        )
-        plugin = CheckScriptXrefForm(fake_context)
-
-        results = list(plugin.run())
-
-        self.assertEqual(len(results), 1)
-        self.assertIsInstance(results[0], LinterError)
```

### Comparing `troubadix-23.4.2/tests/plugins/test_script_xref_url.py` & `troubadix-23.4.3/tests/plugins/test_vt_file_permissions.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,51 +13,47 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from pathlib import Path
 
-from tests.plugins import PluginTestCase
 from troubadix.plugin import LinterError
-from troubadix.plugins.script_xref_url import CheckScriptXrefUrl
+from troubadix.plugins.vt_file_permissions import CheckVTFilePermissions
 
+from . import PluginTestCase
 
-class CheckScriptXrefUrlTestCase(PluginTestCase):
-    path = Path("some/file.nasl")
 
+class CheckVTFilePermissionsTestCase(PluginTestCase):
     def test_ok(self):
-        content = '  script_xref(name:"URL", value:"http://www.example.com");\n'
         fake_context = self.create_file_plugin_context(
-            nasl_file=self.path, file_content=content
+            nasl_file=Path(__file__).parent
+            / "test_files"
+            / "ok_permissions.nasl"
         )
-        plugin = CheckScriptXrefUrl(fake_context)
 
-        results = list(plugin.run())
-
-        self.assertEqual(len(results), 0)
-
-    def test_exclude_inc_file(self):
-        path = Path("some/file.inc")
-        fake_context = self.create_file_plugin_context(nasl_file=path)
-        plugin = CheckScriptXrefUrl(fake_context)
+        plugin = CheckVTFilePermissions(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_invalid_url(self):
-        content = '  script_xref(name:"URL", value:"www.example.com");\n'
+    def test_nok(self):
         fake_context = self.create_file_plugin_context(
-            nasl_file=self.path, file_content=content
+            nasl_file=Path(__file__).parent
+            / "test_files"
+            / "fail_permissions.nasl"
         )
-        plugin = CheckScriptXrefUrl(fake_context)
+
+        plugin = CheckVTFilePermissions(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
         self.assertEqual(
-            'script_xref(name:"URL", value:"www.example.com");: Invalid URL'
-            " value",
             results[0].message,
+            "VT has invalid file permissions: -rwxr-xr-x.\n"
+            "NASL scripts must not be executable.\n"
+            "Typical file permissions are '644' (-rw-r--r-) "
+            "and `664` (-rw-rw-r-)",
         )
```

### Comparing `troubadix-23.4.2/tests/plugins/test_security_messages.py` & `troubadix-23.4.3/tests/plugins/test_security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_set_get_kb_calls.py` & `troubadix-23.4.3/tests/plugins/test_set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_solution_text.py` & `troubadix-23.4.3/tests/plugins/test_solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_solution_type.py` & `troubadix-23.4.3/tests/plugins/test_solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_spelling.py` & `troubadix-23.4.3/tests/plugins/test_tabs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,57 @@
-#  Copyright (c) 2022 Greenbone AG
+# Copyright (C) 2022 Greenbone AG
 #
-#  SPDX-License-Identifier: GPL-3.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 #
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from pathlib import Path
 
 from troubadix.plugin import LinterError
-from troubadix.plugins.spelling import CheckSpelling
+from troubadix.plugins.tabs import CheckTabs
 
 from . import PluginTestCase
 
 
-class CheckSpellingTestCase(PluginTestCase):
+class CheckTabsTestCase(PluginTestCase):
     def test_ok(self):
-        nasl_file = Path(__file__).parent / "test.nasl"
-        fake_context = self.create_files_plugin_context(nasl_files=[nasl_file])
-        plugin = CheckSpelling(fake_context)
+        path = Path("tests/file.nasl")
+        content = "What ever."
+        fake_context = self.create_file_plugin_context(
+            nasl_file=path, lines=content.splitlines()
+        )
+        plugin = CheckTabs(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_nok(self):
-        nasl_file = Path(__file__).parent / "test_files" / "fail_spelling.nasl"
-        fake_context = self.create_files_plugin_context(nasl_files=[nasl_file])
-        plugin = CheckSpelling(fake_context)
+    def test_with_tabs(self):
+        path = Path("tests/file.nasl")
 
-        results = list(plugin.run())
+        content = "\t\t\t\t\t\t\n1234456789"
 
-        self.assertEqual(len(results), 3)
-
-        self.assertIsInstance(results[0], LinterError)
-        self.assertEqual(
-            f"{nasl_file}:1: soltuion ==> solution",
-            results[0].message,
+        fake_context = self.create_file_plugin_context(
+            nasl_file=path, lines=content.splitlines()
         )
-
-        self.assertIsInstance(results[1], LinterError)
-        self.assertEqual(
-            f"{nasl_file}:1: aviaalable ==> available",
-            results[1].message,
-        )
-
-        self.assertIsInstance(results[2], LinterError)
-        self.assertEqual(
-            f"{nasl_file}:2: upated ==> updated",
-            results[2].message,
-        )
-
-    def test_local_files_nok(self):
-        codespell_additions = Path("codespell.additions")
-        codespell_additions.write_text("", encoding="utf-8")
-
-        nasl_file = Path(__file__).parent / "test_files" / "fail_spelling.nasl"
-        fake_context = self.create_files_plugin_context(nasl_files=[nasl_file])
-        plugin = CheckSpelling(fake_context)
+        plugin = CheckTabs(fake_context)
 
         results = list(plugin.run())
+        self.assertEqual(len(results), 1)
 
-        codespell_additions.unlink()
-
-        self.assertEqual(len(results), 2)
         self.assertIsInstance(results[0], LinterError)
         self.assertEqual(
-            f"{nasl_file}:1: soltuion ==> solution",
             results[0].message,
+            "VT uses tabs instead of spaces.",
         )
-        self.assertEqual(
-            f"{nasl_file}:2: upated ==> updated",
-            results[1].message,
-        )
+        self.assertEqual(results[0].line, 1)
```

### Comparing `troubadix-23.4.2/tests/plugins/test_todo_tbd.py` & `troubadix-23.4.3/tests/plugins/test_todo_tbd.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_trailing_spaces_tabs.py` & `troubadix-23.4.3/tests/plugins/test_trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_using_display.py` & `troubadix-23.4.3/tests/plugins/test_using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_valid_oid.py` & `troubadix-23.4.3/tests/plugins/test_valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/plugins/test_vt_file_permissions.py` & `troubadix-23.4.3/troubadix/plugins/script_xref_form.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,49 +11,42 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+import re
 from pathlib import Path
+from typing import Iterator
 
-from troubadix.plugin import LinterError
-from troubadix.plugins.vt_file_permissions import CheckVTFilePermissions
+from troubadix.helper.patterns import get_xref_pattern
+from troubadix.plugin import FileContentPlugin, LinterError, LinterResult
 
-from . import PluginTestCase
 
+class CheckScriptXrefForm(FileContentPlugin):
+    name = "check_script_xref_form"
 
-class CheckVTFilePermissionsTestCase(PluginTestCase):
-    def test_ok(self):
-        fake_context = self.create_file_plugin_context(
-            nasl_file=Path(__file__).parent
-            / "test_files"
-            / "ok_permissions.nasl"
-        )
-
-        plugin = CheckVTFilePermissions(fake_context)
-
-        results = list(plugin.run())
-
-        self.assertEqual(len(results), 0)
-
-    def test_nok(self):
-        fake_context = self.create_file_plugin_context(
-            nasl_file=Path(__file__).parent
-            / "test_files"
-            / "fail_permissions.nasl"
-        )
-
-        plugin = CheckVTFilePermissions(fake_context)
-
-        results = list(plugin.run())
-
-        self.assertEqual(len(results), 1)
-        self.assertIsInstance(results[0], LinterError)
-        self.assertEqual(
-            results[0].message,
-            "VT has invalid file permissions: -rwxr-xr-x.\n"
-            "NASL scripts must not be executable.\n"
-            "Typical file permissions are '644' (-rw-r--r-) "
-            "and `664` (-rw-rw-r-)",
-        )
+    def check_content(
+        self,
+        nasl_file: Path,
+        file_content: str,
+    ) -> Iterator[LinterResult]:
+        """
+        Checks for correct parameters for script_xref calls
+        """
+        if nasl_file.suffix == ".inc":
+            return
+
+        matches = re.finditer(r"script_xref\(.*\);", file_content)
+        if matches:
+            for match in matches:
+                if match:
+                    if not get_xref_pattern(name=r".*", value=r".*").match(
+                        match.group(0)
+                    ):
+                        yield LinterError(
+                            f"{match.group(0)}: does not conform to"
+                            ' script_xref(name:"<name>", value:<value>);',
+                            file=nasl_file,
+                            plugin=self.name,
+                        )
```

### Comparing `troubadix-23.4.2/tests/plugins/test_vt_placement.py` & `troubadix-23.4.3/tests/plugins/test_vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/__init__.py` & `troubadix-23.4.3/tests/standalone_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/changed_packages/__init__.py` & `troubadix-23.4.3/tests/standalone_plugins/changed_packages/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/changed_packages/markers/__init__.py` & `troubadix-23.4.3/tests/standalone_plugins/changed_packages/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py` & `troubadix-23.4.3/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/changed_packages/markers/test_added_release.py` & `troubadix-23.4.3/tests/standalone_plugins/changed_packages/markers/test_added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py` & `troubadix-23.4.3/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/changed_packages/markers/test_changed_update.py` & `troubadix-23.4.3/tests/standalone_plugins/changed_packages/markers/test_changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py` & `troubadix-23.4.3/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/changed_packages/test_changed_packages.py` & `troubadix-23.4.3/tests/standalone_plugins/changed_packages/test_changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/changed_packages/test_package.py` & `troubadix-23.4.3/tests/standalone_plugins/changed_packages/test_package.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/test_changed_cves.py` & `troubadix-23.4.3/tests/standalone_plugins/test_changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/test_changed_oid.py` & `troubadix-23.4.3/tests/standalone_plugins/test_changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/test_last_modification.py` & `troubadix-23.4.3/tests/standalone_plugins/test_last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/test_no_solution.py` & `troubadix-23.4.3/tests/standalone_plugins/test_no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/standalone_plugins/test_version_updated.py` & `troubadix-23.4.3/tests/standalone_plugins/test_version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/test_argparser.py` & `troubadix-23.4.3/tests/test_argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/test_helper.py` & `troubadix-23.4.3/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/test_naslinter.py` & `troubadix-23.4.3/tests/test_naslinter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/test_reporter.py` & `troubadix-23.4.3/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/test_results.py` & `troubadix-23.4.3/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/tests/test_runner.py` & `troubadix-23.4.3/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/__init__.py` & `troubadix-23.4.3/troubadix/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/argparser.py` & `troubadix-23.4.3/troubadix/argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/codespell/codespell.exclude` & `troubadix-23.4.3/troubadix/codespell/codespell.exclude`

 * *Files 0% similar despite different names*

```diff
@@ -348,14 +348,15 @@
 Fix java detection on machines with too many cpus CVE-2018-10583: An information disclosure vulnerability occured when
 Fix %posttrans script execution (fixes #265) The scripts are execuable.
 - Fix removeing links before update-alternatives run. bnc#931702
 fix SOLVER_FLAG_FOCUS_BEST updateing packages without reason
 Fix source-download commnds help (bsc#1180663)
 fixtext = 'Add rules to audit the system calls "creat", "open/openat" and "truncate/ftruncate" in
 	Fix typo in preference name: "password" misspelled as "pasword".
+"fo",
 #<FONT SIZE="+3">S</FONT>EARCH
  - For backwards compatability, setting --log-driver=json-file in podman
 foreach dir( make_list_unique( "/ag", "/ang", "/guestbook", "/anguestbook", http_cgi_dirs( port:port ) ) ) {
 foreach dir(make_list_unique("/", "/annonce", http_cgi_dirs(port:port))) {
 foreach dir( make_list_unique( "/", "/cas", "/cas-server-webapp", http_cgi_dirs( port:port ) ) ) {
 foreach dir( make_list_unique( "/", "/fom", http_cgi_dirs( port:port ) ) ) {
   foreach url( make_list( dir + "/ans.pl?p=../../../../../usr/bin/id|&blah",
```

### Comparing `troubadix-23.4.2/troubadix/codespell/codespell.ignore` & `troubadix-23.4.3/troubadix/codespell/codespell.ignore`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/helper/__init__.py` & `troubadix-23.4.3/troubadix/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/helper/helper.py` & `troubadix-23.4.3/troubadix/helper/helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/helper/linguistic_exception_handler.py` & `troubadix-23.4.3/troubadix/helper/linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/helper/patterns.py` & `troubadix-23.4.3/troubadix/helper/patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugin.py` & `troubadix-23.4.3/troubadix/plugin.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/__init__.py` & `troubadix-23.4.3/troubadix/plugins/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from .creation_date import CheckCreationDate
 from .cve_format import CheckCVEFormat
 from .cvss_format import CheckCVSSFormat
 from .dependencies import CheckDependencies
 from .dependency_category_order import CheckDependencyCategoryOrder
 from .deprecated_dependency import CheckDeprecatedDependency
 from .deprecated_functions import CheckDeprecatedFunctions
-from .description import CheckDescription
 from .double_end_points import CheckDoubleEndPoints
 from .duplicate_oid import CheckDuplicateOID
 from .duplicated_script_tags import CheckDuplicatedScriptTags
 from .encoding import CheckEncoding
 from .forking_nasl_functions import CheckForkingNaslFunctions
 from .get_kb_on_services import CheckGetKBOnServices
 from .grammar import CheckGrammar
@@ -45,15 +44,14 @@
 from .missing_desc_exit import CheckMissingDescExit
 from .missing_tag_solution import CheckMissingTagSolution
 from .newlines import CheckNewlines
 from .overlong_script_tags import CheckOverlongScriptTags
 from .prod_svc_detect_in_vulnvt import CheckProdSvcDetectInVulnvt
 from .qod import CheckQod
 from .reporting_consistency import CheckReportingConsistency
-from .risk_factor import CheckRiskFactor
 from .script_add_preference_type import CheckScriptAddPreferenceType
 from .script_calls_empty_values import CheckScriptCallsEmptyValues
 from .script_calls_recommended import CheckScriptCallsRecommended
 from .script_category import CheckScriptCategory
 from .script_copyright import CheckScriptCopyright
 from .script_family import CheckScriptFamily
 from .script_tag_form import CheckScriptTagForm
@@ -87,15 +85,14 @@
     CheckCreationDate,
     CheckCVEFormat,
     CheckCVSSFormat,
     CheckDependencies,
     CheckDependencyCategoryOrder,
     CheckDeprecatedDependency,
     CheckDeprecatedFunctions,
-    CheckDescription,
     CheckDoubleEndPoints,
     CheckDuplicatedScriptTags,
     CheckEncoding,
     CheckForkingNaslFunctions,
     CheckGetKBOnServices,
     CheckGrammar,
     CheckHttpLinksInTags,
@@ -106,15 +103,14 @@
     CheckMissingDescExit,
     CheckMissingTagSolution,
     CheckNewlines,
     CheckOverlongScriptTags,
     CheckProdSvcDetectInVulnvt,
     CheckQod,
     CheckReportingConsistency,
-    CheckRiskFactor,
     CheckScriptAddPreferenceType,
     CheckScriptCallsEmptyValues,
     CheckScriptCallsRecommended,
     CheckScriptCategory,
     CheckScriptCopyright,
     CheckScriptFamily,
     CheckScriptTagForm,
```

### Comparing `troubadix-23.4.2/troubadix/plugins/badwords.py` & `troubadix-23.4.3/troubadix/plugins/badwords.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/copyright_text.py` & `troubadix-23.4.3/troubadix/plugins/copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/copyright_year.py` & `troubadix-23.4.3/troubadix/plugins/copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/creation_date.py` & `troubadix-23.4.3/troubadix/plugins/creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/cve_format.py` & `troubadix-23.4.3/troubadix/plugins/cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/cvss_format.py` & `troubadix-23.4.3/troubadix/plugins/cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/dependencies.py` & `troubadix-23.4.3/troubadix/plugins/dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/dependency_category_order.py` & `troubadix-23.4.3/troubadix/plugins/dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/deprecated_dependency.py` & `troubadix-23.4.3/troubadix/plugins/deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/deprecated_functions.py` & `troubadix-23.4.3/troubadix/plugins/deprecated_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,43 +22,44 @@
 
 
 class CheckDeprecatedFunctions(FilePlugin):
     name = "check_deprecated_functions"
 
     def run(self) -> Iterator[LinterResult]:
         """
-        Following functions / description items are outdated:
+        Following functions / description items are deprecated:
         script_summary()
         script_id()
         security_note()
         security_warning()
         security_hole()
         script_description()
-        script_tag("risk_factor", SEVERITY);
+        script_tag(name:"risk_factor", value:"SEVERITY");
         script_bugtraq_id()
 
-        This script checks if any of those are used
+        This script checks and reports if any of those are used
 
         Args:
             nasl_file: Name of the VT to be checked
         """
         deprecated_functions = {
-            "script_summary(), use script_tag"
-            '(name:"summary", value:"") instead': r"script_summary\s*\([^)]*\)",
-            "script_id(), use script_oid() with "
-            "the full OID instead": r"script_id\s*\([0-9]+\)",
-            "security_note()": r"security_note\s*\([^)]*\)",
-            "security_warning()": r"security_warning\s*\([^)]*\)",
-            "security_hole()": r"security_hole\s*\([^)]*\)",
-            "script_description()": r"script_description\s*\([^)]*\)",
-            'script_tag(name:"risk_factor", value: '
-            "SEVERITY)": r'script_tag\s*\(\s*name:\s*"risk_factor"[^)]*\)',
-            "script_bugtraq_id()": r"script_bugtraq_id\s*\([^)]*\)",
+            'script_summary();, use script_tag(name:"summary", value:""); '
+            "instead": r"script_summary\s*\([^)]*\);",
+            "script_id();, use script_oid(); with "
+            "the full OID instead": r"script_id\s*\([0-9]+\);",
+            "security_note();": r"security_note\s*\([^)]*\);",
+            "security_warning();": r"security_warning\s*\([^)]*\);",
+            "security_hole();": r"security_hole\s*\([^)]*\);",
+            "script_description();": r"script_description\s*\([^)]*\);",
+            'script_tag(name:"risk_factor", value:'
+            '"SEVERITY");': r'script_tag\s*\(\s*name:\s*"risk_factor"[^)]*\);',
+            "script_bugtraq_id();": r"script_bugtraq_id\s*\([^)]*\);",
         }
 
         for description, pattern in deprecated_functions.items():
-            if re.search(pattern, self.context.file_content):
+            if re.search(pattern, self.context.file_content, re.MULTILINE):
                 yield LinterError(
-                    f"Found a deprecated function call: {description}",
+                    "Found a deprecated function call / description item: "
+                    f"{description}",
                     file=self.context.nasl_file,
                     plugin=self.name,
                 )
```

### Comparing `troubadix-23.4.2/troubadix/plugins/description.py` & `troubadix-23.4.3/troubadix/plugins/script_calls_empty_values.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,72 @@
-#  Copyright (c) 2022 Greenbone AG
+# Copyright (C) 2022 Greenbone AG
 #
-#  SPDX-License-Identifier: GPL-3.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 #
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import re
+from pathlib import Path
 from typing import Iterator
 
-from troubadix.plugin import FilePlugin, LinterError, LinterResult
-
-
-class CheckDescription(FilePlugin):
-    name = "check_description"
+from troubadix.helper.patterns import (
+    _get_special_script_tag_pattern,
+    _get_tag_pattern,
+    get_xref_pattern,
+)
+from troubadix.plugin import FileContentPlugin, LinterError, LinterResult
+
+# For the future
+SPECIAL_SCRIPT_TAG_LIST = []
+
+
+class CheckScriptCallsEmptyValues(FileContentPlugin):
+    name = "check_script_calls_empty_values"
+
+    def check_content(
+        self,
+        nasl_file: Path,
+        file_content: str,
+    ) -> Iterator[LinterResult]:
+        """
+        Checks for empty 'value:""' in script calls. Excepted from this is
+        script_add_preferences().
+        """
+        if nasl_file.suffix == ".inc":
+            return
 
-    def run(self) -> Iterator[LinterResult]:
-        """This script checks if some NVTs are still using script_description
+        matches = _get_tag_pattern(name=r".*", value=r"").finditer(file_content)
+        for match in matches:
+            yield LinterError(
+                f"{match.group(0)} does not contain a value",
+                file=nasl_file,
+                plugin=self.name,
+            )
 
-        Args:
-            nasl_file:    The VT / Include that is going to be checked
-            file_content: The content of the file that is going to be
-                          checked
-        """
-        script_description = re.compile(
-            r"script_description", re.IGNORECASE
-        ).search(self.context.file_content)
-        if script_description:
+        matches = get_xref_pattern(name=r".*", value=r"").finditer(file_content)
+        for match in matches:
             yield LinterError(
-                "VT/Include is using deprecated 'script_description'",
-                file=self.context.nasl_file,
+                f"{match.group(0)} does not contain a value",
+                file=nasl_file,
                 plugin=self.name,
             )
+
+        for call in SPECIAL_SCRIPT_TAG_LIST:
+            matches = _get_special_script_tag_pattern(
+                name=call.value, value=""
+            ).finditer(file_content)
+            for match in matches:
+                yield LinterError(
+                    f"{match.group(0)} does not contain a value",
+                    file=nasl_file,
+                    plugin=self.name,
+                )
```

### Comparing `troubadix-23.4.2/troubadix/plugins/double_end_points.py` & `troubadix-23.4.3/troubadix/plugins/double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/duplicate_oid.py` & `troubadix-23.4.3/troubadix/plugins/duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/duplicated_script_tags.py` & `troubadix-23.4.3/troubadix/plugins/duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/encoding.py` & `troubadix-23.4.3/troubadix/plugins/encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/forking_nasl_functions.py` & `troubadix-23.4.3/troubadix/plugins/forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/get_kb_on_services.py` & `troubadix-23.4.3/troubadix/plugins/get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/grammar.py` & `troubadix-23.4.3/troubadix/plugins/grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/http_links_in_tags.py` & `troubadix-23.4.3/troubadix/plugins/http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/illegal_characters.py` & `troubadix-23.4.3/troubadix/plugins/illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/log_messages.py` & `troubadix-23.4.3/troubadix/plugins/log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/malformed_dependencies.py` & `troubadix-23.4.3/troubadix/plugins/malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/misplaced_compare_in_if.py` & `troubadix-23.4.3/troubadix/plugins/misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/missing_desc_exit.py` & `troubadix-23.4.3/troubadix/plugins/missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/missing_tag_solution.py` & `troubadix-23.4.3/troubadix/plugins/missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/newlines.py` & `troubadix-23.4.3/troubadix/plugins/newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/overlong_script_tags.py` & `troubadix-23.4.3/troubadix/plugins/overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/prod_svc_detect_in_vulnvt.py` & `troubadix-23.4.3/troubadix/plugins/prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/qod.py` & `troubadix-23.4.3/troubadix/plugins/qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/reporting_consistency.py` & `troubadix-23.4.3/troubadix/plugins/reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/risk_factor.py` & `troubadix-23.4.3/troubadix/plugins/tabs.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,31 +11,26 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import re
 from typing import Iterator
 
 from troubadix.plugin import FilePlugin, LinterError, LinterResult
 
 
-class CheckRiskFactor(FilePlugin):
-    name = "check_risk_factor"
+class CheckTabs(FilePlugin):
+    name = "check_tabs"
 
     def run(self) -> Iterator[LinterResult]:
-        """This script checks if a VT with risk_factor tag exist."""
-        match = re.search(
-            r'script_tag\(name:"risk_factor", value:"(?P<risk>.+)"\);',
-            self.context.file_content,
-        )
-
-        if not match:
-            return
-
-        yield LinterError(
-            f'Deprecated function "risk factor" found: {match.group("risk")}',
-            file=self.context.nasl_file,
-            plugin=self.name,
-        )
+        """This script checks if a VT is using one or
+        more tabs instead of spaces."""
+        for nr, line in enumerate(self.context.lines, 1):
+            if "\t" in line:
+                yield LinterError(
+                    "VT uses tabs instead of spaces.",
+                    file=self.context.nasl_file,
+                    plugin=self.name,
+                    line=nr,
+                )
```

### Comparing `troubadix-23.4.2/troubadix/plugins/script_add_preference_type.py` & `troubadix-23.4.3/troubadix/plugins/script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/script_calls_empty_values.py` & `troubadix-23.4.3/troubadix/plugins/solution_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,62 +11,68 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+import re
 from pathlib import Path
 from typing import Iterator
 
-from troubadix.helper.patterns import (
-    _get_special_script_tag_pattern,
-    _get_tag_pattern,
-    get_xref_pattern,
-)
 from troubadix.plugin import FileContentPlugin, LinterError, LinterResult
 
-# For the future
-SPECIAL_SCRIPT_TAG_LIST = []
+VALUES = (
+    "Workaround",
+    "Mitigation",
+    "VendorFix",
+    "NoneAvailable",
+    "WillNotFix",
+)
+
 
+class CheckSolutionType(FileContentPlugin):
+    """
+    This script checks the passed VT for the existence/format of its
+    solution_type with the help of regular expression.An error will be thrown
+    if the VT does not contain a solution_type at all or of the solution_type
+    contains an invalid value.
+    """
 
-class CheckScriptCallsEmptyValues(FileContentPlugin):
-    name = "check_script_calls_empty_values"
+    name = "check_solution_type"
 
     def check_content(
         self,
         nasl_file: Path,
         file_content: str,
     ) -> Iterator[LinterResult]:
-        """
-        Checks for empty 'value:""' in script calls. Excepted from this is
-        script_add_preferences().
-        """
         if nasl_file.suffix == ".inc":
             return
 
-        matches = _get_tag_pattern(name=r".*", value=r"").finditer(file_content)
-        for match in matches:
-            yield LinterError(
-                f"{match.group(0)} does not contain a value",
-                file=nasl_file,
-                plugin=self.name,
-            )
-
-        matches = get_xref_pattern(name=r".*", value=r"").finditer(file_content)
-        for match in matches:
-            yield LinterError(
-                f"{match.group(0)} does not contain a value",
-                file=nasl_file,
-                plugin=self.name,
-            )
+        has_severity = True
+        cvss_detect = re.search(
+            r"script_tag\s*\(name\s*:\s*\"cvss_base\","
+            r"\s*value:\s*\"(\d{1,2}\.\d)\"\)",
+            file_content,
+        )
+        if cvss_detect is not None and cvss_detect.group(1) == "0.0":
+            has_severity = False
+
+        match = re.search(
+            r"script_tag\s*\(name\s*:\s*\"(solution_type)\"\s*,"
+            r"\s*value\s*:\s*\"([a-zA-Z\s]+)\"\s*\)\s*;",
+            file_content,
+        )
 
-        for call in SPECIAL_SCRIPT_TAG_LIST:
-            matches = _get_special_script_tag_pattern(
-                name=call.value, value=""
-            ).finditer(file_content)
-            for match in matches:
+        if has_severity:
+            if match is None or match.group(1) is None:
                 yield LinterError(
-                    f"{match.group(0)} does not contain a value",
+                    "VT does not contain a solution_type",
                     file=nasl_file,
                     plugin=self.name,
                 )
+        if match is not None and match.group(2) not in VALUES:
+            yield LinterError(
+                "VT does not contain a valid solution_type 'value'",
+                file=nasl_file,
+                plugin=self.name,
+            )
```

### Comparing `troubadix-23.4.2/troubadix/plugins/script_calls_recommended.py` & `troubadix-23.4.3/troubadix/plugins/script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/script_category.py` & `troubadix-23.4.3/troubadix/plugins/script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/script_copyright.py` & `troubadix-23.4.3/troubadix/plugins/script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/script_family.py` & `troubadix-23.4.3/troubadix/plugins/script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/script_tag_form.py` & `troubadix-23.4.3/troubadix/plugins/script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/script_tag_whitespaces.py` & `troubadix-23.4.3/troubadix/plugins/script_tag_whitespaces.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/script_tags_mandatory.py` & `troubadix-23.4.3/troubadix/plugins/script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/script_version_and_last_modification_tags.py` & `troubadix-23.4.3/troubadix/plugins/script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/script_xref_form.py` & `troubadix-23.4.3/troubadix/plugins/todo_tbd.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Greenbone AG
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -13,40 +13,44 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import re
 from pathlib import Path
-from typing import Iterator
+from typing import Iterable, Iterator
 
-from troubadix.helper.patterns import get_xref_pattern
-from troubadix.plugin import FileContentPlugin, LinterError, LinterResult
+from ..helper import is_ignore_file
+from ..plugin import LineContentPlugin, LinterResult, LinterWarning
 
+_IGNORE_FILES = [
+    "gb_openvas",
+    "gb_gsa_",
+    "http_func.inc",
+    "misc_func.inc",
+]
 
-class CheckScriptXrefForm(FileContentPlugin):
-    name = "check_script_xref_form"
 
-    def check_content(
+class CheckTodoTbd(LineContentPlugin):
+    """This step checks if a given VT contains the words TODO, TBD
+    or @todo as a comment.
+    """
+
+    name = "check_todo_tbd"
+
+    def check_lines(
         self,
         nasl_file: Path,
-        file_content: str,
+        lines: Iterable[str],
     ) -> Iterator[LinterResult]:
-        """
-        Checks for correct parameters for script_xref calls
-        """
-        if nasl_file.suffix == ".inc":
+        if is_ignore_file(nasl_file, _IGNORE_FILES):
             return
 
-        matches = re.finditer(r"script_xref\(.*\);", file_content)
-        if matches:
-            for match in matches:
-                if match:
-                    if not get_xref_pattern(name=r".*", value=r".*").match(
-                        match.group(0)
-                    ):
-                        yield LinterError(
-                            f"{match.group(0)}: does not conform to"
-                            ' script_xref(name:"<name>", value:<value>);',
-                            file=nasl_file,
-                            plugin=self.name,
-                        )
+        for index, line in enumerate(lines, start=1):
+            match = re.search("##? *(TODO|TBD|@todo):?", line)
+            if match is not None:
+                yield LinterWarning(
+                    "VT contains #TODO/TBD/@todo keywords.",
+                    file=nasl_file,
+                    plugin=self.name,
+                    line=index,
+                )
```

### Comparing `troubadix-23.4.2/troubadix/plugins/script_xref_url.py` & `troubadix-23.4.3/troubadix/plugins/script_xref_url.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/security_messages.py` & `troubadix-23.4.3/troubadix/plugins/security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/set_get_kb_calls.py` & `troubadix-23.4.3/troubadix/plugins/set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/solution_text.py` & `troubadix-23.4.3/troubadix/plugins/solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/solution_type.py` & `troubadix-23.4.3/troubadix/plugins/vt_placement.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Greenbone AG
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,67 +12,80 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import re
+from itertools import chain
 from pathlib import Path
 from typing import Iterator
 
+from troubadix.helper import ScriptTag, SpecialScriptTag, get_script_tag_pattern
+from troubadix.helper.helper import ENTERPRISE_FOLDERS, FEED_VERSIONS
+from troubadix.helper.patterns import _get_special_script_tag_pattern
 from troubadix.plugin import FileContentPlugin, LinterError, LinterResult
 
-VALUES = (
-    "Workaround",
-    "Mitigation",
-    "VendorFix",
-    "NoneAvailable",
-    "WillNotFix",
-)
 
+class CheckVTPlacement(FileContentPlugin):
+    """The script checks if the passed VT is using one of the
+    two following families:
 
-class CheckSolutionType(FileContentPlugin):
-    """
-    This script checks the passed VT for the existence/format of its
-    solution_type with the help of regular expression.An error will be thrown
-    if the VT does not contain a solution_type at all or of the solution_type
-    contains an invalid value.
+    - script_family("Service detection");
+    - script_family("Product detection");
+
+    and is correctly placed into the "root" of the VTs directory.
     """
 
-    name = "check_solution_type"
+    name = "check_vt_placement"
 
     def check_content(
         self,
         nasl_file: Path,
         file_content: str,
     ) -> Iterator[LinterResult]:
+        """
+        Args:
+            nasl_file: The VT that shall be checked
+            file_content: str representing the file content
+
+        Returns:
+            if no problem
+        """
+
         if nasl_file.suffix == ".inc":
             return
 
-        has_severity = True
-        cvss_detect = re.search(
-            r"script_tag\s*\(name\s*:\s*\"cvss_base\","
-            r"\s*value:\s*\"(\d{1,2}\.\d)\"\)",
-            file_content,
-        )
-        if cvss_detect is not None and cvss_detect.group(1) == "0.0":
-            has_severity = False
+        root = self.context.root
 
-        match = re.search(
-            r"script_tag\s*\(name\s*:\s*\"(solution_type)\"\s*,"
-            r"\s*value\s*:\s*\"([a-zA-Z\s]+)\"\s*\)\s*;",
-            file_content,
-        )
+        match = _get_special_script_tag_pattern(
+            name=SpecialScriptTag.FAMILY.value,
+            value=r"(Product|Service) detection",
+            flags=re.MULTILINE,
+        ).search(file_content)
+        if match is None:
+            return
 
-        if has_severity:
-            if match is None or match.group(1) is None:
-                yield LinterError(
-                    "VT does not contain a solution_type",
-                    file=nasl_file,
-                    plugin=self.name,
-                )
-        if match is not None and match.group(2) not in VALUES:
-            yield LinterError(
-                "VT does not contain a valid solution_type 'value'",
-                file=nasl_file,
-                plugin=self.name,
-            )
+        tag_pattern = get_script_tag_pattern(ScriptTag.DEPRECATED)
+
+        match = tag_pattern.search(file_content)
+        if match is not None:
+            return
+
+        if any(
+            (root / vers / nasl_file.name) == nasl_file
+            for vers in FEED_VERSIONS
+        ):
+            return
+
+        for folder in chain(["attic"], ENTERPRISE_FOLDERS):
+            if any(
+                (root / vers / folder / nasl_file.name) == nasl_file
+                for vers in FEED_VERSIONS
+            ):
+                return
+
+        yield LinterError(
+            f"VT should be placed in the root directory ({root}).",
+            file=nasl_file,
+            plugin=self.name,
+        )
```

### Comparing `troubadix-23.4.2/troubadix/plugins/spelling.py` & `troubadix-23.4.3/troubadix/plugins/spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/tabs.py` & `troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Greenbone AG
+# Copyright (C) 2023 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,26 +11,24 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Iterator
+from typing import List
 
-from troubadix.plugin import FilePlugin, LinterError, LinterResult
+from troubadix.standalone_plugins.changed_packages.package import (
+    Direction,
+    Package,
+    Reasons,
+)
 
+from .marker import Marker
 
-class CheckTabs(FilePlugin):
-    name = "check_tabs"
 
-    def run(self) -> Iterator[LinterResult]:
-        """This script checks if a VT is using one or
-        more tabs instead of spaces."""
-        for nr, line in enumerate(self.context.lines, 1):
-            if "\t" in line:
-                yield LinterError(
-                    "VT uses tabs instead of spaces.",
-                    file=self.context.nasl_file,
-                    plugin=self.name,
-                    line=nr,
-                )
+class AddedUdeb(Marker):
+    @staticmethod
+    def mark(new_packages: List[Package]):
+        for package in new_packages:
+            if package.name.endswith("-udeb"):
+                package.reasons[Reasons.ADDED_UDEB] = Direction.ACTIVE
```

### Comparing `troubadix-23.4.2/troubadix/plugins/todo_tbd.py` & `troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone AG
+# Copyright (C) 2023 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,46 +11,41 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import re
-from pathlib import Path
-from typing import Iterable, Iterator
-
-from ..helper import is_ignore_file
-from ..plugin import LineContentPlugin, LinterResult, LinterWarning
-
-_IGNORE_FILES = [
-    "gb_openvas",
-    "gb_gsa_",
-    "http_func.inc",
-    "misc_func.inc",
-]
-
-
-class CheckTodoTbd(LineContentPlugin):
-    """This step checks if a given VT contains the words TODO, TBD
-    or @todo as a comment.
-    """
-
-    name = "check_todo_tbd"
-
-    def check_lines(
-        self,
-        nasl_file: Path,
-        lines: Iterable[str],
-    ) -> Iterator[LinterResult]:
-        if is_ignore_file(nasl_file, _IGNORE_FILES):
-            return
-
-        for index, line in enumerate(lines, start=1):
-            match = re.search("##? *(TODO|TBD|@todo):?", line)
-            if match is not None:
-                yield LinterWarning(
-                    "VT contains #TODO/TBD/@todo keywords.",
-                    file=nasl_file,
-                    plugin=self.name,
-                    line=index,
-                )
+from typing import List
+
+from troubadix.standalone_plugins.changed_packages.package import (
+    Direction,
+    Package,
+    Reasons,
+)
+
+from .marker import Marker
+
+
+class DroppedArchitecture(Marker):
+    @classmethod
+    def mark(cls, missing_packages: List[Package], new_packages: List[Package]):
+        for package in missing_packages:
+            if not ":" in package.name:
+                continue
+
+            other_package = cls._find_package(
+                Package(
+                    package.name.split(":")[0],
+                    package.version,
+                    package.release,
+                ),
+                new_packages,
+            )
+
+            if not other_package:
+                continue
+
+            package.reasons[Reasons.DROPPED_ARCHITECTURE] = Direction.PASSIVE
+            other_package.reasons[
+                Reasons.DROPPED_ARCHITECTURE
+            ] = Direction.ACTIVE
```

### Comparing `troubadix-23.4.2/troubadix/plugins/trailing_spaces_tabs.py` & `troubadix-23.4.3/troubadix/plugins/trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/using_display.py` & `troubadix-23.4.3/troubadix/plugins/using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/valid_oid.py` & `troubadix-23.4.3/troubadix/plugins/valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/valid_script_tag_names.py` & `troubadix-23.4.3/troubadix/plugins/valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/variable_assigned_in_if.py` & `troubadix-23.4.3/troubadix/plugins/variable_assigned_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/plugins/vt_file_permissions.py` & `troubadix-23.4.3/troubadix/plugins/vt_file_permissions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/reporter.py` & `troubadix-23.4.3/troubadix/reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/results.py` & `troubadix-23.4.3/troubadix/results.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/runner.py` & `troubadix-23.4.3/troubadix/runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/standalone_plugins/changed_cves.py` & `troubadix-23.4.3/troubadix/standalone_plugins/changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/standalone_plugins/changed_oid.py` & `troubadix-23.4.3/troubadix/standalone_plugins/changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/changed_packages.py` & `troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/marker/__init__.py` & `troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/marker/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py` & `troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/marker/added_release.py` & `troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/marker/added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py` & `troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/marker/marker.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import List
+from typing import Iterable
 
-from troubadix.standalone_plugins.changed_packages.package import (
-    Direction,
-    Package,
-    Reasons,
-)
+from troubadix.standalone_plugins.changed_packages.package import Package
 
-from .marker import Marker
 
-
-class AddedUdeb(Marker):
+class Marker:
     @staticmethod
-    def mark(new_packages: List[Package]):
-        for package in new_packages:
-            if package.name.endswith("-udeb"):
-                package.reasons[Reasons.ADDED_UDEB] = Direction.ACTIVE
+    def _find_package(package: Package, packages: Iterable[Package]):
+        result = next(
+            (
+                other_package
+                for other_package in packages
+                if other_package.name == package.name
+                and other_package.version == package.version
+                and other_package.release == package.release
+            ),
+            None,
+        )
+        return result
```

### Comparing `troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/marker/changed_update.py` & `troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/marker/changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/standalone_plugins/changed_packages/package.py` & `troubadix-23.4.3/troubadix/standalone_plugins/changed_packages/package.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/standalone_plugins/common.py` & `troubadix-23.4.3/troubadix/standalone_plugins/common.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/standalone_plugins/last_modification.py` & `troubadix-23.4.3/troubadix/standalone_plugins/last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/standalone_plugins/no_solution.py` & `troubadix-23.4.3/troubadix/standalone_plugins/no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/standalone_plugins/version_updated.py` & `troubadix-23.4.3/troubadix/standalone_plugins/version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/troubadix/troubadix.py` & `troubadix-23.4.3/troubadix/troubadix.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.4.2/PKG-INFO` & `troubadix-23.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troubadix
-Version: 23.4.2
+Version: 23.4.3
 Summary: A linting and QA check tool for NASL files
 Home-page: https://github.com/greenbone/troubadix
 License: GPL-3.0-or-later
 Author: Greenbone
 Author-email: info@greenbone.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

